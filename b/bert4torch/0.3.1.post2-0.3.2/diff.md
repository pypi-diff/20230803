# Comparing `tmp/bert4torch-0.3.1.post2.tar.gz` & `tmp/bert4torch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.3.1.post2.tar", last modified: Tue Jul 25 16:14:03 2023, max compression
+gzip compressed data, was "bert4torch-0.3.2.tar", last modified: Thu Aug  3 16:08:07 2023, max compression
```

## Comparing `bert4torch-0.3.1.post2.tar` & `bert4torch-0.3.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.875301 bert4torch-0.3.1.post2/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.1.post2/LICENSE
--rw-rw-rw-   0        0        0    27580 2023-07-25 16:14:03.874314 bert4torch-0.3.1.post2/PKG-INFO
--rw-rw-rw-   0        0        0    27322 2023-07-25 16:13:19.000000 bert4torch-0.3.1.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.831302 bert4torch-0.3.1.post2/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.1.post2/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.1.post2/bert4torch/activations.py
--rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    40539 2023-07-19 13:35:56.000000 bert4torch-0.3.1.post2/bert4torch/generation.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.846301 bert4torch-0.3.1.post2/bert4torch/layers/
--rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/__init__.py
--rw-rw-rw-   0        0        0    25499 2023-07-19 14:29:14.000000 bert4torch-0.3.1.post2/bert4torch/layers/attention.py
--rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/core.py
--rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/crf.py
--rw-rw-rw-   0        0        0     4738 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/layers/global_point.py
--rw-rw-rw-   0        0        0    17536 2023-07-22 13:42:00.000000 bert4torch-0.3.1.post2/bert4torch/layers/misc.py
--rw-rw-rw-   0        0        0    13868 2023-07-19 14:29:40.000000 bert4torch-0.3.1.post2/bert4torch/layers/position_encoding.py
--rw-rw-rw-   0        0        0    16281 2023-07-21 13:58:57.000000 bert4torch-0.3.1.post2/bert4torch/layers/transformer_block.py
--rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.1.post2/bert4torch/losses.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.872309 bert4torch-0.3.1.post2/bert4torch/models/
--rw-rw-rw-   0        0        0     7712 2023-07-18 14:14:06.000000 bert4torch-0.3.1.post2/bert4torch/models/__init__.py
--rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/albert.py
--rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/bart.py
--rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.1.post2/bert4torch/models/base.py
--rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/bert.py
--rw-rw-rw-   0        0        0      760 2023-07-22 15:51:05.000000 bert4torch-0.3.1.post2/bert4torch/models/bloom.py
--rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/deberta.py
--rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/electra.py
--rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/erinie.py
--rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/gau_alpha.py
--rw-rw-rw-   0        0        0    10808 2023-07-22 14:30:17.000000 bert4torch-0.3.1.post2/bert4torch/models/glm.py
--rw-rw-rw-   0        0        0     4566 2023-07-22 13:03:58.000000 bert4torch-0.3.1.post2/bert4torch/models/gpt.py
--rw-rw-rw-   0        0        0     2294 2023-07-22 13:18:50.000000 bert4torch-0.3.1.post2/bert4torch/models/llama.py
--rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/nezha.py
--rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/roformer.py
--rw-rw-rw-   0        0        0    10336 2023-07-21 13:58:57.000000 bert4torch-0.3.1.post2/bert4torch/models/t5.py
--rw-rw-rw-   0        0        0     6769 2023-07-22 13:26:18.000000 bert4torch-0.3.1.post2/bert4torch/models/transformer.py
--rw-rw-rw-   0        0        0     9219 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/models/transformer_xl.py
--rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/uie.py
--rw-rw-rw-   0        0        0     4808 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/models/xlnet.py
--rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.1.post2/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.1.post2/bert4torch/quantization.py
--rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.1.post2/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.1.post2/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.837291 bert4torch-0.3.1.post2/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    27580 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 16:14:03.875301 bert4torch-0.3.1.post2/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-07-25 16:12:24.000000 bert4torch-0.3.1.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:08:07.692382 bert4torch-0.3.2/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    27910 2023-08-03 16:08:07.691377 bert4torch-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27658 2023-08-03 16:02:02.000000 bert4torch-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 16:08:07.618391 bert4torch-0.3.2/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.2/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.2/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    40539 2023-07-19 13:35:56.000000 bert4torch-0.3.2/bert4torch/generation.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:08:07.658393 bert4torch-0.3.2/bert4torch/layers/
+-rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/layers/__init__.py
+-rw-rw-rw-   0        0        0    25499 2023-07-19 14:29:14.000000 bert4torch-0.3.2/bert4torch/layers/attention.py
+-rw-rw-rw-   0        0        0     8515 2023-07-26 13:50:33.000000 bert4torch-0.3.2/bert4torch/layers/core.py
+-rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/layers/crf.py
+-rw-rw-rw-   0        0        0     4738 2023-07-20 15:32:46.000000 bert4torch-0.3.2/bert4torch/layers/global_point.py
+-rw-rw-rw-   0        0        0    17536 2023-07-22 13:42:00.000000 bert4torch-0.3.2/bert4torch/layers/misc.py
+-rw-rw-rw-   0        0        0    13868 2023-07-19 14:29:40.000000 bert4torch-0.3.2/bert4torch/layers/position_encoding.py
+-rw-rw-rw-   0        0        0    16281 2023-07-21 13:58:57.000000 bert4torch-0.3.2/bert4torch/layers/transformer_block.py
+-rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.2/bert4torch/losses.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:08:07.689376 bert4torch-0.3.2/bert4torch/models/
+-rw-rw-rw-   0        0        0     7712 2023-07-18 14:14:06.000000 bert4torch-0.3.2/bert4torch/models/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/albert.py
+-rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/bart.py
+-rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.2/bert4torch/models/base.py
+-rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.2/bert4torch/models/bert.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 15:51:05.000000 bert4torch-0.3.2/bert4torch/models/bloom.py
+-rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/deberta.py
+-rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/electra.py
+-rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/erinie.py
+-rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.2/bert4torch/models/gau_alpha.py
+-rw-rw-rw-   0        0        0    10808 2023-07-22 14:30:17.000000 bert4torch-0.3.2/bert4torch/models/glm.py
+-rw-rw-rw-   0        0        0     4566 2023-07-22 13:03:58.000000 bert4torch-0.3.2/bert4torch/models/gpt.py
+-rw-rw-rw-   0        0        0     2294 2023-07-22 13:18:50.000000 bert4torch-0.3.2/bert4torch/models/llama.py
+-rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/nezha.py
+-rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.2/bert4torch/models/roformer.py
+-rw-rw-rw-   0        0        0    10336 2023-07-21 13:58:57.000000 bert4torch-0.3.2/bert4torch/models/t5.py
+-rw-rw-rw-   0        0        0     6769 2023-07-22 13:26:18.000000 bert4torch-0.3.2/bert4torch/models/transformer.py
+-rw-rw-rw-   0        0        0     9219 2023-07-20 15:32:46.000000 bert4torch-0.3.2/bert4torch/models/transformer_xl.py
+-rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.2/bert4torch/models/uie.py
+-rw-rw-rw-   0        0        0     4808 2023-07-20 15:32:46.000000 bert4torch-0.3.2/bert4torch/models/xlnet.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.2/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.2/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.2/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.2/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-08-03 16:08:07.632375 bert4torch-0.3.2/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    27910 2023-08-03 16:08:07.000000 bert4torch-0.3.2/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-08-03 16:08:07.000000 bert4torch-0.3.2/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 16:08:07.000000 bert4torch-0.3.2/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-03 16:08:07.000000 bert4torch-0.3.2/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-03 16:08:07.000000 bert4torch-0.3.2/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 16:08:07.692382 bert4torch-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-08-03 16:00:00.000000 bert4torch-0.3.2/setup.py
```

### Comparing `bert4torch-0.3.1.post2/LICENSE` & `bert4torch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/PKG-INFO` & `bert4torch-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.3.1.post2
+Version: 0.3.2
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,15 +63,15 @@
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
 |          功能                | bert4torch |  transformers | 备注 |
