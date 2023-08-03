# Comparing `tmp/deprl-0.1.8.tar.gz` & `tmp/deprl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprl-0.1.8.tar", max compression
+gzip compressed data, was "deprl-0.2.0.tar", max compression
```

## Comparing `deprl-0.1.8.tar` & `deprl-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,98 @@
--rw-r--r--   0        0        0     1083 2023-06-24 08:15:25.085768 deprl-0.1.8/LICENSE
--rw-r--r--   0        0        0     8744 2023-07-17 20:54:31.856231 deprl-0.1.8/README.md
--rw-r--r--   0        0        0      563 2023-07-17 19:00:57.722034 deprl-0.1.8/deprl/__init__.py
--rw-r--r--   0        0        0     6481 2023-07-17 19:01:02.334145 deprl-0.1.8/deprl/custom_agents.py
--rw-r--r--   0        0        0     8956 2023-06-24 10:36:54.750864 deprl-0.1.8/deprl/custom_distributed.py
--rw-r--r--   0        0        0     3639 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/custom_mpo_torch.py
--rw-r--r--   0        0        0     3541 2023-07-17 19:00:57.722034 deprl-0.1.8/deprl/custom_test_environment.py
--rw-r--r--   0        0        0     1244 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/custom_torso.py
--rw-r--r--   0        0        0     5910 2023-07-17 19:48:36.494493 deprl-0.1.8/deprl/custom_trainer.py
--rw-r--r--   0        0        0     7373 2023-04-09 21:53:51.364949 deprl-0.1.8/deprl/dep_controller.py
--rw-r--r--   0        0        0      132 2023-06-24 12:25:57.343025 deprl-0.1.8/deprl/env_wrappers/__init__.py
--rw-r--r--   0        0        0     6471 2023-07-17 19:00:57.730034 deprl-0.1.8/deprl/env_wrappers/wrappers.py
--rw-r--r--   0        0        0     2175 2023-07-17 19:00:57.730034 deprl-0.1.8/deprl/log.py
--rw-r--r--   0        0        0     7722 2023-06-24 09:16:24.447868 deprl-0.1.8/deprl/main.py
--rw-r--r--   0        0        0      704 2023-06-24 12:25:57.351026 deprl-0.1.8/deprl/param_files/default_agents.json
--rw-r--r--   0        0        0     9156 2023-07-17 19:01:02.334145 deprl-0.1.8/deprl/play.py
--rw-r--r--   0        0        0    11578 2023-06-04 08:48:50.159176 deprl-0.1.8/deprl/play_plot.py
--rw-r--r--   0        0        0       80 2023-05-14 15:41:46.780895 deprl-0.1.8/deprl/plot.py
--rw-r--r--   0        0        0     9570 2023-06-05 17:53:13.795777 deprl-0.1.8/deprl/record_data_myoleg.py
--rw-r--r--   0        0        0     9458 2023-06-04 21:20:27.262283 deprl-0.1.8/deprl/record_video_myoleg.py
--rw-r--r--   0        0        0     8951 2023-07-12 16:45:11.388605 deprl-0.1.8/deprl/save_actor.py
--rw-r--r--   0        0        0     8754 2023-06-03 11:57:19.300487 deprl-0.1.8/deprl/time_play_baoding.py
--rw-r--r--   0        0        0      230 2023-07-17 19:00:57.734034 deprl-0.1.8/deprl/utils/__init__.py
--rw-r--r--   0        0        0     3053 2023-06-24 12:24:30.438761 deprl-0.1.8/deprl/utils/analysis_utils.py
--rw-r--r--   0        0        0     9582 2023-06-01 15:04:44.000000 deprl-0.1.8/deprl/utils/resources/exp_gait.zml
--rw-r--r--   0        0        0     6188 2023-07-17 21:32:46.311048 deprl-0.1.8/deprl/utils/utils.py
--rw-r--r--   0        0        0    16024 2023-06-04 09:09:44.415824 deprl-0.1.8/deprl/utils/utils_scone_gait_sto.py
--rw-r--r--   0        0        0       39 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/__init__.py
--rwxr-xr-x   0        0        0       80 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/.gitignore
--rw-r--r--   0        0        0     1110 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/LICENSE
--rw-r--r--   0        0        0      207 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/__init__.py
--rw-r--r--   0        0        0      178 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/agents/__init__.py
--rw-r--r--   0        0        0     1255 2023-07-17 19:01:02.334145 deprl-0.1.8/deprl/vendor/tonic/agents/agent.py
--rw-r--r--   0        0        0     3954 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/agents/basic.py
--rw-r--r--   0        0        0      293 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/environments/__init__.py
--rw-r--r--   0        0        0     5731 2023-07-17 19:48:36.094486 deprl-0.1.8/deprl/vendor/tonic/environments/builders.py
--rw-r--r--   0        0        0     6612 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/environments/distributed.py
--rw-r--r--   0        0        0     1914 2023-04-27 12:08:50.580729 deprl-0.1.8/deprl/vendor/tonic/environments/wrappers.py
--rw-r--r--   0        0        0      175 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/explorations/__init__.py
--rw-r--r--   0        0        0     2939 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/explorations/noisy.py
--rw-r--r--   0        0        0     8754 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/play.py
--rw-r--r--   0        0        0    18151 2023-05-14 15:41:47.404899 deprl-0.1.8/deprl/vendor/tonic/plot.py
--rw-r--r--   0        0        0      167 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/replays/__init__.py
--rw-r--r--   0        0        0     3636 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/replays/buffers.py
--rw-r--r--   0        0        0     2815 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/replays/segments.py
--rw-r--r--   0        0        0      821 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/replays/utils.py
--rw-r--r--   0        0        0      103 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/__init__.py
--rw-r--r--   0        0        0      303 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/__init__.py
--rw-r--r--   0        0        0     4630 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/a2c.py
--rw-r--r--   0        0        0      519 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/agent.py
--rw-r--r--   0        0        0     1456 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/d4pg.py
--rw-r--r--   0        0        0     4327 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/ddpg.py
--rw-r--r--   0        0        0     4089 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/mpo.py
--rw-r--r--   0        0        0     2452 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/ppo.py
--rw-r--r--   0        0        0     1868 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/sac.py
--rw-r--r--   0        0        0     2181 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/td3.py
--rw-r--r--   0        0        0     1448 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/td4.py
--rw-r--r--   0        0        0     3754 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/trpo.py
--rw-r--r--   0        0        0      819 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     6247 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/actor_critics.py
--rw-r--r--   0        0        0     4849 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/actors.py
--rw-r--r--   0        0        0     3046 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/critics.py
--rw-r--r--   0        0        0      734 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/encoders.py
--rw-r--r--   0        0        0      627 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1339 2023-04-27 12:08:50.584729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/normalizers/returns.py
--rw-r--r--   0        0        0     1260 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/__init__.py
--rw-r--r--   0        0        0    19301 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/actors.py
--rw-r--r--   0        0        0    13820 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/critics.py
--rw-r--r--   0        0        0     4232 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
--rw-r--r--   0        0        0      193 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/utils.py
--rw-r--r--   0        0        0      103 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/__init__.py
--rw-r--r--   0        0        0      277 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/__init__.py
--rw-r--r--   0        0        0     5287 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/a2c.py
--rw-r--r--   0        0        0     1441 2023-05-14 15:41:46.528893 deprl-0.1.8/deprl/vendor/tonic/torch/agents/agent.py
--rw-r--r--   0        0        0     1522 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/d4pg.py
--rw-r--r--   0        0        0     4551 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/ddpg.py
--rw-r--r--   0        0        0     4446 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/mpo.py
--rw-r--r--   0        0        0     2608 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/ppo.py
--rw-r--r--   0        0        0     2102 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/sac.py
--rw-r--r--   0        0        0     2315 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/td3.py
--rw-r--r--   0        0        0     4077 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/agents/trpo.py
--rw-r--r--   0        0        0      817 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/__init__.py
--rw-r--r--   0        0        0     5824 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/actor_critics.py
--rw-r--r--   0        0        0     4874 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/actors.py
--rw-r--r--   0        0        0     3177 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/critics.py
--rw-r--r--   0        0        0     1084 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/encoders.py
--rw-r--r--   0        0        0      791 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/models/utils.py
--rw-r--r--   0        0        0       88 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/normalizers/__init__.py
--rw-r--r--   0        0        0     2615 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1429 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/normalizers/returns.py
--rw-r--r--   0        0        0     1156 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/updaters/__init__.py
--rw-r--r--   0        0        0    20504 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/updaters/actors.py
--rw-r--r--   0        0        0    11054 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/updaters/critics.py
--rw-r--r--   0        0        0     4317 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/updaters/optimizers.py
--rw-r--r--   0        0        0      156 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/torch/updaters/utils.py
--rw-r--r--   0        0        0     5722 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/train.py
--rw-r--r--   0        0        0      213 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/utils/__init__.py
--rw-r--r--   0        0        0      822 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/utils/csv_utils.py
--rw-r--r--   0        0        0     8867 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/utils/logger.py
--rw-r--r--   0        0        0     5477 2023-04-27 12:08:50.588729 deprl-0.1.8/deprl/vendor/tonic/utils/trainer.py
--rw-r--r--   0        0        0     1227 2023-07-17 22:25:45.103654 deprl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 deprl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-02 09:47:22.460278 deprl-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8525 2023-08-03 14:28:25.285964 deprl-0.2.0/README.md
+-rw-r--r--   0        0        0      563 2023-08-03 09:45:29.163679 deprl-0.2.0/deprl/__init__.py
+-rw-r--r--   0        0        0     5872 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/custom_agents.py
+-rw-r--r--   0        0        0     8958 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/custom_distributed.py
+-rw-r--r--   0        0        0     3639 2023-08-03 08:26:00.182582 deprl-0.2.0/deprl/custom_mpo_torch.py
+-rw-r--r--   0        0        0     3541 2023-08-03 09:39:15.940090 deprl-0.2.0/deprl/custom_test_environment.py
+-rw-r--r--   0        0        0     1244 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/custom_torso.py
+-rw-r--r--   0        0        0     5910 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/custom_trainer.py
+-rw-r--r--   0        0        0     7576 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/dep_controller.py
+-rw-r--r--   0        0        0      596 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/env_wrappers/__init__.py
+-rw-r--r--   0        0        0     1466 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/env_wrappers/dm_wrapper.py
+-rw-r--r--   0        0        0     1626 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/env_wrappers/gym_wrapper.py
+-rw-r--r--   0        0        0     3263 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/env_wrappers/wrappers.py
+-rw-r--r--   0        0        0     2175 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/log.py
+-rw-r--r--   0        0        0     7722 2023-08-03 13:49:51.878318 deprl-0.2.0/deprl/main.py
+-rw-r--r--   0        0        0      704 2023-08-03 09:39:15.940090 deprl-0.2.0/deprl/param_files/default_agents.json
+-rw-r--r--   0        0        0     9870 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/play.py
+-rw-r--r--   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/plot.py
+-rw-r--r--   0        0        0      166 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/utils/__init__.py
+-rw-r--r--   0        0        0     6166 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/utils/utils.py
+-rw-r--r--   0        0        0       39 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/.gitignore
+-rw-r--r--   0        0        0     1110 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/LICENSE
+-rw-r--r--   0        0        0      207 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/agents/__init__.py
+-rw-r--r--   0        0        0     1255 2023-07-27 09:20:08.926773 deprl-0.2.0/deprl/vendor/tonic/agents/agent.py
+-rw-r--r--   0        0        0     3954 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/agents/basic.py
+-rw-r--r--   0        0        0      293 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/environments/__init__.py
+-rw-r--r--   0        0        0     5779 2023-08-03 14:28:25.285964 deprl-0.2.0/deprl/vendor/tonic/environments/builders.py
+-rw-r--r--   0        0        0     6612 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/environments/distributed.py
+-rw-r--r--   0        0        0     1914 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/environments/wrappers.py
+-rw-r--r--   0        0        0      175 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/explorations/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/explorations/noisy.py
+-rw-r--r--   0        0        0     8754 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/play.py
+-rw-r--r--   0        0        0    18151 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/plot.py
+-rw-r--r--   0        0        0      167 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/replays/__init__.py
+-rw-r--r--   0        0        0     3636 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/replays/buffers.py
+-rw-r--r--   0        0        0     2815 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/replays/segments.py
+-rw-r--r--   0        0        0      821 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/replays/utils.py
+-rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/__init__.py
+-rw-r--r--   0        0        0     4630 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/a2c.py
+-rw-r--r--   0        0        0      519 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/agent.py
+-rw-r--r--   0        0        0     1456 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/d4pg.py
+-rw-r--r--   0        0        0     4327 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/ddpg.py
+-rw-r--r--   0        0        0     4089 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/mpo.py
+-rw-r--r--   0        0        0     2452 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/ppo.py
+-rw-r--r--   0        0        0     1868 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/sac.py
+-rw-r--r--   0        0        0     2181 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/td3.py
+-rw-r--r--   0        0        0     1448 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/td4.py
+-rw-r--r--   0        0        0     3754 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/trpo.py
+-rw-r--r--   0        0        0      819 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     6247 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/actor_critics.py
+-rw-r--r--   0        0        0     4849 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/actors.py
+-rw-r--r--   0        0        0     3046 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/critics.py
+-rw-r--r--   0        0        0      734 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/encoders.py
+-rw-r--r--   0        0        0      627 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/utils.py
+-rw-r--r--   0        0        0       88 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
+-rw-r--r--   0        0        0     2442 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1339 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/normalizers/returns.py
+-rw-r--r--   0        0        0     1260 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/__init__.py
+-rw-r--r--   0        0        0    19301 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/actors.py
+-rw-r--r--   0        0        0    13820 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/critics.py
+-rw-r--r--   0        0        0     4232 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
+-rw-r--r--   0        0        0      193 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/utils.py
+-rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/__init__.py
+-rw-r--r--   0        0        0     5287 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/a2c.py
+-rw-r--r--   0        0        0     1562 2023-07-27 09:20:08.926773 deprl-0.2.0/deprl/vendor/tonic/torch/agents/agent.py
+-rw-r--r--   0        0        0     1522 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/d4pg.py
+-rw-r--r--   0        0        0     4551 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/ddpg.py
+-rw-r--r--   0        0        0     4446 2023-05-17 09:04:59.808056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/mpo.py
+-rw-r--r--   0        0        0     2608 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/ppo.py
+-rw-r--r--   0        0        0     2102 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/sac.py
+-rw-r--r--   0        0        0     2315 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/td3.py
+-rw-r--r--   0        0        0     4077 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/agents/trpo.py
+-rw-r--r--   0        0        0      817 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/__init__.py
+-rw-r--r--   0        0        0     5824 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/actor_critics.py
+-rw-r--r--   0        0        0     4874 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/actors.py
+-rw-r--r--   0        0        0     3177 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/critics.py
+-rw-r--r--   0        0        0     1084 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/encoders.py
+-rw-r--r--   0        0        0      791 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/models/utils.py
+-rw-r--r--   0        0        0       88 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/normalizers/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1429 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/normalizers/returns.py
+-rw-r--r--   0        0        0     1156 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/updaters/__init__.py
+-rw-r--r--   0        0        0    20504 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/updaters/actors.py
+-rw-r--r--   0        0        0    11054 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/updaters/critics.py
+-rw-r--r--   0        0        0     4317 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/updaters/optimizers.py
+-rw-r--r--   0        0        0      156 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/torch/updaters/utils.py
+-rw-r--r--   0        0        0     5722 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/train.py
+-rw-r--r--   0        0        0      213 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/utils/__init__.py
+-rw-r--r--   0        0        0      822 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/utils/csv_utils.py
+-rw-r--r--   0        0        0     8867 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/utils/logger.py
+-rw-r--r--   0        0        0     5477 2023-05-17 09:04:59.812056 deprl-0.2.0/deprl/vendor/tonic/utils/trainer.py
+-rw-r--r--   0        0        0     1447 2023-08-03 14:28:25.289964 deprl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9291 1970-01-01 00:00:00.000000 deprl-0.2.0/PKG-INFO
```

### Comparing `deprl-0.1.8/LICENSE` & `deprl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/README.md` & `deprl-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,22 +47,18 @@
 
 ## Installation
 
 We provide a python package for easy installation:
 ```
 pip install deprl
 ```
