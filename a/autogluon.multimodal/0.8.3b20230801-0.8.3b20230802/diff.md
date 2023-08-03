# Comparing `tmp/autogluon.multimodal-0.8.3b20230801.tar.gz` & `tmp/autogluon.multimodal-0.8.3b20230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.8.3b20230801.tar", last modified: Tue Aug  1 09:04:14 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.8.3b20230802.tar", last modified: Wed Aug  2 09:04:19 2023, max compression
```

## Comparing `autogluon.multimodal-0.8.3b20230801.tar` & `autogluon.multimodal-0.8.3b20230802.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.393188 autogluon.multimodal-0.8.3b20230801/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-01 09:04:14.393188 autogluon.multimodal-0.8.3b20230801/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:04:14.393188 autogluon.multimodal-0.8.3b20230801/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.381188 autogluon.multimodal-0.8.3b20230801/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.381188 autogluon.multimodal-0.8.3b20230801/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.381188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.381188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.385188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.389188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.389188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86789 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.389188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.389188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.389188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   120647 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.393188 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22986 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-01 09:03:42.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:04:14.381188 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:04:14.000000 autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.955074 autogluon.multimodal-0.8.3b20230802/
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-02 09:04:19.955074 autogluon.multimodal-0.8.3b20230802/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:04:19.955074 autogluon.multimodal-0.8.3b20230802/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.939074 autogluon.multimodal-0.8.3b20230802/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.939074 autogluon.multimodal-0.8.3b20230802/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.943074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.947074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.947074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.947074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86709 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.947074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.951074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.951074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120569 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.951074 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22986 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-02 09:03:48.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:04:19.939074 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:04:19.000000 autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.8.3b20230801/PKG-INFO` & `autogluon.multimodal-0.8.3b20230802/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230801
+Version: 0.8.3b20230802
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.8.3b20230801/setup.py` & `autogluon.multimodal-0.8.3b20230802/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     "scipy",  # version range defined in `core/_setup_utils.py`
     "pandas",  # version range defined in `core/_setup_utils.py`
     "scikit-learn",  # version range defined in `core/_setup_utils.py`
     "Pillow",  # version range defined in `core/_setup_utils.py`
     "tqdm",  # version range defined in `core/_setup_utils.py`
     "boto3",  # version range defined in `core/_setup_utils.py`
     "torch",  # version range defined in `core/_setup_utils.py`
+    "pytorch-lightning",  # version range defined in `core/_setup_utils.py`
     "requests>=2.21,<3",
     "jsonschema>=4.14,<4.18",
     "seqeval>=1.2.2,<1.3.0",
     "evaluate>=0.2.2,<0.4.0",
     "accelerate>=0.9,<0.17",
     "timm>=0.9.2,<0.10.0",
     "torchvision>=0.14.0,<0.16.0",  # torch 1.13 requires torchvision 0.14. Increase it to 0.15 when dropping the support of torch 1.13.
     "scikit-image>=0.19.1,<0.20.0",
-    "pytorch-lightning>=1.9.0,<1.10.0",
     "text-unidecode>=1.3,<1.4",
     "torchmetrics>=1.0.0,<1.1.0",
     "transformers[sentencepiece]>=4.23.0,<4.27.0",
     "nptyping>=1.4.4,<2.5.0",
     "omegaconf>=2.1.1,<2.3.0",
     f"autogluon.core[raytune]=={version}",
     f"autogluon.features=={version}",
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,14 +838,15 @@
             lr_schedule=config.optimization.lr_schedule,
             lr=config.optimization.learning_rate,
             lr_decay=config.optimization.lr_decay,
             end_lr=config.optimization.end_lr,
             lr_mult=config.optimization.lr_mult,
             weight_decay=config.optimization.weight_decay,
             warmup_steps=config.optimization.warmup_steps,
+            track_grad_norm=OmegaConf.select(config, "optimization.track_grad_norm", default=-1),
         )
         metrics_kwargs = dict(
             validation_metric=validation_metric,
             validation_metric_name=validation_metric_name,
             custom_metric_func=custom_metric_func,
         )
 
