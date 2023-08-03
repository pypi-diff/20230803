# Comparing `tmp/xron-1.0.2.tar.gz` & `tmp/xron-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xron-1.0.2.tar", last modified: Thu Aug  3 07:55:33 2023, max compression
+gzip compressed data, was "xron-1.0.3.tar", last modified: Thu Aug  3 08:03:37 2023, max compression
```

## Comparing `xron-1.0.2.tar` & `xron-1.0.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:55:33.772614 xron-1.0.2/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    35149 2023-08-03 07:43:33.000000 xron-1.0.2/LICENSE
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4308 2023-08-03 07:55:33.772614 xron-1.0.2/PKG-INFO
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3789 2023-08-03 07:43:33.000000 xron-1.0.2/README.md
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       38 2023-08-03 07:55:33.772614 xron-1.0.2/setup.cfg
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1902 2023-08-03 07:52:30.000000 xron-1.0.2/setup.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:55:33.768614 xron-1.0.2/xron/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      329 2023-08-03 07:43:33.000000 xron-1.0.2/xron/__init__.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      309 2023-08-03 07:43:33.000000 xron-1.0.2/xron/_version.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3766 2023-08-03 07:43:33.000000 xron-1.0.2/xron/entry.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1121 2023-08-03 07:43:33.000000 xron-1.0.2/xron/gen_conf.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5298 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nn.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:55:33.768614 xron-1.0.2/xron/nrhmm/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      292 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/__init__.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    49992 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2588 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm_eval.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17587 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm_input.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8833 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm_relabel.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    23885 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm_test.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17717 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hmm_train.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    16562 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/hybrid_data.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    11800 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/kmer2seq.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5589 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/method_illustration.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    10138 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/prepare_data.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4599 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/profile.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2159 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/relabel_test.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2541 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/split_chunks.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4468 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/tandem_repeat_resquiggle.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5149 2023-08-03 07:43:33.000000 xron-1.0.2/xron/nrhmm/transition_speed_test.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8540 2023-08-03 07:43:33.000000 xron-1.0.2/xron/test_VQVAE_speech.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:55:33.772614 xron-1.0.2/xron/utils/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      328 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/__init__.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    14351 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/align.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    10215 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/conformer.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    15478 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/easy_assembler.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1671 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/extract_seqs.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1703 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/fast5_op.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1713 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/fastIO.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1312 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/index.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2839 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/merge_datasets.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1381 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/merge_signal.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    25166 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/prepare_chunk.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17801 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/seq_op.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     9673 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/tagging.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2115 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/transfer_bonito.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6724 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/transfer_methylation.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5947 2023-08-03 07:43:33.000000 xron-1.0.2/xron/utils/vq.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8169 2023-08-03 07:43:33.000000 xron-1.0.2/xron/watch_training_progress.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3743 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_annotate.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    23598 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_eval.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      610 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_init.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5158 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_input.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8767 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_label.py
--rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    27496 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_model.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    11963 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_rcnn_train.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6710 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_test.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4730 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_train.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6895 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_train_base.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     9498 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_train_embedding.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17017 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_train_supervised.py
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    14859 2023-08-03 07:43:33.000000 xron-1.0.2/xron/xron_train_variational.py
-drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 07:55:33.768614 xron-1.0.2/xron.egg-info/
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4308 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/PKG-INFO
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1438 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/SOURCES.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        1 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/dependency_links.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       41 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/entry_points.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      333 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/requires.txt
--rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        5 2023-08-03 07:55:33.000000 xron-1.0.2/xron.egg-info/top_level.txt
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:03:37.299789 xron-1.0.3/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    35149 2023-08-03 07:43:33.000000 xron-1.0.3/LICENSE
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4308 2023-08-03 08:03:37.299789 xron-1.0.3/PKG-INFO
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3789 2023-08-03 07:43:33.000000 xron-1.0.3/README.md
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       38 2023-08-03 08:03:37.299789 xron-1.0.3/setup.cfg
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1902 2023-08-03 08:02:42.000000 xron-1.0.3/setup.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:03:37.295789 xron-1.0.3/xron/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      329 2023-08-03 07:43:33.000000 xron-1.0.3/xron/__init__.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      309 2023-08-03 08:03:09.000000 xron-1.0.3/xron/_version.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3766 2023-08-03 07:43:33.000000 xron-1.0.3/xron/entry.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1121 2023-08-03 07:43:33.000000 xron-1.0.3/xron/gen_conf.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5298 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nn.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:03:37.295789 xron-1.0.3/xron/nrhmm/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      292 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/__init__.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    49992 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2588 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm_eval.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17587 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm_input.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8833 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm_relabel.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    23885 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm_test.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17717 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hmm_train.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    16562 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/hybrid_data.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    11800 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/kmer2seq.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5589 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/method_illustration.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    10138 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/prepare_data.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4599 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/profile.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2159 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/relabel_test.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2541 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/split_chunks.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4468 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/tandem_repeat_resquiggle.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5149 2023-08-03 07:43:33.000000 xron-1.0.3/xron/nrhmm/transition_speed_test.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8540 2023-08-03 07:43:33.000000 xron-1.0.3/xron/test_VQVAE_speech.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:03:37.299789 xron-1.0.3/xron/utils/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      328 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/__init__.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    14351 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/align.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    10215 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/conformer.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    15478 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/easy_assembler.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1671 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/extract_seqs.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1703 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/fast5_op.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1713 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/fastIO.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1312 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/index.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2839 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/merge_datasets.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1381 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/merge_signal.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    25166 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/prepare_chunk.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17801 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/seq_op.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     9673 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/tagging.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     2115 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/transfer_bonito.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6724 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/transfer_methylation.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5947 2023-08-03 07:43:33.000000 xron-1.0.3/xron/utils/vq.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8169 2023-08-03 07:43:33.000000 xron-1.0.3/xron/watch_training_progress.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     3743 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_annotate.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    23598 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_eval.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      610 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_init.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     5158 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_input.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     8767 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_label.py
+-rwxrwxr-x   0 haotiant  (1001) haotiant  (1001)    27496 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_model.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    11963 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_rcnn_train.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6710 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_test.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4730 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_train.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     6895 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_train_base.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     9498 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_train_embedding.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    17017 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_train_supervised.py
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)    14859 2023-08-03 07:43:33.000000 xron-1.0.3/xron/xron_train_variational.py
+drwxrwxr-x   0 haotiant  (1001) haotiant  (1001)        0 2023-08-03 08:03:37.295789 xron-1.0.3/xron.egg-info/
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     4308 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/PKG-INFO
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)     1438 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/SOURCES.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        1 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/dependency_links.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)       41 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/entry_points.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)      333 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/requires.txt
+-rw-rw-r--   0 haotiant  (1001) haotiant  (1001)        5 2023-08-03 08:03:37.000000 xron-1.0.3/xron.egg-info/top_level.txt
```

### Comparing `xron-1.0.2/LICENSE` & `xron-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/PKG-INFO` & `xron-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xron
-Version: 1.0.2
+Version: 1.0.3
 Summary: A deep neural network basecaller for nanopore sequencing.
 Home-page: https://github.com/haotianteng/Xron
 Download-URL: https://github.com/haotianteng/Xron/archive/1.0.0.tar.gz
 Author: Haotian Teng
 Author-email: havens.teng@gmail.com
 License: GPL 3.0
 Keywords: basecaller,nanopore,sequencing,neural network,RNA methylation
