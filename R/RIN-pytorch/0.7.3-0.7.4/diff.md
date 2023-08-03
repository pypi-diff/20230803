# Comparing `tmp/RIN-pytorch-0.7.3.tar.gz` & `tmp/RIN-pytorch-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIN-pytorch-0.7.3.tar", last modified: Tue Jun 20 19:50:50 2023, max compression
+gzip compressed data, was "RIN-pytorch-0.7.4.tar", last modified: Thu Aug  3 14:58:58 2023, max compression
```

## Comparing `RIN-pytorch-0.7.3.tar` & `RIN-pytorch-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.545798 RIN-pytorch-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 19:50:50.000000 RIN-pytorch-0.7.3/RIN_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:50:50.541798 RIN-pytorch-0.7.3/rin_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/rin_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32662 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/rin_pytorch/rin_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:50:50.545798 RIN-pytorch-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 19:50:26.000000 RIN-pytorch-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:58.916451 RIN-pytorch-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 14:58:49.000000 RIN-pytorch-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 14:58:58.912451 RIN-pytorch-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-08-03 14:58:49.000000 RIN-pytorch-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:58.912451 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 14:58:58.000000 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-03 14:58:58.000000 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:58:58.000000 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 14:58:58.000000 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:58:58.000000 RIN-pytorch-0.7.4/RIN_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:58.912451 RIN-pytorch-0.7.4/rin_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 14:58:49.000000 RIN-pytorch-0.7.4/rin_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33174 2023-08-03 14:58:49.000000 RIN-pytorch-0.7.4/rin_pytorch/rin_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:58:58.916451 RIN-pytorch-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 14:58:49.000000 RIN-pytorch-0.7.4/setup.py
```

### Comparing `RIN-pytorch-0.7.3/LICENSE` & `RIN-pytorch-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RIN-pytorch-0.7.3/PKG-INFO` & `RIN-pytorch-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIN-pytorch
-Version: 0.7.3
+Version: 0.7.4
 Summary: RIN - Recurrent Interface Network - Pytorch
 Home-page: https://github.com/lucidrains/RIN-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,denoising diffusion,image and video generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RIN-pytorch-0.7.3/README.md` & `RIN-pytorch-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `RIN-pytorch-0.7.3/RIN_pytorch.egg-info/PKG-INFO` & `RIN-pytorch-0.7.4/RIN_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIN-pytorch
-Version: 0.7.3
+Version: 0.7.4
 Summary: RIN - Recurrent Interface Network - Pytorch
 Home-page: https://github.com/lucidrains/RIN-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanism,denoising diffusion,image and video generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RIN-pytorch-0.7.3/rin_pytorch/rin_pytorch.py` & `RIN-pytorch-0.7.4/rin_pytorch/rin_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from einops import rearrange, reduce, repeat
 from einops.layers.torch import Rearrange
 
 from PIL import Image
 from tqdm.auto import tqdm
 from ema_pytorch import EMA
 
-from accelerate import Accelerator
+from accelerate import Accelerator, DistributedDataParallelKwargs
 
 # helpers functions
 
 def exists(x):
     return x is not None
 
 def identity(x):
@@ -909,15 +909,16 @@
         split_batches = True,
         convert_image_to = None
     ):
         super().__init__()
 
         self.accelerator = Accelerator(
             split_batches = split_batches,
-            mixed_precision = 'fp16' if fp16 else 'no'
+            mixed_precision = 'fp16' if fp16 else 'no',
+            kwargs_handlers = [DistributedDataParallelKwargs(find_unused_parameters=True)]
         )
 
         self.accelerator.native_amp = amp
 
         self.model = diffusion_model
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
@@ -940,19 +941,22 @@
 
         # optimizer
 
         self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = betas)
 
         # for logging results in a folder periodically
 
+        self.results_folder = Path(results_folder)
+
+        if self.accelerator.is_local_main_process:
+            self.results_folder.mkdir(exist_ok = True)
+
         if self.accelerator.is_main_process:
             self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
 
-            self.results_folder = Path(results_folder)
-            self.results_folder.mkdir(exist_ok = True)
 
         # step counter state
 
         self.step = 0
 
         # prepare model, dataloader, optimizer with accelerator
 
@@ -976,15 +980,17 @@
         data = torch.load(str(self.results_folder / f'model-{milestone}.pt'))
 
         model = self.accelerator.unwrap_model(self.model)
         model.load_state_dict(data['model'])
 
         self.step = data['step']
         self.opt.load_state_dict(data['opt'])
-        self.ema.load_state_dict(data['ema'])
+
+        if self.accelerator.is_main_process:
+            self.ema.load_state_dict(data['ema'])
 
         if exists(self.accelerator.scaler) and exists(data['scaler']):
             self.accelerator.scaler.load_state_dict(data['scaler'])
 
     def train(self):
         accelerator = self.accelerator
         device = accelerator.device
@@ -994,43 +1000,50 @@
             while self.step < self.train_num_steps:
 
                 total_loss = 0.
 
                 for _ in range(self.gradient_accumulate_every):
                     data = next(self.dl).to(device)
 
-                    with self.accelerator.autocast():
+                    with accelerator.autocast():
                         loss = self.model(data)
                         loss = loss / self.gradient_accumulate_every
                         total_loss += loss.item()
 
-                    self.accelerator.backward(loss)
+                    accelerator.backward(loss)
 
                 pbar.set_description(f'loss: {total_loss:.4f}')
 
                 accelerator.wait_for_everyone()
 
                 self.opt.step()
                 self.opt.zero_grad()
 
                 accelerator.wait_for_everyone()
 
-                if accelerator.is_main_process:
-                    self.ema.to(device)
-                    self.ema.update()
-
-                    if self.step != 0 and self.step % self.save_and_sample_every == 0:
-                        self.ema.ema_model.eval()
-
-                        with torch.no_grad():
-                            milestone = self.step // self.save_and_sample_every
-                            batches = num_to_groups(self.num_samples, self.batch_size)
-                            all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
+                # save milestone on every local main process, sample only on global main process
+
+                if accelerator.is_local_main_process:
+                    milestone = self.step // self.save_and_sample_every
+                    save_and_sample = self.step != 0 and self.step % self.save_and_sample_every == 0
+                    
+                    if accelerator.is_main_process:
+                        self.ema.to(device)
+                        self.ema.update()
+
+                        if save_and_sample:
+                            self.ema.ema_model.eval()
+
+                            with torch.no_grad():
+                                batches = num_to_groups(self.num_samples, self.batch_size)
+                                all_images_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
+
+                            all_images = torch.cat(all_images_list, dim = 0)
+                            utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
 
-                        all_images = torch.cat(all_images_list, dim = 0)
-                        utils.save_image(all_images, str(self.results_folder / f'sample-{milestone}.png'), nrow = int(math.sqrt(self.num_samples)))
+                    if save_and_sample:
                         self.save(milestone)
 
                 self.step += 1
                 pbar.update(1)
 
         accelerator.print('training complete')
```

### Comparing `RIN-pytorch-0.7.3/setup.py` & `RIN-pytorch-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'RIN-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.7.3',
+  version = '0.7.4',
   license='MIT',
   description = 'RIN - Recurrent Interface Network - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/RIN-pytorch',
   keywords = [
```

