# Comparing `tmp/GANDLF-0.0.17.dev20230802.tar.gz` & `tmp/GANDLF-0.0.17.dev20230803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230802.tar", last modified: Wed Aug  2 03:13:05 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230803.tar", last modified: Thu Aug  3 03:13:53 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230802.tar` & `GANDLF-0.0.17.dev20230803.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.113397 GANDLF-0.0.17.dev20230802/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.057393 GANDLF-0.0.17.dev20230802/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.057393 GANDLF-0.0.17.dev20230802/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.061394 GANDLF-0.0.17.dev20230802/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.065394 GANDLF-0.0.17.dev20230802/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.065394 GANDLF-0.0.17.dev20230802/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.069394 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/hed_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.069394 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.073394 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.073394 GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.077395 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.081395 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.081395 GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.085395 GANDLF-0.0.17.dev20230802/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.089395 GANDLF-0.0.17.dev20230802/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.097396 GANDLF-0.0.17.dev20230802/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.105396 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.105396 GANDLF-0.0.17.dev20230802/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.105396 GANDLF-0.0.17.dev20230802/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.113397 GANDLF-0.0.17.dev20230802/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 03:12:57.000000 GANDLF-0.0.17.dev20230802/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:13:05.057393 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-02 03:13:05.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-02 03:13:05.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:13:05.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:10:32.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 03:13:05.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 03:13:05.000000 GANDLF-0.0.17.dev20230802/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-02 03:13:05.113397 GANDLF-0.0.17.dev20230802/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 03:13:05.113397 GANDLF-0.0.17.dev20230802/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-02 03:10:14.000000 GANDLF-0.0.17.dev20230802/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.745451 GANDLF-0.0.17.dev20230803/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.661450 GANDLF-0.0.17.dev20230803/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.669450 GANDLF-0.0.17.dev20230803/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.673450 GANDLF-0.0.17.dev20230803/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.681450 GANDLF-0.0.17.dev20230803/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.681450 GANDLF-0.0.17.dev20230803/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.685450 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/hed_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.685450 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.685450 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.689450 GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.693450 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.697450 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.697450 GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.701450 GANDLF-0.0.17.dev20230803/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.705450 GANDLF-0.0.17.dev20230803/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.721451 GANDLF-0.0.17.dev20230803/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.733451 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.737451 GANDLF-0.0.17.dev20230803/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.737451 GANDLF-0.0.17.dev20230803/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.745451 GANDLF-0.0.17.dev20230803/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 03:13:45.000000 GANDLF-0.0.17.dev20230803/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 03:13:53.665450 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-03 03:13:53.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-03 03:13:53.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:13:53.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 03:10:52.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 03:13:53.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 03:13:53.000000 GANDLF-0.0.17.dev20230803/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-03 03:13:53.745451 GANDLF-0.0.17.dev20230803/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 03:13:53.745451 GANDLF-0.0.17.dev20230803/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-03 03:10:27.000000 GANDLF-0.0.17.dev20230803/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230802/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230803/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230803/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230803/Dockerfile-CPU`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 LABEL version=1.0
 
 # Install fresh Python and dependencies for build-from-source
 RUN apt-get update && apt-get install -y python3.8 python3-pip libjpeg8-dev zlib1g-dev python3-dev libpython3.8-dev libffi-dev libgl1
 RUN python3.8 -m pip install --upgrade pip
 # EXPLICITLY install cpu versions of torch/torchvision (not all versions have +cpu modes on PyPI...)
 RUN python3.8 -m pip install torch==1.13.1+cpu torchvision==0.14.1+cpu torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cpu
-RUN python3.8 -m pip install openvino-dev==2022.1.0 opencv-python-headless mlcube_docker
+RUN python3.8 -m pip install openvino-dev==2023.0.1 opencv-python-headless mlcube_docker
 
 # Do some dependency installation separately here to make layer caching more efficient
 COPY ./setup.py ./setup.py
 RUN python3.8 -c "from setup import requirements; file = open('requirements.txt', 'w'); file.writelines([req + '\n' for req in requirements]); file.close()" \
     && python3.8 -m pip install -r ./requirements.txt
 
 COPY . /GaNDLF
