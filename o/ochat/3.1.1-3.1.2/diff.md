# Comparing `tmp/ochat-3.1.1.tar.gz` & `tmp/ochat-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ochat-3.1.1.tar", last modified: Tue Aug  1 17:53:29 2023, max compression
+gzip compressed data, was "ochat-3.1.2.tar", last modified: Thu Aug  3 11:12:54 2023, max compression
```

## Comparing `ochat-3.1.1.tar` & `ochat-3.1.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 17:53:19.000000 ochat-3.1.1/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-01 17:53:19.000000 ochat-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-01 17:53:19.000000 ochat-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-01 17:53:29.585908 ochat-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-08-01 17:53:19.000000 ochat-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-01 17:53:19.000000 ochat-3.1.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   568121 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/embeddings.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68349 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/logo_new.png
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/vicuna_gpt35.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/vicuna_gpt4.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 17:53:19.000000 ochat-3.1.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 17:53:19.000000 ochat-3.1.1/docker/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 17:53:19.000000 ochat-3.1.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/config/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/clean_sharegpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/filter_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/filter_sharegpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/generate_dataset_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/merge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/run_data_pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.533907 ochat-3.1.1/ochat/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/conversation_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.557907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/
--rw-r--r--   0 runner    (1001) docker     (123)   491290 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   902939 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   384612 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1013894 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   687182 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1293180 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1341960 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   855574 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   816845 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   863272 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   770081 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   618185 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   638443 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   616281 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   413258 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   441275 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   725193 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   984109 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1870311 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   614065 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   251485 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   942794 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   852090 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   900774 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   807604 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   809832 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   669168 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.557907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/
--rw-r--r--   0 runner    (1001) docker     (123) 11708109 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/zs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.577908 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/
--rw-r--r--   0 runner    (1001) docker     (123)    92097 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   638524 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   235210 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   626756 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1003390 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   103531 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   970033 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   102321 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.581908 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/
--rw-r--r--   0 runner    (1001) docker     (123)    54425 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   227316 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    89913 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   115064 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   182364 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   113342 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    73824 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   201521 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   247838 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   155266 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    84517 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    99515 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    98794 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   161261 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    91553 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   326806 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    62891 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    92422 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   184818 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   227141 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   276090 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   184755 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    92710 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.581908 ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/
--rw-r--r--   0 runner    (1001) docker     (123)   265442 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/match_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/run_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/view_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/generate_dataset_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    62488 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/sharegpt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/test_multipack_dataloader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/text_length.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/train_alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/verify_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/verify_dataset_orca.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/models/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/models/unpadded_llama.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/serving/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/async_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/openai_api_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/openai_api_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/training_deepspeed/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/deepspeed_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/multipack_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-01 17:53:19.000000 ochat-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:53:29.585908 ochat-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.737276 ochat-3.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.681275 ochat-3.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.681275 ochat-3.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-03 11:12:46.000000 ochat-3.1.2/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-03 11:12:46.000000 ochat-3.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-03 11:12:46.000000 ochat-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-03 11:12:54.737276 ochat-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-08-03 11:12:46.000000 ochat-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-03 11:12:46.000000 ochat-3.1.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   568121 2023-08-03 11:12:46.000000 ochat-3.1.2/assets/embeddings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68349 2023-08-03 11:12:46.000000 ochat-3.1.2/assets/logo_new.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-08-03 11:12:46.000000 ochat-3.1.2/assets/vicuna_gpt35.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-03 11:12:46.000000 ochat-3.1.2/assets/vicuna_gpt4.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 11:12:46.000000 ochat-3.1.2/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 11:12:46.000000 ochat-3.1.2/docker/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-03 11:12:46.000000 ochat-3.1.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/ochat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/ochat/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/config/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/ochat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/clean_sharegpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/filter_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/filter_sharegpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/generate_dataset_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/data/run_data_pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/ochat/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/conversation_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.681275 ochat-3.1.2/ochat/evaluation/eval_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.681275 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.709275 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/
+-rw-r--r--   0 runner    (1001) docker     (123)   491290 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   902939 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   384612 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1013894 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   687182 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1293180 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1341960 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   855574 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   816845 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   863272 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   770081 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   618185 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   638443 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   616281 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   413258 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   441275 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   725193 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   984109 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1870311 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   614065 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   251485 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   942794 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   852090 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   900774 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   807604 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   809832 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   669168 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.713275 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/
+-rw-r--r--   0 runner    (1001) docker     (123) 11708109 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.681275 ochat-3.1.2/ochat/evaluation/eval_data/zs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.729276 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/
+-rw-r--r--   0 runner    (1001) docker     (123)    92097 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   638524 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   235210 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   626756 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1003390 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   103531 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   970033 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   102321 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.733276 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/
+-rw-r--r--   0 runner    (1001) docker     (123)    54425 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   227316 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    89913 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   115064 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   182364 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   113342 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    73824 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   201521 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   247838 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   155266 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    84517 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    99515 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    98794 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   161261 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    91553 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   326806 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    62891 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    92422 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   184818 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   227141 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   276090 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   184755 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    92710 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.733276 ochat-3.1.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/
+-rw-r--r--   0 runner    (1001) docker     (123)   265442 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/match_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/run_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/evaluation/view_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.737276 ochat-3.1.2/ochat/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/generate_dataset_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62488 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/sharegpt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/test_multipack_dataloader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/text_length.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/train_alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/verify_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/experimental/verify_dataset_orca.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.737276 ochat-3.1.2/ochat/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/models/unpadded_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.737276 ochat-3.1.2/ochat/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/serving/async_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/serving/openai_api_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/serving/openai_api_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.737276 ochat-3.1.2/ochat/training_deepspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/training_deepspeed/deepspeed_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/training_deepspeed/multipack_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/training_deepspeed/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-08-03 11:12:46.000000 ochat-3.1.2/ochat/training_deepspeed/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:12:54.685275 ochat-3.1.2/ochat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-03 11:12:54.000000 ochat-3.1.2/ochat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-08-03 11:12:54.000000 ochat-3.1.2/ochat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:12:54.000000 ochat-3.1.2/ochat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 11:12:54.000000 ochat-3.1.2/ochat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 11:12:54.000000 ochat-3.1.2/ochat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-03 11:12:46.000000 ochat-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:12:54.737276 ochat-3.1.2/setup.cfg
```

### Comparing `ochat-3.1.1/.gitignore` & `ochat-3.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/LICENSE` & `ochat-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/PKG-INFO` & `ochat-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochat
-Version: 3.1.1
+Version: 3.1.2
 Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat
 Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ochat-3.1.1/README.md` & `ochat-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/SECURITY.md` & `ochat-3.1.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/assets/embeddings.svg` & `ochat-3.1.2/assets/embeddings.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/assets/logo_new.png` & `ochat-3.1.2/assets/logo_new.png`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/assets/vicuna_gpt35.svg` & `ochat-3.1.2/assets/vicuna_gpt35.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/assets/vicuna_gpt4.svg` & `ochat-3.1.2/assets/vicuna_gpt4.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/docker-compose.yml` & `ochat-3.1.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/config/model_config.py` & `ochat-3.1.2/ochat/config/model_config.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/clean_sharegpt.py` & `ochat-3.1.2/ochat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/filter_language.py` & `ochat-3.1.2/ochat/data/filter_language.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/filter_sharegpt.py` & `ochat-3.1.2/ochat/data/filter_sharegpt.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/generate_dataset.py` & `ochat-3.1.2/ochat/data/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/generate_dataset_orca.py` & `ochat-3.1.2/ochat/data/generate_dataset_orca.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/merge.py` & `ochat-3.1.2/ochat/data/merge.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/data/run_data_pipeline.sh` & `ochat-3.1.2/ochat/data/run_data_pipeline.sh`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/conversation_templates.py` & `ochat-3.1.2/ochat/evaluation/conversation_templates.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl` & `ochat-3.1.2/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/match_answer.py` & `ochat-3.1.2/ochat/evaluation/match_answer.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/run_eval.py` & `ochat-3.1.2/ochat/evaluation/run_eval.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/evaluation/view_results.py` & `ochat-3.1.2/ochat/evaluation/view_results.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/generate_dataset_old.py` & `ochat-3.1.2/ochat/experimental/generate_dataset_old.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/sharegpt.ipynb` & `ochat-3.1.2/ochat/experimental/sharegpt.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/test_multipack_dataloader.ipynb` & `ochat-3.1.2/ochat/experimental/test_multipack_dataloader.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/text_length.ipynb` & `ochat-3.1.2/ochat/experimental/text_length.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/train_alpaca.py` & `ochat-3.1.2/ochat/experimental/train_alpaca.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/verify_dataset.ipynb` & `ochat-3.1.2/ochat/experimental/verify_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/experimental/verify_dataset_orca.ipynb` & `ochat-3.1.2/ochat/experimental/verify_dataset_orca.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/models/unpadded_llama.py` & `ochat-3.1.2/ochat/models/unpadded_llama.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/serving/async_tokenizer.py` & `ochat-3.1.2/ochat/serving/async_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/serving/openai_api_protocol.py` & `ochat-3.1.2/ochat/serving/openai_api_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 class ChatCompletionRequest(BaseModel):
     model: str
     messages: Union[str, List[Dict[str, str]]]
     temperature: Optional[float] = 0.7
     top_p: Optional[float] = 1.0
     n: Optional[int] = 1
     max_tokens: Optional[int] = 768