```

### Comparing `xron-1.0.2/README.md` & `xron-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/setup.py` & `xron-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/entry.py` & `xron-1.0.3/xron/entry.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/gen_conf.py` & `xron-1.0.3/xron/gen_conf.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nn.py` & `xron-1.0.3/xron/nn.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm.py` & `xron-1.0.3/xron/nrhmm/hmm.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm_eval.py` & `xron-1.0.3/xron/nrhmm/hmm_eval.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm_input.py` & `xron-1.0.3/xron/nrhmm/hmm_input.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm_relabel.py` & `xron-1.0.3/xron/nrhmm/hmm_relabel.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm_test.py` & `xron-1.0.3/xron/nrhmm/hmm_test.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hmm_train.py` & `xron-1.0.3/xron/nrhmm/hmm_train.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/hybrid_data.py` & `xron-1.0.3/xron/nrhmm/hybrid_data.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/kmer2seq.py` & `xron-1.0.3/xron/nrhmm/kmer2seq.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/method_illustration.py` & `xron-1.0.3/xron/nrhmm/method_illustration.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/prepare_data.py` & `xron-1.0.3/xron/nrhmm/prepare_data.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/profile.py` & `xron-1.0.3/xron/nrhmm/profile.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/relabel_test.py` & `xron-1.0.3/xron/nrhmm/relabel_test.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/split_chunks.py` & `xron-1.0.3/xron/nrhmm/split_chunks.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/tandem_repeat_resquiggle.py` & `xron-1.0.3/xron/nrhmm/tandem_repeat_resquiggle.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/nrhmm/transition_speed_test.py` & `xron-1.0.3/xron/nrhmm/transition_speed_test.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/test_VQVAE_speech.py` & `xron-1.0.3/xron/test_VQVAE_speech.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/align.py` & `xron-1.0.3/xron/utils/align.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/conformer.py` & `xron-1.0.3/xron/utils/conformer.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/easy_assembler.py` & `xron-1.0.3/xron/utils/easy_assembler.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/extract_seqs.py` & `xron-1.0.3/xron/utils/extract_seqs.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/fast5_op.py` & `xron-1.0.3/xron/utils/fast5_op.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/fastIO.py` & `xron-1.0.3/xron/utils/fastIO.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/index.py` & `xron-1.0.3/xron/utils/index.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/merge_datasets.py` & `xron-1.0.3/xron/utils/merge_datasets.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/merge_signal.py` & `xron-1.0.3/xron/utils/merge_signal.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/prepare_chunk.py` & `xron-1.0.3/xron/utils/prepare_chunk.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/seq_op.py` & `xron-1.0.3/xron/utils/seq_op.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/tagging.py` & `xron-1.0.3/xron/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/transfer_bonito.py` & `xron-1.0.3/xron/utils/transfer_bonito.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/transfer_methylation.py` & `xron-1.0.3/xron/utils/transfer_methylation.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/utils/vq.py` & `xron-1.0.3/xron/utils/vq.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/watch_training_progress.py` & `xron-1.0.3/xron/watch_training_progress.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_annotate.py` & `xron-1.0.3/xron/xron_annotate.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_eval.py` & `xron-1.0.3/xron/xron_eval.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_init.py` & `xron-1.0.3/xron/xron_init.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_input.py` & `xron-1.0.3/xron/xron_input.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_label.py` & `xron-1.0.3/xron/xron_label.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_model.py` & `xron-1.0.3/xron/xron_model.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_rcnn_train.py` & `xron-1.0.3/xron/xron_rcnn_train.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_test.py` & `xron-1.0.3/xron/xron_test.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_train.py` & `xron-1.0.3/xron/xron_train.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_train_base.py` & `xron-1.0.3/xron/xron_train_base.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_train_embedding.py` & `xron-1.0.3/xron/xron_train_embedding.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_train_supervised.py` & `xron-1.0.3/xron/xron_train_supervised.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron/xron_train_variational.py` & `xron-1.0.3/xron/xron_train_variational.py`

 * *Files identical despite different names*

### Comparing `xron-1.0.2/xron.egg-info/PKG-INFO` & `xron-1.0.3/xron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xron
-Version: 1.0.2
+Version: 1.0.3
 Summary: A deep neural network basecaller for nanopore sequencing.
 Home-page: https://github.com/haotianteng/Xron
 Download-URL: https://github.com/haotianteng/Xron/archive/1.0.0.tar.gz
 Author: Haotian Teng
 Author-email: havens.teng@gmail.com
 License: GPL 3.0
 Keywords: basecaller,nanopore,sequencing,neural network,RNA methylation
```

### Comparing `xron-1.0.2/xron.egg-info/SOURCES.txt` & `xron-1.0.3/xron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