-|-----------------------------|------------|:--------------|--------|
+|-----------------------------|------------|----------------|--------|
 |训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
 |分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
 |各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
 |大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
 |大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
 |丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
 |代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
@@ -82,60 +82,56 @@
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
-<details><summary><b>点击查看</b></summary>
+<details><summary><b>4.1 版本历史</b></summary>
 
-**版本说明**
-- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
-- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
-- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
-- **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
-- **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
-- **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
-- **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
-- **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
-- **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
-- **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
-- **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
-- **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
-- **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
-- **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
-- **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
-- **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
-- **v0.1.3**：20220409 初始版本
-
-**版本对应关系**
-
-| bert4torch版本 | torch4keras版本 |
-| ---------------- | ----------------- |
-| 0.3.1.post2    | 0.1.0.post2     |
-| 0.3.0          | 0.0.9           |
-| 0.2.9          | 0.0.8           |
-| 0.2.8          | 0.0.7.post3     |
-| 0.2.7.post2    | 0.0.6           |
-| 0.2.7          | 0.0.6           |
-| 0.2.6          | 0.0.5           |
-| 0.2.5          | 0.0.4           |
-| 0.2.4          | 0.0.3.post2     |
-| 0.2.3          | 0.0.2           |
-| <0.2.3         | ——            |
+|更新日期| bert4torch版本 | torch4keras版本 | 版本说明 |
+|------| ---------------- | ----------------- |----------- |
+|20230804| 0.3.2          | 0.1.1     |修改依赖的torch4keras, 主要是进度条和logger, tensorboard的同步|
+|20230726| 0.3.1.post2    | 0.1.0.post2     |修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)|
+|20230716| 0.3.0          | 0.0.9           |修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan|
+|20230705| 0.2.9          | 0.0.8           |使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调|
+|20230518| 0.2.8          | 0.0.7.post3     |1）新增模型: 增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; <br/>2）generation: 生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；<br/>3）其他: 修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段|
+|20230310| 0.2.7.post2    | 0.0.6           |增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug|
+|20230213| 0.2.7          | 0.0.6           |修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback|
+|20221231| 0.2.6          | 0.0.5           |build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size|
+|20221127| 0.2.5          | 0.0.4           |对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置|
+|20221120| 0.2.4          | 0.0.3.post2     |删除SpTokenizer基类中的rematch, 增加deberta_v2模型|
+|20221023| 0.2.3          | 0.0.2           |虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint|
+|20220922| 0.2.2         | ——            |修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)|
+|20220905| 0.2.1         | ——            |兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志|
+|20220823| 0.2.0         | ——            |兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply|
+|20220808| 0.1.9         | ——            |增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量|
+|20220717| 0.1.8         | ——            |修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题|
+|20220710| 0.1.7         | ——            |增加EarlyStop，CRF中自带转bool类型|
+|20220605| 0.1.6         | ——            |增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug|
+|20220504| 0.1.5         | ——            |增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)|
+|20220421| 0.1.4         | ——            |增加了VAT，修复了linux下apply_embedding返回项有问题的情况|
+|20220409| 0.1.3         | ——            |初始版本|
 