```

### Comparing `GANDLF-0.0.17.dev20230802/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230803/Dockerfile-CUDA11.6`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Install instructions for NVIDIA Container Toolkit allowing you to use the host's GPU: https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html
 # Note that to do this on a Windows host you need experimental feature "CUDA on WSL" -- not yet stable.
 
 # Explicitly install python3.8 (this uses 11.1 for now, as PyTorch LTS 1.8.2 is built against it)
 RUN apt-get update && apt-get install -y python3.8 python3-pip libjpeg8-dev zlib1g-dev python3-dev libpython3.8-dev libffi-dev libgl1
 RUN python3.8 -m pip install --upgrade pip
 RUN python3.8 -m pip install torch==1.13.1+cu116 torchvision==0.14.1+cu116 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu116
-RUN python3.8 -m pip install openvino-dev==2022.1.0 opencv-python-headless mlcube_docker
+RUN python3.8 -m pip install openvino-dev==2023.0.1 opencv-python-headless mlcube_docker
 
 # Do some dependency installation separately here to make layer caching more efficient
 COPY ./setup.py ./setup.py
 RUN python3.8 -c "from setup import requirements; file = open('requirements.txt', 'w'); file.writelines([req + '\n' for req in requirements]); file.close()" \
     && python3.8 -m pip install -r ./requirements.txt
 
 COPY . /GaNDLF
```

### Comparing `GANDLF-0.0.17.dev20230802/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230803/Dockerfile-ROCm`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 LABEL version=1.0
 
 # Quick start instructions on using Docker with ROCm: https://github.com/RadeonOpenCompute/ROCm-docker/blob/master/quick-start.md
 
 # The base image contains ROCm, python 3.8 and pytorch already, no need to install those
 RUN python3 -m pip install --upgrade pip
 RUN python3.8 -m pip install torch==1.13.1+rocm5.2 torchvision==0.14.1+rocm5.2 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/rocm5.2
-RUN python3 -m pip install --upgrade pip && python3 -m pip install openvino-dev==2022.1.0 opencv-python-headless mlcube_docker
+RUN python3 -m pip install --upgrade pip && python3 -m pip install openvino-dev==2023.0.1 opencv-python-headless mlcube_docker
 RUN apt-get update && apt-get install -y libgl1
 
 # Do some dependency installation separately here to make layer caching more efficient
 COPY ./setup.py ./setup.py
 RUN python3.8 -c "from setup import requirements; file = open('requirements.txt', 'w'); file.writelines([req + '\n' for req in requirements]); file.close()" \
     && python3.8 -m pip install -r ./requirements.txt
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230803/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/generate_metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import yaml
 from pprint import pprint
 import pandas as pd
 from tqdm import tqdm
 import torch
 import torchio
 import SimpleITK as sitk