-### CUDA
-If you would like to use `jax` with CUDA support, which is recommended for DEP-RL training, we recommend:
-```
-pip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
-```
 
- ### CPU only
- As the current version of PyTorch (2.0.1.) defaults to CUDA, on CPU-only machines you might want to run:
+### CPU only
+ If the default PyTorch version defaults to CUDA and you generate an exception on a CPU-only machine, consider running:
+
 ```
  pip install torch --index-url https://download.pytorch.org/whl/cpu
 ```
 after installation.
 
  ### Environments
```

### Comparing `deprl-0.1.8/deprl/__init__.py` & `deprl-0.2.0/deprl/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/custom_agents.py` & `deprl-0.2.0/deprl/custom_agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,24 @@
     1: InitExploreDEP -> Just DEP exploration to initially fill the buffer.
     2: DetSwitchDEP -> Deterministic switching between DEP and RL agent.
     3: StochSwitchDEP -> Stochastic switching between DEP and RL agent.
     """
 
     class UnmixedAgent(instance.__class__):
         def step(
-            self, observations, steps, tendon_states=None, greedy_episode=None
+            self, observations, steps, muscle_states=None, greedy_episode=None
         ):
             return super().step(observations, steps)
 
-        def test_step(self, observations, steps, tendon_states=None):
+        def test_step(self, observations, steps, muscle_states=None):
             return super().test_step(observations, steps)
 
         def reset(self):
             pass
 
-        def noisy_test_step(self, observations, steps, tendon_states=None):
-            actions = self._step(observations).numpy(force=True)
-            self.last_observations = observations.copy()
-            self.last_actions = actions.copy()
-            return actions
-
     class BaseDep(instance.__class__):
         """
         Dep basis. Here, DEP exploration is only initially used to pre-fill
         the replay buffer before training.
         """
 
         def __init__(self, *args, **kwargs):
@@ -43,52 +37,46 @@
             self.expl = DEP()
 
         def initialize(self, observation_space, action_space, seed=None):
             super().initialize(observation_space, action_space, seed)
             self.expl.initialize(observation_space, action_space, seed)
 
         def step(
-            self, observations, steps, tendon_states=None, greedy_episode=None
+            self, observations, steps, muscle_states=None, greedy_episode=None
         ):
             if steps > (self.replay.steps_before_batches / 1):
                 return super().step(observations, steps)
-            actions = self.dep_step(tendon_states, steps)
+            actions = self.dep_step(muscle_states, steps)
             self.last_observations = observations.copy()
             self.last_actions = actions.copy()
 
             return actions
 
         def test_step(
-            self, observations, steps, tendon_states=None, greedy_episode=None
+            self, observations, steps, muscle_states=None, greedy_episode=None
         ):
             return super().test_step(observations, steps)
 
         def update(self, *args, **kwargs):
             super().update(*args, **kwargs)
 
         def reset(self):
             pass
 
-        def dep_step(self, tendon_states, steps):
-            return self.expl.step(tendon_states, steps)
-
-        def noisy_test_step(self, observations, steps, tendon_states=None):
-            actions = self._step(observations).numpy(force=True)
-            self.last_observations = observations.copy()
-            self.last_actions = actions.copy()
-            return actions
+        def dep_step(self, muscle_states, steps):
+            return self.expl.step(muscle_states, steps)
 
     class DetSwitchDep(BaseDep):
         def __init__(self, *args, **kwargs):
             self.switch = 0
             self.since_switch = 1
             return super().__init__(*args, **kwargs)
 
         def step(
-            self, observations, steps, tendon_states=None, greedy_episode=None
+            self, observations, steps, muscle_states=None, greedy_episode=None
         ):
             if steps > (self.replay.steps_before_batches / 1):
                 if (
                     self.switch
                     and not self.since_switch % self.expl.intervention_length
                 ):
                     self.switch = 0
@@ -97,17 +85,17 @@
                     not self.switch
                     and not self.since_switch % self.expl.rl_length
                 ):
                     self.switch = 1
                     self.since_switch = 1
                 self.since_switch += 1
                 if not self.switch:
-                    self.dep_step(tendon_states, steps)
+                    self.dep_step(muscle_states, steps)
                     return super().step(observations, steps)
-            actions = self.dep_step(tendon_states, steps)
+            actions = self.dep_step(muscle_states, steps)
 
             self.last_observations = observations.copy()
             self.last_actions = actions.copy()
             return actions
 
         def update(self, *args, **kwargs):
             super().update(*args, **kwargs)
@@ -115,55 +103,54 @@
     class StochSwitchDep(DetSwitchDep):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             # want policy to start first
             self.since_switch = 500
 
         def step(
-            self, observations, steps, tendon_states=None, greedy_episode=False
+            self, observations, steps, muscle_states=None, greedy_episode=False
         ):
             if steps > (self.replay.steps_before_batches / 1):
                 if greedy_episode:
                     return super(DetSwitchDep, self).step(
-                        observations, steps, tendon_states
+                        observations, steps, muscle_states
                     )
                 if self.since_switch > self.expl.intervention_length:
                     # important for Dep to keep learning
-                    self.dep_step(tendon_states, steps)
+                    self.dep_step(muscle_states, steps)
                     if np.random.uniform() < self.expl.intervention_proba:
                         self.since_switch = 0
                     self.since_switch += 1
                     return super(DetSwitchDep, self).step(
-                        observations, steps, tendon_states
+                        observations, steps, muscle_states
                     )
-            actions = self.dep_step(tendon_states, steps)
+            actions = self.dep_step(muscle_states, steps)
             self.last_observations = observations.copy()
             self.last_actions = actions.copy()
             self.since_switch += 1
             return actions
 
     class PureDep(BaseDep):
         def step(
-            self, observations, steps, tendon_states=None, greedy_episode=False
+            self, observations, steps, muscle_states=None, greedy_episode=False
         ):
-            if np.any(np.isnan(tendon_states)):
+            if np.any(np.isnan(muscle_states)):
                 print("tendon nan!")
-            return self.dep_step(tendon_states, steps)
+            return self.dep_step(muscle_states, steps)
 
         def update(self, *args, **kwargs):
             pass
 
         def test_update(self, *args, **kwargs):
             pass
 
         def test_step(
-            self, observations, steps, tendon_states=None, greedy_episode=False
+            self, observations, steps, muscle_states=None, greedy_episode=False
         ):
-            # return self.dep_step(tendon_states, steps)[0, :]
-            return self.dep_step(tendon_states, steps)
+            return self.dep_step(muscle_states, steps)
 
     if mix == 1:
         logger.log("Initial exploration DEP")
         return BaseDep
     elif mix == 2:
         logger.log("Deterministic Switch-DEP.")
         return DetSwitchDep
```

### Comparing `deprl-0.1.8/deprl/custom_distributed.py` & `deprl-0.2.0/deprl/custom_distributed.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,57 +33,57 @@
     def initialize(self, seed):
         for i, environment in enumerate(self.environments):
             environment.seed(seed + i)
 
     def start(self):
         """Used once to get the initial observations."""
         observations = [env.reset() for env in self.environments]
-        tendon_states = [env.tendon_states for env in self.environments]
+        muscle_states = [env.muscle_states for env in self.environments]
         self.lengths = np.zeros(len(self.environments), int)
         return np.array(observations, np.float32), np.array(
-            tendon_states, np.float32
+            muscle_states, np.float32
         )
 
     def step(self, actions):
         next_observations = []  # Observations for the transitions.
         rewards = []
         resets = []
         terminations = []
         observations = []  # Observations for the actions selection.
-        tendon_states = []
+        muscle_states = []
 
         for i in range(len(self.environments)):
             ob, rew, term, env_info = self.environments[i].step(actions[i])
-            muscle = self.environments[i].tendon_states
+            muscle = self.environments[i].muscle_states
             self.lengths[i] += 1
             # Timeouts trigger resets but are not true terminations.
             reset = term or self.lengths[i] == self._max_episode_steps
             next_observations.append(ob)
             rewards.append(rew)
             resets.append(reset)
 
             terminations.append(term)
 
             if reset:
                 ob = self.environments[i].reset()
-                muscle = self.environments[i].tendon_states
+                muscle = self.environments[i].muscle_states
                 self.lengths[i] = 0
 
             observations.append(ob)
-            tendon_states.append(muscle)
+            muscle_states.append(muscle)
 
         observations = np.array(observations, np.float32)
-        tendon_states = np.array(tendon_states, np.float32)
+        muscle_states = np.array(muscle_states, np.float32)
         infos = dict(
             observations=np.array(next_observations, np.float32),
             rewards=np.array(rewards, np.float32),
             resets=np.array(resets, bool),
             terminations=np.array(terminations, bool),
         )
-        return observations, tendon_states, infos
+        return observations, muscle_states, infos
 
     def render(self, mode="human", *args, **kwargs):
         outs = []
         for env in self.environments:
             out = env.render(mode=mode, *args, **kwargs)
             outs.append(out)
         if mode != "human":
@@ -159,23 +159,23 @@
             process.start()
 
     def start(self):
         """Used once to get the initial observations."""
         assert not self.started
         self.started = True
         observations_list = [None for _ in range(self.worker_groups)]
-        tendon_states_list = [None for _ in range(self.worker_groups)]
+        muscle_states_list = [None for _ in range(self.worker_groups)]
 
         for _ in range(self.worker_groups):
-            index, (observations, tendon_states) = self.output_queue.get()
+            index, (observations, muscle_states) = self.output_queue.get()
             observations_list[index] = observations
-            tendon_states_list[index] = tendon_states
+            muscle_states_list[index] = muscle_states
 
         self.observations_list = np.array(observations_list)
-        self.tendon_states_list = np.array(tendon_states_list)
+        self.muscle_states_list = np.array(muscle_states_list)
         self.next_observations_list = np.zeros_like(self.observations_list)
         self.rewards_list = np.zeros(
             (self.worker_groups, self.workers_per_group), np.float32
         )
         self.resets_list = np.zeros(
             (self.worker_groups, self.workers_per_group), bool
         )
@@ -183,44 +183,44 @@
             (self.worker_groups, self.workers_per_group), bool
         )
         self.terminations_list = np.zeros(
             (self.worker_groups, self.workers_per_group), bool
         )
 
         return np.concatenate(self.observations_list), np.concatenate(
-            self.tendon_states_list
+            self.muscle_states_list
         )
 
     def step(self, actions):
         actions_list = np.split(actions, self.worker_groups)
         for actions, pipe in zip(actions_list, self.action_pipes):
             pipe.send(actions)
 
         for _ in range(self.worker_groups):
             index, (
                 observations,
-                tendon_state,
+                muscle_states,
                 infos,
             ) = self.output_queue.get()
             self.observations_list[index] = observations
             self.next_observations_list[index] = infos["observations"]
             self.rewards_list[index] = infos["rewards"]
             self.resets_list[index] = infos["resets"]
             self.terminations_list[index] = infos["terminations"]
-            self.tendon_states_list[index] = tendon_state
+            self.muscle_states_list[index] = muscle_states
 
         observations = np.concatenate(self.observations_list)
-        tendon_states = np.concatenate(self.tendon_states_list)
+        muscle_states = np.concatenate(self.muscle_states_list)
         infos = dict(
             observations=np.concatenate(self.next_observations_list),
             rewards=np.concatenate(self.rewards_list),
             resets=np.concatenate(self.resets_list),
             terminations=np.concatenate(self.terminations_list),
         )
-        return observations, tendon_states, infos
+        return observations, muscle_states, infos
 
 
 def distribute(
     build_dict, worker_groups=1, workers_per_group=1, env_args=None
 ):
     """Distributes workers over parallel and sequential groups."""
```

### Comparing `deprl-0.1.8/deprl/custom_mpo_torch.py` & `deprl-0.2.0/deprl/custom_mpo_torch.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/custom_test_environment.py` & `deprl-0.2.0/deprl/custom_test_environment.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/custom_torso.py` & `deprl-0.2.0/deprl/custom_torso.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/custom_trainer.py` & `deprl-0.2.0/deprl/custom_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def run(self, params, steps=0, epochs=0, episodes=0):
         """Runs the main training loop."""
 
         start_time = last_epoch_time = time.time()
 
         # Start the environments.
-        observations, tendon_states = self.environment.start()
+        observations, muscle_states = self.environment.start()
 
         num_workers = len(observations)
         scores = np.zeros(num_workers)
         lengths = np.zeros(num_workers, int)
         self.steps, epoch_steps = steps, 0
         steps_since_save = 0
 
@@ -55,22 +55,22 @@
                 greedy_episode = (
                     not episodes % self.agent.expl.test_episode_every
                 )
             else:
                 greedy_episode = None
             assert not np.isnan(observations.sum())
             actions = self.agent.step(
-                observations, self.steps, tendon_states, greedy_episode
+                observations, self.steps, muscle_states, greedy_episode
             )
             assert not np.isnan(actions.sum())
             # raise Exception(f'{type(self.environment.environments[0])}')
             logger.store("train/action", actions, stats=True)
 
             # Take a step in the environments.
-            observations, tendon_states, info = self.environment.step(actions)
+            observations, muscle_states, info = self.environment.step(actions)
             if "env_infos" in info:
                 info.pop("env_infos")
 
             self.agent.update(**info, steps=self.steps)
 
             scores += info["rewards"]
             lengths += 1
```

### Comparing `deprl-0.1.8/deprl/dep_controller.py` & `deprl-0.2.0/deprl/dep_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 import os
 from collections import deque
 
 import gym
-import jax.numpy as jnp
-import numpy as onp
+import torch
 
-# jax.config.update('jax_platform_name', 'cpu')
+torch.set_default_dtype(torch.float32)
 
 
 class DEP:
     """
     DEP Implementation from Der et al.(2015).
     Jax is used instead of numpy to speed up computation, GPU strongly
     recommended.