-</details>
 
+</details>
 
 ## 5. 更新历史：
-<details><summary><b>点击查看</b></summary>
 
+<details><summary><b>5.1 即将更新</b></summary>
+
+- [✓] llama系列的微调
+- [ ] 大模型的deepspeed使用
+- [ ] chatgpt三阶段的训练
+
+</details>
+
+<details><summary><b>5.2 更新历史</b></summary>
+
+- **20230729**：增加llama-2的微调
 - **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
@@ -166,61 +162,61 @@
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
 </details>
 
 ## 6. 预训练权重
 
-- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
-| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
-| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
-| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
-| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
-| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-base.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
 | roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
 | roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
-| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_simbert.py) |
 | simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
-| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_GAU_alpha.py) |
 | wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
 | nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
-| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
-| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
-| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
-| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
-| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
-| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt_CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
-| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
-| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
-| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| llama | facebook| [github](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| llama-2 | facebook| [github](https://github.com/facebookresearch/llama), [7b](https://huggingface.co/meta-llama/Llama-2-7b-hf), [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [13b](https://huggingface.co/meta-llama/Llama-2-13b-hf), [13b-chat](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+|chinese_llama_alpaca|Yiming Cui|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bloom.py) |
 
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
@@ -243,15 +239,15 @@
   <tbody>
     <tr align="center" >
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
-         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo"><img width="200" height="300" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信群</a> 
       </td>
     </tr>
   </tbody>
 </table>
 
 - Star History Chart
```

### Comparing `bert4torch-0.3.1.post2/README.md` & `bert4torch-0.3.2/bert4torch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.3.2
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -53,15 +63,15 @@
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
 |          功能                | bert4torch |  transformers | 备注 |
-|-----------------------------|------------|:--------------|--------|
+|-----------------------------|------------|----------------|--------|
 |训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
 |分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
 |各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
 |大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
 |大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
 |丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
 |代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
@@ -72,60 +82,56 @@
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
-<details><summary><b>点击查看</b></summary>
+<details><summary><b>4.1 版本历史</b></summary>
 
-**版本说明**
-- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
-- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
-- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
-- **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
-- **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
-- **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
-- **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
-- **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
-- **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
-- **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
-- **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
-- **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
-- **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
-- **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
-- **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
-- **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
-- **v0.1.3**：20220409 初始版本
-
-**版本对应关系**
-
-| bert4torch版本 | torch4keras版本 |
-| ---------------- | ----------------- |
-| 0.3.1.post2    | 0.1.0.post2     |
-| 0.3.0          | 0.0.9           |
-| 0.2.9          | 0.0.8           |
-| 0.2.8          | 0.0.7.post3     |
-| 0.2.7.post2    | 0.0.6           |
-| 0.2.7          | 0.0.6           |
-| 0.2.6          | 0.0.5           |
-| 0.2.5          | 0.0.4           |
-| 0.2.4          | 0.0.3.post2     |
-| 0.2.3          | 0.0.2           |
-| <0.2.3         | ——            |
+|更新日期| bert4torch版本 | torch4keras版本 | 版本说明 |
+|------| ---------------- | ----------------- |----------- |
+|20230804| 0.3.2          | 0.1.1     |修改依赖的torch4keras, 主要是进度条和logger, tensorboard的同步|
+|20230726| 0.3.1.post2    | 0.1.0.post2     |修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)|
+|20230716| 0.3.0          | 0.0.9           |修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan|
+|20230705| 0.2.9          | 0.0.8           |使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调|
+|20230518| 0.2.8          | 0.0.7.post3     |1）新增模型: 增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; <br/>2）generation: 生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；<br/>3）其他: 修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段|
+|20230310| 0.2.7.post2    | 0.0.6           |增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug|
+|20230213| 0.2.7          | 0.0.6           |修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback|
+|20221231| 0.2.6          | 0.0.5           |build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size|
+|20221127| 0.2.5          | 0.0.4           |对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置|
+|20221120| 0.2.4          | 0.0.3.post2     |删除SpTokenizer基类中的rematch, 增加deberta_v2模型|
+|20221023| 0.2.3          | 0.0.2           |虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint|
+|20220922| 0.2.2         | ——            |修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)|
+|20220905| 0.2.1         | ——            |兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志|
+|20220823| 0.2.0         | ——            |兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply|
+|20220808| 0.1.9         | ——            |增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量|
+|20220717| 0.1.8         | ——            |修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题|
+|20220710| 0.1.7         | ——            |增加EarlyStop，CRF中自带转bool类型|
+|20220605| 0.1.6         | ——            |增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug|
+|20220504| 0.1.5         | ——            |增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)|
+|20220421| 0.1.4         | ——            |增加了VAT，修复了linux下apply_embedding返回项有问题的情况|
+|20220409| 0.1.3         | ——            |初始版本|
 