@@ -189,14 +190,38 @@
                 torch.Tensor: The output tensor in the format that torchmetrics expects.
             """
             if input_tensor.shape[-1] == 1:
                 return input_tensor.squeeze(-1).unsqueeze(0)
             else:
                 return input_tensor
 
+        def __percentile_clip(input_tensor, reference_tensor=None, p_min=0.5, p_max=99.5, strictlyPositive=True):
+            """Normalizes a tensor based on percentiles. Clips values below and above the percentile.
+            Percentiles for normalization can come from another tensor.
+
+            Args:
+                input_tensor (torch.Tensor): Tensor to be normalized based on the data from the reference_tensor.
+                    If reference_tensor is None, the percentiles from this tensor will be used.
+                reference_tensor (torch.Tensor, optional): The tensor used for obtaining the percentiles.
+                p_min (float, optional): Lower end percentile. Defaults to 0.5.
+                p_max (float, optional): Upper end percentile. Defaults to 99.5.
+                strictlyPositive (bool, optional): Ensures that really all values are above 0 before normalization. Defaults to True.
+
+            Returns:
+                torch.Tensor: The input_tensor normalized based on the percentiles of the reference tensor.
+            """
+            reference_tensor = input_tensor if reference_tensor is None else reference_tensor
+            v_min, v_max = np.percentile(reference_tensor, [p_min,p_max]) #get p_min percentile and p_max percentile
+
+            # set lower bound to be 0 if strictlyPositive is enabled
+            v_min = max(v_min, 0.0) if strictlyPositive else v_min
+            output_tensor = np.clip(input_tensor,v_min,v_max) #clip values to percentiles from reference_tensor
+            output_tensor = (output_tensor - v_min)/(v_max-v_min) #normalizes values to [0;1]
+            return output_tensor
+
         for _, row in tqdm(input_df.iterrows(), total=input_df.shape[0]):
             current_subject_id = row[headers["subjectid"]]
             overall_stats_dict[current_subject_id] = {}
             target_image = __fix_2d_tensor(
                 torchio.ScalarImage(row[headers["target"]]).data
             )
             pred_image = __fix_2d_tensor(
@@ -215,17 +240,17 @@
             # Get Infill region (we really are only interested in the infill region)
             output_infill = (pred_image * mask).float()
             gt_image_infill = (target_image * mask).float()
 
             # Normalize to [0;1] based on GT (otherwise MSE will depend on the image intensity range)
             normalize = parameters.get("normalize", True)
             if normalize:
-                v_max = gt_image_infill.max()
-                output_infill /= v_max
-                gt_image_infill /= v_max
+                reference_tensor = target_image * ~mask #use all the tissue that is not masked for normalization
+                gt_image_infill = __percentile_clip(gt_image_infill, reference_tensor=reference_tensor, p_min=0.5, p_max=99.5, strictlyPositive=True)
+                output_infill = __percentile_clip(output_infill, reference_tensor=reference_tensor, p_min=0.5, p_max=99.5, strictlyPositive=True)
 
             overall_stats_dict[current_subject_id][
                 "ssim"
             ] = structural_similarity_index(gt_image_infill, output_infill, mask).item()
 
             # ncc metrics
             overall_stats_dict[current_subject_id]["ncc_mean"] = ncc_mean(
@@ -254,16 +279,21 @@
                 gt_image_infill, output_infill
             ).item()
 
             overall_stats_dict[current_subject_id]["mae"] = mean_absolute_error(
                 gt_image_infill, output_infill
             ).item()
 
+            #TODO: use data_range=1.0 as parameter for PSNR when the Pull request is accepted that introduces the data_range parameter!
             # PSNR - similar to pytorch PeakSignalNoiseRatio until 4 digits after decimal point
             overall_stats_dict[current_subject_id]["psnr"] = peak_signal_noise_ratio(
                 gt_image_infill, output_infill
             ).item()
 
+            overall_stats_dict[current_subject_id]["psnr_eps"] = peak_signal_noise_ratio(
+                gt_image_infill, output_infill, epsilon=sys.float_info.epsilon
+            ).item()
+
     pprint(overall_stats_dict)
     if outputfile is not None:
         with open(outputfile, "w") as outfile:
             yaml.dump(overall_stats_dict, outfile)
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/post_training_model_optimization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import os
 from GANDLF.compute import create_pytorch_objects
 from GANDLF.parseConfig import parseConfig
 from GANDLF.utils import version_check, load_model, optimize_and_save_model
 
 
-def post_training_model_optimization(model_path, config_path):
+def post_training_model_optimization(model_path: str, config_path: str) -> bool:
     """
     CLI function to optimize a model for deployment.
 
     Args:
         model_path (str): Path to the model file.
         config_path (str): Path to the config file.
 
     Returns:
         bool: True if successful, False otherwise.
     """
-
+    # Load the model and its parameters from the given paths
     main_dict = load_model(model_path, "cpu")
     parameters = main_dict.get("parameters", None)
+
+    # If parameters are not available in the model file, parse them from the config file
     parameters = (
         parseConfig(config_path, version_check_flag=False)
         if parameters is None
         else parameters
     )
-    (
-        model,
-        _,
-        _,
-        _,
-        _,
-        parameters,
-    ) = create_pytorch_objects(parameters, device="cpu")
+
+    # Create PyTorch objects and set onnx_export to True for optimization
+    model, _, _, _, _, parameters = create_pytorch_objects(parameters, device="cpu")
     parameters["model"]["onnx_export"] = True
 
+    # Perform version check and load the model's state dictionary
     version_check(parameters["version"], version_to_check=main_dict["version"])
     model.load_state_dict(main_dict["model_state_dict"])
+
+    # Optimize the model and save it to an ONNX file
     optimize_and_save_model(model, parameters, model_path, onnx_export=True)
+
+    # Check if the optimized model file exists
     optimized_model_path = model_path.replace("pth.tar", "onnx")
     if not os.path.exists(optimized_model_path):
-        print("Error while optimizing model.")
+        print("Error while optimizing the model.")
         return False
+
     return True
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230803/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230803/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/hed_augs.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/hed_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230803/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230803/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230803/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230803/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230803/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230803/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230803/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230803/GANDLF/metrics/synthesis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import sys
 import SimpleITK as sitk
 import PIL.Image
 import numpy as np
 import torch
 from torchmetrics import (
     StructuralSimilarityIndexMeasure,
     MeanSquaredError,
     MeanSquaredLogError,
     MeanAbsoluteError,
+    PeakSignalNoiseRatio,
 )
 from GANDLF.utils import get_image_from_tensor
 
 
 def structural_similarity_index(target, prediction, mask=None) -> torch.Tensor:
     """
     Computes the structural similarity index between the target and prediction.
