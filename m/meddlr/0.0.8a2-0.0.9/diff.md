# Comparing `tmp/meddlr-0.0.8a2.tar.gz` & `tmp/meddlr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meddlr-0.0.8a2.tar", last modified: Sat Apr 29 20:22:37 2023, max compression
+gzip compressed data, was "meddlr-0.0.9.tar", last modified: Thu Aug  3 20:52:23 2023, max compression
```

## Comparing `meddlr-0.0.8a2.tar` & `meddlr-0.0.9.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/checkpoint/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.589338 meddlr-0.0.8a2/meddlr/config/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.593338 meddlr-0.0.8a2/meddlr/data/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.593338 meddlr-0.0.8a2/meddlr/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/datasets/register_mrco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.597338 meddlr-0.0.8a2/meddlr/data/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/group_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/slice_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.601338 meddlr-0.0.8a2/meddlr/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/noiseandmotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    27768 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/subsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/data/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.605338 meddlr-0.0.8a2/meddlr/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/model_zoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/sharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/train_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.605338 meddlr-0.0.8a2/meddlr/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/recon_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/scan_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/seg_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/evaluation/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.609338 meddlr-0.0.8a2/meddlr/forward/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/forward/mri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.609338 meddlr-0.0.8a2/meddlr/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/metrics/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/sem_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/functional/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/lpip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/sem_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/metrics/ssfd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.613338 meddlr-0.0.8a2/meddlr/modeling/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/conv_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/blocks/fuse_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.617338 meddlr-0.0.8a2/meddlr/modeling/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/layers2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/layers/layers3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/loss_computer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.621338 meddlr-0.0.8a2/meddlr/modeling/meta_arch/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/cs_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/generalized_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/m2r.py
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/n2r.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/nm2r.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/ssdu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/unrolled.py
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/modeling/meta_arch/vortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.625338 meddlr-0.0.8a2/meddlr/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/ops/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.625338 meddlr-0.0.8a2/meddlr/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/solver/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/base/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/builtin/mri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.629338 meddlr-0.0.8a2/meddlr/transforms/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/functional/mri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.633339 meddlr-0.0.8a2/meddlr/transforms/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/gen/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/param_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/tf_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/transforms/transform_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/meddlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/cfl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/meddlr/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.585338 meddlr-0.0.8a2/meddlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 20:22:37.000000 meddlr-0.0.8a2/meddlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:22:37.637338 meddlr-0.0.8a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/tests/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-29 20:19:12.000000 meddlr-0.0.8a2/tests/test_reproducibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.336065 meddlr-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 20:48:22.000000 meddlr-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 20:52:23.336065 meddlr-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-03 20:48:22.000000 meddlr-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.260065 meddlr-0.0.9/meddlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.264065 meddlr-0.0.9/meddlr/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/checkpoint/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.264065 meddlr-0.0.9/meddlr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/config/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.268065 meddlr-0.0.9/meddlr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.268065 meddlr-0.0.9/meddlr/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/datasets/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/datasets/register_mrco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.272065 meddlr-0.0.9/meddlr/data/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/samplers/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/samplers/group_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/slice_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.276065 meddlr-0.0.9/meddlr/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/noiseandmotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29808 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/data/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.280065 meddlr-0.0.9/meddlr/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/model_zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/train_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.284065 meddlr-0.0.9/meddlr/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/recon_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/scan_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/seg_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/evaluation/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.284065 meddlr-0.0.9/meddlr/forward/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/forward/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.288065 meddlr-0.0.9/meddlr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.292065 meddlr-0.0.9/meddlr/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/functional/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/functional/sem_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/functional/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/sem_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/metrics/ssfd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.292065 meddlr-0.0.9/meddlr/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.292065 meddlr-0.0.9/meddlr/modeling/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/blocks/conv_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/blocks/fuse_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.300065 meddlr-0.0.9/meddlr/modeling/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/layers2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/layers3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/layers/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/loss_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.308065 meddlr-0.0.9/meddlr/modeling/meta_arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/cs_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/generalized_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/m2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/n2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/nm2r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/ssdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/unrolled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/modeling/meta_arch/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.312065 meddlr-0.0.9/meddlr/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/ops/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.312065 meddlr-0.0.9/meddlr/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/solver/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/solver/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/solver/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.316065 meddlr-0.0.9/meddlr/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.320065 meddlr-0.0.9/meddlr/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/base/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/base/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/base/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/base/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.320065 meddlr-0.0.9/meddlr/transforms/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/builtin/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.324065 meddlr-0.0.9/meddlr/transforms/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/functional/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.324065 meddlr-0.0.9/meddlr/transforms/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/gen/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/param_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/tf_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/transforms/transform_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.332065 meddlr-0.0.9/meddlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/cfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-08-03 20:48:22.000000 meddlr-0.0.9/meddlr/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.260065 meddlr-0.0.9/meddlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 20:52:23.000000 meddlr-0.0.9/meddlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-03 20:52:23.000000 meddlr-0.0.9/meddlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:52:23.000000 meddlr-0.0.9/meddlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-03 20:52:23.000000 meddlr-0.0.9/meddlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 20:52:23.000000 meddlr-0.0.9/meddlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:48:22.000000 meddlr-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 20:52:23.336065 meddlr-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-08-03 20:48:22.000000 meddlr-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:52:23.336065 meddlr-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-03 20:48:22.000000 meddlr-0.0.9/tests/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-03 20:48:22.000000 meddlr-0.0.9/tests/test_reproducibility.py
```

### Comparing `meddlr-0.0.8a2/LICENSE` & `meddlr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/PKG-INFO` & `meddlr-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.8a2
+Version: 0.0.9
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -57,14 +57,26 @@
 # OR set these as environment variables.
 os.environ["MEDDLR_RESULTS_DIR"] = "/path/to/save/results"
 os.environ["MEDDLR_DATASETS_DIR"] = "/path/to/datasets"
 ```
 
 Detailed instructions are available in [Getting Started](GETTING_STARTED.md).
 
+## Visualizations
+Use [MeddlrViz](https://github.com/ad12/meddlr-viz) to visualize your medical imaging datasets, ML models, and more!
+
+```bash
+pip install meddlr-viz
+```
+
+<div align="center">
+
+<image src="https://github.com/ad12/meddlr-viz/blob/main/static/brats.gif" height=400 alt="A gallery of images from the BRATS dataset" />
+</div>
+
 ## 🐘 Model Zoo
 Easily serve and download pretrained models from the model zoo. A (evolving) list of pre-trained models can be found [here](MODEL_ZOO.md), on [HuggingFace 🤗](https://huggingface.co/arjundd), and in [project folders](projects).
 
 To use them, pass the URLs for the config and weights (model) files to `mr.get_model_from_zoo`:
 
 ```python
 import meddlr as mr
```

### Comparing `meddlr-0.0.8a2/README.md` & `meddlr-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,26 @@
 # OR set these as environment variables.
 os.environ["MEDDLR_RESULTS_DIR"] = "/path/to/save/results"
 os.environ["MEDDLR_DATASETS_DIR"] = "/path/to/datasets"
 ```
 
 Detailed instructions are available in [Getting Started](GETTING_STARTED.md).
 
+## Visualizations
+Use [MeddlrViz](https://github.com/ad12/meddlr-viz) to visualize your medical imaging datasets, ML models, and more!
+
+```bash
+pip install meddlr-viz
+```
+
+<div align="center">
+
+<image src="https://github.com/ad12/meddlr-viz/blob/main/static/brats.gif" height=400 alt="A gallery of images from the BRATS dataset" />
+</div>
+
 ## 🐘 Model Zoo
 Easily serve and download pretrained models from the model zoo. A (evolving) list of pre-trained models can be found [here](MODEL_ZOO.md), on [HuggingFace 🤗](https://huggingface.co/arjundd), and in [project folders](projects).
 
 To use them, pass the URLs for the config and weights (model) files to `mr.get_model_from_zoo`:
 
 ```python
 import meddlr as mr
```

### Comparing `meddlr-0.0.8a2/meddlr/checkpoint/checkpoint.py` & `meddlr-0.0.9/meddlr/checkpoint/checkpoint.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/config/compat.py` & `meddlr-0.0.9/meddlr/config/compat.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/config/config.py` & `meddlr-0.0.9/meddlr/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """CfgNode implementation.
 """
 import functools
 import inspect
 import logging
 import re
-from typing import Any, Mapping
+from typing import Any, List, Mapping, Tuple
 
 import numpy as np
 from fvcore.common.config import CfgNode as _CfgNode
 
 
 class CfgNode(_CfgNode):
     """
@@ -113,22 +113,16 @@
 
         Raises:
             KeyError: If the key is not found and no default was provided.
         """
         d = self
         try:
             for k in key.split("."):
-                # Extract groups matching sequence-indexing syntax (e.g. 'field[0]').
-                match_val = re.match("^(?P<field>[a-zA-Z0-9_]+)\[(?P<index>[-?0-9]+)\]$", k)
-                if match_val:
-                    k = match_val.group("field")
-                    index = int(match_val.group("index"))
-                    d = d[k][index]
-                else:
-                    d = d[k]
+                k, index = _extract_field_index(k)
+                d = d[k] if index is None else d[k][index]
         except KeyError:
             if default != np._NoValue:
                 return default
             raise KeyError("Config does not have key '{}'".format(key))
         return d
 
     def set_recursive(self, name: str, value: Any):