@@ -923,35 +924,34 @@
             grad_steps = max(
                 config.env.batch_size // (config.env.per_gpu_batch_size * num_gpus * config.env.num_nodes),
                 1,
             )
 
         if not hpo_mode:
             if num_gpus <= 1:
-                strategy = None
+                strategy = "auto"
             else:
                 strategy = config.env.strategy
         else:
-            # we don't support running each trial in parallel without ray lightning
             # TODO: checkout lightning support for ray tune for multi gpu support
-            strategy = None
+            strategy = "auto"
             num_gpus = min(num_gpus, 1)
 
         config.env.num_gpus = num_gpus
         config.env.precision = precision
         config.env.strategy = strategy
         self._config = config
         # save artifacts for the current running, except for model checkpoint, which will be saved in trainer
         self.save(save_path)
 
         blacklist_msgs = ["already configured with model summary"]
         log_filter = LogFilter(blacklist_msgs)
         with apply_log_filter(log_filter):
             trainer = pl.Trainer(
-                accelerator="gpu" if num_gpus > 0 else None,
+                accelerator="gpu" if num_gpus > 0 else "auto",
                 devices=get_available_devices(
                     num_gpus=num_gpus,
                     auto_select_gpus=config.env.auto_select_gpus,
                 ),
                 num_nodes=config.env.num_nodes,
                 precision=precision,
                 strategy=strategy,
@@ -966,15 +966,14 @@
                 gradient_clip_algorithm=OmegaConf.select(
                     config, "optimization.gradient_clip_algorithm", default="norm"
                 ),
                 accumulate_grad_batches=grad_steps,
                 log_every_n_steps=OmegaConf.select(config, "optimization.log_every_n_steps", default=10),
                 enable_progress_bar=enable_progress_bar,
                 fast_dev_run=config.env.fast_dev_run,
-                track_grad_norm=OmegaConf.select(config, "optimization.track_grad_norm", default=-1),
                 val_check_interval=config.optimization.val_check_interval,
                 check_val_every_n_epoch=config.optimization.check_val_every_n_epoch
                 if hasattr(config.optimization, "check_val_every_n_epoch")
                 else 1,
                 reload_dataloaders_every_n_epochs=1,
             )
 