-</details>
 
+</details>
 
 ## 5. 更新历史：
-<details><summary><b>点击查看</b></summary>
 
+<details><summary><b>5.1 即将更新</b></summary>
+
+- [✓] llama系列的微调
+- [ ] 大模型的deepspeed使用
+- [ ] chatgpt三阶段的训练
+
+</details>
+
+<details><summary><b>5.2 更新历史</b></summary>
+
+- **20230729**：增加llama-2的微调
 - **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
@@ -156,61 +162,61 @@
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
 </details>
 
 ## 6. 预训练权重
 
-- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
-| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
-| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
-| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
-| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
-| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-base.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
 | roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
 | roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
-| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_simbert.py) |
 | simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
-| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_GAU_alpha.py) |
 | wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
 | nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
-| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
-| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
-| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
-| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
-| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
-| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt_CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
-| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
-| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
-| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| llama | facebook| [github](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| llama-2 | facebook| [github](https://github.com/facebookresearch/llama), [7b](https://huggingface.co/meta-llama/Llama-2-7b-hf), [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [13b](https://huggingface.co/meta-llama/Llama-2-13b-hf), [13b-chat](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+|chinese_llama_alpaca|Yiming Cui|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bloom.py) |
 
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
@@ -233,15 +239,15 @@
   <tbody>
     <tr align="center" >
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
-         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo"><img width="200" height="300" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信群</a> 
       </td>
     </tr>
   </tbody>
 </table>
 
 - Star History Chart
@@ -251,8 +257,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.3.1.post2/bert4torch/activations.py` & `bert4torch-0.3.2/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/callbacks.py` & `bert4torch-0.3.2/bert4torch/callbacks.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/generation.py` & `bert4torch-0.3.2/bert4torch/generation.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/attention.py` & `bert4torch-0.3.2/bert4torch/layers/attention.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/core.py` & `bert4torch-0.3.2/bert4torch/layers/core.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/crf.py` & `bert4torch-0.3.2/bert4torch/layers/crf.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/global_point.py` & `bert4torch-0.3.2/bert4torch/layers/global_point.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/misc.py` & `bert4torch-0.3.2/bert4torch/layers/misc.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/position_encoding.py` & `bert4torch-0.3.2/bert4torch/layers/position_encoding.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/layers/transformer_block.py` & `bert4torch-0.3.2/bert4torch/layers/transformer_block.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/losses.py` & `bert4torch-0.3.2/bert4torch/losses.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/__init__.py` & `bert4torch-0.3.2/bert4torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/albert.py` & `bert4torch-0.3.2/bert4torch/models/albert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/bart.py` & `bert4torch-0.3.2/bert4torch/models/bart.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/base.py` & `bert4torch-0.3.2/bert4torch/models/base.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/bert.py` & `bert4torch-0.3.2/bert4torch/models/bert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/bloom.py` & `bert4torch-0.3.2/bert4torch/models/bloom.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/deberta.py` & `bert4torch-0.3.2/bert4torch/models/deberta.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/electra.py` & `bert4torch-0.3.2/bert4torch/models/electra.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/erinie.py` & `bert4torch-0.3.2/bert4torch/models/erinie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/gau_alpha.py` & `bert4torch-0.3.2/bert4torch/models/gau_alpha.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/glm.py` & `bert4torch-0.3.2/bert4torch/models/glm.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/gpt.py` & `bert4torch-0.3.2/bert4torch/models/gpt.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/llama.py` & `bert4torch-0.3.2/bert4torch/models/llama.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/roformer.py` & `bert4torch-0.3.2/bert4torch/models/roformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/t5.py` & `bert4torch-0.3.2/bert4torch/models/t5.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/transformer.py` & `bert4torch-0.3.2/bert4torch/models/transformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/transformer_xl.py` & `bert4torch-0.3.2/bert4torch/models/transformer_xl.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/uie.py` & `bert4torch-0.3.2/bert4torch/models/uie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/models/xlnet.py` & `bert4torch-0.3.2/bert4torch/models/xlnet.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/optimizers.py` & `bert4torch-0.3.2/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/quantization.py` & `bert4torch-0.3.2/bert4torch/quantization.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/snippets.py` & `bert4torch-0.3.2/bert4torch/snippets.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch/tokenizers.py` & `bert4torch-0.3.2/bert4torch/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.3.1.post2
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -63,15 +53,15 @@
   Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
   test_acc: 0.98280. best_test_acc: 0.98280
 
   2022-10-28 23:16:44 - Finish Training
   ```
 
 |          功能                | bert4torch |  transformers | 备注 |
-|-----------------------------|------------|:--------------|--------|
+|-----------------------------|------------|----------------|--------|
 |训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
 |分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
 |各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
 |大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
 |大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
 |丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
 |代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
@@ -82,60 +72,56 @@
 
 - [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
-<details><summary><b>点击查看</b></summary>
+<details><summary><b>4.1 版本历史</b></summary>
 
-**版本说明**
-- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
-- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
-- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
-- **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
-- **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
-- **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
-- **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
-- **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
-- **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
-- **v0.2.2**：20220922 修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)
-- **v0.2.1**：20220905 兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志
-- **v0.2.0**：20220823 兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply
-- **v0.1.9**：20220808 增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量
-- **v0.1.8**：20220717 修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题
-- **v0.1.7**：20220710 增加EarlyStop，CRF中自带转bool类型
-- **v0.1.6**：20220605 增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug
-- **v0.1.5**：20220504 增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)
-- **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
-- **v0.1.3**：20220409 初始版本
-
-**版本对应关系**
-
-| bert4torch版本 | torch4keras版本 |
-| ---------------- | ----------------- |
-| 0.3.1.post2    | 0.1.0.post2     |
-| 0.3.0          | 0.0.9           |
-| 0.2.9          | 0.0.8           |
-| 0.2.8          | 0.0.7.post3     |
-| 0.2.7.post2    | 0.0.6           |
-| 0.2.7          | 0.0.6           |
-| 0.2.6          | 0.0.5           |
-| 0.2.5          | 0.0.4           |
-| 0.2.4          | 0.0.3.post2     |
-| 0.2.3          | 0.0.2           |
-| <0.2.3         | ——            |
+|更新日期| bert4torch版本 | torch4keras版本 | 版本说明 |
+|------| ---------------- | ----------------- |----------- |
+|20230804| 0.3.2          | 0.1.1     |修改依赖的torch4keras, 主要是进度条和logger, tensorboard的同步|
+|20230726| 0.3.1.post2    | 0.1.0.post2     |修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)|
+|20230716| 0.3.0          | 0.0.9           |修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan|
+|20230705| 0.2.9          | 0.0.8           |使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调|
+|20230518| 0.2.8          | 0.0.7.post3     |1）新增模型: 增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; <br/>2）generation: 生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；<br/>3）其他: 修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段|
+|20230310| 0.2.7.post2    | 0.0.6           |增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug|
+|20230213| 0.2.7          | 0.0.6           |修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback|
+|20221231| 0.2.6          | 0.0.5           |build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size|
+|20221127| 0.2.5          | 0.0.4           |对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置|
+|20221120| 0.2.4          | 0.0.3.post2     |删除SpTokenizer基类中的rematch, 增加deberta_v2模型|
+|20221023| 0.2.3          | 0.0.2           |虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint|
+|20220922| 0.2.2         | ——            |修复t5的norm_mode问题，允许hidden_size不整除num_attention_heads，支持多个schedule(如同时ema+warmup)|
+|20220905| 0.2.1         | ——            |兼容torch<=1.7.1的torch.div无rounding_mode，增加自定义metrics，支持断点续训，增加默认Logger和Tensorboard日志|
+|20220823| 0.2.0         | ——            |兼容torch1.9.0的缺失take_along_dim，修复bart中位置向量514的问题，修复Sptokenizer对符号不转换，打印Epoch开始的时间戳，增加parallel_apply|
+|20220808| 0.1.9         | ——            |增加mixup/manifold_mixup/temporal_ensembling策略，修复pgd策略param.grad为空的问题，修改tokenizer支持批量|
+|20220717| 0.1.8         | ——            |修复原来CRF训练中loss陡增的问题，修复xlnet的token_type_ids输入显存占用大的问题|
+|20220710| 0.1.7         | ——            |增加EarlyStop，CRF中自带转bool类型|
+|20220605| 0.1.6         | ——            |增加transformer_xl、xlnet、t5_pegasus模型，prompt、预训练等示例，支持增加embedding输入，EMA策略，修复tokenizer和sinusoid的bug|
+|20220504| 0.1.5         | ——            |增加GAU-alpha，混合梯度，梯度裁剪，单机多卡(DP、DDP)|
+|20220421| 0.1.4         | ——            |增加了VAT，修复了linux下apply_embedding返回项有问题的情况|
+|20220409| 0.1.3         | ——            |初始版本|
 
-</details>
 
+</details>
 
 ## 5. 更新历史：
-<details><summary><b>点击查看</b></summary>
 
+<details><summary><b>5.1 即将更新</b></summary>
+
+- [✓] llama系列的微调
+- [ ] 大模型的deepspeed使用
+- [ ] chatgpt三阶段的训练
+
+</details>
+
+<details><summary><b>5.2 更新历史</b></summary>
+
+- **20230729**：增加llama-2的微调
 - **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
@@ -166,61 +152,61 @@
 - **20220322**：添加GPT、GPT2、T5模型
 - **20220312**：初版提交
 
 </details>
 
 ## 6. 预训练权重
 
-- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)
+- 部分权重是要加载修改的[config.json](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)
 
 
 | 模型分类| 权重来源| 权重链接 | 备注(若有)|
 | ----- | ----- | ----- | ----- |
-| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert| 谷歌原版bert(即bert-base-chinese) | [tf](https://github.com/google-research/bert)，[torch](https://huggingface.co/bert-base-chinese) | [tf转pytorch命令](https://huggingface.co/docs/transformers/converting_tensorflow_models)，[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | bert| 哈工大chinese-bert-wwm-ext| [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-bert-wwm-ext)| |
-| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bert-base-chinese.py) |
+| bert-base-multilingual-cased| huggingface | [torch](https://huggingface.co/bert-base-multilingual-cased) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bert-base-chinese.py) |
 | macbert | 哈工大chinese-macbert-base/large| [tf/torch](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | roberta | 哈工大chinese-roberta-wwm-ext | [tf/torch](https://github.com/ymcui/Chinese-BERT-wwm)，[torch](https://huggingface.co/hfl/chinese-roberta-wwm-ext) | |
-| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-small.py) |
-| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_roberta-base.py) |
-| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_deberta_v2.py)|
-| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_guwenbert-base.py)|
-| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
+| roberta-small/tiny| 追一科技 & UER| [tf](https://github.com/ZhuiyiTechnology/pretrained-models)，[torch](https://huggingface.co/uer) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-small.py) |
+| roberta-base (english)| huggingface | [torch](https://huggingface.co/roberta-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_roberta-base.py) |
+| deberta_v2| IDEA Erlangshen-DeBERTa-v2| [torch](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_deberta_v2.py)|
+| guwenbert | 古文bert| [torch](https://huggingface.co/ethanyt/guwenbert-base) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_guwenbert-base.py)|
+| xlnet | 哈工大xlnet | [tf/torch](https://github.com/ymcui/Chinese-XLNet) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
 | electra | 哈工大electra | [tf](https://github.com/ymcui/Chinese-ELECTRA)，[torch](https://huggingface.co/hfl/chinese-electra-base-discriminator) | |
 | macbert | 哈工大macbert | [tf](https://github.com/ymcui/MacBERT)，[torch](https://huggingface.co/hfl/chinese-macbert-base) | |
 | albert| brightmart| [tf](https://github.com/brightmart/albert_zh)，[torch](https://huggingface.co/voidful)，[torch](https://github.com/lonePatient/albert_pytorch) | |
 | ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[torch](https://huggingface.co/nghuyong)| |
 | roformer| 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer)，[torch](https://huggingface.co/junnyu/roformer_chinese_base) | |
 | roformer_v2 | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-v2)，[torch](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)| |
-| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_simbert.py) |
+| simbert | 追一科技| [tf](https://github.com/ZhuiyiTechnology/simbert)，[torch_base](https://huggingface.co/peterchou/simbert-chinese-base/tree/main) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_simbert.py) |
 | simbert_v2/roformer-sim | 追一科技| [tf](https://github.com/ZhuiyiTechnology/roformer-sim)，[torch](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)| |
-| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_GAU_alpha.py) |
+| gau-alpha | 追一科技| [tf](https://github.com/ZhuiyiTechnology/GAU-alpha)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_GAU_alpha.py) |
 | wobert| 追一科技| [tf](https://github.com/ZhuiyiTechnology/WoBERT)，[torch_base](https://huggingface.co/junnyu/wobert_chinese_base)，[torch_plus_base](https://huggingface.co/junnyu/wobert_chinese_plus_base) | |
 | nezha | 华为| [tf](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-TensorFlow)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch) | |
-| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt__CDial-GPT-LCCC.py) |
-| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__cmp_lm_2.6b.py) |
-| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__gpt2-ml.py) |
-| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_gpt2__uer-gpt2-chinese.py)|
-| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
-| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
+| gpt | thu-coai/CDial-GPT| [torch](https://github.com/thu-coai/CDial-GPT) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt_CDial-GPT-LCCC.py) |
+| gpt2| 清华26亿 cmp_lm | [torch](https://github.com/TsinghuaAI/CPM-1-Generate)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_cmp_lm_2.6b.py) |
+| gpt2| 中文GPT2_ML模型 | [tf](https://github.com/imcaspar/gpt2-ml)，[torch](https://github.com/ghosthamlet/gpt2-ml-torch) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_gpt2-ml.py) |
+| gpt2| UER | [torch](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_gpt2_uer-gpt2-chinese.py)|
+| t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_t5_pegasus.py)|
+| bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
-| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| llama2 | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
-| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
-| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
-| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bloom.py) |
+| chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/README.md)|
+| chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_chatglm.py) |
+| llama | facebook| [github](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| llama-2 | facebook| [github](https://github.com/facebookresearch/llama), [7b](https://huggingface.co/meta-llama/Llama-2-7b-hf), [7b-chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [13b](https://huggingface.co/meta-llama/Llama-2-13b-hf), [13b-chat](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+|chinese_llama_alpaca|Yiming Cui|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_llama_hf.py) |
+| bloom | bigscience | [560m](https://huggingface.co/bigscience/bloom-560m) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/convert_script/convert_bloom.py) |
 
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
@@ -243,15 +229,15 @@
   <tbody>
     <tr align="center" >
       <td>
          <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信号</a> 
       </td>
       <td>
-         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo"><img width="200" height="300" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
          <a href="https://github.com/Tongjilibo">微信群</a> 
       </td>
     </tr>
   </tbody>
 </table>
 
 - Star History Chart
@@ -261,8 +247,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.3.1.post2/bert4torch.egg-info/SOURCES.txt` & `bert4torch-0.3.2/bert4torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1.post2/setup.py` & `bert4torch-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.3.1.post2',
+    version='v0.3.2',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.1.0.post2'],
+    install_requires=['torch>1.6', 'torch4keras>=0.1.1'],
     packages=find_packages()
 )
```