@@ -39,31 +38,32 @@
         action_space = gym.spaces.Box(
             low=-1, high=1, shape=(action_space.shape)
         )
         self.num_sensors = action_space.shape[0]
         self.num_motors = action_space.shape[0]
         self.n_env = 1
 
-        self.act_scale = self.act_high = action_space.high
+        self.act_scale = self.act_high = torch.tensor(action_space.high)
 
         self.action_space = action_space
         self.obs_spec = observation_space.shape
         self.set_params(self.params)
 
     def step(self, observations, steps=None):
         """
         Main step function. Takes in an observation consisting of
         muscle_lengths + alpha * muscle_forces. Alpha can also be 0.
         """
+        observations = torch.tensor(observations, dtype=torch.float32)
         if observations.shape != self.obs_spec:
             self.obs_spec = observations.shape
             self._reset(observations.shape)
         if len(observations.shape) == 1:
-            observations = observations[jnp.newaxis, :]
-        return onp.array(self._get_action(observations)).copy()
+            observations = observations[None, :]
+        return self._get_action(observations).numpy(force=True)
 
     def set_params(self, param_dict):
         for k, v in param_dict.items():
             setattr(self, k, v)
         self._reset()
 
     def _reset(self, obs_shape=None):
@@ -75,65 +75,65 @@
         it is assumed that num_motors = num_sensors, where the sensors
         directly mirror an actuator state. E.g. joint angle or muscle
         length.
         """
         if obs_shape:
             self.n_env = [obs_shape[0] if len(obs_shape) > 1 else 1][0]
         # Identity model matrix
-        self.M = jnp.broadcast_to(
-            -jnp.eye(self.num_motors, self.num_sensors),
+        self.M = torch.broadcast_to(
+            -torch.eye(self.num_motors, self.num_sensors),
             (self.n_env, self.num_motors, self.num_sensors),
         )
         # Unnormalized controller matrix
-        self.C = jnp.zeros((self.n_env, self.num_motors, self.num_sensors))
+        self.C = torch.zeros((self.n_env, self.num_motors, self.num_sensors))
         # Normalized controller matrix
-        self.C_norm = jnp.zeros(
+        self.C_norm = torch.zeros(
             (self.n_env, self.num_motors, self.num_sensors)
         )
         # Controller biases
-        self.Cb = jnp.zeros((self.n_env, self.num_motors))
+        self.Cb = torch.zeros((self.n_env, self.num_motors))
         # Filtered observation
-        self.obs_smoothed = jnp.zeros((self.n_env, self.num_sensors))
+        self.obs_smoothed = torch.zeros((self.n_env, self.num_sensors))
         # Observation and action buffer
         self.buffer = deque(maxlen=self.buffer_size)
         # smoothed_observation
-        self.obs_smoothed = jnp.zeros(self.obs_spec)
+        self.obs_smoothed = torch.zeros(self.obs_spec)
         # time
         self.t = 0
 
     def _get_action(self, obs):
         """
         Performs rolling average smoothing on the observation and
         computes a DEP learning step.
         """
         # smoothing
         if self.s4avg > 1 and self.t > 0:
             self.obs_smoothed += (obs - self.obs_smoothed) / self.s4avg
         else:
             self.obs_smoothed = obs
 
-        self.buffer.append([self.obs_smoothed.copy(), None])
+        self.buffer.append([self.obs_smoothed.detach().clone(), None])
         # learning step
         if self.with_learning and len(self.buffer) > (2 + self.time_dist):
             self._learn_controller()
         # new action
         y = self._compute_action()
-        self.buffer[-1][1] = y.copy()
+        self.buffer[-1][1] = y.detach().clone()
         self.t += 1
         return y
 
     def _q_norm(self, q):
         """
         Normalization function for intermediate action
         obtained by applying the controller matrix to the
         input q = C @ x.
         """
         reg = 10.0 ** (-self.regularization)
         if self.q_norm_selector == "l2":
-            q_norm = 1.0 / (jnp.linalg.norm(q, axis=-1) + reg)
+            q_norm = 1.0 / (torch.linalg.norm(q, axis=-1) + reg)
         elif self.q_norm_selector == "max":
             q_norm = 1.0 / (max(abs(q), axis=-1) + reg)
         elif self.q_norm_selector == "none":
             q_norm = 1.0
         else:
             raise NotImplementedError(
                 "q normalization {self.q_norm_selector} not implemented."
@@ -143,74 +143,79 @@
 
     def _compute_action(
         self,
     ):
         """
         Compute a DEP action from the current C matrix
         """
-        q = jnp.einsum("ijk, ik->ij", self.C_norm, self.obs_smoothed)
+        q = torch.einsum("ijk, ik->ij", self.C_norm, self.obs_smoothed)
 
-        q = jnp.einsum(
+        q = torch.einsum(
             "ij, i->ij",
             q,
             self._q_norm(q),
         )
-        y = jnp.maximum(-1, jnp.minimum(1, jnp.tanh(q * self.kappa + self.Cb)))
-        y = jnp.einsum("ij, j->ij", y, self.act_scale)
+        y = torch.maximum(
+            torch.tensor([-1.0]),
+            torch.minimum(
+                torch.tensor([1.0]), torch.tanh(q * self.kappa + self.Cb)
+            ),
+        )
+        y = torch.einsum("ij, j->ij", y, self.act_scale)
         return y
 
     def _learn_controller(self):
         """
         Update DEP by one learning step.
         """
         self.C = self._compute_C()
         # linear response in motor space (action -> action)
-        R = jnp.einsum("ijk, imk->ijm", self.C, self.M)
+        R = torch.einsum("ijk, imk->ijm", self.C, self.M)
         reg = 10.0 ** (-self.regularization)
         # controller normalization c.f. Der et al (2015).
         if self.normalization == "independent":
-            factor = self.kappa / (jnp.linalg.norm(R, axis=-1) + reg)
-            self.C_norm = jnp.einsum("ijk,ik->ijk", self.C, factor)
+            factor = self.kappa / (torch.linalg.norm(R, axis=-1) + reg)
+            self.C_norm = torch.einsum("ijk,ik->ijk", self.C, factor)
         elif self.normalization == "none":
             self.C_norm = self.C
         elif self.normalization == "global":
-            norm = jnp.linalg.norm(R)
+            norm = torch.linalg.norm(R)
             self.C_norm = self.C * self.kappa / (norm + reg)
         else:
             raise NotImplementedError(
                 f"Controller matrix normalization {self.normalization} not implemented."
             )
 
         if self.bias_rate >= 0:
             yy = self.buffer[-2][1]
             self.Cb -= (
-                jnp.clip(yy * self.bias_rate, -0.05, 0.05) + self.Cb * 0.001
+                torch.clip(yy * self.bias_rate, -0.05, 0.05) + self.Cb * 0.001
             )
         else:
             self.Cb *= 0
 
     def _compute_C(self):
         """
         Recompute the controller matrix C from the
         buffer of recent transitions. This is similar
         to the rolling average shown in the publication, but without
         recency weighting.
         """
-        C = jnp.zeros_like(self.C)
+        C = torch.zeros_like(self.C)
         for s in range(2, min(self.t - self.time_dist, self.tau)):
             x = self.buffer[-s][0][:, : self.num_sensors]
             xx = self.buffer[-s - 1][0][:, : self.num_sensors]
             xx_t = (
                 x
                 if self.time_dist == 0
                 else self.buffer[-s - self.time_dist][0][:, : self.num_sensors]
             )
             xxx_t = self.buffer[-s - 1 - self.time_dist][0][
                 :, : self.num_sensors
             ]
 
             chi = x - xx
             v = xx_t - xxx_t
-            mu = jnp.einsum("ijk, ik->ij", self.M, chi)
+            mu = torch.einsum("ijk, ik->ij", self.M, chi)
 
-            C += jnp.einsum("ij, ik->ijk", mu, v)
+            C += torch.einsum("ij, ik->ijk", mu, v)
         return C
```

### Comparing `deprl-0.1.8/deprl/log.py` & `deprl-0.2.0/deprl/log.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import os
 import time
 
+import wandb
 import yaml
 
-import wandb
 from deprl.vendor.tonic import utils
 
 
 class WandbProcessor:
     def __init__(self, path):
         self._path = path
         self._current_line_number = 0
```

### Comparing `deprl-0.1.8/deprl/main.py` & `deprl-0.2.0/deprl/main.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/param_files/default_agents.json` & `deprl-0.2.0/deprl/param_files/default_agents.json`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/play.py` & `deprl-0.2.0/deprl/vendor/tonic/play.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 """Script used to play with trained agents."""
 
 import argparse
 import os
 
 import numpy as np
+import tonic  # noqa
 import yaml
 
-from deprl import env_wrappers, mujoco_render
-
-from .vendor.tonic import logger
-
 
 def play_gym(agent, environment):
     """Launches an agent in a Gym-based environment."""
-    environment = env_wrappers.apply_wrapper(environment)
-    observations = environment.reset()
-    tendon_states = environment.tendon_states
+
+    environment = tonic.environments.distribute(lambda: environment)
+
+    observations = environment.start()
+    environment.render()
 
     score = 0
     length = 0
     min_reward = float("inf")
     max_reward = -float("inf")
     global_min_reward = float("inf")
     global_max_reward = -float("inf")
     steps = 0
     episodes = 0
 
     while True:
-        actions = agent.test_step(
-            observations, tendon_states=tendon_states, steps=1e6
-        )
-        # actions = agent.noisy_test_step(
-        #     observations, tendon_states=tendon_states, steps=1e6
-        # )
-        if len(actions.shape) > 1:
-            actions = actions[0, :]
-        observations, reward, done, info = environment.step(actions)
-        tendon_states = environment.tendon_states
-        mujoco_render(environment)
+        actions = agent.test_step(observations, steps)
+        observations, infos = environment.step(actions)
+        agent.test_update(**infos, steps=steps)
+        environment.render()
 
         steps += 1
+        reward = infos["rewards"][0]
         score += reward
         min_reward = min(min_reward, reward)
         max_reward = max(max_reward, reward)
         global_min_reward = min(global_min_reward, reward)
         global_max_reward = max(global_max_reward, reward)
         length += 1
 
-        if done or length >= environment.max_episode_steps:
+        if infos["resets"][0]:
+            term = infos["terminations"][0]
             episodes += 1
 
             print()
             print(f"Episodes: {episodes:,}")
             print(f"Score: {score:,.3f}")
             print(f"Length: {length:,}")
-            print(f"Terminal: {done:}")
+            print(f"Terminal: {term:}")
             print(f"Min reward: {min_reward:,.3f}")
             print(f"Max reward: {max_reward:,.3f}")
             print(f"Global min reward: {min_reward:,.3f}")
             print(f"Global max reward: {max_reward:,.3f}")
-            environment.reset()
 
             score = 0
             length = 0
             min_reward = float("inf")
             max_reward = -float("inf")
 
 
@@ -83,15 +76,14 @@
             self.infos = None
             self.steps = 0
             self.episodes = 0
             self.min_reward = float("inf")
             self.max_reward = -float("inf")
             self.global_min_reward = float("inf")
             self.global_max_reward = -float("inf")
-            self.max_vel = 0
 
         def reset(self):
             """Mimics a dm_control reset for the viewer."""
 
             self.observations = self.environment.reset()[None]
 
             self.score = 0
@@ -134,54 +126,45 @@
                 rewards=np.array([rew]),
                 resets=np.array([done]),
                 terminations=np.array([term]),
             )
 
             return self.unwrapped.last_time_step
 
-        @property
-        def tendon_states(self):
-            return self.environment.tendon_states
-
     # Wrap the environment for the viewer.
-    environment = env_wrappers.apply_wrapper(environment)
     environment = Wrapper(environment)
 
     def policy(timestep):
         """Mimics a dm_control policy for the viewer."""
+
         if environment.infos is not None:
             agent.test_update(**environment.infos, steps=environment.steps)
             environment.steps += 1
-        tendon_states = environment.tendon_states
-        return agent.test_step(
-            environment.observations,
-            tendon_states=tendon_states,
-            steps=environment.steps,
-        )
+        return agent.test_step(environment.observations, environment.steps)
 
     # Launch the viewer with the wrapped environment and policy.
     viewer.launch(environment, policy)
 
 
 def play(path, checkpoint, seed, header, agent, environment):
     """Reloads an agent and an environment from a previous experiment."""
 
     checkpoint_path = None
 
     if path:
-        logger.log(f"Loading experiment from {path}")
+        tonic.logger.log(f"Loading experiment from {path}")
 
         # Use no checkpoint, the agent is freshly created.
         if checkpoint == "none" or agent is not None:
-            logger.log("Not loading any weights")
+            tonic.logger.log("Not loading any weights")
 
         else:
             checkpoint_path = os.path.join(path, "checkpoints")
             if not os.path.isdir(checkpoint_path):
-                logger.error(f"{checkpoint_path} is not a directory")
+                tonic.logger.error(f"{checkpoint_path} is not a directory")
                 checkpoint_path = None
 
             # List all the checkpoints.
             checkpoint_ids = []
             for file in os.listdir(checkpoint_path):
                 if file[:5] == "step_":
                     checkpoint_id = file.split(".")[0]
@@ -199,22 +182,22 @@
                 else:
                     checkpoint_id = int(checkpoint)
                     if checkpoint_id in checkpoint_ids:
                         checkpoint_path = os.path.join(
                             checkpoint_path, f"step_{checkpoint_id}"
                         )
                     else:
-                        logger.error(
+                        tonic.logger.error(
                             f"Checkpoint {checkpoint_id} "
                             f"not found in {checkpoint_path}"
                         )
                         checkpoint_path = None
 
             else:
-                logger.error(f"No checkpoint found in {checkpoint_path}")
+                tonic.logger.error(f"No checkpoint found in {checkpoint_path}")
                 checkpoint_path = None
 
         # Load the experiment configuration.
         arguments_path = os.path.join(path, "config.yaml")
         with open(arguments_path, "r") as config_file:
             config = yaml.load(config_file, Loader=yaml.FullLoader)
         config = argparse.Namespace(**config)
@@ -233,31 +216,37 @@
         raise ValueError("No agent specified.")
     agent = eval(agent)
 
     # Build the environment.
     environment = eval(environment)
     environment.seed(seed)
 
-    # Adapt mpo specific settings
-    if "config" in locals():
-        if "mpo_args" in config:
-            agent.set_params(**config.mpo_args)
     # Initialize the agent.
     agent.initialize(
         observation_space=environment.observation_space,
         action_space=environment.action_space,
         seed=seed,
     )
 
     # Load the weights of the agent form a checkpoint.
     if checkpoint_path:
         agent.load(checkpoint_path)
-    if "ontrol" in type(environment).__name__:
+
+    # Play with the agent in the environment.
+    if isinstance(environment, tonic.environments.wrappers.ActionRescaler):
+        environment_type = environment.env.__class__.__name__
+    else:
+        environment_type = environment.__class__.__name__
+
+    if environment_type == "ControlSuiteEnvironment":
         play_control_suite(agent, environment)
-    play_gym(agent, environment)
+    else:
+        if "Bullet" in environment_type:
+            environment.render()
+        play_gym(agent, environment)
 
 
 if __name__ == "__main__":
     # Argument parsing.
     parser = argparse.ArgumentParser()
     parser.add_argument("--path")
     parser.add_argument("--checkpoint", default="last")
```

### Comparing `deprl-0.1.8/deprl/play_plot.py` & `deprl-0.2.0/deprl/play.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,86 +2,55 @@
 
 import argparse
 import os
 
 import numpy as np
 import yaml
 
-from deprl import env_wrappers
+from deprl import env_wrappers, mujoco_render
 
 from .vendor.tonic import logger
-import matplotlib.pyplot as plt
-from deprl.utils import ScoreKeeper
 
 
-def play_gym(agent, environment):
+def play_gym(agent, environment, noisy, no_render, num_episodes):
     """Launches an agent in a Gym-based environment."""
-    environment = env_wrappers.apply_wrapper(environment)
     observations = environment.reset()
-    tendon_states = environment.tendon_states
-    environment.render()
-    scorekeeper = ScoreKeeper()
+    muscle_states = environment.muscle_states
 
     score = 0
     length = 0
     min_reward = float("inf")
     max_reward = -float("inf")
     global_min_reward = float("inf")
     global_max_reward = -float("inf")
     steps = 0
     episodes = 0
 
-    rews = {k:[] for k in environment.rwd_dict.keys()}
     while True:
-        if hasattr(environment, "rwd_dict"):
-            info = {
-                'hip_left': environment.sim.data.get_joint_qpos('hip_flexion_l'),
-                'hip_right': environment.sim.data.get_joint_qpos('hip_flexion_r'),
-                'knee_left': environment.sim.data.get_joint_qpos('knee_angle_l'),
-                'knee_right': environment.sim.data.get_joint_qpos('knee_angle_r'),
-                'ankle_left': environment.sim.data.get_joint_qpos('ankle_angle_l'),
-                'ankle_right': environment.sim.data.get_joint_qpos('ankle_angle_r'),
-                'knee_sensor_left': environment.sim.data.get_sensor('knee_l_limfrc'),
-                'knee_sensor_right': environment.sim.data.get_sensor('knee_r_limfrc'),
-                'ankle_sensor_left': environment.sim.data.get_sensor('ankle_l_limfrc'),
-                'ankle_sensor_right': environment.sim.data.get_sensor('ankle_r_limfrc'),
-                'hip_sensor_flexion_left': environment.sim.data.get_sensor('hip_flexion_l_limfrc'),
-                'hip_sensor_flexion_right': environment.sim.data.get_sensor('hip_flexion_r_limfrc'),
-                'hip_sensor_adduction_left': environment.sim.data.get_sensor('hip_adduction_l_limfrc'),
-                'hip_sensor_adduction_right': environment.sim.data.get_sensor('hip_adduction_r_limfrc'),
-                'hip_sensor_rotation_left': environment.sim.data.get_sensor('hip_rotation_l_limfrc'),
-                'hip_sensor_rotation_right': environment.sim.data.get_sensor('hip_rotation_r_limfrc'),
-                }
-            scorekeeper.store(info)
-            for k, v in environment.rwd_dict.items():
-                rews[k].append(v)
-
-
-        # from pudb import set_trace; set_trace()
-        # actions = agent.test_step(
-        #     observations, tendon_states=tendon_states, steps=1e6
-        # )
-        actions = agent.noisy_step(
-            observations, tendon_states=tendon_states, steps=1e6
-        )
-        actions = np.clip(actions, -100, 0.5)
+        if not noisy:
+            actions = agent.test_step(
+                observations, muscle_states=muscle_states, steps=1e6
+            )
+        else:
+            actions = agent.noisy_test_step(
+                observations, muscle_states=muscle_states, steps=1e6
+            )
         if len(actions.shape) > 1:
             actions = actions[0, :]
         observations, reward, done, info = environment.step(actions)
-        tendon_states = environment.tendon_states
-        environment.render()
-        
+        muscle_states = environment.muscle_states
+        if not no_render:
+            mujoco_render(environment)
+
         steps += 1
         score += reward
         min_reward = min(min_reward, reward)
         max_reward = max(max_reward, reward)
         global_min_reward = min(global_min_reward, reward)
         global_max_reward = max(global_max_reward, reward)
-        # scorekeeper.adapt_plot(["knee_sensor_left", "knee_sensor_right", "ankle_sensor_left",\
-        #                        "ankle_sensor_right", "hip_sensor_flexion_left", "hip_sensor_flexion_right", "hip_sensor_adduction_left", "hip_sensor_adduction_right", "hip_sensor_rotation_left", "hip_sensor_rotation_right"])
         length += 1
 
         if done or length >= environment.max_episode_steps:
             episodes += 1
 
             print()
             print(f"Episodes: {episodes:,}")
@@ -89,25 +58,24 @@
             print(f"Length: {length:,}")
             print(f"Terminal: {done:}")
             print(f"Min reward: {min_reward:,.3f}")
             print(f"Max reward: {max_reward:,.3f}")
             print(f"Global min reward: {min_reward:,.3f}")
             print(f"Global max reward: {max_reward:,.3f}")
             environment.reset()
-            for k, v in rews.items():
-                print(f'{k=} {np.sum(v)}')
-
 
             score = 0
             length = 0
             min_reward = float("inf")
             max_reward = -float("inf")
+            if episodes >= num_episodes:
+                break
 
 
-def play_control_suite(agent, environment):
+def play_control_suite(agent, environment, num_episodes):
     """Launches an agent in a DeepMind Control Suite-based environment."""
 
     from dm_control import viewer
 
     class Wrapper:
         """Wrapper used to plug a Tonic environment in a dm_control viewer."""
 
@@ -167,45 +135,54 @@
             self.observations = ob[None]
             self.infos = dict(
                 observations=ob[None],
                 rewards=np.array([rew]),
                 resets=np.array([done]),
                 terminations=np.array([term]),
             )
-
             return self.unwrapped.last_time_step
 
         @property
-        def tendon_states(self):
-            return self.environment.tendon_states
+        def muscle_states(self):
+            return self.environment.muscle_states
 
     # Wrap the environment for the viewer.
-    environment = env_wrappers.apply_wrapper(environment)
     environment = Wrapper(environment)
 
     def policy(timestep):
         """Mimics a dm_control policy for the viewer."""
         if environment.infos is not None:
             agent.test_update(**environment.infos, steps=environment.steps)
             environment.steps += 1
-        tendon_states = environment.tendon_states
+        muscle_states = environment.muscle_states
         return agent.test_step(
             environment.observations,
-            tendon_states=tendon_states,
+            muscle_states=muscle_states,
             steps=environment.steps,
         )
 
     # Launch the viewer with the wrapped environment and policy.
     viewer.launch(environment, policy)
 
 
-def play(path, checkpoint, seed, header, agent, environment):
+def play(
+    path,
+    checkpoint,
+    seed,
+    header,
+    agent,
+    environment,
+    noisy,
+    no_render,
+    num_episodes,
+):
     """Reloads an agent and an environment from a previous experiment."""
 
     checkpoint_path = None
+    config = None
 
     if path:
         logger.log(f"Loading experiment from {path}")
 
         # Use no checkpoint, the agent is freshly created.
         if checkpoint == "none" or agent is not None:
             logger.log("Not loading any weights")
@@ -268,40 +245,50 @@
     if not agent:
         raise ValueError("No agent specified.")
     agent = eval(agent)
 
     # Build the environment.
     environment = eval(environment)
     environment.seed(seed)
+    environment = env_wrappers.apply_wrapper(environment)
+    if config and "env_args" in config:
+        environment.merge_args(config.env_args)
+        environment.apply_args()
 
     # Adapt mpo specific settings
-    if "config" in locals():
-        if "mpo_args" in config:
-            agent.set_params(**config.mpo_args)
+    if config and "mpo_args" in config:
+        agent.set_params(**config.mpo_args)
     # Initialize the agent.
     agent.initialize(
         observation_space=environment.observation_space,
         action_space=environment.action_space,
         seed=seed,
     )
 
-    # Load the weights of the agent form a checkpoint.
+    # Load the weights of the agent from a checkpoint.
     if checkpoint_path:
         agent.load(checkpoint_path)
-    if "ontrol" in type(environment).__name__:
-        play_control_suite(agent, environment)
-    import torch
-    torch.save(agent.model.actor.state_dict(), 'actor_weights.pt')
-    play_gym(agent, environment)
+
+    if "control" in str(environment).lower():
+        if no_render or num_episodes != 5:
+            logger.log(
+                "no_render and num_episodes only implemented for gym tasks"
+            )
+        play_control_suite(agent, environment, num_episodes)
+    else:
+        play_gym(agent, environment, noisy, no_render, num_episodes)
 
 
 if __name__ == "__main__":
     # Argument parsing.
     parser = argparse.ArgumentParser()
     parser.add_argument("--path")
     parser.add_argument("--checkpoint", default="last")
     parser.add_argument("--seed", type=int, default=0)
+    parser.add_argument("--num_episodes", type=int, default=5)
+    parser.add_argument("--noisy", action="store_true")
+    parser.add_argument("--no_render", action="store_true")
     parser.add_argument("--header")
     parser.add_argument("--agent")
     parser.add_argument("--environment", "--env")
     args = vars(parser.parse_args())
     play(**args)
```

### Comparing `deprl-0.1.8/deprl/utils/utils.py` & `deprl-0.2.0/deprl/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 def load_baseline(environment):
     identifier = (
         environment.env_name
         if hasattr(environment, "env_name")
         else str(environment)
     )
-    print(identifier)
     if "myoLegWalk" in identifier:
         logger.log("Load LegWalk Baseline")
         return load_baseline_myolegwalk(environment)
     if "myoChallengeChaseTagP1" in identifier:
         logger.log("Load ChaseTagP1 Baseline")
         return load_baseline_myochasetagp1(environment, noisy=True)
     if "myoChallengeRelocateP1" in identifier:
```

### Comparing `deprl-0.1.8/deprl/vendor/tonic/LICENSE` & `deprl-0.2.0/deprl/vendor/tonic/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/agents/agent.py` & `deprl-0.2.0/deprl/vendor/tonic/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/agents/basic.py` & `deprl-0.2.0/deprl/vendor/tonic/agents/basic.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/environments/builders.py` & `deprl-0.2.0/deprl/vendor/tonic/environments/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
     def _builder(name, *args, **kwargs):
         domain, task = name.split("-")
         environment = ControlSuiteEnvironment(
             domain_name=domain, task_name=task, *args, **kwargs
         )
         time_limit = int(environment.environment._step_limit)
-        environment.spec = SimpleNamespace(max_episode_steps=time_limit)
+        environment.spec = SimpleNamespace(
+            max_episode_steps=time_limit, id="ostrichrl-dmcontrol"
+        )
         return gym.wrappers.TimeLimit(environment, time_limit)
 
     return build_environment(_builder, *args, **kwargs)
 
 
 def build_environment(
     builder,
```

### Comparing `deprl-0.1.8/deprl/vendor/tonic/environments/distributed.py` & `deprl-0.2.0/deprl/vendor/tonic/environments/distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/environments/wrappers.py` & `deprl-0.2.0/deprl/vendor/tonic/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/explorations/noisy.py` & `deprl-0.2.0/deprl/vendor/tonic/explorations/noisy.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/plot.py` & `deprl-0.2.0/deprl/vendor/tonic/plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/replays/buffers.py` & `deprl-0.2.0/deprl/vendor/tonic/replays/buffers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/replays/segments.py` & `deprl-0.2.0/deprl/vendor/tonic/replays/segments.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/replays/utils.py` & `deprl-0.2.0/deprl/vendor/tonic/replays/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/a2c.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/agent.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/d4pg.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/ddpg.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/mpo.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/ppo.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/sac.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/td3.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/td4.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/td4.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/agents/trpo.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/__init__.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/actor_critics.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/actors.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/critics.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/encoders.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/models/utils.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/normalizers/returns.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/__init__.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/actors.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/critics.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/tensorflow/updaters/optimizers.py` & `deprl-0.2.0/deprl/vendor/tonic/tensorflow/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/a2c.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/agent.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,7 +39,10 @@
             logger.log(f"Loading failed, policy mismatch with checkpoint: {e}")
 
     def _load_weights(self, state_dict, full=False):
         if full:
             self.model.load_state_dict(state_dict)
         else:
             self.model.actor.load_state_dict(state_dict)
+
+    def noisy_test_step(self, observations, *args, **kwargs):
+        return self._step(observations).numpy(force=True)
```

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/d4pg.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/ddpg.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/mpo.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/ppo.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/sac.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/td3.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/agents/trpo.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/__init__.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/actor_critics.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/actors.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/critics.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/encoders.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/models/utils.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/normalizers/mean_stds.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/normalizers/returns.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/updaters/__init__.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/updaters/actors.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/updaters/critics.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/torch/updaters/optimizers.py` & `deprl-0.2.0/deprl/vendor/tonic/torch/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/train.py` & `deprl-0.2.0/deprl/vendor/tonic/train.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/utils/csv_utils.py` & `deprl-0.2.0/deprl/vendor/tonic/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/utils/logger.py` & `deprl-0.2.0/deprl/vendor/tonic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/deprl/vendor/tonic/utils/trainer.py` & `deprl-0.2.0/deprl/vendor/tonic/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.8/pyproject.toml` & `deprl-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 [tool.poetry]
 name = "deprl"
-version = "0.1.8"
+version = "0.2.0"
 description = "DEP-RL, a method for robust control of musculoskeletal systems."
 authors = ["Pierre Schumacher <pierre.schumacher@tuebingen.mpg.de>"]
 license = "MIT"
 readme = "README.md"
 
+
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.9, <=3.11.4"
 pyyaml = "^6.0"
 numpy = "^1.22.4"
 termcolor = "^2.2.0"
-jaxlib = "^0.4.7"
-jax = "^0.4.8"
 pandas = "^2.0.1"
 gdown = "^4.7.1"
-gym = "0.13.0"
-pytest = "^7.4.0"
-torch = "^2.0.1"
+# torch = {version = "^2.0.1+cpu", source = "pytorch-cpu"}
+torch = "^2.0.0"
+
 
 [tool.poetry.group.dev.dependencies]
 pudb = "*"
 pre-commit = "*"
-wandb = "^0.13.11"
 ostrichrl = {git = "https://github.com/P-Schumacher/ostrichrl.git", branch="fix/setuptools"}
 warmup = {git = "https://github.com/P-Schumacher/warmup.git"}
+gym = "0.13.0"
+wandb = "^0.15.4"
 myosuite = "^1.7.0"
+sphinx = "5.3.0"
+sphinx-rtd-theme = "^1.2.2"
+pytest = "^7.4.0"
+sphinx-copybutton = "^0.5.2"
 
 
 [tool.poetry.scripts]
 log = "deprl.log:main"
 plot = "deprl.plot:main"
 
+
+[[tool.poetry.source]]
+name = "pytorch-cpu"
+url = "https://download.pytorch.org/whl/cpu"
+priority = "explicit"
+
+
 [tool.black]
 line-length = 79
 target-version = ["py310"]
 
+
 [tool.isort]
 profile = "black"
 filter_files = "True"
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
+
 [tool.ruff]
 ignore = ["C901", "F403", "F405"]
 line-length = 120
 target-version= "py310"
 
 
 [build-system]
```

### Comparing `deprl-0.1.8/PKG-INFO` & `deprl-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: deprl
-Version: 0.1.8
+Version: 0.2.0
 Summary: DEP-RL, a method for robust control of musculoskeletal systems.
 License: MIT
 Author: Pierre Schumacher
 Author-email: pierre.schumacher@tuebingen.mpg.de
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<=3.11.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gdown (>=4.7.1,<5.0.0)
-Requires-Dist: gym (==0.13.0)
-Requires-Dist: jax (>=0.4.8,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # DEP-RL: Embodied Exploration for Reinforcement Learning in Overactuated and Musculoskeletal Systems
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![PyPI](https://img.shields.io/pypi/v/deprl)](https://pypi.org/project/deprl/)
  [![Downloads](https://pepy.tech/badge/deprl)](https://pepy.tech/project/deprl)
 
@@ -72,22 +68,18 @@
 
 ## Installation
 
 We provide a python package for easy installation:
 ```
 pip install deprl
 ```
-### CUDA
-If you would like to use `jax` with CUDA support, which is recommended for DEP-RL training, we recommend:
-```
-pip install --upgrade "jax[cuda12_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
-```
 
- ### CPU only
- As the current version of PyTorch (2.0.1.) defaults to CUDA, on CPU-only machines you might want to run:
+### CPU only
+ If the default PyTorch version defaults to CUDA and you generate an exception on a CPU-only machine, consider running:
+
 ```
  pip install torch --index-url https://download.pytorch.org/whl/cpu
 ```
 after installation.
 
  ### Environments
```