@@ -137,17 +131,30 @@
         Args:
             name (str): The dot-separated key.
             value (object): The value to set.
         """
         cfg = self
         keys = name.split(".")
         for k in keys[:-1]:
-            cfg = cfg[k]
+            # Extract groups matching sequence-indexing syntax (e.g. 'field[0]').
+            k, index = _extract_field_index(k)
+            cfg = cfg[k] if index is None else cfg[k][index]
+
+        k, index = _extract_field_index(keys[-1])
+        if index is not None:
+            if not isinstance(cfg[k], (list, tuple)):
+                raise TypeError(f"Cannot set index {index} for non-sequence field '{name}'")
+            current_value = cfg[k]
+            if isinstance(current_value, tuple):
+                current_value = list(current_value)
+            current_value[index] = value
+            current_value = type(cfg[k])(current_value)
+            value = current_value
 
-        setattr(cfg, keys[-1], value)
+        setattr(cfg, k, value)
 
     def update_recursive(self, mapping: Mapping[str, Any]):
         """
         Update this CfgNode and all of its children recursively.
 
         Args:
             mapping (dict): a dict to update this CfgNode and all of its children.
@@ -366,51 +373,90 @@
     if isinstance(kwargs.pop("cfg", None), (_CfgNode, DictConfig)):
         return True
     # `from_config`'s first argument is forced to be "cfg".
     # So the above check covers all cases.
     return False
 
 
-def _find_format_str_keys(cfg: Mapping, prefix="", accum=()):
-    accum = set(accum)
-    for k, v in cfg.items():
-        k_prefix = prefix + "." + k if prefix else k
-        if isinstance(v, Mapping):
-            accum |= _find_format_str_keys(cfg[k], prefix=k_prefix, accum=accum)
-        elif isinstance(v, str) and (
-            (v.startswith('f"') and v.endswith('"')) or (v.startswith("f'") and v.endswith("'"))
-        ):
-            accum |= {(k_prefix, v)}
+def _find_format_str_keys(value: Mapping, prefix=""):
+    accum = set()
+
+    if isinstance(value, str) and (
+        (value.startswith('f"') and value.endswith('"'))
+        or (value.startswith("f'") and value.endswith("'"))
+    ):
+        return {(prefix, value)}
+    elif not isinstance(value, (Mapping, List, Tuple)):
+        return accum
+
+    if isinstance(value, Mapping):
+        for k, v in value.items():
+            k_prefix = f"{prefix}.{k}" if prefix else k
+            accum |= _find_format_str_keys(v, prefix=k_prefix)
+    elif isinstance(value, (list, tuple)):
+        for i in range(len(value)):
+            accum |= _find_format_str_keys(value[i], prefix=f"{prefix}[{i}]")
     return accum
 
 
 def _unroll_value_to_str(value) -> str:
     if isinstance(value, (tuple, list)):
         return "-".join(_unroll_value_to_str(v) for v in value)
     elif isinstance(value, dict):
         return "-".join(f"{k}={_unroll_value_to_str(v)}" for k, v in value.items())
     else:
         return str(value)
 
 