@@ -21,15 +21,15 @@
         prediction (torch.Tensor): The prediction tensor.
         mask (torch.Tensor, optional): The mask tensor. Defaults to None.
 
     Returns:
         torch.Tensor: The structural similarity index.
     """
     ssim = StructuralSimilarityIndexMeasure(return_full_image=True)
-    _, ssim_idx_full_image = ssim(target, prediction)
+    _, ssim_idx_full_image = ssim(preds=prediction, target=target)
     mask = torch.ones_like(ssim_idx_full_image) if mask is None else mask
     try:
         ssim_idx = ssim_idx_full_image[mask]
     except Exception as e:
         print(f"Error: {e}")
         if len(ssim_idx_full_image.shape) == 0:
             ssim_idx = torch.ones_like(mask) * ssim_idx_full_image
@@ -41,55 +41,62 @@
     Computes the mean squared error between the target and prediction.
 
     Args:
         target (torch.Tensor): The target tensor.
         prediction (torch.Tensor): The prediction tensor.
     """
     mse = MeanSquaredError()
-    return mse(target, prediction)
+    return mse(preds=prediction, target=target)
 
 
-def peak_signal_noise_ratio(target, prediction) -> torch.Tensor:
+def peak_signal_noise_ratio(target, prediction, data_range=None, epsilon=None) -> torch.Tensor:
     """
     Computes the peak signal to noise ratio between the target and prediction.
 
     Args:
         target (torch.Tensor): The target tensor.
         prediction (torch.Tensor): The prediction tensor.
+        data_range (float, optional): If not None, this data range is used as enumerator instead of computing it from the given data. Defaults to None.
+        epsilon (float, optional): If not None, this epsilon is added to the denominator of the fraction to avoid infinity as output. Defaults to None.
     """
-    mse = mean_squared_error(target, prediction)
-    return (
-        10.0
-        * torch.log10((torch.max(target) - torch.min(target)) ** 2)
-        / (mse + sys.float_info.epsilon)
-    )
+
+    if epsilon == None:
+        psnr = PeakSignalNoiseRatio(data_range=data_range)
+        return psnr(preds=prediction, target=target)
+    else: # implementation of PSNR that does not give 'inf'/'nan' when 'mse==0'
+        mse = mean_squared_error(target, prediction)
+        if data_range == None: #compute data_range like torchmetrics if not given
+            min_v = 0 if torch.min(target) > 0 else torch.min(target) #look at this line
+            max_v = torch.max(target)
+            data_range = max_v - min_v
+        return 10.0 * torch.log10((data_range ** 2) / (mse + epsilon))
 
 
 def mean_squared_log_error(target, prediction) -> torch.Tensor:
     """
     Computes the mean squared log error between the target and prediction.
 
     Args:
         target (torch.Tensor): The target tensor.
         prediction (torch.Tensor): The prediction tensor.
     """
     mle = MeanSquaredLogError()
-    return mle(target, prediction)
+    return mle(preds=prediction, target=target)
 
 
 def mean_absolute_error(target, prediction) -> torch.Tensor:
     """
     Computes the mean absolute error between the target and prediction.
 
     Args:
         target (torch.Tensor): The target tensor.
         prediction (torch.Tensor): The prediction tensor.
     """
     mae = MeanAbsoluteError()
-    return mae(target, prediction)
+    return mae(preds=prediction, target=target)
 
 
 def _get_ncc_image(target, prediction) -> sitk.Image:
     """
     Computes normalized cross correlation image between target and prediction.
 
     Args:
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230803/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230803/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230803/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230803/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230803/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/modelio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-import os, hashlib, pkg_resources, subprocess
+import hashlib
+import os
+import subprocess
+from typing import Any, Dict
+
 import torch
 
-from .generic import get_unique_timestamp
 from ..version import __version__
+from .generic import get_unique_timestamp
 
 # these are the base keys for the model dictionary to save
 model_dict_full = {
     "epoch": 0,
     "model_state_dict": None,
     "optimizer_state_dict": None,
     "loss": None,
@@ -27,52 +31,55 @@
 
 
 def optimize_and_save_model(model, params, path, onnx_export=True):
     """
     Perform post-training optimization and save it to a file.
 
     Args:
-        model (torch model): Trained torch model.
+        model (torch.nn.Module): Trained torch model.
         params (dict): The parameter dictionary.
         path (str): The path to save the model dictionary to.
         onnx_export (bool): Whether to export to ONNX and OpenVINO.
     """
+    # Check if ONNX export is enabled in the parameter dictionary
     onnx_export = params["model"].get("onnx_export", onnx_export)
-    # check for incompatible topologies and disable onnx export
-    # customized imagenet_vgg no longer supported for onnx export: https://github.com/pytorch/pytorch/issues/42653
+
+    # Check for incompatible topologies and disable ONNX export
+    # Customized imagenet_vgg no longer supported for ONNX export
     if onnx_export:
-        if (params["model"]["architecture"] in ["sdnet", "brain_age"]) or (
-            "imagenet_vgg" in params["model"]["architecture"]
-        ):
+        architecture = params["model"]["architecture"]
+        if architecture in ["sdnet", "brain_age"] or "imagenet_vgg" in architecture:
             onnx_export = False
 
-    if not (onnx_export):
+    if not onnx_export:
+        # Print a warning if ONNX export is disabled and not already warned
         if "onnx_print" not in params:
             print("WARNING: Current model is not supported by ONNX/OpenVINO!")
             params["onnx_print"] = True
         return
     else:
         try:
-            print("Optimizing best model.")
+            print("Optimizing the best model.")
             num_channel = params["model"]["num_channels"]
             model_dimension = params["model"]["dimension"]
-            ov_output_data_type = params["model"].get("data_type", "FP32")
             input_shape = params["patch_size"]
             onnx_path = path
-            if not (onnx_path.endswith(".onnx")):
+            if not onnx_path.endswith(".onnx"):
                 onnx_path = onnx_path.replace("pth.tar", "onnx")
+
             if model_dimension == 2:
                 dummy_input = torch.randn(
                     (1, num_channel, input_shape[0], input_shape[1])
                 )
             else:
                 dummy_input = torch.randn(
                     (1, num_channel, input_shape[0], input_shape[1], input_shape[2])
                 )
 
+            # Export the model to ONNX format
             with torch.no_grad():
                 torch.onnx.export(
                     model.to("cpu"),
                     dummy_input.to("cpu"),
                     onnx_path,
                     opset_version=11,
                     export_params=True,
@@ -82,103 +89,101 @@
                 )
 
             ov_output_dir = os.path.dirname(os.path.abspath(path))
         except RuntimeWarning:
             print("WARNING: Cannot export to ONNX model.")
             return
 
-        # https://github.com/mlcommons/GaNDLF/issues/605
+        # Check if OpenVINO is present and try to convert the ONNX model
         openvino_present = False
         try:
-            import openvino
-
-            openvino_present = True
+            import openvino as ov
+            from openvino.tools.mo import convert_model
+            from openvino.runtime import get_version
+            openvino_present = False
+            # check for the correct openvino version to prevent inadvertent api breaks
+            if "2023.0.1" in get_version():
+                openvino_present = True
         except ImportError:
             print("WARNING: OpenVINO is not present.")
 
         if openvino_present:
+            xml_path = onnx_path.replace("onnx", "xml")
+            bin_path = onnx_path.replace("onnx", "bin")
             try:
                 if model_dimension == 2:
-                    subprocess.call(
-                        [
-                            "mo",
-                            "--input_model",
-                            "{0}".format(onnx_path),
-                            "--input_shape",
-                            "[1,{0},{1},{2}]".format(
-                                num_channel, input_shape[0], input_shape[1]
-                            ),
-                            "--data_type",
-                            "{0}".format(ov_output_data_type),
-                            "--output_dir",
-                            "{0}".format(ov_output_dir),
-                        ],
+                    ov_model = convert_model(
+                        onnx_path,
+                        input_shape=(1, num_channel, input_shape[0], input_shape[1]),
                     )
                 else:
-                    subprocess.call(
-                        [
-                            "mo",
-                            "--input_model",
-                            "{0}".format(onnx_path),
-                            "--input_shape",
-                            "[1,{0},{1},{2},{3}]".format(
-                                num_channel,
-                                input_shape[0],
-                                input_shape[1],
-                                input_shape[2],
-                            ),
-                            "--data_type",
-                            "{0}".format(ov_output_data_type),
-                            "--output_dir",
-                            "{0}".format(ov_output_dir),
-                        ],
+                    ov_model = convert_model(
+                        onnx_path,
+                        input_shape=(
+                            1,
+                            num_channel,
+                            input_shape[0],
+                            input_shape[1],
+                            input_shape[2],
+                        ),
                     )
-            except subprocess.CalledProcessError:
-                print("WARNING: OpenVINO Model Optimizer IR conversion failed.")
+                ov.runtime.serialize(ov_model, xml_path=xml_path, bin_path=bin_path)
+            except Exception as e:
+                print("WARNING: OpenVINO Model Optimizer IR conversion failed: " + e)
 
 
-def save_model(model_dict, model, params, path, onnx_export=True):
+def save_model(
+    model_dict: Dict[str, Any],
+    model: torch.nn.Module,
+    params: Dict[str, Any],
+    path: str,
+    onnx_export: bool = True,
+):
     """
     Save the model dictionary to a file.
 
     Args:
         model_dict (dict): Model dictionary to save.