@@ -1286,15 +1285,15 @@
             blacklist_msgs.append("IPU available")
             blacklist_msgs.append("HPU available")
             blacklist_msgs.append("select gpus")
             blacklist_msgs.append("LOCAL_RANK")
         log_filter = LogFilter(blacklist_msgs)
         with apply_log_filter(log_filter):
             evaluator = pl.Trainer(
-                accelerator="gpu" if num_gpus > 0 else None,
+                accelerator="gpu" if num_gpus > 0 else "auto",
                 devices=get_available_devices(num_gpus=num_gpus, auto_select_gpus=self._config.env.auto_select_gpus),
                 num_nodes=self._config.env.num_nodes,
                 precision=precision,
                 strategy=strategy,
                 benchmark=False,
                 enable_progress_bar=self._enable_progress_bar,
                 deterministic=self._config.env.deterministic,
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Callable, List, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
 from omegaconf import DictConfig
+from pytorch_lightning.utilities import grad_norm
 from torch import nn
 from torch.nn.modules.loss import _Loss
 from torchmetrics.aggregation import BaseAggregator
 
 from ..constants import AUTOMM, FEATURES, LOGITS, WEIGHT
 from ..models.utils import run_model
 from .utils import apply_layerwise_lr_decay, apply_single_lr, apply_two_stages_lr, get_lr_scheduler, get_optimizer
@@ -51,14 +52,15 @@
         output_feature_adaptor: Optional[nn.Module] = None,
         output_feature_loss_func: Optional[_Loss] = None,
         rkd_loss_func: Optional[nn.Module] = None,
         validation_metric: Optional[torchmetrics.Metric] = None,
         validation_metric_name: Optional[str] = None,
         custom_metric_func: Callable = None,
         test_metric: Optional[torchmetrics.Metric] = None,
+        track_grad_norm: Optional[Union[int, str]] = -1,
     ):
         """
         Parameters
         ----------
         student_model
             The student model in knowledge distillation.
         teacher_model
@@ -133,14 +135,17 @@
             e.g., torchmetrics.MeanMetric, whose name can't reflect the real metric name.
         custom_metric_func
             A customized metric function in case that torchmetrics doesn't have the metric.
             It is generally used together with torchmetrics' aggregators, e.g., torchmetrics.MeanMetric.
             Refer to https://github.com/PyTorchLightning/metrics/blob/master/torchmetrics/aggregation.py
         test_metric
             A torchmetrics module used in the test stage, e.g., torchmetrics.Accuracy().
+        track_grad_norm
+            Track the p-norm of gradients during training. May be set to ‘inf’ infinity-norm.
+            If using Automatic Mixed Precision (AMP), the gradients will be unscaled before logging them.
         """
         super().__init__()
         self.optim_type = optim_type
         self.save_hyperparameters(
             ignore=[
                 "student_model",
                 "teacher_model",
@@ -181,14 +186,15 @@
                 f"validation_metric {validation_metric} is an aggregation metric,"
                 "which must be used with a customized metric function."
             )
         self.custom_metric_func = custom_metric_func
 
         self.output_feature_adaptor = output_feature_adaptor
         self.rkd_loss_func = rkd_loss_func
+        self.track_grad_norm = track_grad_norm
 
     def _compute_hard_label_loss(
         self,
         output: dict,
         label: torch.Tensor,
     ):
         loss = 0
@@ -509,7 +515,12 @@
             lr_schedule=self.hparams.lr_schedule,
             end_lr=self.hparams.end_lr,
         )
 
         sched = {"scheduler": scheduler, "interval": "step"}
         logger.debug("done configuring optimizer and scheduler")
         return [optimizer], [sched]
+
+    def on_before_optimizer_step(self, optimizer):
+        # If using mixed precision, the gradients are already unscaled here
+        if self.track_grad_norm != -1:
+            self.log_dict(grad_norm(self, norm_type=self.track_grad_norm))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Callable, Dict, List, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 import torchmetrics
 from omegaconf import DictConfig
+from pytorch_lightning.utilities import grad_norm
 from torch import nn
 from torch.nn.modules.loss import _Loss
 from torchmetrics.aggregation import BaseAggregator
 
 from ..constants import AUTOMM, FEATURES, LOGIT_SCALE, PROBABILITY, QUERY, RESPONSE
 from ..models.utils import run_model
 from ..utils.matcher import compute_matching_probability
@@ -51,14 +52,15 @@
         warmup_steps: Optional[int] = None,
         loss_func: Optional[_Loss] = None,
         miner_func: Optional[_Loss] = None,
         validation_metric: Optional[torchmetrics.Metric] = None,
         validation_metric_name: Optional[str] = None,
         custom_metric_func: Callable = None,
         test_metric: Optional[torchmetrics.Metric] = None,