-    stop: Optional[Union[str, List[str]]] = Field(default_factory=list)
+    stop: Optional[Union[str, List[str]]] = None
     stream: Optional[bool] = False
     presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
     logit_bias: Optional[Dict[str, float]] = None
     user: Optional[str] = None
```

### Comparing `ochat-3.1.1/ochat/serving/openai_api_server.py` & `ochat-3.1.2/ochat/serving/openai_api_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     try:
         sampling_params = SamplingParams(
             n=request.n,
             presence_penalty=request.presence_penalty,
             frequency_penalty=request.frequency_penalty,
             temperature=request.temperature,
             top_p=request.top_p,
-            stop=[model.eot_token],
+            stop=request.stop,
             max_tokens=request.max_tokens
         )
     except ValueError as e:
         return create_error_response(HTTPStatus.BAD_REQUEST, str(e))
 
     result_generator = engine.generate(prompt=None,
                                        prompt_token_ids=input_ids,
```

### Comparing `ochat-3.1.1/ochat/training_deepspeed/multipack_dataloader.py` & `ochat-3.1.2/ochat/training_deepspeed/multipack_dataloader.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/training_deepspeed/parquet_dataset.py` & `ochat-3.1.2/ochat/training_deepspeed/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat/training_deepspeed/train.py` & `ochat-3.1.2/ochat/training_deepspeed/train.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/ochat.egg-info/PKG-INFO` & `ochat-3.1.2/ochat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochat
-Version: 3.1.1
+Version: 3.1.2
 Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat
 Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ochat-3.1.1/ochat.egg-info/SOURCES.txt` & `ochat-3.1.2/ochat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ochat-3.1.1/pyproject.toml` & `ochat-3.1.2/pyproject.toml`

 * *Files identical despite different names*

