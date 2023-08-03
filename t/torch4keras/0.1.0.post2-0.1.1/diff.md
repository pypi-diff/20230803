# Comparing `tmp/torch4keras-0.1.0.post2.tar.gz` & `tmp/torch4keras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.1.0.post2.tar", last modified: Tue Jul 25 16:05:39 2023, max compression
+gzip compressed data, was "torch4keras-0.1.1.tar", last modified: Thu Aug  3 15:23:30 2023, max compression
```

## Comparing `torch4keras-0.1.0.post2.tar` & `torch4keras-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.880020 torch4keras-0.1.0.post2/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.1.0.post2/LICENSE
--rw-rw-rw-   0        0        0     8165 2023-07-25 16:05:39.870512 torch4keras-0.1.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0     7905 2023-07-25 16:05:19.000000 torch4keras-0.1.0.post2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 16:05:39.880020 torch4keras-0.1.0.post2/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-07-25 15:47:02.000000 torch4keras-0.1.0.post2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.864512 torch4keras-0.1.0.post2/torch4keras/
--rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.1.0.post2/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    50431 2023-07-25 15:59:20.000000 torch4keras-0.1.0.post2/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    31097 2023-07-25 15:49:22.000000 torch4keras-0.1.0.post2/torch4keras/model.py
--rw-rw-rw-   0        0        0    17218 2023-07-25 15:39:03.000000 torch4keras-0.1.0.post2/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.869512 torch4keras-0.1.0.post2/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     8165 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 15:23:30.846396 torch4keras-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8453 2023-08-03 15:23:30.845400 torch4keras-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8199 2023-08-02 15:37:50.000000 torch4keras-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:23:30.846396 torch4keras-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-08-01 12:36:14.000000 torch4keras-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:23:30.840399 torch4keras-0.1.1/torch4keras/
+-rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.1.1/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    52263 2023-08-03 14:14:41.000000 torch4keras-0.1.1/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    33617 2023-08-01 14:58:02.000000 torch4keras-0.1.1/torch4keras/model.py
+-rw-rw-rw-   0        0        0    20606 2023-08-03 14:48:06.000000 torch4keras-0.1.1/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:23:30.844428 torch4keras-0.1.1/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     8453 2023-08-03 15:23:30.000000 torch4keras-0.1.1/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-08-03 15:23:30.000000 torch4keras-0.1.1/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:23:30.000000 torch4keras-0.1.1/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 15:23:30.000000 torch4keras-0.1.1/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.1.0.post2/LICENSE` & `torch4keras-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.1.0.post2/PKG-INFO` & `torch4keras-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.1.0.post2
+Version: 0.1.1
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -87,14 +87,15 @@
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230802**: 增加指标平滑的SmoothMetricCallback，统一管理指标平滑的问题, 增加SKIP_METRICS，NO_SMOOTH_METRICS，ROUND_PRECISION，默认对指标会进行平滑，修改tensorboard和wandb的callback, 允许跳过nan的指标, Tensorboard可以记录gpu等系统信息
 - **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
 - **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
```

### Comparing `torch4keras-0.1.0.post2/README.md` & `torch4keras-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230802**: 增加指标平滑的SmoothMetricCallback，统一管理指标平滑的问题, 增加SKIP_METRICS，NO_SMOOTH_METRICS，ROUND_PRECISION，默认对指标会进行平滑，修改tensorboard和wandb的callback, 允许跳过nan的指标, Tensorboard可以记录gpu等系统信息
 - **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
 - **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
```

### Comparing `torch4keras-0.1.0.post2/setup.py` & `torch4keras-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='v0.1.0.post2',
+    version='v0.1.1',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.1.0.post2/torch4keras/callbacks.py` & `torch4keras-0.1.1/torch4keras/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,179 +4,36 @@
 import numpy as np
 from datetime import datetime
 import warnings
 from collections import deque
 import json
 import copy
 import os
-from torch4keras.snippets import log_error, send_email
+from torch4keras.snippets import log_info, log_error, log_warn, send_email
 
+# 忽略nan的指标
+IGNORE_NAN_VALUES = os.environ.get('IGNORE_NAN_VALUES', False)
 
-SKIP_METRICS = {'size'}
+# 不记录的metrics
+SKIP_METRICS = os.environ.get('SKIP_METRICS', {})
+SKIP_METRICS = eval(SKIP_METRICS) if isinstance(SKIP_METRICS, str) else SKIP_METRICS
 
+# 不能平滑的指标
+NO_SMOOTH_METRICS = os.environ.get('NO_SMOOTH_METRICS', {'lr'})
+NO_SMOOTH_METRICS = eval(NO_SMOOTH_METRICS) if isinstance(NO_SMOOTH_METRICS, str) else NO_SMOOTH_METRICS
 
-def _process_stateful_metrics(stateful_metrics):
-    ''''''
-    if stateful_metrics is None:
-        stateful_metrics_new = set()
-    elif isinstance(stateful_metrics, str):
-        stateful_metrics_new = {stateful_metrics}
-    elif isinstance(stateful_metrics, (set, tuple, list)):
-        stateful_metrics_new = set(stateful_metrics)
-    else:
-        raise ValueError('Args `stateful_metrics` only support `int/set/tuple/list` format')
-    stateful_metrics_new.add('lr')  # 学习率是不能平滑
-    return stateful_metrics_new
-
-
-class Progbar(object):
-    """进度条，直接从keras引入"""
-    def __init__(self, target, width=30, verbose=1, time_interval=0.05, stateful_metrics=None, smooth_interval=None):
-        '''
-        :param target: 进度条的step数量
-        :param width: 进度条的宽度
-        :param verbose: 是否展示进度条
-        :param time_interval: 更新进度条的最短时间间隔
-        :param stateful_metrics: list, 以状态量记录指标的格式
-        :param smooth_interval: int, 平滑时候使用的的step个数
-        '''
-        self.target = target
-        self.width = width
-        self.verbose = verbose
-        self.time_interval = time_interval
-        assert (smooth_interval is None) or isinstance(smooth_interval, int), 'Args `smooth_interval` only support `int` format'
-        self.smooth_interval = smooth_interval
-        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
-        
-        self._dynamic_display = ((hasattr(sys.stdout, 'isatty') and sys.stdout.isatty()) or 'ipykernel' in sys.modules)
-        self._total_width = 0
-        self._seen_so_far = 0
-        self._values = collections.OrderedDict()  # OrderedDict([('loss', [11.60657262802124, 5]), ('acc', [0.25, 5])])
-        self._smooth_values = dict()  # 存储滑动平均的结果，stateful_metrics时候滑动平均结果和不滑动一致
-        self._start = time.time()
-        self._last_update = 0
-
-    def update(self, current, values=None):
-        """Updates the progress bar."""
-        values = values or []
-        for k, v in values:
-            if k not in self.stateful_metrics:
-                if k not in self._values:
-                    self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
-                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 1):
-                    # 如果定义了累积smooth_interval，则需要重新累计
-                    self._values[k] = [v, 1]
-                else:
-                    self._values[k][0] += v * (current - self._seen_so_far)
-                    self._values[k][1] += (current - self._seen_so_far)
-            else:
-                # Stateful metrics output a numeric value.  This representation
-                # means "take an average from a single value" but keeps the
-                # numeric formatting.
-                self._values[k] = [v, 1]
-        
-        self._seen_so_far = current
-
-        now = time.time()
-        info = ' - %.0fs' % (now - self._start)
-        if self.verbose == 1:
-            if (now - self._last_update < self.time_interval and self.target is not None and current < self.target):
-                # 训练每个step太快了，则不更新进度条，累计达到一定的时间间隔再更新进度条
-                return
-
-            prev_total_width = self._total_width
-            if self._dynamic_display:
-                sys.stdout.write('\b' * prev_total_width)
-                sys.stdout.write('\r')
-            else:
-                sys.stdout.write('\n')
-
-            if self.target is not None:
-                numdigits = int(np.floor(np.log10(self.target))) + 1
-                barstr = '%%%dd/%d [' % (numdigits, self.target)
-                bar = barstr % current
-                prog = float(current) / self.target
-                prog_width = int(self.width * prog)
-                if prog_width > 0:
-                    bar += ('=' * (prog_width - 1))
-                    if current < self.target:
-                        bar += '>'
-                    else:
-                        bar += '='
-                bar += ('.' * (self.width - prog_width))
-                bar += ']'
-            else:
-                bar = '%7d/Unknown' % current
-
-            self._total_width = len(bar)
-            sys.stdout.write(bar)
+# 指标的精度
+ROUND_PRECISION = int(os.environ.get('ROUND_PRECISION', 4))
+_round_precision = eval(f"1e-{ROUND_PRECISION-1}")
 