-        model (torch model): Trained torch model.
+        model (torch.nn.Module): Trained torch model.
         params (dict): The parameter dictionary.
         path (str): The path to save the model dictionary to.
         onnx_export (bool): Whether to export to ONNX and OpenVINO.
     """
     model_dict["timestamp"] = get_unique_timestamp()
     model_dict["timestamp_hash"] = hashlib.sha256(
         str(model_dict["timestamp"]).encode("utf-8")
     ).hexdigest()
     model_dict["version"] = __version__
     model_dict["parameters"] = params
+
     try:
         model_dict["git_hash"] = (
             subprocess.check_output(["git", "rev-parse", "HEAD"])
             .decode("ascii")
             .strip()
         )
     except subprocess.CalledProcessError:
         model_dict["git_hash"] = None
+
     torch.save(model_dict, path)
 
     # post-training optimization
     optimize_and_save_model(model, params, path, onnx_export=onnx_export)
 
 
-def load_model(path, device, full_sanity_check=True):
+def load_model(
+    path: str, device: torch.device, full_sanity_check: bool = True
+) -> Dict[str, Any]:
     """
     Load a model dictionary from a file.
 
     Args:
         path (str): The path to save the model dictionary to.
         device (torch.device): The device to run the model on.
-        full_sanity_check (bool): Whether to run full sanity checking on model.
+        full_sanity_check (bool): Whether to run full sanity checking on the model.
 
     Returns:
         dict: Model dictionary containing model parameters and metadata.
     """
     model_dict = torch.load(path, map_location=device)
 
     # check if the model dictionary is complete
@@ -201,15 +206,15 @@
             "Model dictionary is incomplete; the following keys are missing:",
             incomplete_required_keys,
         )
 
     return model_dict
 
 
-def load_ov_model(path, device="CPU"):
+def load_ov_model(path: str, device: str = "CPU"):
     """
     Load an OpenVINO IR model from an .xml file.
 
     Args:
         path (str): The path to the OpenVINO .xml file.
         device (str): The device to run inference, can be "CPU", "GPU" or "MULTI:CPU,GPU". Default to be "CPU".
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230803/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230803/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230802
+Version: 0.0.17.dev20230803
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230802 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230803 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230802/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230803/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/LICENSE` & `GANDLF-0.0.17.dev20230803/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/PKG-INFO` & `GANDLF-0.0.17.dev20230803/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230802
+Version: 0.0.17.dev20230803
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230802 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230803 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230802/README.md` & `GANDLF-0.0.17.dev20230803/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/SECURITY.md` & `GANDLF-0.0.17.dev20230803/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230803/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_collectStats` & `GANDLF-0.0.17.dev20230803/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230803/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230803/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_deploy` & `GANDLF-0.0.17.dev20230803/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230803/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230803/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230803/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_preprocess` & `GANDLF-0.0.17.dev20230803/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230803/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_run` & `GANDLF-0.0.17.dev20230803/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230803/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230802/setup.py` & `GANDLF-0.0.17.dev20230803/setup.py`

 * *Files identical despite different names*