+def _format_str(val_str: str, *, cfg: CfgNode, unroll: bool):
+    start = [x.start() for x in re.finditer("\{", val_str)]
+    end = [x.start() for x in re.finditer("\}", val_str)]
+    assert len(start) == len(end), f"Could not determine formatting string: {val_str}"
+
+    if len(start) == 0:
+        return val_str
+
+    cfg_keys_to_search = [val_str[s + 1 : e] for s, e in zip(start, end)]
+    values = [cfg.get_recursive(v) for v in cfg_keys_to_search]
+
+    if unroll:
+        values = [_unroll_value_to_str(v) for v in values]
+
+    fmt_str = ""
+    idxs = [0] + [y for x in zip(start, end) for y in x] + [len(val_str)]
+    for i in range(len(idxs) // 2):
+        fmt_str += val_str[idxs[2 * i] : idxs[2 * i + 1] + 1]
+    fmt_str = eval(fmt_str.format(*values))
+    return fmt_str
+
+
 def format_config_fields(cfg: CfgNode, unroll=False, inplace=False):
     keys_and_val_str = _find_format_str_keys(cfg)
     values_list = []
-    for k, val_str in keys_and_val_str:
-        start = [x.start() for x in re.finditer("\{", val_str)]
-        end = [x.start() for x in re.finditer("\}", val_str)]
-        assert len(start) == len(end), f"Could not determine formatting string: {val_str}"
-        cfg_keys_to_search = [val_str[s + 1 : e] for s, e in zip(start, end)]
-        values = [cfg.get_recursive(v) for v in cfg_keys_to_search]
-        if unroll:
-            values = [_unroll_value_to_str(v) for v in values]
-
-        fmt_str = ""
-        idxs = [0] + [y for x in zip(start, end) for y in x] + [len(val_str)]
-        for i in range(len(idxs) // 2):
-            fmt_str += val_str[idxs[2 * i] : idxs[2 * i + 1] + 1]
-        fmt_str = eval(fmt_str.format(*values))
-        values_list.extend([k, fmt_str])
+    for k, value in keys_and_val_str:
+        if isinstance(value, (list, tuple)):
+            fmt_str = type(value)(
+                _format_str(v, cfg=cfg, unroll=unroll) if isinstance(v, str) else v for v in value
+            )
+        else:
+            assert isinstance(value, str)
+            fmt_str = _format_str(value, cfg=cfg, unroll=unroll)
+        values_list.append([k, fmt_str])
     if not inplace:
         cfg.clone()
-    cfg.defrost().merge_from_list(values_list)
+
+    # TODO: Determine if we want to enforce the checks in merge_from_list.
+    # This may be important if we want to handle renamed or deprecated keys.
+    # cfg.defrost().merge_from_list(values_list)
+    cfg.defrost()
+    for k, fmt_str in values_list:
+        cfg.set_recursive(k, fmt_str)
+
     return cfg
+
+
+def _extract_field_index(key):
+    match_val = re.match("^(?P<field>[a-zA-Z0-9_]+)\[(?P<index>[-?0-9]+)\]$", key)
+    if match_val:
+        return match_val.group("field"), int(match_val.group("index"))
+    else:
+        return key, None
```

### Comparing `meddlr-0.0.8a2/meddlr/config/defaults.py` & `meddlr-0.0.9/meddlr/config/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,34 @@
 _C.MODEL.UNET.NUM_POOL_LAYERS = 4
 _C.MODEL.UNET.DROPOUT = 0.0
 _C.MODEL.UNET.NORMALIZE = False
 # BLOCK_ORDER only applies to GeneralizedUNet
 _C.MODEL.UNET.BLOCK_ORDER = ("conv", "relu", "conv", "relu", "batchnorm", "dropout")
 
 # -----------------------------------------------------------------------------
+# ResNet model
+# -----------------------------------------------------------------------------
+_C.MODEL.RESNET = CN()
+_C.MODEL.RESNET.IN_CHANNELS = 2
+_C.MODEL.RESNET.CHANNELS = 256
+_C.MODEL.RESNET.NUM_BLOCKS = 2
+_C.MODEL.RESNET.KERNEL_SIZE = (3,)
+_C.MODEL.RESNET.DROPOUT = 0.0
+_C.MODEL.RESNET.PADDING = ""
+_C.MODEL.RESNET.PRE_CONV = False
+_C.MODEL.RESNET.POST_CONV = False
+_C.MODEL.RESNET.BIAS = True
+_C.MODEL.RESNET.CONV_BLOCK = CN()
+_C.MODEL.RESNET.CONV_BLOCK.NUM_BLOCKS = 2
+_C.MODEL.RESNET.CONV_BLOCK.ACTIVATION = "relu"
+_C.MODEL.RESNET.CONV_BLOCK.NORM = "none"
+_C.MODEL.RESNET.CONV_BLOCK.NORM_AFFINE = False
+_C.MODEL.RESNET.CONV_BLOCK.ORDER = ("norm", "act", "drop", "conv")
+
+# -----------------------------------------------------------------------------
 # Denoising model
 # -----------------------------------------------------------------------------
 _C.MODEL.DENOISING = CN()
 _C.MODEL.DENOISING.META_ARCHITECTURE = "GeneralizedUnrolledCNN"
 _C.MODEL.DENOISING.NOISE = CN()
 # Noise standard deviation to use for augmentations.
 _C.MODEL.DENOISING.NOISE.STD_DEV = (1,)
@@ -211,14 +231,16 @@
 # SSDU model
 # -----------------------------------------------------------------------------
 _C.MODEL.SSDU = CN()
 _C.MODEL.SSDU.META_ARCHITECTURE = "GeneralizedUnrolledCNN"
 _C.MODEL.SSDU.MASKER = CN()
 _C.MODEL.SSDU.MASKER.PARAMS = CN(new_allowed=True)
 _C.MODEL.SSDU.AUGMENTOR = _MRI_RECON_TFM.clone()
+_C.MODEL.SSDU.POSTPROCESSOR = CN()
+_C.MODEL.SSDU.POSTPROCESSOR.NAME = ""
 
 # -----------------------------------------------------------------------------
 # MONAI wrapper
 # -----------------------------------------------------------------------------
 _C.MODEL.MONAI = CN(new_allowed=True)
 
 # -----------------------------------------------------------------------------
@@ -411,7 +433,14 @@
 # Project name for logging to Weights & Biases
 _C.DESCRIPTION.PROJECT_NAME = "ss_recon"
 # Experiment name for logging to Weights & Biases
 _C.DESCRIPTION.EXP_NAME = ""
 # Tags associated with experiment.
 # e.g. "fastmri_knee_mc" for fastMRI dataset; "unrolled" for using unrolled network; etc.
 _C.DESCRIPTION.TAGS = ()
+
+# ---------------------------------------------------------------------------- #
+# Miscellaneous
+# This is a free field that can be used to add any extra config fields without
+# affecting loading of any particular config.
+# ---------------------------------------------------------------------------- #
+_C.MISC = CN(new_allowed=True)
```

### Comparing `meddlr-0.0.8a2/meddlr/config/util.py` & `meddlr-0.0.9/meddlr/config/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/__init__.py` & `meddlr-0.0.9/meddlr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/build.py` & `meddlr-0.0.9/meddlr/data/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     logger = logging.getLogger(__name__)
 
     state = random.Random(seed)
     limit_scans = (
         num_scans_total > 0 if isinstance(num_scans_total, (float, int)) else bool(num_scans_total)
     )
-    if limit_scans or num_scans_subsample > 0:
+    if limit_scans or num_scans_subsample != 0:
         # Sort to ensure same order for all users.
         # Shuffle for randomness.
         dataset_dicts = sorted(dataset_dicts, key=lambda x: x["file_name"])
         state.shuffle(dataset_dicts)
 
     if filter_by:
         for k, v in filter_by:
@@ -104,14 +104,16 @@
         dataset_dicts = _limit_data_by_group(dataset_dicts, num_scans_total)
 
     num_after = len(dataset_dicts)
     logger.info(
         "Dropped {} scans. {} scans remaining".format(num_after_filter - num_after, num_after)
     )
 
+    if num_scans_subsample == -1:
+        num_scans_subsample = len(dataset_dicts)
     num_scans_subsample = max(0, num_scans_subsample)
     if num_scans_subsample > 0:
         if num_scans_subsample > len(dataset_dicts):
             raise ValueError("")
         for dd in dataset_dicts[:num_scans_subsample]:
             dd["_is_unsupervised"] = True
             # Select the maximum acceleration when doing undersampling.
```

### Comparing `meddlr-0.0.8a2/meddlr/data/catalog.py` & `meddlr-0.0.9/meddlr/data/catalog.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/collate.py` & `meddlr-0.0.9/meddlr/data/collate.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/data_utils.py` & `meddlr-0.0.9/meddlr/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/datasets/builtin.py` & `meddlr-0.0.9/meddlr/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/datasets/register_mrco.py` & `meddlr-0.0.9/meddlr/data/datasets/register_mrco.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/samplers/build.py` & `meddlr-0.0.9/meddlr/data/samplers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/samplers/group_sampler.py` & `meddlr-0.0.9/meddlr/data/samplers/group_sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/samplers/sampler.py` & `meddlr-0.0.9/meddlr/data/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/slice_dataset.py` & `meddlr-0.0.9/meddlr/data/slice_dataset.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/transforms/motion.py` & `meddlr-0.0.9/meddlr/data/transforms/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/transforms/noise.py` & `meddlr-0.0.9/meddlr/data/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/transforms/noiseandmotion.py` & `meddlr-0.0.9/meddlr/data/transforms/noiseandmotion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/data/transforms/subsample.py` & `meddlr-0.0.9/meddlr/data/transforms/subsample.py`

 * *Files 4% similar despite different names*

```diff
@@ -375,14 +375,61 @@
         Expected `kspace` shape (batch, ky, kz, ...).
         """
         # TODO: dims should be configured based on the number of dimenions in the input.
         return get_cartesian_edge_mask(kspace, dims=(1, 2), out_shape=out_shape)
 
 
 @MASK_FUNC_REGISTRY.register()
+class EquispacedMaskFunc1D(MaskFunc):
+    """
+
+    Adapted from https://github.com/facebookresearch/fastMRI/blob/master/common/subsample.py
+    """
+
+    def __init__(self, accelerations, calib_size=None, center_fractions=None):
+        if not calib_size and not center_fractions:
+            raise ValueError("Either calib_size or center_fractions must be specified.")
+        if calib_size and center_fractions:
+            raise ValueError("Only one of calib_size or center_fractions can be specified")
+        assert not center_fractions, "Center fractions not supported for equispaced sampling."
+
+        self.center_fractions = center_fractions
+        self.calib_size = calib_size
+        super().__init__(accelerations)
+
+    def choose_acceleration(self) -> int:
+        # Accelerations for equispaced sampling must be an integer.
+        acc = super().choose_acceleration()
+        return int(round(acc))
+
+    def __call__(self, shape, seed: int = None, acceleration: int = None):
+        """
+        Args:
+            shape (iterable[int]): The shape of the mask to be created. The shape should have
+                at least 3 dimensions. Samples are drawn along the second last dimension.
+            seed (int, optional): Seed for the random number generator. Setting the seed
+                ensures the same mask is generated each time for the same shape.
+        Returns:
+            torch.Tensor: A mask of the specified shape.
+        """
+        if len(shape) < 3:
+            raise ValueError("Shape should have 3 or more dimensions")
+
+        calib = self.calib_size
+        if acceleration is None:
+            acceleration = self.choose_acceleration()
+
+        return equispaced_mask(shape, accel=acceleration, calib=calib, dim=1)
+
+    def get_edge_mask(self, kspace: torch.Tensor, out_shape: Sequence[int] = None):
+        # TODO: dims should be configured based on the number of dimenions in the input.
+        return get_cartesian_edge_mask(kspace, dims=(1, 2), out_shape=out_shape)
+
+
+@MASK_FUNC_REGISTRY.register()
 class EquispacedMaskFunc2D(MaskFunc):
     """
 
     Adapted from https://github.com/facebookresearch/fastMRI/blob/master/common/subsample.py
     """
 
     def __init__(self, accelerations, calib_size=None, center_fractions=None):
```

### Comparing `meddlr-0.0.8a2/meddlr/data/transforms/transform.py` & `meddlr-0.0.9/meddlr/data/transforms/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,19 @@
         assert self._postprocessor in ["", "hard_dc_edge", "hard_dc_all"], self._postprocessor
 
         # Build augmentation pipeline.
         self.augmentor = None
         if not is_test and cfg.AUG_TRAIN.MRI_RECON.TRANSFORMS:
             self.augmentor = MRIReconAugmentor.from_cfg(cfg, aug_kind="aug_train", seed=seed)
 
+    def _get_mask(self, masked_kspace):
+        # If any of the coils are non-zero at a coordinate, we assume
+        assert torch.is_complex(masked_kspace)
+        return cplx.get_mask(masked_kspace, coil_dim=-1)
+
     def _call_augmentor(
         self, kspace, maps, target, fname, slice_id, is_fixed, acceleration: int = None
     ):
         assert not self._is_test, "Augmentor is not supported with testing yet"
 
         # Convert everything from numpy arrays to tensors
         kspace = cplx.to_tensor(kspace).unsqueeze(0)
@@ -284,14 +289,15 @@
         return {
             "kspace": masked_kspace,
             "maps": maps,
             "target": target,
             "mean": mean,
             "std": std,
             "norm": norm,
+            "mask": self._get_mask(masked_kspace),
         }
 
     def __call__(
         self, kspace, maps, target, fname, slice_id, is_fixed, acceleration: int = None
     ) -> Dict[str, Any]:
         """
         Args:
@@ -389,11 +395,12 @@
             "kspace": masked_kspace,
             "maps": maps,
             "target": target,
             "mean": mean,
             "std": std,
             "norm": norm,
             "edge_mask": edge_mask.squeeze(0),
+            "mask": self._get_mask(masked_kspace),
         }
         if postprocessing_mask is not None:
             out["postprocessing_mask"] = postprocessing_mask.squeeze(0)
         return out
```

### Comparing `meddlr-0.0.8a2/meddlr/engine/defaults.py` & `meddlr-0.0.9/meddlr/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/engine/hooks.py` & `meddlr-0.0.9/meddlr/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/engine/model_zoo.py` & `meddlr-0.0.9/meddlr/engine/model_zoo.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/engine/sharing.py` & `meddlr-0.0.9/meddlr/engine/sharing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/engine/train_loop.py` & `meddlr-0.0.9/meddlr/engine/train_loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,18 +232,24 @@
         except StopIteration:
             # Epoch has ended, reinitialize the iterator.
             self._data_loader_iter = iter(self.data_loader)
             inputs = next(self._data_loader_iter)
 
         data_time = time.perf_counter() - start
 
+        # Pop keys that the model doesnt need.
+        profiler = inputs.pop("_profiler", {})
+
         """
         If your want to do something with the losses, you can wrap the model.
         """
+        forward_time = time.perf_counter()
         output_dict = self.model(inputs)
+        forward_time = time.perf_counter() - forward_time
+
         output_dict.update({k: inputs[k] for k in ["mean", "std", "norm"] if k in inputs})
         loss_dict = {k: v for k, v in output_dict.items() if "loss" in k}
         loss_dict.update(self.loss_computer(inputs, output_dict))
 
         # losses = sum(v for k, v in loss_dict.items() if "loss" in k)
         losses = loss_dict["loss"]
         self._detect_anomaly(losses, loss_dict)
@@ -251,16 +257,23 @@
         metrics_dict = loss_dict
         metrics_dict.update(
             flatten_dict(
                 {k: v for k, v in inputs.get("metrics", {}).items() if k not in metrics_dict}
             )
         )
         metrics_dict["data_time"] = data_time
+        metrics_dict["forward_time"] = forward_time
         metrics_dict["total_loss"] = losses
         metrics_dict.update(self.metrics_computer(output_dict) if self.metrics_computer else {})
+
+        if profiler is not None:
+            metrics_dict.update(flatten_dict({"profiler": profiler}))
+        # for k in ["_profiler", "profiler"]:
+        #     if k in inputs:
+        #         metrics_dict.update(flatten_dict({k.strip("_"): inputs[k]}))
         self._write_metrics(metrics_dict)
 
         """
         If you need accumulate gradients or something similar, you can
         wrap the optimizer with your custom `zero_grad()` method.
         """
         self.optimizer.zero_grad()
```

### Comparing `meddlr-0.0.8a2/meddlr/engine/trainer.py` & `meddlr-0.0.9/meddlr/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/evaluation/evaluator.py` & `meddlr-0.0.9/meddlr/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/evaluation/recon_evaluation.py` & `meddlr-0.0.9/meddlr/evaluation/recon_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/evaluation/scan_evaluator.py` & `meddlr-0.0.9/meddlr/evaluation/scan_evaluator.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/evaluation/seg_evaluation.py` & `meddlr-0.0.9/meddlr/evaluation/seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/evaluation/testing.py` & `meddlr-0.0.9/meddlr/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/forward/mri.py` & `meddlr-0.0.9/meddlr/forward/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/build.py` & `meddlr-0.0.9/meddlr/metrics/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/collection.py` & `meddlr-0.0.9/meddlr/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/functional/image.py` & `meddlr-0.0.9/meddlr/metrics/functional/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/functional/sem_seg.py` & `meddlr-0.0.9/meddlr/metrics/functional/sem_seg.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     y_pred = mFutil.to_bool(y_pred)
     y_true = mFutil.to_bool(y_true)
     y_pred, y_true = mFutil.flatten_other_dims((y_pred, y_true), dim=(0, 1))
 
     count_nonzero = torch.count_nonzero if is_tensor else np.count_nonzero
     intersection = count_nonzero(y_true & y_pred, -1)
     union = count_nonzero(y_true | y_pred, -1)
-    union = union.type(torch.float) if is_tensor else union.astype(np.float)
+    union = union.type(torch.float) if is_tensor else union.astype("float")
 
     return 1 - intersection / union
 
 
 def coefficient_variation(y_pred, y_true):
     """Computes coefficient of variation.
```

### Comparing `meddlr-0.0.8a2/meddlr/metrics/functional/util.py` & `meddlr-0.0.9/meddlr/metrics/functional/util.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/image.py` & `meddlr-0.0.9/meddlr/metrics/image.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/lpip.py` & `meddlr-0.0.9/meddlr/metrics/lpip.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/metric.py` & `meddlr-0.0.9/meddlr/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/sem_seg.py` & `meddlr-0.0.9/meddlr/metrics/sem_seg.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/metrics/ssfd.py` & `meddlr-0.0.9/meddlr/metrics/ssfd.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/blocks/conv_blocks.py` & `meddlr-0.0.9/meddlr/modeling/blocks/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/blocks/fuse_blocks.py` & `meddlr-0.0.9/meddlr/modeling/blocks/fuse_blocks.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/layers/build.py` & `meddlr-0.0.9/meddlr/modeling/layers/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/layers/conv.py` & `meddlr-0.0.9/meddlr/modeling/layers/conv.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/layers/gauss.py` & `meddlr-0.0.9/meddlr/modeling/layers/gauss.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/layers/layers2D.py` & `meddlr-0.0.9/meddlr/modeling/layers/layers3D.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,158 @@
-"""Implementation of 2D base layers.
 """
-
-from typing import Tuple, Union
+Implementations of different CNNs.
+"""
 
 from torch import nn
 
-from meddlr.modeling.layers.conv import ConvWS2d
+from meddlr.utils.transforms import center_crop
 
 
-def _get_same_padding(kernel_size: Union[int, Tuple[int, int]]):
-    if isinstance(kernel_size, int):
-        kernel_size = (kernel_size, kernel_size)
-    else:
-        assert len(kernel_size) == 2
-    if not all(k % 2 == 1 for k in kernel_size):
-        raise ValueError("Kernel size must be odd - got {}".format(kernel_size))
-    padding = tuple(k // 2 for k in kernel_size)
+class SeparableConv3d(nn.Module):
+    """
+    A separable 3D convolutional operator.
+    """
+
+    def __init__(self, in_chans, out_chans, kernel_size, spatial_chans=None, act_type="relu"):
+        """
+        Args:
+            in_chans (int): Number of channels in the input.
+            out_chans (int): Number of channels in the output.
+            kernel_size (int): Size of kernel (repeated for all three dimensions).
+        """
+        super().__init__()
+
+        sp_kernel_size = (1, kernel_size, kernel_size)
+        sp_pad_size = (0, 1, 1)
+        t_kernel_size = (kernel_size, 1, 1)
+        t_pad_size = (1, 0, 0)
+
+        if spatial_chans is None:
+            # Force number of spatial features, such that the total number of
+            # parameters is the same as a nn.Conv3D(in_chans, out_chans)
+            spatial_chans = (kernel_size**3) * in_chans * out_chans
+            spatial_chans /= (kernel_size**2) * in_chans + kernel_size * out_chans
+            spatial_chans = int(spatial_chans)
+
+        # Define each layer in SeparableConv3d block
+        spatial_conv = nn.Conv3d(
+            in_chans, spatial_chans, kernel_size=sp_kernel_size, padding=sp_pad_size
+        )
+        temporal_conv = nn.Conv3d(
+            spatial_chans, out_chans, kernel_size=t_kernel_size, padding=t_pad_size
+        )
 
-    return padding
+        # Define choices for intermediate activation layer
+        activations = nn.ModuleDict([["none", nn.Identity()]["relu", nn.ReLU()]])
+
+        # Define the forward pass
+        self.layers = nn.Sequential(spatial_conv, activations[act_type], temporal_conv)
+
+    def forward(self, input):
+        """
+        Args:
+            input (torch.Tensor): Input tensor of shape ``(B,C_{in},D,H,W)``.
+
+        Returns:
+            (torch.Tensor): Output tensor of shape ``(B,C_{in},D,H,W)``.
+        """
+        return self.layers(input)
 
 
 class ConvBlock(nn.Module):
     """
-    A 2D Convolutional Block that consists of Norm -> ReLU -> Dropout -> Conv
+    A 3D Convolutional Block that consists of Norm -> ReLU -> Dropout -> Conv
 
     Based on implementation described by:
         K He, et al. "Identity Mappings in Deep Residual Networks" arXiv:1603.05027
     """
 
     def __init__(
         self,
-        in_chans: int,
-        out_chans: int,
-        kernel_size: Union[int, Tuple[int, int]],
-        drop_prob: float,
-        act_type: str = "relu",
-        norm_type: str = "none",
-        norm_affine: bool = False,
-        order: Tuple[str, str, str, str] = ("norm", "act", "drop", "conv"),
+        in_chans,
+        out_chans,
+        kernel_size,
+        drop_prob,
+        conv_type="conv3d",
+        act_type="relu",
+        norm_type="none",
     ):
         """
         Args:
             in_chans (int): Number of channels in the input.
             out_chans (int): Number of channels in the output.
             drop_prob (float): Dropout probability.
         """
         super().__init__()
 
         self.in_chans = in_chans
         self.out_chans = out_chans
         self.drop_prob = drop_prob
 
-        if isinstance(kernel_size, int):
-            kernel_size = (kernel_size, kernel_size)
-        else:
-            assert len(kernel_size) == 2
-        if not all(k % 2 == 1 for k in kernel_size):
-            raise ValueError("Kernel size must be odd - got {}".format(kernel_size))
-
-        padding = tuple(k // 2 for k in kernel_size)
-
         # Define choices for each layer in ConvBlock
-        conv_idx = order.index([x for x in order if "conv" in x][0])
-        conv_after_norm = "norm" in order and conv_idx > order.index("norm")
-        norm_channels = in_chans if conv_after_norm else out_chans
-        normalizations = dict(
-            none=lambda: nn.Identity(),
-            instance=lambda: nn.InstanceNorm2d(norm_channels, affine=norm_affine),
-            batch=lambda: nn.BatchNorm2d(norm_channels, affine=norm_affine),
-            group=lambda: nn.GroupNorm(norm_channels // 8, norm_channels, affine=norm_affine),
-        )
-        activations = {"relu": lambda: nn.ReLU(), "leaky_relu": lambda: nn.LeakyReLU()}
-
-        if norm_type not in normalizations:
-            raise ValueError(
-                f"Unknown norm_type '{norm_type}'. Must be one of {normalizations.keys()}"
-            )
-
-        layer_dict = {
-            "conv": lambda: nn.Conv2d(
-                in_chans, out_chans, kernel_size=kernel_size, padding=padding
-            ),
-            "conv+ws": lambda: ConvWS2d(
-                in_chans, out_chans, kernel_size=kernel_size, padding=padding
-            ),
-            "drop": lambda: nn.Dropout2d(p=drop_prob),
-            "act": activations[act_type],
-            "norm": normalizations[norm_type],
-        }
-        layers = [layer_dict[lyr]() for lyr in order]
+        normalizations = nn.ModuleDict(
+            [
+                ["none", nn.Identity()],
+                ["instance", nn.InstanceNorm3d(in_chans, affine=False)],
+                ["batch", nn.BatchNorm3d(in_chans, affine=False)],
+            ]
+        )
+        activations = nn.ModuleDict([["relu", nn.ReLU()], ["leaky_relu", nn.LeakyReLU()]])
+        dropout = nn.Dropout3d(p=drop_prob, inplace=True)
+
+        # Note: don't use ModuleDict here. Otherwise, the parameters for the un-selected
+        # convolution type will still be initialized and added to model.parameters()
+        if conv_type == "conv3d":
+            convolution = nn.Conv3d(in_chans, out_chans, kernel_size=kernel_size, padding=1)
+        else:
+            convolution = SeparableConv3d(in_chans, out_chans, kernel_size=kernel_size, padding=1)
 
         # Define forward pass
-        self.layers = nn.Sequential(*layers)
+        self.layers = nn.Sequential(
+            normalizations[norm_type], activations[act_type], dropout, convolution
+        )
 
     def forward(self, input):
         """
         Args:
             input (torch.Tensor): Input tensor of shape ``(B,C_{in},D,H,W)``.
 
         Returns:
             (torch.Tensor): Output tensor of shape ``(B,C_{in},D,H,W)``.
         """
         return self.layers(input)
 
+    def __repr__(self):
+        return (
+            f"ConvBlock3D(in_chans={self.in_chans}, out_chans={self.out_chans}, "
+            f"drop_prob={self.drop_prob})"
+        )
+
 
 class ResBlock(nn.Module):
     """
-    A ResNet block that consists of two convolutional layers
-    followed by a residual connection.
+    A ResNet block that consists of two convolutional layers followed by a residual connection.
     """
 
-    def __init__(
-        self,
-        in_chans,
-        out_chans,
-        kernel_size,
-        drop_prob,
-        act_type: str = "relu",
-        norm_type: str = "none",
-        norm_affine: bool = False,
-        order: Tuple[str, str, str, str] = ("norm", "act", "drop", "conv"),
-    ):
+    def __init__(self, in_chans, out_chans, kernel_size, drop_prob):
         """
         Args:
             in_chans (int): Number of channels in the input.
             out_chans (int): Number of channels in the output.
             drop_prob (float): Dropout probability.
         """
         super().__init__()
 
         self.layers = nn.Sequential(
-            ConvBlock(
-                in_chans, out_chans, kernel_size, drop_prob, act_type, norm_type, norm_affine, order
-            ),  # noqa
-            ConvBlock(
-                out_chans,
-                out_chans,
-                kernel_size,
-                drop_prob,
-                act_type,
-                norm_type,
-                norm_affine,
-                order,
-            ),  # noqa
+            ConvBlock(in_chans, out_chans, kernel_size, drop_prob),
+            ConvBlock(out_chans, out_chans, kernel_size, drop_prob),
         )
 
         if in_chans != out_chans:
-            self.resample = nn.Conv2d(in_chans, out_chans, kernel_size=1)
+            self.resample = nn.Conv3d(in_chans, out_chans, kernel_size=1)
         else:
             self.resample = nn.Identity()
 
     def forward(self, input):
         """
         Args:
             input (torch.Tensor): Input tensor of shape ``(B,C_{in},D,H,W)``.
@@ -166,72 +168,43 @@
 
 
 class ResNet(nn.Module):
     """
     Prototype for 3D ResNet architecture
     """
 
-    def __init__(
-        self,
-        num_resblocks,
-        in_chans,
-        chans,
-        kernel_size,
-        drop_prob,
-        circular_pad=False,
-        act_type: str = "relu",
-        norm_type: str = "none",
-        norm_affine: bool = False,
-        order: Tuple[str, str, str, str] = ("norm", "act", "drop", "conv"),
-    ):
+    def __init__(self, num_resblocks, in_chans, chans, kernel_size, drop_prob, circular_pad=True):
         """ """
         super().__init__()
 
-        if circular_pad:
-            raise NotImplementedError(
-                "Circular padding is not available. "
-                "It is retained in the init to be used in the future."
-            )
         self.circular_pad = circular_pad
         self.pad_size = 2 * num_resblocks + 1
 
-        resblock_params = {
-            "act_type": act_type,
-            "norm_type": norm_type,
-            "norm_affine": norm_affine,
-            "order": order,
-            "kernel_size": kernel_size,
-            "drop_prob": drop_prob,
-        }
         # Declare ResBlock layers
-        self.res_blocks = nn.ModuleList([ResBlock(in_chans, chans, **resblock_params)])
+        self.res_blocks = nn.ModuleList([ResBlock(in_chans, chans, kernel_size, drop_prob)])
         for _ in range(num_resblocks - 1):
-            self.res_blocks += [ResBlock(chans, chans, **resblock_params)]
+            self.res_blocks += [ResBlock(chans, chans, kernel_size, drop_prob)]
 
         # Declare final conv layer (down-sample to original in_chans)
-        padding = _get_same_padding(kernel_size)
-        self.final_layer = nn.Conv2d(chans, in_chans, kernel_size=kernel_size, padding=padding)
+        self.final_layer = nn.Conv3d(chans, in_chans, kernel_size=kernel_size, padding=1)
 
     def forward(self, input):
         """
         Args:
             input (torch.Tensor): Input tensor of shape ``(B,C_{in},D,H,W)``.
 
         Returns:
             (torch.Tensor): Output tensor of shape ``(B,C_{in},D,H,W)``.
         """
 
-        # orig_shape = input.shape
-        # if self.circular_pad:
-        #     input = nn.functional.pad(
-        #         input, 2 * (self.pad_size,) + (0, 0), mode="circular"
-        #     )
+        orig_shape = input.shape
+        if self.circular_pad:
+            input = nn.functional.pad(input, (0, 0, 0, 0) + 2 * (self.pad_size,), mode="circular")
+            # input = nn.functional.pad(input, 4*(self.pad_size,) + (0,0), mode='replicate')
 
         # Perform forward pass through the network
         output = input
         for res_block in self.res_blocks:
             output = res_block(output)
         output = self.final_layer(output) + input
 
-        # return center_crop(output, orig_shape)
-
-        return output
+        return center_crop(output, orig_shape)
```

### Comparing `meddlr-0.0.8a2/meddlr/modeling/loss_computer.py` & `meddlr-0.0.9/meddlr/modeling/loss_computer.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/__init__.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/build.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/cs_model.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/cs_model.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/denoising.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/denoising.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/generalized_unet.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/generalized_unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/m2r.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/m2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/n2r.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/n2r.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from meddlr.config.config import configurable
 from meddlr.data.transforms.noise import NoiseModel
 from meddlr.modeling.meta_arch.build import META_ARCH_REGISTRY, build_model
 from meddlr.modeling.meta_arch.ssdu import SSDUModel
 from meddlr.ops import complex as cplx
 from meddlr.utils.events import get_event_storage
+from meddlr.utils.general import nested_apply
 
 
 @META_ARCH_REGISTRY.register()
 class N2RModel(nn.Module):
     """Noise2Recon model.
 
     Reference:
@@ -74,15 +75,17 @@
         Returns:
             Dict[str, Any]: The input dictionary with the kspace polluted
                 with additive masked complex Gaussian noise.
         """
         kspace = inputs["kspace"].clone()
         aug_kspace = self.noiser(kspace, clone=False)
 
-        inputs = {k: v.clone() for k, v in inputs.items() if k != "kspace"}
+        inputs = {
+            k: nested_apply(v, lambda _v: _v.clone()) for k, v in inputs.items() if k != "kspace"
+        }
         inputs["kspace"] = aug_kspace
         return inputs
 
     @torch.no_grad()
     def visualize_aug_training(self, kspace, kspace_aug, preds, preds_base, target=None):
         """Visualize training of augmented data.
 
@@ -184,17 +187,15 @@
             raise ValueError("Examples not formatted in the proper way")
         # Whether to use self-supervised via data undersampling (SSDU) for reconstruction.
         is_ssdu_enabled = isinstance(self.model, SSDUModel)
         output_dict = {}
 
         # Reconstruction (supervised).
         if is_ssdu_enabled:
-            output_dict["recon"] = self.model(
-                inputs,
-            )
+            output_dict["recon"] = self.model(inputs)
         elif inputs_supervised is not None:
             output_dict["recon"] = self.model(
                 inputs_supervised, return_pp=True, vis_training=vis_training
             )
 
         # Consistency (unsupervised).
         # kspace_aug = kspace + U \sigma \mathcal{N}
```

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/nm2r.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/nm2r.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/ssdu.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/ssdu.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from meddlr.forward.mri import SenseModel
 from meddlr.modeling.meta_arch.build import META_ARCH_REGISTRY, build_model
 from meddlr.ops import complex as cplx
 from meddlr.transforms.base.mask import KspaceMaskTransform
 from meddlr.transforms.builtin.mri import MRIReconAugmentor
 from meddlr.transforms.gen.mask import RandomKspaceMask
 from meddlr.utils.events import get_event_storage
-from meddlr.utils.general import move_to_device
+from meddlr.utils.general import move_to_device, nested_apply
 
 
 @META_ARCH_REGISTRY.register()
 class SSDUModel(nn.Module):
     """Self-supervised learning via data undersampling.
 
     This model is the relaxed form of the SSDU model that can be
@@ -38,34 +38,37 @@
 
     @configurable
     def __init__(
         self,
         model: nn.Module,
         masker: RandomKspaceMask,
         augmentor: MRIReconAugmentor = None,
+        postprocessor: str = None,
         vis_period: int = None,
     ):
         """
         Args:
             model (nn.Module): The base model.
             masker (NoiseModel): The masking model.
             augmentor: An augmentation model that can be used
+            postprocessor: The postprocessing to perform on the image.
         """
         super().__init__()
         self.model = model
         self.masker = masker
         self.augmentor = augmentor
         # Visualization done by this model
         if hasattr(self.model, "vis_period"):
             if vis_period is not None:
                 self.model.vis_period = vis_period
             else:
                 vis_period = self.model.vis_period
             self.model.vis_period = -1
         self.vis_period = vis_period
+        self.postprocessor = postprocessor
 
     def augment(self, inputs):
         """Noise augmentation module for the consistency branch.
 
         Args:
             inputs (Dict[str, Any]): The input dictionary.
                 It must contain a key ``'kspace'``, which traditionally
@@ -76,29 +79,46 @@
 
         Returns:
             Dict[str, Any]: The input dictionary with the kspace polluted
                 with additive masked complex Gaussian noise.
         """
         masker = self.masker
         kspace = inputs["kspace"].clone()
-        mask = cplx.get_mask(kspace)
+        mask = inputs.get("mask", None)
+        if mask is None:
+            mask = cplx.get_mask(kspace)
         edge_mask = inputs["edge_mask"]
 
         tfm: KspaceMaskTransform = masker.get_transform(kspace)
         train_mask = tfm.generate_mask(kspace, channels_last=True)
         loss_mask = mask - train_mask
 
+        # The loss mask should be a subset of the original mask.
+        # TODO (arjundd): See if we can remove this check for speed reasons.
+        is_loss_mask_valid = torch.all(loss_mask >= 0)
+        if not is_loss_mask_valid:
+            idx = torch.where(loss_mask < 0)
+            print("keys", inputs.keys())
+            raise ValueError(
+                "Train mask is not a subset of the original mask.\n"
+                f"Invalid indices: {idx}\n"
+                f"Mask: {mask[idx]}\n"
+                f"Mask (coils): {mask[idx[:-1]]}\n"
+                f"Train mask: {train_mask[idx[:-1]]}\n"
+                f"Loss mask: {loss_mask[idx]}\n"
+            )
+        assert is_loss_mask_valid
+
         # Pad the train mask so that all unacquired kspace points
         # are included in the train_mask.
         train_mask = (train_mask.type(torch.bool) | edge_mask.type(torch.bool)).type(torch.float32)
 
-        # TODO (arjundd): See if we can remove this check for speed reasons.
-        assert torch.all(loss_mask >= 0)
-
-        inputs = {k: v.clone() for k, v in inputs.items() if k != "kspace"}
+        inputs = {
+            k: nested_apply(v, lambda _v: _v.clone()) for k, v in inputs.items() if k != "kspace"
+        }
         inputs["kspace"] = train_mask * kspace
         inputs["mask"] = train_mask
 
         if self.augmentor is not None:
             out, _, _ = self.augmentor(kspace=inputs["kspace"], maps=inputs["maps"])
             inputs["kspace"] = out["kspace"]
 
@@ -151,16 +171,16 @@
         storage = get_event_storage()
         vis_training = self.training and self.vis_period > 0 and storage.iter % self.vis_period == 0
 
         # Put supervised and unsupervised scans in a single tensor.
         sup = inputs.get("supervised", {})
         unsup = inputs.get("unsupervised", {})
         # TODO: Make the cat operation recursive.
-        sup = {k: v for k, v in sup.items() if k != "metrics"}
-        unsup = {k: v for k, v in unsup.items() if k != "metrics"}
+        sup = {k: v for k, v in sup.items() if k not in ["metrics", "_profiler", "stats"]}
+        unsup = {k: v for k, v in unsup.items() if k not in ["metrics", "_profiler", "stats"]}
         if sup or unsup:
             inputs = {
                 k: torch.cat([sup.get(k, torch.tensor([])), unsup.get(k, torch.tensor([]))])
                 for k in sup.keys() | unsup.keys()
             }
         assert all(k in inputs for k in ["kspace"])
 
@@ -177,14 +197,26 @@
         target_img, zf_image = outputs.get("target", None), outputs.get("zf_image", None)
 
         # Use signal model (SENSE) to get weighted kspace.
         A = SenseModel(maps=inputs_aug["maps"])  # no weights - we do not want to mask the data.
         loss_pred_kspace = loss_mask * A(outputs["pred"], adjoint=False)
         loss_kspace = loss_mask * kspace
 
+        # TODO: Refactor post processing to be general to all reconstruction networks.
+        postprocessing_mask = None
+        if self.postprocessor == "hard_dc_edge":
+            postprocessing_mask = inputs["edge_mask"]
+        elif self.postprocessor == "hard_dc_all":
+            postprocessing_mask = train_mask
+        # Do this for differentiability reasons.
+        if postprocessing_mask is not None:
+            loss_pred_kspace = (
+                1 - postprocessing_mask
+            ) * loss_pred_kspace + postprocessing_mask * inputs["kspace"]
+
         # A hacky way to prepare the predictions and target for the loss.
         # This may result in inaccurate training metrics outside of the loss.
         # TODO (arjundd): Fix this.
         # Shape: B x H x W x #coils
         outputs["pred"] = oF.ifft2c(loss_pred_kspace, channels_last=True)
         outputs["target"] = oF.ifft2c(loss_kspace, channels_last=True)
 
@@ -231,8 +263,12 @@
 
         # Build augmentor.
         aug_cfg = cfg.MODEL.SSDU.AUGMENTOR
         if aug_cfg.TRANSFORMS:
             augmentor = MRIReconAugmentor.from_cfg(aug_cfg, aug_kind=None, seed=cfg.SEED)
             init_kwargs["augmentor"] = augmentor
 
+        # Build postprocessor.
+        postprocessor = cfg.MODEL.SSDU.POSTPROCESSOR.NAME or None
+        init_kwargs["postprocessor"] = postprocessor
+
         return init_kwargs
```

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/unet.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/unet.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/unrolled.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/unrolled.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 import torchvision.utils as tv_utils
 from torch import nn
 
 import meddlr.ops.complex as cplx
 from meddlr.config import CfgNode
 from meddlr.config.config import configurable
 from meddlr.forward.mri import SenseModel
+from meddlr.modeling.meta_arch.resnet import ResNetModel
 from meddlr.ops.opt import conjgrad
 from meddlr.utils.events import get_event_storage
 from meddlr.utils.general import move_to_device
 
-from ..layers.layers2D import ResNet
 from .build import META_ARCH_REGISTRY, build_model
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
 __all__ = ["GeneralizedUnrolledCNN"]
 
 
 @META_ARCH_REGISTRY.register()
 class GeneralizedUnrolledCNN(nn.Module):
     """Unrolled compressed sensing model.
 
@@ -177,14 +182,32 @@
         image = image.permute(0, 2, 3, 1).reshape(dims[0:3] + (self.num_emaps, 2))
         if not image.is_contiguous():
             image = image.contiguous()
         if use_cplx:
             image = torch.view_as_complex(image)
         return image
 
+    def step(
+        self,
+        *,
+        image: torch.Tensor,
+        model: nn.Module,
+        A: SenseModel,
+        zf_image: torch.Tensor,
+        step_size: Union[torch.Tensor, float],
+        dims: torch.Size
+    ):
+        if self._dc_first:
+            image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
+            image = self.reg(image=image, model=model, dims=dims)
+        else:
+            image = self.reg(image=image, model=model, dims=dims)
+            image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
+        return image
+
     def forward(self, inputs: Dict[str, Any], return_pp: bool = False, vis_training: bool = False):
         """Reconstructs the image from the kspace.
 
         Dimension ``(,2)`` indicates optional dimension for real-valued view of complex tensors.
         For example, a real-valued tensor of shape BxHxWx2 will be interpreted as
         a complex-valued tensor of shape BxHxW.
 
@@ -252,20 +275,22 @@
 
         # Compute zero-filled image reconstruction
         zf_image = A(kspace, adjoint=True)
 
         # Begin unrolled proximal gradient descent
         image = zf_image
         for resnet, step_size in zip(conv_blocks, step_sizes):
-            if self._dc_first:
-                image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
-                image = self.reg(image=image, model=resnet, dims=dims)
-            else:
-                image = self.reg(image=image, model=resnet, dims=dims)
-                image = self.dc(image=image, A=A, zf_image=zf_image, step_size=step_size)
+            image = self.step(
+                image=image,
+                model=resnet,
+                A=A,
+                zf_image=zf_image,
+                step_size=step_size,
+                dims=dims,
+            )
 
         # pred: shape [batch, height, width, #maps, 2]
         # target: shape [batch, height, width, #maps, 2]
         output_dict = {
             "pred": image,
             "target": target,
             "signal_model": A,
@@ -333,39 +358,44 @@
         }
         out.update(kwargs)
         return out
 
 
 @META_ARCH_REGISTRY.register()
 class CGUnrolledCNN(GeneralizedUnrolledCNN):
-    """Unrolled CNN with conjugate gradient descent (CG) data consistency."""
+    """Unrolled CNN with conjugate gradient descent (CG) data consistency.
+
+    Identical to MoDL.
+    """
 
     @configurable
     def __init__(
         self,
         blocks: Union[nn.Module, Sequence[nn.Module]],
         step_sizes: Union[float, Sequence[float]] = -2,
         fix_step_size: bool = False,
         num_emaps: int = 1,
         vis_period: int = -1,
         num_grad_steps: int = None,
         cg_max_iter: int = 10,
         cg_eps: float = 1e-4,
+        cg_init: Literal["zeros", "reg"] = None,
     ):
         super().__init__(
             blocks=blocks,
             step_sizes=step_sizes,
             fix_step_size=fix_step_size,
             num_emaps=num_emaps,
             vis_period=vis_period,
             num_grad_steps=num_grad_steps,
             order=("reg", "dc"),
         )
         self.cg_max_iter = cg_max_iter
         self.cg_eps = cg_eps
+        self.cg_init = cg_init
 
         for step_size in self.step_sizes:
             if step_size < 0:
                 raise ValueError("Step size must be non-negative.")
 
     def dc(
         self,
@@ -385,14 +415,46 @@
             mu=step_size,
             max_iter=self.cg_max_iter,
             pbar=False,
             eps=self.cg_eps,
         )
         return x_opt
 
+    def step(
+        self,
+        *,
+        image: torch.Tensor,
+        model: nn.Module,
+        A: SenseModel,
+        zf_image: torch.Tensor,
+        step_size: Union[torch.Tensor, float],
+        dims: torch.Size
+    ):
+        def A_op(x):
+            return A(A(x), adjoint=True)
+
+        x_reg = self.reg(image=image, model=model, dims=dims)
+
+        cg_init = image
+        if self.cg_init == "zeros":
+            cg_init = torch.zeros_like(image)
+        elif self.cg_init == "reg":
+            cg_init = x_reg
+
+        x_opt = conjgrad(
+            x=cg_init,
+            b=zf_image + step_size * x_reg,
+            A_op=A_op,
+            mu=step_size,
+            max_iter=self.cg_max_iter,
+            pbar=False,
+            eps=self.cg_eps,
+        )
+        return x_opt
+
     @classmethod
     def from_config(cls, cfg: CfgNode, **kwargs) -> Dict[str, Any]:
         """Build :cls:`CGUnrolledCNN` from a config.
 
         Args:
             cfg: The config.
             kwargs: Keyword arguments to override config-specified parameters.
@@ -403,15 +465,15 @@
         init_kwargs = super().from_config(cfg=cfg, **kwargs)
         init_kwargs["cg_max_iter"] = cfg.MODEL.UNROLLED.DC.MAX_ITER
         init_kwargs["cg_eps"] = cfg.MODEL.UNROLLED.DC.EPS
         init_kwargs.update(kwargs)
         return init_kwargs
 
 
-def _build_resblock(cfg: CfgNode) -> ResNet:
+def _build_resblock(cfg: CfgNode) -> ResNetModel:
     """Build the resblock for unrolled network.
 
     Args:
         cfg (CfgNode): The network configuration.
 
     Note:
         This is a temporary method used as a base case for building
@@ -422,20 +484,20 @@
     num_emaps = cfg.MODEL.UNROLLED.NUM_EMAPS
 
     # ResNet parameters
     kernel_size = cfg.MODEL.UNROLLED.KERNEL_SIZE
     if len(kernel_size) == 1:
         kernel_size = kernel_size[0]
     resnet_params = dict(
-        num_resblocks=cfg.MODEL.UNROLLED.NUM_RESBLOCKS,
-        in_chans=2 * num_emaps,  # complex -> real/imag
-        chans=cfg.MODEL.UNROLLED.NUM_FEATURES,
+        num_blocks=cfg.MODEL.UNROLLED.NUM_RESBLOCKS,
+        in_channels=2 * num_emaps,  # complex -> real/imag
+        channels=cfg.MODEL.UNROLLED.NUM_FEATURES,
         kernel_size=kernel_size,
-        drop_prob=cfg.MODEL.UNROLLED.DROPOUT,
+        dropout=cfg.MODEL.UNROLLED.DROPOUT,
         circular_pad=cfg.MODEL.UNROLLED.PADDING == "circular",
         act_type=cfg.MODEL.UNROLLED.CONV_BLOCK.ACTIVATION,
         norm_type=cfg.MODEL.UNROLLED.CONV_BLOCK.NORM,
         norm_affine=cfg.MODEL.UNROLLED.CONV_BLOCK.NORM_AFFINE,
         order=cfg.MODEL.UNROLLED.CONV_BLOCK.ORDER,
     )
 
-    return ResNet(**resnet_params)
+    return ResNetModel(**resnet_params)
```

### Comparing `meddlr-0.0.8a2/meddlr/modeling/meta_arch/vortex.py` & `meddlr-0.0.9/meddlr/modeling/meta_arch/vortex.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/ops/__init__.py` & `meddlr-0.0.9/meddlr/ops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ifft3c,
     ifftc,
     ifftnc,
     ifftshift,
 )
 from meddlr.ops.utils import (  # noqa: F401
     center_crop,
+    constant_pad,
     normalize,
     normalize_instance,
     pad,
     roll,
     sliding_window,
     time_average,
     zero_pad,
```

### Comparing `meddlr-0.0.8a2/meddlr/ops/categorical.py` & `meddlr-0.0.9/meddlr/ops/categorical.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/ops/complex.py` & `meddlr-0.0.9/meddlr/ops/complex.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,34 +256,44 @@
     if is_complex(x):
         return x.permute((0,) + tuple(range(2, x.ndim) + (1,)))
     else:
         order = (0,) + tuple(range(2, x.ndim - 2)) + (1, x.ndim - 1)
         return x.permute(order)
 
 
-def get_mask(x, eps=1e-11):
+def get_mask(x, eps=1e-11, coil_dim=None):
     """Returns a binary mask for where ``x`` is nonzero with ``eps`` tolerance.
 
       - 0, if both real and imaginary components are zero.
       - 1, if either real and imaginary components are non-zero.
 
     Args:
         x (torch.Tensor): A complex-valued tensor.
         eps (float): Tolerance for zer0-value.
+        coil_dim (int): The coil dimension.
+            When this is provided, if a pixel is non-zero for any coil,
+            we assume that pixel was acquired. This is useful when
+            a coil ``i`` has zero signal but the location was actually
+            acquired.
 
     Returns:
         torch.Tensor: A binary mask of shape ``x.shape``.
     """
     unsqueeze = True
     if is_complex(x):
         unsqueeze = False
         x = torch.view_as_real(x)
     assert x.size(-1) == 2
-    absx = abs(x)  # squashes last dimension
-    mask = torch.where(absx > eps, torch.ones_like(absx), torch.zeros_like(absx))
+
+    absx = abs(x)
+    loc = absx > eps  # squashes last dimension
+    if coil_dim is not None:
+        loc = loc.any(coil_dim, keepdims=True)
+    mask = torch.where(loc, torch.ones_like(absx), torch.zeros_like(absx))
+
     if unsqueeze:
         mask = mask.unsqueeze(-1)
     return mask
 
 
 def matmul(X, Y):
     """
```

### Comparing `meddlr-0.0.8a2/meddlr/ops/fft.py` & `meddlr-0.0.9/meddlr/ops/fft.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/ops/opt.py` & `meddlr-0.0.9/meddlr/ops/opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     Adapted from https://github.com/bo-10000/MoDL_PyTorch/blob/master/models/modl.py.
 
     Args:
         x: The initial input. Shape (B, ...).
         b: The residual. Shape (B, ...). Must be same shape as `x`.
         A_op: The function performing the normal equations.
             For complex numbers, this should be adjoint(A) * A.
+        mu: The L2 lambda, or regularization parameter (must be positive).
         max_iter: Maximum number of times to run conjugate gradient descent.
-        l2lam: The L2 lambda, or regularization parameter (must be positive).
         eps: Determines how small the residuals must be before termination.
             Stopping criterion is conj(r).T * r < eps ** 2.
         pbar: Whether to show a progress bar.
 
     Returns:
         torch.Tensor: x for the minimization equation above.
```

### Comparing `meddlr-0.0.8a2/meddlr/ops/utils.py` & `meddlr-0.0.9/meddlr/ops/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Sequence
+from typing import Any, Sequence
 
 import torch
 import torch.nn.functional as F
 
 import meddlr.ops.complex as cplx
 
 __all__ = [
     "roll",
     "pad",
     "zero_pad",
+    "constant_pad",
     "time_average",
     "sliding_window",
     "center_crop",
     "normalize",
     "normalize_instance",
 ]
 
@@ -100,14 +101,18 @@
         >>> out = zero_pad(x, (200, 250))
         >>> out.shape
         torch.Size([1, 200, 250, 3])
     """
     return pad(x, shape, mode="constant", value=0)
 
 
+def constant_pad(x: torch.Tensor, shape: Sequence[int], value: Any) -> torch.Tensor:
+    return pad(x, shape, mode="constant", value=value)
+
+
 def time_average(x, dim, eps=1e-6, keepdim=True):
     """
     Computes time average across a specified axis.
     """
     mask = cplx.get_mask(x)
     return x.sum(dim, keepdim=keepdim) / (mask.sum(dim, keepdim=keepdim) + eps)
```

### Comparing `meddlr-0.0.8a2/meddlr/solver/build.py` & `meddlr-0.0.9/meddlr/solver/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List
 
 import torch
 
 from meddlr.config import CfgNode
 
 from .lr_scheduler import NoOpLR, WarmupCosineLR, WarmupMultiStepLR
-from .optimizer import GradAccumOptimizer
+from .optimizer import GradAccumOptimizer, SophiaG
 
 
 def build_optimizer(cfg: CfgNode, model: torch.nn.Module) -> torch.optim.Optimizer:
     """
     Build an optimizer from config.
     """
     params: List[Dict[str, Any]] = []
@@ -32,14 +32,17 @@
 
 def _build_opt(params, cfg):
     optim = cfg.SOLVER.OPTIMIZER
     if optim == "SGD":
         optimizer = torch.optim.SGD(params, cfg.SOLVER.BASE_LR, momentum=cfg.SOLVER.MOMENTUM)
     elif optim == "Adam":
         optimizer = torch.optim.Adam(params, cfg.SOLVER.BASE_LR)
+    elif optim == "SophiaG":
+        # weight decay handled by build_optimizer
+        optimizer = SophiaG(params, cfg.SOLVER.BASE_LR, weight_decay=0.0)
     else:
         raise ValueError(f"Optimizer {optim} not supported")
 
     # Gradient accumulation wrapper.
     num_grad_accum = cfg.SOLVER.GRAD_ACCUM_ITERS
     if num_grad_accum < 1:
         raise ValueError(f"cfg.SOLVER.GRAD_ACCUM_ITERS must be >= 1. Got {num_grad_accum}")
```

### Comparing `meddlr-0.0.8a2/meddlr/solver/lr_scheduler.py` & `meddlr-0.0.9/meddlr/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/base/mask.py` & `meddlr-0.0.9/meddlr/transforms/base/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/base/motion.py` & `meddlr-0.0.9/meddlr/transforms/base/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/base/noise.py` & `meddlr-0.0.9/meddlr/transforms/base/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/base/spatial.py` & `meddlr-0.0.9/meddlr/transforms/base/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/build.py` & `meddlr-0.0.9/meddlr/transforms/build.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/builtin/mri.py` & `meddlr-0.0.9/meddlr/transforms/builtin/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/functional/mri.py` & `meddlr-0.0.9/meddlr/transforms/functional/mri.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/gen/choice.py` & `meddlr-0.0.9/meddlr/transforms/gen/choice.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/gen/mask.py` & `meddlr-0.0.9/meddlr/transforms/gen/mask.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/gen/motion.py` & `meddlr-0.0.9/meddlr/transforms/gen/motion.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/gen/noise.py` & `meddlr-0.0.9/meddlr/transforms/gen/noise.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/gen/spatial.py` & `meddlr-0.0.9/meddlr/transforms/gen/spatial.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/mixins.py` & `meddlr-0.0.9/meddlr/transforms/mixins.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/tf_scheduler.py` & `meddlr-0.0.9/meddlr/transforms/tf_scheduler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/transform.py` & `meddlr-0.0.9/meddlr/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/transforms/transform_gen.py` & `meddlr-0.0.9/meddlr/transforms/transform_gen.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/cfl.py` & `meddlr-0.0.9/meddlr/utils/cfl.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/cluster.py` & `meddlr-0.0.9/meddlr/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/collect_env.py` & `meddlr-0.0.9/meddlr/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/comm.py` & `meddlr-0.0.9/meddlr/utils/comm.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/deprecated.py` & `meddlr-0.0.9/meddlr/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/env.py` & `meddlr-0.0.9/meddlr/utils/env.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/events.py` & `meddlr-0.0.9/meddlr/utils/events.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/general.py` & `meddlr-0.0.9/meddlr/utils/general.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import List, Mapping
+from typing import List, Mapping, Union
 
 import torch
 
 from meddlr.utils import env
 
 _PATH_MANAGER = env.get_path_manager()
 
@@ -98,7 +98,33 @@
         if isinstance(v, Mapping):
             v = flatten_dict(v)
             for kk, vv in v.items():
                 r[k + delimiter + kk] = vv
         else:
             r[k] = v
     return r
+
+
+_NestedTensor = Mapping[str, torch.Tensor]
+NestedTensor = Mapping[str, Union[_NestedTensor, torch.Tensor]]
+
+
+def nested_apply(x: NestedTensor, fn):
+    if isinstance(x, Mapping):
+        return {k: nested_apply(v, fn) for k, v in x.items()}
+    assert isinstance(x, torch.Tensor)
+    return fn(x)
+
+
+def nested_cat(x: List[NestedTensor], dim=0):
+    """Concatenate a nested tensor."""
+    xtype = type(x[0])
+    for _x in x[1:]:
+        if not isinstance(_x, xtype):
+            raise ValueError(
+                "All inputs must have the same type. Got {} and {}".format(xtype, type(_x))
+            )
+
+    if isinstance(x[0], Mapping):
+        return {k: nested_cat([_x[k] for _x in x], dim=dim) for k in x[0].keys()}
+    assert isinstance(x[0], torch.Tensor)
+    return torch.cat(x, dim=dim)
```

### Comparing `meddlr-0.0.8a2/meddlr/utils/logger.py` & `meddlr-0.0.9/meddlr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/memory.py` & `meddlr-0.0.9/meddlr/utils/memory.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/path.py` & `meddlr-0.0.9/meddlr/utils/path.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/profiler.py` & `meddlr-0.0.9/meddlr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/registry.py` & `meddlr-0.0.9/meddlr/utils/registry.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr/utils/transforms.py` & `meddlr-0.0.9/meddlr/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/meddlr.egg-info/PKG-INFO` & `meddlr-0.0.9/meddlr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meddlr
-Version: 0.0.8a2
+Version: 0.0.9
 Summary: Meddlr is a config-driven framework built to simplify ML-based medical image reconstruction and analysis.
 Home-page: https://github.com/ad12/meddlr
 Author: The Meddlr Team
 Author-email: arjundd@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -57,14 +57,26 @@
 # OR set these as environment variables.
 os.environ["MEDDLR_RESULTS_DIR"] = "/path/to/save/results"
 os.environ["MEDDLR_DATASETS_DIR"] = "/path/to/datasets"
 ```
 
 Detailed instructions are available in [Getting Started](GETTING_STARTED.md).
 
+## Visualizations
+Use [MeddlrViz](https://github.com/ad12/meddlr-viz) to visualize your medical imaging datasets, ML models, and more!
+
+```bash
+pip install meddlr-viz
+```
+
+<div align="center">
+
+<image src="https://github.com/ad12/meddlr-viz/blob/main/static/brats.gif" height=400 alt="A gallery of images from the BRATS dataset" />
+</div>
+
 ## 🐘 Model Zoo
 Easily serve and download pretrained models from the model zoo. A (evolving) list of pre-trained models can be found [here](MODEL_ZOO.md), on [HuggingFace 🤗](https://huggingface.co/arjundd), and in [project folders](projects).
 
 To use them, pass the URLs for the config and weights (model) files to `mr.get_model_from_zoo`:
 
 ```python
 import meddlr as mr
```

### Comparing `meddlr-0.0.8a2/meddlr.egg-info/SOURCES.txt` & `meddlr-0.0.9/meddlr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,24 @@
 meddlr/modeling/blocks/fuse_blocks.py
 meddlr/modeling/layers/__init__.py
 meddlr/modeling/layers/build.py
 meddlr/modeling/layers/conv.py
 meddlr/modeling/layers/gauss.py
 meddlr/modeling/layers/layers2D.py
 meddlr/modeling/layers/layers3D.py
+meddlr/modeling/layers/scale.py
 meddlr/modeling/meta_arch/__init__.py
 meddlr/modeling/meta_arch/build.py
 meddlr/modeling/meta_arch/cs_model.py
 meddlr/modeling/meta_arch/denoising.py
 meddlr/modeling/meta_arch/generalized_unet.py
 meddlr/modeling/meta_arch/m2r.py
 meddlr/modeling/meta_arch/n2r.py
 meddlr/modeling/meta_arch/nm2r.py
+meddlr/modeling/meta_arch/resnet.py
 meddlr/modeling/meta_arch/ssdu.py
 meddlr/modeling/meta_arch/unet.py
 meddlr/modeling/meta_arch/unrolled.py
 meddlr/modeling/meta_arch/vortex.py
 meddlr/ops/__init__.py
 meddlr/ops/categorical.py
 meddlr/ops/complex.py
```

### Comparing `meddlr-0.0.8a2/meddlr.egg-info/requires.txt` & `meddlr-0.0.9/meddlr.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 pyxb
 h5py
 matplotlib
-numpy
+numpy<=1.23.5
 tensorboard
 fvcore
 mridata
 scikit-image>=0.18.2
 sigpy>=0.1.17
 ismrmrd
 pandas
 silx
 tqdm
 omegaconf
-torchmetrics>=0.5.1
+torchmetrics<=0.11.4,>=0.5.1
 iopath
 packaging
 
 [all]
-monai
-lpips
 medpy
-gdown<4.6.0
 iocursor
 requests
+monai
+gdown<4.6.0
+lpips
 
 [alldev]
-flake8-bugbear
-lpips
 sphinx-rtd-theme
-sphinxcontrib-bibtex
-pooch
 flake8
-requests
-tifffile<=2022.5.4
-coverage
+monai
+pooch
+pytest
 medpy
+tifffile<=2022.5.4
+sphinxcontrib-bibtex
+sphinx
 wrapt
+requests
+black==22.12.0
+parameterized
 flake8-comprehensions
-pytest
-gdown<4.6.0
-sphinx
+flake8-bugbear
+iocursor
+m2r2
 sphinxcontrib.bibtex
-isort
-parameterized
 pre-commit>=2.9.3
-black==22.12.0
-monai
-m2r2
-iocursor
+gdown<4.6.0
+coverage
+lpips
+isort
 
 [benchmarking]
 medpy
 
 [deployment]
 gdown<4.6.0
 requests
```

### Comparing `meddlr-0.0.8a2/setup.cfg` & `meddlr-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/setup.py` & `meddlr-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,26 +182,27 @@
 URL = "https://github.com/ad12/meddlr"
 REQUIRES_PYTHON = ">=3.6"
 
 REQUIRED = [
     "pyxb",  # need to install before ismrmrd
     "h5py",
     "matplotlib",
-    "numpy",
+    # Pin the numpy version because other libraries dont handle the np.float dtype yet.
+    "numpy<=1.23.5",
     "tensorboard",
     "fvcore",
     "mridata",
     "scikit-image>=0.18.2",
     "sigpy>=0.1.17",
     "ismrmrd",
     "pandas",
     "silx",
     "tqdm",
     "omegaconf",
-    "torchmetrics>=0.5.1",
+    "torchmetrics>=0.5.1,<=0.11.4",
     "iopath",
     "packaging",
 ]
 
 EXTRAS = {
     "dev": [
         # Formatting
```

### Comparing `meddlr-0.0.8a2/tests/test_experiments.py` & `meddlr-0.0.9/tests/test_experiments.py`

 * *Files identical despite different names*

### Comparing `meddlr-0.0.8a2/tests/test_reproducibility.py` & `meddlr-0.0.9/tests/test_reproducibility.py`

 * *Files identical despite different names*