+        track_grad_norm: Optional[Union[int, str]] = -1,
     ):
         """
         Parameters
         ----------
         query_model
             The query model.
         response_model
@@ -113,14 +115,17 @@
             e.g., torchmetrics.MeanMetric, whose name can't reflect the real metric name.
         custom_metric_func
             A customized metric function in case that torchmetrics doesn't have the metric.
             It is generally used together with torchmetrics' aggregators, e.g., torchmetrics.MeanMetric.
             Refer to https://github.com/PyTorchLightning/metrics/blob/master/torchmetrics/aggregation.py
         test_metric
             A torchmetrics module used in the test stage, e.g., torchmetrics.Accuracy().
+        track_grad_norm
+            Track the p-norm of gradients during training. May be set to ‘inf’ infinity-norm.
+            If using Automatic Mixed Precision (AMP), the gradients will be unscaled before logging them.
         """
         super().__init__()
         self.save_hyperparameters(
             ignore=[
                 "query_model",
                 "response_model",
                 "validation_metric",
@@ -150,14 +155,15 @@
         self.reverse_prob = match_label == 0
 
         logger.debug(f"match label: {match_label}")
         logger.debug(f"reverse probability: {self.reverse_prob}")
 
         self.loss_func = loss_func
         self.miner_func = miner_func
+        self.track_grad_norm = track_grad_norm
 
     def _compute_loss(
         self,
         query_embeddings: torch.Tensor,
         response_embeddings: torch.Tensor,
         label: torch.Tensor,
         logit_scale: Optional[torch.tensor] = None,
@@ -426,7 +432,12 @@
             lr_schedule=self.hparams.lr_schedule,
             end_lr=self.hparams.end_lr,
         )
 
         sched = {"scheduler": scheduler, "interval": "step"}
         logger.debug("done configuring optimizer and scheduler")
         return [optimizer], [sched]
+
+    def on_before_optimizer_step(self, optimizer):
+        # If using mixed precision, the gradients are already unscaled here
+        if self.track_grad_norm != -1:
+            self.log_dict(grad_norm(self, norm_type=self.track_grad_norm))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import Callable, Optional, Union
 
 import pytorch_lightning as pl
 import torchmetrics
-from omegaconf import DictConfig
-from torch import nn
+from pytorch_lightning.utilities import grad_norm
 from torch.nn.modules.loss import _Loss
 from torchmetrics.aggregation import BaseAggregator
 
 from ..constants import BBOX, IMAGE, LABEL
 from .utils import (
     apply_layerwise_lr_decay,
     apply_single_lr,
@@ -43,14 +42,15 @@
         warmup_steps: Optional[int] = None,
         loss_func: Optional[_Loss] = None,
         validation_metric: Optional[torchmetrics.Metric] = None,
         validation_metric_name: Optional[str] = None,
         custom_metric_func: Callable = None,
         test_metric: Optional[torchmetrics.Metric] = None,
         efficient_finetune: Optional[str] = None,
+        track_grad_norm: Optional[Union[int, str]] = -1,
     ):
         super().__init__()  # TODO: inherit LitModule
         self.save_hyperparameters(
             ignore=[
                 "model",
                 "validation_metric",
                 "test_metric",
@@ -61,14 +61,15 @@
         self.model = model
         self.validation_metric = validation_metric
         self.validation_metric_name = f"val_{validation_metric_name}"
         self.use_loss = isinstance(validation_metric, BaseAggregator)
         self.id2label = self.model.id2label
         self.input_data_key = self.model.prefix + "_" + IMAGE
         self.input_label_key = self.model.prefix + "_" + LABEL
+        self.track_grad_norm = track_grad_norm
 
     def _base_step(self, batch, mode):
         ret = self.model(batch=batch[self.input_data_key], mode=mode)
 
         return ret
 
     def _predict_step(self, batch):
@@ -152,15 +153,15 @@
         if self.use_loss:
             losses = self._loss_step(batch=batch)
             total_loss = self.sum_and_log_step_results(losses, logging=False)
             self.validation_metric.update(total_loss)
         else:
             self.evaluate(batch, "val")
 
-    def validation_epoch_end(self, validation_step_outputs):
+    def on_validation_epoch_end(self):
         val_result = self.validation_metric.compute()
         if self.use_loss:
             self.log_dict({"val_direct_loss": val_result}, sync_dist=True)
         else:
             # TODO: add mAP/mAR_per_class
             val_result.pop("classes", None)  # introduced in torchmetrics v1.0.0
             mAPs = {"val_" + k: v for k, v in val_result.items()}
@@ -250,7 +251,12 @@
             lr_schedule=self.hparams.lr_schedule,
             end_lr=self.hparams.end_lr,
         )
 
         sched = {"scheduler": scheduler, "interval": "step"}
         logger.debug("done configuring optimizer and scheduler")
         return [optimizer], [sched]
+
+    def on_before_optimizer_step(self, optimizer):
+        # If using mixed precision, the gradients are already unscaled here
+        if self.track_grad_norm != -1:
+            self.log_dict(grad_norm(self, norm_type=self.track_grad_norm))
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 from typing import Callable, Dict, List, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
+from pytorch_lightning.strategies import DeepSpeedStrategy
+from pytorch_lightning.utilities import grad_norm
 from torch import nn
 from torch.nn.modules.loss import _Loss
 from torchmetrics.aggregation import BaseAggregator
 
 from ..constants import AUTOMM, LM_TARGET, LOGITS, T_FEW, TEMPLATE_LOGITS, WEIGHT
 from ..data.mixup import MixupModule, multimodel_mixup
 from ..models.utils import run_model
@@ -43,14 +45,15 @@
         test_metric: Optional[torchmetrics.Metric] = None,
         efficient_finetune: Optional[str] = None,
         trainable_param_names: Optional[List] = None,
         mixup_fn: Optional[MixupModule] = None,
         mixup_off_epoch: Optional[int] = 0,
         model_postprocess_fn: Callable = None,
         skip_final_val: Optional[bool] = False,
+        track_grad_norm: Optional[Union[int, str]] = -1,
     ):
         """
         Parameters
         ----------
         model
             A Pytorch model
         optim_type
@@ -105,14 +108,17 @@
             We support options such as:
 
             - bit_fit (only finetune the bias terms)
             - norm_fit (only finetune the weights in norm layers / bias layer)
             - lora, lora_bias, lora_norm (only finetunes decomposition matrices inserted into model, in combination with either bit_fit or norm_fit)
             - ia3, ia3_bias, ia3_norm (adds vector that scales activations by learned vectors, in combination with either bit_fit or norm_fit)
             - None (do not use efficient finetuning strategies)
+        track_grad_norm
+            Track the p-norm of gradients during training. May be set to ‘inf’ infinity-norm.
+            If using Automatic Mixed Precision (AMP), the gradients will be unscaled before logging them.
 
         """
         super().__init__()
         self.save_hyperparameters(
             ignore=["model", "validation_metric", "test_metric", "loss_func", "model_postprocess_fn"]
         )
         self.model = model
@@ -125,14 +131,15 @@
                 f"validation_metric {validation_metric} is an aggregation metric,"
                 "which must be used with a customized metric function."
             )
         self.custom_metric_func = custom_metric_func
         self.model_postprocess_fn = model_postprocess_fn
         self.trainable_param_names = trainable_param_names if trainable_param_names else []
         self.skip_final_val = skip_final_val
+        self.track_grad_norm = track_grad_norm
 
     def _compute_template_loss(
         self,
         per_output: Dict,
         label: torch.Tensor,
     ):
         logits = per_output[TEMPLATE_LOGITS]
@@ -235,22 +242,23 @@
         """
         output, loss = self._shared_step(batch)
         self.log("train_loss", loss)
         return loss
 
     def on_validation_start(self) -> None:
         if self.skip_final_val and self.trainer.should_stop:
-            self.trainer.val_dataloaders = []  # skip the final validation by setting val_dataloaders empty
             self.log(
                 self.validation_metric_name,
                 self.validation_metric,
                 on_step=False,
                 on_epoch=True,
             )
-        return super().on_validation_start()
+            return None
+        else:
+            return super().on_validation_start()
 
     def validation_step(self, batch, batch_idx):
         """
         Per validation step. This function is registered by pl.LightningModule.
         Refer to https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#validation
 
         Parameters
@@ -350,15 +358,15 @@
             optimizer_grouped_parameters=grouped_parameters,
             lr=self.hparams.lr,
             weight_decay=self.hparams.weight_decay,
         )
 
         logger.debug(f"trainer.max_steps: {self.trainer.max_steps}")
         if self.trainer.max_steps is None or -1:
-            if "deepspeed" in self.trainer.strategy.strategy_name:
+            if isinstance(self.trainer.strategy, DeepSpeedStrategy):
                 max_steps = 1
             else:
                 max_steps = (
                     len(self.trainer.datamodule.train_dataloader())
                     * self.trainer.max_epochs
                     // self.trainer.accumulate_grad_batches
                 )
@@ -385,7 +393,12 @@
             lr_schedule=self.hparams.lr_schedule,
             end_lr=self.hparams.end_lr,
         )
 
         sched = {"scheduler": scheduler, "interval": "step"}
         logger.debug("done configuring optimizer and scheduler")
         return [optimizer], [sched]
+
+    def on_before_optimizer_step(self, optimizer):
+        # If using mixed precision, the gradients are already unscaled here
+        if self.track_grad_norm != -1:
+            self.log_dict(grad_norm(self, norm_type=self.track_grad_norm))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         custom_metric_func: Callable = None,
         test_metric: Optional[torchmetrics.Metric] = None,
         efficient_finetune: Optional[str] = None,
         trainable_param_names: Optional[List] = None,
         mixup_fn: Optional[MixupModule] = None,
         mixup_off_epoch: Optional[int] = 0,
         model_postprocess_fn: Callable = None,
+        track_grad_norm: Optional[Union[int, str]] = -1,
     ):
         """
         Parameters
         ----------
         model
             A Pytorch model
         optim_type
@@ -104,37 +105,41 @@
             We support options such as:
 
             - bit_fit (only finetune the bias terms)
             - norm_fit (only finetune the weights in norm layers / bias layer)
             - lora, lora_bias, lora_norm (only finetunes decomposition matrices inserted into model, in combination with either bit_fit or norm_fit)
             - ia3, ia3_bias, ia3_norm (adds vector that scales activations by learned vectors, in combination with either bit_fit or norm_fit)
             - None (do not use efficient finetuning strategies)
+        track_grad_norm
+            Track the p-norm of gradients during training. May be set to ‘inf’ infinity-norm.
+            If using Automatic Mixed Precision (AMP), the gradients will be unscaled before logging them.
 
         """
         super().__init__(
-            model,
-            optim_type,
-            lr_choice,
-            lr_schedule,
-            lr,
-            lr_decay,
-            end_lr,
-            lr_mult,
-            weight_decay,
-            warmup_steps,
-            loss_func,
-            validation_metric,
-            validation_metric_name,
-            custom_metric_func,
-            test_metric,
-            efficient_finetune,
-            trainable_param_names,
-            mixup_fn,
-            mixup_off_epoch,
-            model_postprocess_fn,
+            model=model,
+            optim_type=optim_type,
+            lr_choice=lr_choice,
+            lr_schedule=lr_schedule,
+            lr=lr,
+            lr_decay=lr_decay,
+            end_lr=end_lr,
+            lr_mult=lr_mult,
+            weight_decay=weight_decay,
+            warmup_steps=warmup_steps,
+            loss_func=loss_func,
+            validation_metric=validation_metric,
+            validation_metric_name=validation_metric_name,
+            custom_metric_func=custom_metric_func,
+            test_metric=test_metric,
+            efficient_finetune=efficient_finetune,
+            trainable_param_names=trainable_param_names,
+            mixup_fn=mixup_fn,
+            mixup_off_epoch=mixup_off_epoch,
+            model_postprocess_fn=model_postprocess_fn,
+            track_grad_norm=track_grad_norm,
         )
 
     def _compute_loss(
         self,
         output: Dict,
         label: torch.Tensor,
     ):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import transformers
 import yaml
 from omegaconf import OmegaConf
 from packaging import version