-            if current:
-                time_per_unit = (now - self._start) / current
-            else:
-                time_per_unit = 0
-            if self.target is not None and current < self.target:
-                eta = time_per_unit * (self.target - current)
-                if eta > 3600:
-                    eta_format = ('%d:%02d:%02d' % (eta // 3600, (eta % 3600) // 60, eta % 60))
-                elif eta > 60:
-                    eta_format = '%d:%02d' % (eta // 60, eta % 60)
-                else:
-                    eta_format = '%ds' % eta
 
-                info = ' - ETA: %s' % eta_format
-            else:
-                if time_per_unit >= 1:
-                    info += ' %.0fs/step' % time_per_unit
-                elif time_per_unit >= 1e-3:
-                    info += ' %.0fms/step' % (time_per_unit * 1e3)
-                else:
-                    info += ' %.0fus/step' % (time_per_unit * 1e6)
-
-            for k in self._values:
-                info += ' - %s:' % k
-                if isinstance(self._values[k], list):
-                    avg = np.mean(self._values[k][0] / max(1, self._values[k][1]))  # 指标平滑
-                    self._smooth_values[k] = avg  # 存储滑动平均的结果
-                    if abs(avg) > 1e-3:
-                        info += ' %.4f' % avg
-                    else:
-                        info += ' %.4e' % avg
-                else:
-                    info += ' %s' % self._values[k]
-            info += ' '  # 最后加个空格，防止中途有别的打印
-            self._total_width += len(info)
-            if prev_total_width > self._total_width:
-                info += (' ' * (prev_total_width - self._total_width))
-
-            if self.target is not None and current >= self.target:
-                info += '\n'
-
-            sys.stdout.write(info)
-            sys.stdout.flush()
-
-        elif self.verbose == 2:
-            if self.target is None or current >= self.target:
-                for k in self._values:
-                    info += ' - %s:' % k
-                    avg = np.mean(
-                        self._values[k][0] / max(1, self._values[k][1]))
-                    if avg > 1e-3:
-                        info += ' %.4f' % avg
-                    else:
-                        info += ' %.4e' % avg
-                info += '\n'
-
-                sys.stdout.write(info)
-                sys.stdout.flush()
-
-        self._last_update = now
-
-    def add(self, n, values=None):
-        self.update(self._seen_so_far + n, values)
+def round(v, mode='f'):
+    if abs(v) < _round_precision:
+        mode = 'e'
+    return f"%.{ROUND_PRECISION}{mode}" % v
 
 
 class CallbackList(object):
     '''把原来在model.py中的callback_fun移植出来，参考Keras的CallbackList重构
     '''
     def __init__(self, callbacks=None, queue_length=10, run_callbacks=True):
         callbacks = callbacks or []
@@ -324,31 +181,229 @@
         pass
     def on_dataloader_end(self, logs=None):
         pass
     def on_train_step_end(self, logs=None):
         pass
 
 
-class TerminateOnNaN(Callback):
-    """Loss出现NAN停止训练"""
+def _process_stateful_metrics(stateful_metrics):
+    ''''''
+    if stateful_metrics is None:
+        stateful_metrics_new = set()
+    elif isinstance(stateful_metrics, str):
+        stateful_metrics_new = {stateful_metrics}
+    elif isinstance(stateful_metrics, (set, tuple, list)):
+        stateful_metrics_new = set(stateful_metrics)
+    else:
+        raise ValueError('Args `stateful_metrics` only support `int/set/tuple/list` format')
+    stateful_metrics_new.update(NO_SMOOTH_METRICS)
+    return stateful_metrics_new
+
+
+class SmoothMetric:
+    '''指标平滑'''
+    def __init__(self, interval=None, stateful_metrics=None) -> None:
+        self._values = collections.OrderedDict()  # OrderedDict([('loss', [11.60657262802124, 5]), ('acc', [0.25, 5])])
+        self.interval = interval
+        self.stateful_metrics = stateful_metrics or set()
+        self._seen_so_far = 0
+    
+    def update(self, current, logs:dict):
+        if (self.interval is not None) and (current % self.interval == 1):
+            # 如果定义了累积interval，则需要重新累计
+            self.reset()
+        
+        for k, v in logs.items():
+            if k in SKIP_METRICS:
+                continue
+            elif IGNORE_NAN_VALUES and np.isnan(v):
+                log_error(f'Value `{k}` at {current} step is nan')
+                continue
+            elif (k in NO_SMOOTH_METRICS) or (k in self.stateful_metrics):
+                self._values[k] = [v, 1]
+            elif k not in self._values:
+                self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
+            else:
+                self._values[k][0] += v * (current - self._seen_so_far)
+                self._values[k][1] += (current - self._seen_so_far)
+            
+        self._seen_so_far = current
+        return self._values
+
+    def reset(self):
+        self._values = collections.OrderedDict()
+
+    def get_smooth_logs(self, logs=None):
+        smooth_logs = {k: v[0]/v[1] for k, v in self._values.items() if k not in SKIP_METRICS}
+        
+        if logs is not None:
+            for k, v in logs.items() :
+                if (k in SKIP_METRICS) or (k in smooth_logs):
+                    continue
+                smooth_logs[k] = v
+        return smooth_logs
+
+    def add(self, n, values=None):
+        self.update(self._seen_so_far + n, values)
+
+
+class SmoothMetricsCallback(Callback):
+    '''指标平滑的callback，会inplace修改log，影响后续的callback中log
+    1）适用情形：希望Logger, Tensorboard，Wandb, EarlyStopping等callbacks中使用的累计平滑的指标
+    2）使用方法：初始化后，放在fit()中靠前的位置来对log进行修改
+    3）step的平滑是全局来看的（跨epoch不中断），epoch平滑是对每个epoch分别累计计算
+
+    :param interval: int, 平滑时候使用的的step个数
+    :param stateful_metrics: list, 以状态量记录指标的格式
+    '''
+    def __init__(self, interval=100, stateful_metrics=None, verbose=0, **kwargs):
+        super(SmoothMetricsCallback, self).__init__(**kwargs)
+        self.interval = interval
+        self.stateful_metrics = stateful_metrics
+        self.smooth_metric_step = SmoothMetric(interval=self.interval, stateful_metrics=self.stateful_metrics)
+        if verbose != 0:
+            log_info(f'SmoothMetricCallback calculate {interval} steps average metrics')
+
+    def on_epoch_begin(self, global_step, epoch, logs=None):
+        self.smooth_metric_epoch = SmoothMetric(stateful_metrics=self.stateful_metrics)
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        self.smooth_metric_epoch.get_smooth_logs(logs)
+        smooth_logs = self.smooth_metric_epoch.get_smooth_logs()
+        logs.update(smooth_logs)
+
     def on_batch_end(self, global_step, local_step, logs=None):
-        logs = logs or {}
-        loss = logs.get('loss')
-        if loss is not None:
-            if np.isnan(loss) or np.isinf(loss):
-                log_error('Step %d: Invalid loss, terminating training' % global_step)
-                self.trainer.stop_training = True
+        self.smooth_metric_step.update(global_step+1, logs)
+        self.smooth_metric_epoch.update(local_step+1, logs)
+        smooth_logs = self.smooth_metric_step.get_smooth_logs()
+        logs.update(smooth_logs)
+
+
+class Progbar(object):
+    """进度条，直接从keras引入"""
+    def __init__(self, target, width=30, verbose=1, time_interval=0.05, stateful_metrics=None):
+        '''
+        :param target: 进度条的step数量
+        :param width: 进度条的宽度
+        :param verbose: 是否展示进度条
+        :param time_interval: 更新进度条的最短时间间隔
+        :param stateful_metrics: list, 以状态量记录指标的格式
+        '''
+        self.target = target
+        self.width = width
+        self.verbose = verbose
+        self.time_interval = time_interval
+        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
+        self._dynamic_display = ((hasattr(sys.stdout, 'isatty') and sys.stdout.isatty()) or 'ipykernel' in sys.modules)
+        self._total_width = 0
+        self._start = time.time()
+        self._last_update = 0
+
+    def update(self, current, values=None):
+        """Updates the progress bar."""
+        now = time.time()
+        info = ' - %.0fs' % (now - self._start)
+        if self.verbose == 1:
+            if (now - self._last_update < self.time_interval and self.target is not None and current < self.target):
+                # 训练每个step太快了，则不更新进度条，累计达到一定的时间间隔再更新进度条
+                return
+
+            prev_total_width = self._total_width
+            if self._dynamic_display:
+                sys.stdout.write('\b' * prev_total_width)
+                sys.stdout.write('\r')
+            else:
+                sys.stdout.write('\n')
+
+            if self.target is not None:
+                numdigits = int(np.floor(np.log10(self.target))) + 1
+                barstr = '%%%dd/%d [' % (numdigits, self.target)
+                bar = barstr % current
+                prog = float(current) / self.target
+                prog_width = int(self.width * prog)
+                if prog_width > 0:
+                    bar += ('=' * (prog_width - 1))
+                    if current < self.target:
+                        bar += '>'
+                    else:
+                        bar += '='
+                bar += ('.' * (self.width - prog_width))
+                bar += ']'
+            else:
+                bar = '%7d/Unknown' % current
+
+            self._total_width = len(bar)
+            sys.stdout.write(bar)
+
+            if current:
+                time_per_unit = (now - self._start) / current
+            else:
+                time_per_unit = 0
+            if self.target is not None and current < self.target:
+                eta = time_per_unit * (self.target - current)
+                if eta > 3600:
+                    eta_format = ('%d:%02d:%02d' % (eta // 3600, (eta % 3600) // 60, eta % 60))
+                elif eta > 60:
+                    eta_format = '%d:%02d' % (eta // 60, eta % 60)
+                else:
+                    eta_format = '%ds' % eta
+
+                info = ' - ETA: %s' % eta_format
+            else:
+                if time_per_unit >= 1:
+                    info += ' %.0fs/step' % time_per_unit
+                elif time_per_unit >= 1e-3:
+                    info += ' %.0fms/step' % (time_per_unit * 1e3)
+                else:
+                    info += ' %.0fus/step' % (time_per_unit * 1e6)
+
+            for k in values:
+                info += ' - %s:' % k
+                if isinstance(values[k], list):
+                    avg = np.mean(values[k][0] / max(1, values[k][1]))  # 指标平滑
+                    if abs(avg) > 1e-3:
+                        info += f' %.{ROUND_PRECISION}f' % avg
+                    else:
+                        info += f' %.{ROUND_PRECISION}e' % avg
+                else:
+                    info += ' %s' % values[k]
+            info += ' '  # 最后加个空格，防止中途有别的打印
+            self._total_width += len(info)
+            if prev_total_width > self._total_width:
+                info += (' ' * (prev_total_width - self._total_width))
+
+            if self.target is not None and current >= self.target:
+                info += '\n'
+
+            sys.stdout.write(info)
+            sys.stdout.flush()
+
+        elif self.verbose == 2:
+            if self.target is None or current >= self.target:
+                for k in values:
+                    info += ' - %s:' % k
+                    avg = np.mean(values[k][0] / max(1, values[k][1]))
+                    if avg > 1e-3:
+                        info += f' %.{ROUND_PRECISION}f' % avg
+                    else:
+                        info += f' %.{ROUND_PRECISION}e' % avg
+                info += '\n'
+
+                sys.stdout.write(info)
+                sys.stdout.flush()
+
+        self._last_update = now
 
 
 class KerasProgbar(Callback):
     """ keras进度条 """
-    def __init__(self, stateful_metrics=None, smooth_interval=None, width=30, **kwargs):
+    def __init__(self, stateful_metrics=None, interval=None, width=30, **kwargs):
         super(KerasProgbar, self).__init__(**kwargs)
         self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
-        self.smooth_interval = smooth_interval
+        self.interval = interval
         self.width = width
 
     def add_metrics(self, metrics, stateful_metrics=None, add_position=None):
         '''在指定位置插入metrics指标
         '''
         if add_position is None:
             add_position = len(self.params['metrics'])
@@ -367,136 +422,121 @@
     def on_train_begin(self, logs=None):
         self.verbose = self.params['verbose']
         self.epochs = self.params['epochs']
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Start Training' % (time_start))
 
+    def on_train_end(self, logs=None):
+        if self.verbose:
+            time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            print('\n%s - Finish Training' % (time_start))
+
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
+            print('\n%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
-            self.progbar = Progbar(target=self.target, width=self.width, verbose=self.verbose, 
-                                   stateful_metrics=self.stateful_metrics, smooth_interval=self.smooth_interval)
-        self.seen = 0
+            self.progbar = Progbar(target=self.target, width=self.width, verbose=self.verbose, stateful_metrics=self.stateful_metrics)
+            self.smooth_metric = SmoothMetric(self.interval, self.stateful_metrics)
 
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         logs = logs or {}
-        self.seen += 1
-        log_values = [(k, logs[k]) for k in self.params['metrics'] if k in logs]
-        # Skip progbar update for the last batch;
-        # will be handled by on_epoch_end.
+        log_values = {k:logs[k] for k in self.params['metrics'] if k in logs}
         if self.verbose:
-            self.progbar.update(self.seen, log_values)
-            logs.update(self.progbar._smooth_values)  # 如果进度条是平滑的，那这里的logs也覆盖掉
+            values = self.smooth_metric.update(local_step+1, log_values)
+            self.progbar.update(local_step+1, values)
     
-    def on_train_end(self, logs=None):
-        if self.verbose:
-            time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            print('%s - Finish Training' % (time_start))
         
-
 class TqdmProgbar(KerasProgbar):
     """ Tqdm进度条 """
-    def __init__(self, stateful_metrics=None, smooth_interval=None, width=None, **kwargs):
-        super().__init__(stateful_metrics, smooth_interval, width, **kwargs)
+    def __init__(self, stateful_metrics=None, interval=None, width=None, **kwargs):
+        super().__init__(stateful_metrics, interval, width, **kwargs)
 
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
             from tqdm import tqdm
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
+            print('\n%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
             self.progbar = tqdm(total=self.params['steps'], desc='Training', dynamic_ncols=False, file=sys.stdout, smoothing=0, ncols=self.width)
-        self.seen = 0
-        self._values = collections.OrderedDict()
-        self._smooth_values = dict()
-        self._seen_so_far = 0
+        self.smooth_metric = SmoothMetric(self.interval, self.stateful_metrics)
 
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
-        self.seen += 1
-        logs_new = self.smooth_values(self.seen, logs or {})
+        logs_new = self.smooth_values(local_step+1, logs)
         log_values = [(k, logs_new[k]) for k in self.params['metrics'] if k in logs_new]
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
         if self.verbose:
-            self.progbar.n = self.seen
+            self.progbar.n = local_step+1
             self.progbar.refresh()
             self.progbar.set_postfix(log_values)
-            logs.update(self._smooth_values)
-            if self.seen >= self.target:
-                self.progbar.close()
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        self.progbar.close()
     
     def smooth_values(self, current, values=None):
         '''从Progbar迁移过来'''
-        values = values or []
-        for k, v in values.items():
-            if k not in self.stateful_metrics:
-                if k not in self._values:
-                    self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
-                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 1):
-                    # 如果定义了累积smooth_interval，则需要重新累计
-                    self._values[k] = [v, 1]
-                else:
-                    self._values[k][0] += v * (current - self._seen_so_far)
-                    self._values[k][1] += (current - self._seen_so_far)
-            else:
-                self._values[k] = [v, 1]
-        self._seen_so_far = current
+        _values = self.smooth_metric.update(current, values)
 
         logs = collections.OrderedDict()
-        for k in self._values:
-            if isinstance(self._values[k], list):
-                avg = np.mean(self._values[k][0] / max(1, self._values[k][1]))
-                self._smooth_values[k] = avg
+        for k in _values:
+            if isinstance(_values[k], list):
+                avg = np.mean(_values[k][0] / max(1, _values[k][1]))
                 if abs(avg) > 1e-3:
-                    logs[k] = ' %.4f' % avg
+                    logs[k] = f' %.{ROUND_PRECISION}f' % avg
                 else:
-                    logs[k] = ' %.4e' % avg
+                    logs[k] = f' %.{ROUND_PRECISION}e' % avg
             else:
-                logs[k] = ' %s' % self._values[k]
+                logs[k] = ' %s' % _values[k]
 
         return logs
 
 
 class ProgressBar2Progbar(TqdmProgbar):
     """ progressbar2进度条 """
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
             import progressbar
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
+            print('\n%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
             widgets = [progressbar.SimpleProgress(format='%(value_s)s/%(max_value_s)s'), progressbar.Bar(marker='=', left='[', right=']'), ' ', 
                        progressbar.AdaptiveETA(format='ETA: %(eta)s', format_finished='Time: %(elapsed)s'), ' - ']
             for i, param in enumerate(self.params['metrics']):
                 widgets.append(progressbar.Variable(param, precision=7))
                 if i < len(self.params['metrics'])-1:
                     widgets.append(' - ')
             self.progbar = progressbar.bar.ProgressBar(min_value=0, max_value=self.params['steps'], widgets=widgets, 
                                                        redirect_stdout=True, redirect_stderr=True)
-        self.seen = 0
-        self._values = collections.OrderedDict()
-        self._smooth_values = dict()
-        self._seen_so_far = 0
+        self.smooth_metric = SmoothMetric(self.interval, self.stateful_metrics)
 
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
-        self.seen += 1
-        logs_new = self.smooth_values(self.seen, logs or {})
+        logs_new = self.smooth_values(local_step+1, logs or {})
         logs_new = {k:logs_new[k].strip() for k in self.params['metrics'] if k in logs_new}
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
         if self.verbose:
-            self.progbar.update(self.seen, **logs_new)
-            logs.update(self._smooth_values)
-            if self.seen >= self.target:
-                self.progbar.finish()
+            self.progbar.update(local_step+1, **logs_new)
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        self.progbar.finish()
+
+
+class TerminateOnNaN(Callback):
+    """Loss出现NAN停止训练"""
+    def on_batch_end(self, global_step, local_step, logs=None):
+        logs = logs or {}
+        loss = logs.get('loss')
+        if loss is not None:
+            if np.isnan(loss) or np.isinf(loss):
+                log_error('Step %d: Invalid loss, terminating training' % global_step)
+                self.trainer.stop_training = True
 
 
 class History(Callback):
     """指标历史，默认是fit的返回项, 这里仅记录epoch_end的指标"""
     def on_train_begin(self, logs=None):
         self.epoch = []
         self.history = {}
@@ -738,111 +778,122 @@
         except self.requests.exceptions.RequestException:
             warnings.warn('Warning: could not reach RemoteMonitor root server at ' + str(self.root))
 
 
 class Checkpoint(Callback):
     '''保存Checkpoint, 可以每个epoch或者每隔一定的steps保存
 
+    :param save_dir: str, 保存的文件夹，只定义即可按照默认的文件名保存
     :param model_path: str, 模型保存路径(含文件名)，可以使用{epoch}和{step}占位符
     :param optimizer_path: str, 优化器保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
     :param scheduler_path: str, scheduler保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
     :param steps_params_path: str, 模型训练进度保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
     :param method: str, 按照轮次保存还是按照步数保存，默认为'epoch'表示每个epoch保存一次, 可选['epoch', 'step'] 
-    :param step_interval: int, method设置为'step'时候指定每隔多少步数保存模型，默认为100表示每隔100步保存一次
+    :param interval: int, method设置为'step'时候指定每隔多少步数保存模型，默认为100表示每隔100步保存一次
     '''
-    def __init__(self, model_path, optimizer_path=None, scheduler_path=None, steps_params_path=None, method='epoch', step_interval=100, verbose=0, **kwargs):
+    def __init__(self, save_dir=None, model_path=None, optimizer_path=None, scheduler_path=None, steps_params_path=None,
+                 method='epoch', interval=100, verbose=0, **kwargs):
         super().__init__(**kwargs)
         assert method in {'step', 'epoch'}, 'Args `method` only support `step` or `epoch`'
         self.method = method
+        self.save_dir = save_dir  # 保存文件夹
         self.model_path = model_path  # 保存路径，可设置{epoch}{step}{loss}等占位符
         self.optimizer_path = optimizer_path  # 是否保存优化器
         self.scheduler_path = scheduler_path  # 是否保存scheduler
         self.steps_params_path = steps_params_path  # 是否保存训练步数
-        self.step_interval = step_interval  # method='step'时候生效
+        self.interval = interval  # method='step'时候生效
         self.verbose = verbose
+        self.kwargs = kwargs
     
     def on_epoch_end(self, global_step, epoch, logs=None):
         logs = logs or {}
         if self.method == 'epoch':
             self.process(epoch+1, logs)
 
     def on_batch_end(self, global_step, local_step, logs=None):
         logs = logs or {}
-        if (self.method == 'step') and ((global_step+1) % self.step_interval == 0):
+        if (self.method == 'step') and ((global_step+1) % self.interval == 0):
             self.process(global_step+1, logs)
 
     def process(self, suffix, logs):
         file_paths = []
-        for filepath in [self.model_path, self.optimizer_path, self.scheduler_path, self.steps_params_path]:
+        for filepath in [self.save_dir, self.model_path, self.optimizer_path, self.scheduler_path, self.steps_params_path]:
             if filepath:
                 filepath = filepath.format(epoch=suffix, **logs) if self.method == 'epoch' else filepath.format(step=suffix, **logs)
             file_paths.append(filepath)
 
-        self.trainer.save_to_checkpoint(model_path=file_paths[0], optimizer_path=file_paths[1], scheduler_path=file_paths[2], 
-                                        step_params_path=file_paths[3], verbose=self.verbose)
+        self.trainer.save_to_checkpoint(*file_paths, verbose=self.verbose, **self.kwargs)
 
 
 class Evaluator(Checkpoint):
     '''评估并保存最优Checkpoint, 也可以只评估
 
     :param monitor: str, 监控指标，需要在logs中，默认为'perf'
-    :param verbose: int, 是否打印，默认为1表示打印
+    :param verbose: int, 是否打印，默认为2表示打印
     :param mode: str, 控制监控指标monitor的大小方向，默认为'auto', 可选{'auto', 'min', 'max'}
     :param method: str, 控制是按照epoch还是step来计算，默认为'epoch', 可选{'step', 'epoch'}
     :param baseline: None/float, 基线, 默认为None 
+    :param save_dir: str, 保存的文件夹，只定义即可按照默认的文件名保存
     :param model_path: str, 模型保存路径(含文件名)，可以使用{epoch}和{step}占位符
     :param optimizer_path: str, 优化器保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
     :param scheduler_path: str, scheduler保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
     :param steps_params_path: str, 模型训练进度保存路径(含文件名)，可以使用{epoch}和{step}占位符，默认为None表示不保存
-    :param step_interval: int, method设置为'step'时候指定每隔多少步数保存模型，默认为100表示每隔100步保存一次
+    :param interval: int, method设置为'step'时候指定每隔多少步数保存模型，默认为100表示每隔100步保存一次
     '''
-    def __init__(self, monitor='perf', mode='max', verbose=1, model_path=None, optimizer_path=None, scheduler_path=None,
-                 steps_params_path=None, method='epoch', step_interval=100, **kwargs):
-        super().__init__(model_path, optimizer_path, scheduler_path, steps_params_path, method, step_interval, **kwargs)
+    def __init__(self, monitor='perf', mode='max', verbose=2, save_dir=None, model_path=None, optimizer_path=None, scheduler_path=None,
+                 steps_params_path=None, method='epoch', interval=100, **kwargs):
+        super().__init__(save_dir, model_path, optimizer_path, scheduler_path, steps_params_path, method, interval, **kwargs)
         self.monitor = monitor
         assert mode in {'max', 'min'}, 'Compare performance only support `max/min` mode'
         self.mode = mode
         self.verbose = verbose
         self.best_perf = np.inf if mode == 'min' else -np.inf
 
     def process(self, suffix, logs):
         perf = self.evaluate()
+        # 如果evaluate返回的是字典则使用字典，如果返回的是数值则套上{'perf': perf}
         perf = perf if isinstance(perf, dict) else {'perf': perf}
         logs.update(perf)  # 评估的指标后续可能会用到
         
+        # 不存在
+        if perf.get(self.monitor) is None:
+            warnings.warn('Evaluator callback conditioned on metric `%s` which is not available. Available metrics are: %s' %
+                (self.monitor, ','.join(list(logs.keys()))), RuntimeWarning)
+            return
+
         # 满足条件
         if ((self.mode == 'max') and (perf[self.monitor] >= self.best_perf)) or ((self.mode == 'min') and (perf[self.monitor] <= self.best_perf)):
             self.best_perf = perf[self.monitor]
             # 保存ckpt
             super().process(suffix, logs)
 
-        if self.verbose > 0:
-            print_str = ', '.join([f'{k}: {v:.5f}' for k, v in perf.items()])
-            print(print_str + f'. best_{self.monitor}: {self.best_perf:.5f}\n')
+        if self.verbose != 0:
+            print_str = ', '.join([f'{k}: {round(v)}' for k, v in perf.items()])
+            print(print_str + f'. best_{self.monitor}: {round(self.best_perf)}')
         
     # 定义评价函数
     def evaluate(self):
         # 需要返回一个字典，且self.monitor在字典key中
         # 如果返回的是一个数值型，则默认使用'perf'作为指标名
-        raise NotImplemented
+        return None
 
 
 class Logger(Callback):
     '''默认logging
     对于valid/dev和test的日志需要在evaluate之后对log进行赋值，如log['dev_f1']=f1，并在Evaluator之后调用
     若每隔一定steps对验证集评估，则Logger的interval设置成和Evaluater一致或者约数，保证日志能记录到
 
     :param log_path: str, log文件的保存路径
     :param interval: int, 保存log的间隔
     :param mode: str, log保存的模式, 默认为'a'表示追加
     :param separator: str, 指标间分隔符
     :param verbosity: int, 可选[0,1,2]，指定log的level
     :param name: str, 默认为None
     '''
-    def __init__(self, log_path, interval=10, mode='a', separator='\t', verbosity=1, name=None, **kwargs):
+    def __init__(self, log_path, interval=100, mode='a', separator='\t', verbosity=1, name=None, **kwargs):
         super(Logger, self).__init__(**kwargs)
         self.log_path = log_path
         self.interval = interval
         self.mode = mode
         self.sep = separator
         self.name = name
         self.verbosity = verbosity
@@ -858,70 +909,164 @@
         os.makedirs(save_dir, exist_ok=True)
         fh = logging.FileHandler(self.log_path, self.mode)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
         self.logger.info('Start Training'.center(40, '='))
 
     def on_train_end(self, logs=None):
-        self.logger.info('Finish Training'.center(40, '='))
+        self.logger.info('Finish Training'.center(40, '=') + '\n')
 
     def on_epoch_begin(self, global_step, epoch, logs=None):
         self.logger.info(f'Epoch {epoch+1}'.center(40, '='))
 
     def on_epoch_end(self, global_step, epoch, logs=None):
-        log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in SKIP_METRICS])
+        log_str = f'{self.sep}'.join([f'{k}={round(v)}' for k, v in logs.items() if k not in SKIP_METRICS])
         self.logger.info(f'epoch={epoch+1}{self.sep}{log_str}')
 
     def on_batch_end(self, global_step, local_step, logs=None):
         if (global_step+1) % self.interval == 0:
-            log_str = f'{self.sep}'.join([f'{k}={v:.5f}' for k, v in logs.items() if k not in SKIP_METRICS])
+            log_str = f'{self.sep}'.join([f'{k}={round(v)}' for k, v in logs.items() if k not in SKIP_METRICS])
             self.logger.info(f'step={global_step+1}{self.sep}{log_str}')
 
 
 class Tensorboard(Callback):
     '''默认Tensorboard
     对于valid/dev和test的Tensorboard需要在evaluate之后对log进行赋值，如log['dev/f1']=f1，并在Evaluator之后调用
     赋值需要分栏目的用'/'进行分隔
     若每隔一定steps对验证集评估，则Tensorboard的interval设置成和Evaluater一致或者约数，保证Tensorboard能记录到
 
     :param log_dir: str, tensorboard文件的保存路径
-    :param method: str, 控制是按照epoch还是step来计算，默认为'epoch', 可选{'step', 'epoch'}
     :param interval: int, 保存tensorboard的间隔
     :param prefix: str, tensorboard分栏的前缀，默认为'train'
     '''
-    def __init__(self, log_dir, method='epoch', interval=10, prefix='train', **kwargs):
+    def __init__(self, log_dir, interval=100, prefix='Train', **kwargs):
         super(Tensorboard, self).__init__(**kwargs)
-        assert method in {'step', 'epoch'}, 'Args `method` only support `step` or `epoch`'
-        self.method = method
+        self.log_dir = log_dir
         self.interval = interval
-        self.prefix = prefix+'/' if len(prefix.strip()) > 0 else ''  # 控制默认的前缀，用于区分栏目
+        self.prefix_step = prefix+'/' if len(prefix.strip()) > 0 else ''  # 控制默认的前缀，用于区分栏目
+        self.prefix_epoch = prefix+'_epoch/' if len(prefix.strip()) > 0 else 'Epoch/'  # 控制默认的前缀，用于区分栏目
 
+    def on_train_begin(self, logs=None):
         from tensorboardX import SummaryWriter
-        os.makedirs(log_dir, exist_ok=True)
-        self.writer = SummaryWriter(log_dir=str(log_dir))  # prepare summary writer
+        os.makedirs(self.log_dir, exist_ok=True)
+        self.writer = SummaryWriter(log_dir=str(self.log_dir))  # prepare summary writer
 
     def on_epoch_end(self, global_step, epoch, logs=None):
-        if self.method == 'epoch':
-            # 默认记录的是epoch
-            self.process(epoch+1, logs)
+        if hasattr(self.trainer, 'epochs') and self.trainer.epochs > 1:
+            self.process(epoch+1, logs, self.prefix_epoch)
 
     def on_batch_end(self, global_step, local_step, logs=None):
-        # 默认记录的是global_step
-        if (self.method == 'step') and ((global_step+1) % self.interval == 0):
-            self.process(global_step+1, logs)
+        if (global_step+1) % self.interval == 0:
+            self.process(global_step+1, logs, self.prefix_step)
 
-    def process(self, iteration, logs):
+    def process(self, iteration, logs, prefix):
         logs = logs or {}
         for k, v in logs.items():
             if k in SKIP_METRICS:
                 continue
-            index = k if '/' in k else f"{self.prefix}{k}"
+            index = k if '/' in k else f"{prefix}{k}"
             self.writer.add_scalar(index, v, iteration)
 
 
+class WandbCallback(Callback):
+    """从transformers迁移过来
+    A :class:`~transformers.TrainerCallback` that sends the logs to `Weight and Biases <https://www.wandb.com/>`__.
+
+    :param interval: int, log的的step间隔
+    :param watch (:obj:`str`, `optional` defaults to :obj:`"gradients"`):
+        Can be :obj:`"gradients"`, :obj:`"all"` or :obj:`"false"`. Set to :obj:`"false"` to disable gradient
+        logging or :obj:`"all"` to log gradients and parameters.
+    :param project: str，wandb的project name, 默认为bert4torch
+    :param 
+    """
+    def __init__(self, project='bert4torch', trial_name=None, run_name=None, watch='gradients', 
+                 interval=100, save_code=False, config=None):
+        try:
+            import wandb
+            self._wandb = wandb
+        except:
+            log_warn("WandbCallback requires wandb to be installed. Run `pip install wandb`.")
+            self._wandb = None
+
+        self._initialized = False
+        # log outputs
+        self.project = project
+        if trial_name is None:
+            self.trial_name = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        if run_name is None:
+            self.run_name = self.trial_name
+        self.watch = watch
+        self.interval = interval
+        self.save_code = save_code
+        self.config = config or {}
+        self.run_id = None
+        self.metrics = set()
+
+    def define_metric(self, step_metric, logs=None):
+        if getattr(self._wandb, "define_metric", None):
+            for m in logs.keys():
+                if m not in self.metrics:
+                    self._wandb.define_metric(name=m, step_metric=step_metric, hidden=True if m in SKIP_METRICS else False)
+                    self.metrics.add(m)
+
+    def adjust_logs(self, logs, **kwargs):
+        logs_new = {**logs, **kwargs}
+        return {k:v for k,v in logs_new.items() if k not in SKIP_METRICS}
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        if self._wandb is None:
+            return
+        if hasattr(self.trainer, 'epochs') and self.trainer.epochs > 1:
+            self.define_metric('epoch', logs)
+            self._wandb.log(self.adjust_logs(logs, epoch=epoch+1))
+
+    def on_batch_end(self, global_step, local_step, logs=None):
+        if self._wandb is None:
+            return
+        
+        if (global_step+1) % self.interval == 0:
+            self.define_metric('step', logs)
+            self._wandb.log(self.adjust_logs(logs, step=global_step+1))
+        
+    def on_train_begin(self, logs=None):
+        if self._wandb is None:
+            return
+
+        self._initialized = True
+        combined_dict = {**self.trainer.__dict__, **self.config}
+
+        if hasattr(self.model, "config") and self.model.config is not None:
+            combined_dict = {**self.model.config, **combined_dict}
+        init_args = {}
+        if self.trial_name is not None:
+            run_name = self.trial_name
+            init_args["group"] = self.run_name
+        else:
+            run_name = self.run_name
+
+        if self._wandb.run is None:
+            run = self._wandb.init(project=self.project, name=run_name, save_code=self.save_code, **init_args)
+            self.run_id = run.id
+
+        # add config parameters (run may have been created manually)
+        self._wandb.config.update(combined_dict, allow_val_change=True)
+
+        # keep track of model topology and gradients, unsupported on TPU
+        if self.watch != "false":
+            self._wandb.watch(self.model, log=self.watch, log_freq=max(100, self.interval))
+
+    def on_train_end(self, logs=None):
+        if self._wandb is None:
+            return
+
+        # transformer中的on_log
+        self._wandb.finish()
+        self._initialized = False
+
+
 class LambdaCallback(Callback):
     """lambda表达式
     """
     def __init__(self, on_epoch_begin=None, on_epoch_end=None, on_batch_begin=None, on_batch_end=None, 
                  on_train_begin=None, on_train_end=None, on_dataloader_end=None, **kwargs):
         super(LambdaCallback, self).__init__(**kwargs)
         self.__dict__.update(kwargs)
@@ -978,140 +1123,45 @@
     :param method: str, 控制是按照epoch还是step来发送邮件，默认为'epoch', 可选{'step', 'epoch'}
     :param interval: int, 发送邮件的的step间隔
     :param mail_host: str, 发件服务器host
     :param mail_user: str, 发件人
     :param mail_pwd: str, smtp的第三方密码
     :param sender: str, 发件人邮箱
     '''
-    def __init__(self, receivers, subject='', method='epoch', interval=10, mail_host=None, mail_user=None, mail_pwd=None, sender=None, **kwargs):
+    def __init__(self, receivers, subject='', method='epoch', interval=100, mail_host=None, mail_user=None, mail_pwd=None, sender=None, **kwargs):
         super(EmailCallback, self).__init__(**kwargs)
         self.method = method
         self.interval = interval
         self.receivers = receivers
         self.subject = subject
         self.mail_host = mail_host
         self.mail_user = mail_user
         self.mail_pwd = mail_pwd
         self.sender = sender
 
     def on_epoch_end(self, global_step, epoch, logs=None):
         if self.method == 'epoch':
-            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
+            msg = json.dumps({k:f'{round(v)}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
             subject = f'[INFO] Epoch {epoch+1} performance'
             if self.subject != '':
                 subject = self.subject + ' | ' + subject
             self._email(subject, msg)
 
     def on_batch_end(self, global_step, local_step, logs=None):
         if (self.method == 'step') and ((global_step+1) % self.interval == 0):
-            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
+            msg = json.dumps({k:f'{round(v)}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
             subject = f'[INFO] Step {global_step} performance'
             if self.subject != '':
                 subject = self.subject + ' | ' + subject
             self._email(subject, msg)
 
     def on_train_end(self, logs=None):
-        msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
+        msg = json.dumps({k:f'{round(v)}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
         subject = f'[INFO] Finish training'
         if self.subject != '':
             subject = self.subject + ' | ' + subject
         self._email(subject, msg)
 
     def _email(self, subject, msg):
         send_email(self.receivers, subject=subject, msg=msg, mail_host=self.mail_host,
                    mail_user=self.mail_user, mail_pwd=self.mail_pwd, sender=self.sender)
 
-
-class WandbCallback(Callback):
-    """从transformers迁移过来
-    A :class:`~transformers.TrainerCallback` that sends the logs to `Weight and Biases <https://www.wandb.com/>`__.
-
-    :param method: str, 控制是按照epoch还是step来log，默认为'epoch', 可选{'step', 'epoch'}
-    :param interval: int, log的的step间隔
-    :param watch (:obj:`str`, `optional` defaults to :obj:`"gradients"`):
-        Can be :obj:`"gradients"`, :obj:`"all"` or :obj:`"false"`. Set to :obj:`"false"` to disable gradient
-        logging or :obj:`"all"` to log gradients and parameters.
-    :param project: str，wandb的project name, 默认为bert4torch
-    :param 
-    """
-    def __init__(self, method='epoch', project='bert4torch', trial_name=None, run_name=None, watch='gradients', 
-                 interval=100, save_code=False, config=None):
-        try:
-            import wandb
-            self._wandb = wandb
-        except:
-            print("[WARNING] WandbCallback requires wandb to be installed. Run `pip install wandb`.")
-            self._wandb = None
-
-        self.method = method
-        self._initialized = False
-        # log outputs
-        self.project = project
-        if trial_name is None:
-            self.trial_name = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        if run_name is None:
-            self.run_name = self.trial_name
-        self.watch = watch
-        self.interval = interval
-        self.save_code = save_code
-        self.config = config or {}
-        self.run_id = None
-        self.metrics = set()
-
-    def define_metric(self, logs=None):
-        if getattr(self._wandb, "define_metric", None):
-            for m in logs.keys():
-                if m not in self.metrics:
-                    self._wandb.define_metric(name=m, step_metric=self.method, hidden=True if m in SKIP_METRICS else False)
-                    self.metrics.add(m)
-    def adjust_logs(self, logs, **kwargs):
-        logs_new = {**logs, **kwargs}
-        return {k:v for k,v in logs_new.items() if k not in SKIP_METRICS}
-
-    def on_epoch_end(self, global_step, epoch, logs=None):
-        if self._wandb is None:
-            return
-        if self.method == 'epoch':
-            self.define_metric(logs)
-            self._wandb.log(self.adjust_logs(logs, epoch=epoch+1))
-
-    def on_batch_end(self, global_step, local_step, logs=None):
-        if self._wandb is None:
-            return
-        if (self.method == 'step') and ((global_step+1) % self.interval == 0):
-            self.define_metric(logs)
-            self._wandb.log(self.adjust_logs(logs, step=global_step))
-        
-    def on_train_begin(self, logs=None):
-        if self._wandb is None:
-            return
-
-        self._initialized = True
-        combined_dict = {**self.trainer.__dict__, **self.config}
-
-        if hasattr(self.model, "config") and self.model.config is not None:
-            combined_dict = {**self.model.config, **combined_dict}
-        init_args = {}
-        if self.trial_name is not None:
-            run_name = self.trial_name
-            init_args["group"] = self.run_name
-        else:
-            run_name = self.run_name
-
-        if self._wandb.run is None:
-            run = self._wandb.init(project=self.project, name=run_name, save_code=self.save_code, **init_args)
-            self.run_id = run.id
-
-        # add config parameters (run may have been created manually)
-        self._wandb.config.update(combined_dict, allow_val_change=True)
-
-        # keep track of model topology and gradients, unsupported on TPU
-        if self.watch != "false":
-            self._wandb.watch(self.model, log=self.watch, log_freq=max(100, self.interval))
- 
-    def on_train_end(self, logs=None):
-        if self._wandb is None:
-            return
-
-        # transformer中的on_log
-        self._wandb.finish()
-        self._initialized = False
```

### Comparing `torch4keras-0.1.0.post2/torch4keras/model.py` & `torch4keras-0.1.1/torch4keras/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch import nn
 import torch
 from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, log_info, log_warn, log_error, print_trainable_parameters, colorful
-from torch4keras.callbacks import KerasProgbar, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, History
+from torch4keras.callbacks import KerasProgbar, SmoothMetricsCallback, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, History
 from collections import OrderedDict
 from inspect import isfunction
 import os
 import json
 import math
 
 
@@ -19,41 +19,43 @@
         self.initialize(module)
     
     def initialize(self, module=None):
         # 这里主要是为了外面调用用到
         self.global_step, self.local_step, self.total_steps, self.batch_step, self.epoch, self.steps_per_epoch, self.train_dataloader = 0, 0, 0, 0, 0, None, None
         self.resume_step, self.resume_epoch = 0, 0
         self.retain_graph = False  # loss.backward()是否保留计算图
-        self.move_to_model_device = True  # 自动把tensor转到model所在的device
+        self.move_to_model_device = False  # 自动把tensor转到model所在的device
         self.log_first_step = False  # 是否打印第一个step的数据
         self.callbacks = []
         # 传入Module实例方式
         if module is not None:
             assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
             self.module = module
         # 是否运行Callbacks，目前主要是在DDP模式下运用
         self.run_callbacks = True
 
     def compile(self, loss, optimizer, scheduler=None, clip_grad_norm=None, mixed_precision=False, metrics=None, 
-                grad_accumulation_steps=1, progbar_config=None, **kwargs):
+                grad_accumulation_steps=1, progbar_config=None, smooth_metrics_config=None, **kwargs):
         '''complile: 定义loss, optimizer, metrics等参数
         
         :param loss: loss
         :param optimizer: 优化器
         :param scheduler: scheduler
         :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
         :param mixed_precision: bool, 是否使用混合精度，默认为False
         :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
         :param grad_accumulation_steps: int, 梯度累积步数，默认为1
         :param bar: str, 使用进度条的种类，从kwargs中解析，默认为keras, 可选keras, tqdm, progressbar2
         :param progbar_config: 进度条的配置，默认是对整个epoch计算均值指标
             bar: str, 默认为keras
             stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric，指标抖动会更加明显，默认为None表示使用指标平滑
-            smooth_interval: int, 表示指标平滑时候的累计步数，默认为None表示对整个epoch进行平滑
             width: int, keras进度条下表示进度条的长度
+        :param smooth_metrics_config: 指标平滑的配置，默认为None表示采取默认平滑设置
+            stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric，指标抖动会更加明显，默认为None表示使用指标平滑
+            interval: int, 表示指标平滑时候的累计步数，默认为100
 
         :return: None
         '''
         self.criterion = loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.clip_grad_norm = clip_grad_norm
@@ -84,33 +86,39 @@
                 raise ValueError('Args metrics only support `String, Dict, Callback, List[String, Dict, Callback]` format')
 
         # 梯度累积
         self.grad_accumulation_steps = grad_accumulation_steps
 
         # 进度条参数
         self.progbar_config = progbar_config or {'bar': 'keras', 'stateful_metrics': None}
-        progbar_config_keys = ['bar', 'stateful_metrics', 'smooth_interval', 'width']
-        self.progbar_config.update({k:v for k, v in kwargs.items() if k in progbar_config_keys})  # 直接传参也可以
+        self.progbar_config.update({k:v for k, v in kwargs.items() if k in ['bar', 'stateful_metrics', 'width']})  # 直接传参
         self.progbar_config['bar'] = self.progbar_config.get('bar', 'keras')
         assert self.progbar_config['bar'] in {'keras', 'tqdm', 'progressbar2'}, \
             f'Args `bar`={self.progbar_config["bar"]} illegal, only support `keras, tqdm, progressbar2`'
 
+        # smooth_metrics参数: 默认平滑
+        if smooth_metrics_config is False:  # compile时传入False, 表示不使用平滑
+            self.smooth_metrics_config = None
+        else:
+            self.smooth_metrics_config = smooth_metrics_config or {}
+            self.smooth_metrics_config.update({k:v for k, v in kwargs.items() if k in ['stateful_metrics', 'interval', 'verbose']})  # 直接传参
+
     def print_trainable_parameters(self):
         """打印可训练的参数量"""
         print_trainable_parameters(self.unwrap_model())
 
     @property
     def device(self) -> torch.device:
         """获取model所在的device"""
         return get_parameter_device(self.unwrap_model())
         
     def _move_to_model_device(self, inputs, **input_kwargs):
         '''遍历并转移到model.device上'''
         def _to_device(tensor):
-            if isinstance(tensor, torch.Tensor) and (tensor.device != self.device):
+            if isinstance(tensor, torch.Tensor) and hasattr(self, 'device') and (tensor.device != self.device):
                 return tensor.to(self.device)
             else:
                 return tensor
 
         if self.move_to_model_device:
             if isinstance(inputs, torch.Tensor):  # tensor不展开
                 inputs = _to_device(inputs)
@@ -244,14 +252,22 @@
             elif self.progbar_config['bar'] == 'tqdm':
                 progbarlogger = TqdmProgbar(**self.progbar_config)
             elif self.progbar_config['bar'] == 'progressbar2':
                 progbarlogger = ProgressBar2Progbar(**self.progbar_config)
             else:
                 progbarlogger = KerasProgbar(**self.progbar_config)
             callbacks_.append(progbarlogger)
+
+        # 指标平滑
+        if self.smooth_metrics_config is not None:
+            if any([isinstance(i, SmoothMetricsCallback) for i in callbacks]):
+                log_warn(f'SmoothMetricsCallback already in use and args `smooth_metrics_config` will be ignored')
+            else:
+                callbacks_.append(SmoothMetricsCallback(**self.smooth_metrics_config))
+
         callbacks_  += callbacks + [history]
         self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
         callback_trainer = self
         callback_model = self.unwrap_model()
         params = {
             'epochs': self.epochs,
             'steps': self.steps_per_epoch,
@@ -351,15 +367,15 @@
                 break
         self.callbacks.on_train_end(logs)
         return history
 
     def _log_init(self):
         '''获取batch_size，主要是用于callback中的BaseLogger和Callback
         '''
-        logs = {'size': self.batch_size * self.grad_accumulation_steps}
+        logs = {}
 
         # 添加lr
         try:
             logs['lr'] = self.optimizer.param_groups[0]["lr"]
         except:
             pass
         return logs
@@ -432,65 +448,90 @@
         
         save_dir = os.path.dirname(save_path)
         os.makedirs(save_dir, exist_ok=True)
         torch.save(state_dict_raw, save_path)
         if trainable_only and (verbose > 0):
             params_all = sum(p.numel() for p in self.unwrap_model().parameters())
             params_trainable = sum(p.numel() for p in self.unwrap_model().parameters() if p.requires_grad)
-            print(f"[INFO] Only trainable parameters saved and occupy {params_trainable}/{params_all} {params_trainable/params_all:.2f}%")
+            ratio = params_trainable/params_all*100
+            log_info(f"Only trainable parameters saved and occupy {params_trainable}/{params_all}={ratio:.2f}%")
 
-    def resume_from_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None):
+    def resume_from_checkpoint(self, save_dir=None, model_path=None, optimizer_path=None, scheduler_path=None, steps_params_path=None, 
+                               mapping={}, verbose=0, **kwargs):
         '''同时加载模型、优化器、训练过程参数
 
+        :param save_dir: str, 保存目录
         :param model_path: str, 模型文件路径
         :param optimizer_path: str, 优化器文件路径
         :param scheduler_path: str, scheduler文件路径
-        :param step_params_path: str, 训练过程参数保存路径
+        :param steps_params_path: str, 训练过程参数保存路径
+        :param mapping: dict, 模型文件的mapping
         '''
+        model_path = model_path or os.path.join(save_dir, 'model.pt')
+        optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
+        scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
+        steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
+
+        verbose_str = ''
         # 加载模型权重
         if model_path:
-            self.load_weights(model_path)
+            self.load_weights(model_path, mapping=mapping)
+            verbose_str += f'Model weights successfuly resumed from {model_path}\n'
         # 加载优化器，断点续训使用
         if optimizer_path:
             state_dict = torch.load(optimizer_path, map_location='cpu')
             self.optimizer.load_state_dict(state_dict)
+            verbose_str += f'Optimizer successfuly resumed from {optimizer_path}\n'
         # 加载优化器，断点续训使用
         if scheduler_path:
             state_dict = torch.load(scheduler_path, map_location='cpu')
             self.scheduler.load_state_dict(state_dict)
+            verbose_str += f'Scheduler successfuly resumed from {scheduler_path}\n'
         # 加载训练进度参数，断点续训使用
-        self.load_steps_params(step_params_path)
+        if steps_params_path:
+            self.load_steps_params(steps_params_path)
+            verbose_str += f'Steps_params successfuly resumed from {steps_params_path}'
+        if verbose == 1:
+            print(verbose_str)
 
-    def save_to_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None, mapping={}, verbose=0):
+    def save_to_checkpoint(self, save_dir=None, model_path=None, optimizer_path=None, scheduler_path=None, steps_params_path=None, 
+                           mapping={}, trainable_only=False, verbose=0, **kwargs):
         '''同时保存模型、优化器、训练过程参数、scheduler
 
+        :param save_dir: str, 保存目录
         :param model_path: str, 模型文件路径
         :param optimizer_path: str, 优化器文件路径
         :param scheduler_path: str, scheduler文件路径
-        :param step_params_path: str, 训练过程参数保存路径
+        :param steps_params_path: str, 训练过程参数保存路径
         :param mapping: dict, 模型文件的mapping
+        :param trainable_only
         '''
+        model_path = model_path or os.path.join(save_dir, 'model.pt')
+        optimizer_path = optimizer_path or os.path.join(save_dir, 'optimizer.pt')
+        scheduler_path = scheduler_path or os.path.join(save_dir, 'scheduler.pt')
+        steps_params_path = steps_params_path or os.path.join(save_dir, 'steps_params.pt')
+
         verbose_str = ''
         if model_path:
-            self.save_weights(model_path, mapping=mapping)
-            verbose_str += f'Model weights successfuly saved to {model_path}.\n'
+            self.save_weights(model_path, mapping=mapping, trainable_only=trainable_only)
+            verbose_str += f'Model weights successfuly saved to {model_path}\n'
         if optimizer_path:
             save_dir = os.path.dirname(optimizer_path)
             os.makedirs(save_dir, exist_ok=True)
             torch.save(self.optimizer.state_dict(), optimizer_path)
-            verbose_str += f'Optimizer successfuly saved to {optimizer_path}.\n'
+            verbose_str += f'Optimizer successfuly saved to {optimizer_path}\n'
         if scheduler_path and (self.scheduler is not None):
             save_dir = os.path.dirname(scheduler_path)
             os.makedirs(save_dir, exist_ok=True)
             torch.save(self.scheduler.state_dict(), scheduler_path)
-            verbose_str += f'Scheduler successfuly saved to {scheduler_path}.\n'
-        if step_params_path:
-            self.save_steps_params(step_params_path)
-            verbose_str += f'Steps_params successfuly saved to {step_params_path}.\n'
-        if verbose != 0:
+            verbose_str += f'Scheduler successfuly saved to {scheduler_path}\n'
+        if steps_params_path:
+            self.save_steps_params(steps_params_path)
+            verbose_str += f'Steps_params successfuly saved to {steps_params_path}'
+        if verbose == 1:
             print(verbose_str)
 
     def unwrap_model(self):
         '''返回nn.Module模块
         '''
         if isinstance(self, nn.Module): return self
         return self.module if hasattr(self, 'module') else self
```

### Comparing `torch4keras-0.1.0.post2/torch4keras/snippets.py` & `torch4keras-0.1.1/torch4keras/snippets.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import inspect
 from packaging import version
 from torch.utils.data import Dataset, IterableDataset
 import os
 import random
 import traceback
+import copy
 
 try:
     from sklearn.metrics import roc_auc_score
 except ImportError:
     roc_auc_score = None
         
 def take_along_dim(input_tensor, indices, dim=None):
@@ -442,8 +443,88 @@
     best_num = min(best_num, len(scores))
     topk_idx = (-np.asarray(scores)).argsort()[:best_num]
 
     topk_idx_str = ",".join(map(str, topk_idx))
     log_info(f"SET CUDA_VISIBLE_DEVICES={topk_idx_str}")
     os.environ["CUDA_VISIBLE_DEVICES"] = topk_idx_str
 
-    return topk_idx_str
+    return topk_idx_str
+
+
+def watch_system_state(log_dir, gpu_id_list=None, pid=None):
+    '''监控system的状态
+    
+    :param log_dir: str, tensorboard的地址
+    :param gpu_id_list: List[int], 监控的gpu
+    :param pid: int, 监控的进程号
+    '''
+    import psutil
+    import pynvml
+    from tensorboardX import SummaryWriter
+
+    pynvml.nvmlInit()
+    os.makedirs(log_dir, exist_ok=True)
+    tb_writer = SummaryWriter(log_dir=str(log_dir))  # prepare summary writer
+
+    pre_time_int = int(time.time())
+    pre_time = time.time()
+    pid = None or os.getpid()
+    p = psutil.Process(pid)
+    G = 1024*1024*1024
+
+    pre_read = p.io_counters().read_bytes
+    pre_write = p.io_counters().write_bytes
+    time_str_init = int(time.time())
+
+    log_info("Watching System Info")
+    while True:
+        time.sleep(1)
+        now_time = time.time()
+        time_str = int(now_time) - time_str_init
+        p = psutil.Process(pid)
+
+        # CPU使用情况
+        tb_writer.add_scalar(f"CPU_pid_{pid}/cpu_percent", p.cpu_percent(interval=0.5), time_str)
+
+        # 内存使用情况
+        tb_writer.add_scalar(f"Memory_pid_{pid}/memory_percent", p.memory_percent(), time_str)
+        tb_writer.add_scalar(f"Memory_pid_{pid}/RSS G_byte", p.memory_info().rss/G, time_str)
+        tb_writer.add_scalar(f"Memory_pid_{pid}/VMS G_byte", p.memory_info().vms/G, time_str)
+
+        # 进程IO信息
+        data = p.io_counters()
+        tb_writer.add_scalar(f"IO_pid_{pid}/read M_byte", data.read_bytes/1024, time_str)
+        tb_writer.add_scalar(f"IO_pid_{pid}/write M_byte", data.write_bytes/1024, time_str)
+        if (time_str - pre_time_int)%5 == 0:
+            tb_writer.add_scalar(f"IO_pid_{pid}/readRate M_byte_s", (data.read_bytes - pre_read)/(now_time-pre_time)/1024, time_str)
+            tb_writer.add_scalar(f"IO_pid_{pid}/writeRate M_byte_s", (data.write_bytes - pre_write)/(now_time-pre_time)/1024, time_str)
+            pre_read = data.read_bytes
+            pre_write = data.write_bytes
+            pre_time = now_time
+
+        tesorboard_info_list = []
+        if gpu_id_list is None:
+            deviceCount = pynvml.nvmlDeviceGetCount()
+            device_list = [i for i in range(deviceCount)]
+        else:
+            device_list = gpu_id_list
+
+        tesorboard_info_list = []
+        for i in device_list:
+            tesorboard_info = {}
+            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+            tesorboard_info['gpu_name'] = pynvml.nvmlDeviceGetName(handle)
+            meminfo = pynvml.nvmlDeviceGetMemoryInfo(handle)
+            tesorboard_info['gpu_mem_used'] = meminfo.used/G
+            UTIL = pynvml.nvmlDeviceGetUtilizationRates(handle)
+            tesorboard_info['gpu_gpu_util'] = UTIL.gpu
+            tesorboard_info['gpu_mem_util'] = UTIL.memory
+            tesorboard_info_list.append(copy.deepcopy(tesorboard_info))
+        for tesorboard_info,i in zip(tesorboard_info_list, device_list):
+            tb_writer.add_scalar(f'GPU{i}/gpu_mem_used unit_G', tesorboard_info['gpu_mem_used'], time_str)
+            tb_writer.add_scalar(f'GPU{i}/gpu_gpu_util', tesorboard_info['gpu_gpu_util'], time_str)
+            tb_writer.add_scalar(f'GPU{i}/gpu_mem_util', tesorboard_info['gpu_mem_util'], time_str)
+
+    tb_writer.close()
+    pynvml.nvmlShutdown()
+
+    return
```

### Comparing `torch4keras-0.1.0.post2/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.1.1/torch4keras.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.1.0.post2
+Version: 0.1.1
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -87,14 +87,15 @@
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230802**: 增加指标平滑的SmoothMetricCallback，统一管理指标平滑的问题, 增加SKIP_METRICS，NO_SMOOTH_METRICS，ROUND_PRECISION，默认对指标会进行平滑，修改tensorboard和wandb的callback, 允许跳过nan的指标, Tensorboard可以记录gpu等系统信息
 - **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
 - **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
```