+from pytorch_lightning.strategies import DeepSpeedStrategy
 from torch import nn
 
 from autogluon.common.utils.log_utils import set_logger_verbosity, verbosity2loglevel
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.core.utils import default_holdout_frac, generate_train_test_split_combined
 from autogluon.core.utils.loaders import load_pd
 from autogluon.multimodal.utils.log import get_fit_complete_message, get_fit_start_message
@@ -1296,14 +1297,15 @@
             lr_schedule=config.optimization.lr_schedule,
             lr=config.optimization.learning_rate,
             lr_decay=config.optimization.lr_decay,
             end_lr=config.optimization.end_lr,
             lr_mult=config.optimization.lr_mult,
             weight_decay=config.optimization.weight_decay,
             warmup_steps=config.optimization.warmup_steps,
+            track_grad_norm=OmegaConf.select(config, "optimization.track_grad_norm", default=-1),
         )
         metrics_kwargs = dict(
             validation_metric=validation_metric,
             validation_metric_name=validation_metric_name,
             custom_metric_func=custom_metric_func,
         )
         is_distill = teacher_model is not None
@@ -1446,34 +1448,33 @@
                         stage=3,
                         offload_optimizer=True,
                         offload_parameters=False,
                         allgather_bucket_size=config.env.deepspeed_allgather_size,
                         reduce_bucket_size=config.env.deepspeed_allreduce_size,
                     )
                 else:
-                    strategy = None
+                    strategy = "auto"
             else:
                 strategy = config.env.strategy
         else:
-            # we don't support running each trial in parallel without ray lightning
-            strategy = None
+            strategy = "auto"
             num_gpus = min(num_gpus, 1)
 
         config.env.num_gpus = num_gpus
         config.env.precision = precision
         config.env.strategy = strategy if not config.env.strategy == DEEPSPEED_OFFLOADING else DEEPSPEED_OFFLOADING
         self._config = config
         # save artifacts for the current running, except for model checkpoint, which will be saved in trainer
         self.save(save_path, standalone=standalone)
 
         blacklist_msgs = ["already configured with model summary"]
         log_filter = LogFilter(blacklist_msgs)
         with apply_log_filter(log_filter):
             trainer = pl.Trainer(
-                accelerator="gpu" if num_gpus > 0 else None,
+                accelerator="gpu" if num_gpus > 0 else "auto",
                 devices=get_available_devices(
                     num_gpus=num_gpus,
                     auto_select_gpus=config.env.auto_select_gpus,
                 ),
                 num_nodes=config.env.num_nodes,
                 precision=precision,
                 strategy=strategy,
@@ -1488,15 +1489,14 @@
                 gradient_clip_algorithm=OmegaConf.select(
                     config, "optimization.gradient_clip_algorithm", default="norm"
                 ),
                 accumulate_grad_batches=grad_steps,
                 log_every_n_steps=OmegaConf.select(config, "optimization.log_every_n_steps", default=10),
                 enable_progress_bar=enable_progress_bar,
                 fast_dev_run=config.env.fast_dev_run,
-                track_grad_norm=OmegaConf.select(config, "optimization.track_grad_norm", default=-1),
                 val_check_interval=config.optimization.val_check_interval,
                 check_val_every_n_epoch=config.optimization.check_val_every_n_epoch
                 if hasattr(config.optimization, "check_val_every_n_epoch")
                 else 1,
                 plugins=[custom_checkpoint_plugin],
             )
 
@@ -1655,15 +1655,15 @@
                 old_prefix="student_model",
                 new_prefix="model",
             )
 
         if not standalone:
             checkpoint = {"state_dict": avg_state_dict}
         else:
-            if strategy and hasattr(strategy, "strategy_name") and strategy.strategy_name == DEEPSPEED_STRATEGY:
+            if isinstance(strategy, DeepSpeedStrategy):
                 checkpoint = {
                     "state_dict": {
                         name.partition("module.")[2]: param
                         for name, param in strategy.model._zero3_consolidated_16bit_state_dict().items()
                     }
                 }
             else:
@@ -1775,15 +1775,15 @@
             blacklist_msgs.append("HPU available")
             blacklist_msgs.append("select gpus")
             blacklist_msgs.append("LOCAL_RANK")
         log_filter = LogFilter(blacklist_msgs)
 
         with apply_log_filter(log_filter):
             evaluator = pl.Trainer(
-                accelerator="gpu" if num_gpus > 0 else None,
+                accelerator="gpu" if num_gpus > 0 else "auto",
                 devices=get_available_devices(num_gpus=num_gpus, auto_select_gpus=self._config.env.auto_select_gpus),
                 num_nodes=self._config.env.num_nodes,
                 precision=precision,
                 strategy=strategy,
                 benchmark=False,
                 enable_progress_bar=self._enable_progress_bar,
                 deterministic=self._config.env.deterministic,
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import shutil
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pytorch_lightning as pl
 import torch
-from pytorch_lightning.plugins.io.checkpoint_plugin import CheckpointIO
+from pytorch_lightning.strategies import DeepSpeedStrategy
 from pytorch_lightning.utilities.rank_zero import rank_zero_warn
 
 from ..constants import AUTOMM, DEEPSPEED_STRATEGY
 from .cloud_io import _atomic_save
 from .cloud_io import _load as pl_load
 from .cloud_io import get_filesystem
 
@@ -178,15 +178,15 @@
     For ddp_spawn, the checkpoint_callback.best_k_models will be empty.
     Here, we resolve it by storing the best_models to "SAVE_DIR/best_k_models.yaml".
 
     """
 
     def _save_checkpoint(self, trainer, filepath):
         # Deepspeed saves model and optimizer states in a shared state in a separate folder
-        if trainer.strategy.strategy_name == DEEPSPEED_STRATEGY:
+        if isinstance(trainer.strategy, DeepSpeedStrategy):
             trainer.save_checkpoint(filepath + "-dir", self.save_weights_only)
         else:
             trainer.save_checkpoint(filepath, self.save_weights_only)
 
         # Required to avoid redundant evaluation and checkpointing
         self._last_global_step_saved = trainer.global_step
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     """
     if num_gpus > 0:
         if auto_select_gpus:
             devices = find_usable_cuda_devices(num_gpus)
         else:
             devices = num_gpus
     else:
-        devices = None
+        devices = "auto"
 
     return devices
 
 
 def _get_mmlab_installation_guide(package_name):
     if package_name == "mmdet":
         err_msg = 'Please install MMDetection by: pip install "mmdet>=3.0.0".'
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,15 +509,15 @@
         strategy = "ddp"
 
     if strategy == "ddp" and predictor._fit_called and predictor._problem_type == OBJECT_DETECTION:
         num_gpus = 1  # While using DDP, we can only use single gpu after fit is called
 
     if num_gpus <= 1:
         # Force set strategy to be None if it's cpu-only or we have only one GPU.
-        strategy = None
+        strategy = "auto"
 
     precision = infer_precision(num_gpus=num_gpus, precision=predictor._config.env.precision, cpu_only_warning=False)
 
     if not realtime:
         batch_size = compute_inference_batch_size(
             per_gpu_batch_size=predictor._config.env.per_gpu_batch_size,
             eval_batch_size_ratio=OmegaConf.select(predictor._config, "env.eval_batch_size_ratio"),
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.8.3b20230802/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230801
+Version: 0.8.3b20230802
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230801/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.8.3b20230802/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 Pillow<9.6,>=9.3
 tqdm<5,>=4.38
 boto3<2,>=1.10
 torch<2.1,>=1.13
+pytorch-lightning<2.1,>=2.0.0
 requests<3,>=2.21
 jsonschema<4.18,>=4.14
 seqeval<1.3.0,>=1.2.2
 evaluate<0.4.0,>=0.2.2
 accelerate<0.17,>=0.9
 timm<0.10.0,>=0.9.2
 torchvision<0.16.0,>=0.14.0
 scikit-image<0.20.0,>=0.19.1
-pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<1.1.0,>=1.0.0
 transformers[sentencepiece]<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
-autogluon.core[raytune]==0.8.3b20230801
-autogluon.features==0.8.3b20230801
-autogluon.common==0.8.3b20230801
+autogluon.core[raytune]==0.8.3b20230802
+autogluon.features==0.8.3b20230802
+autogluon.common==0.8.3b20230802
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

