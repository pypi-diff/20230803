# Comparing `tmp/pcalf-1.2.1.tar.gz` & `tmp/pcalf-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcalf-1.2.1.tar", last modified: Wed Jul 26 13:59:45 2023, max compression
+gzip compressed data, was "pcalf-1.2.2.tar", last modified: Thu Aug  3 08:53:18 2023, max compression
```

## Comparing `pcalf-1.2.1.tar` & `pcalf-1.2.2.tar`

### file list

```diff
@@ -1,140 +1,139 @@
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/
--rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-07-24 14:02:32.000000 pcalf-1.2.1/LICENSE.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       44 2023-07-24 14:02:32.000000 pcalf-1.2.1/MANIFEST.in
--rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:59:45.000000 pcalf-1.2.1/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     8049 2023-07-26 13:16:48.000000 pcalf-1.2.1/README.md
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      149 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/core/
--rw-r--r--   0 mmillet    (501) staff       (20)     8938 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/PcalfDB.py
--rw-r--r--   0 mmillet    (501) staff       (20)     2246 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/PcalfSnake.py
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/core/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)     9566 2023-07-26 13:14:00.000000 pcalf-1.2.1/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     2243 2023-07-26 12:47:00.000000 pcalf-1.2.1/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     7822 2023-07-26 09:03:50.000000 pcalf-1.2.1/pcalf/core/__pycache__/biohmm.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    15626 2023-07-26 13:19:23.000000 pcalf-1.2.1/pcalf/core/__pycache__/bioseq.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     1063 2023-07-24 14:09:02.000000 pcalf-1.2.1/pcalf/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    18499 2023-07-26 13:19:22.000000 pcalf-1.2.1/pcalf/core/__pycache__/search.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)     8930 2023-07-26 09:01:06.000000 pcalf-1.2.1/pcalf/core/biohmm.py
--rw-r--r--   0 mmillet    (501) staff       (20)    17629 2023-07-26 12:34:35.000000 pcalf-1.2.1/pcalf/core/bioseq.py
--rw-r--r--   0 mmillet    (501) staff       (20)      993 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)     5167 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/core/pcalf_db_scheme.sql
--rw-r--r--   0 mmillet    (501) staff       (20)    27381 2023-07-26 11:53:50.000000 pcalf-1.2.1/pcalf/core/search.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/datas/
--rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly1.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly1.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly2.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly2.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/Gly3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/GlyX3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/GlyX3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/datas/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      155 2023-07-24 14:09:01.000000 pcalf-1.2.1/pcalf/datas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)      495 2023-07-26 07:22:49.000000 pcalf-1.2.1/pcalf/datas/accession.txt
--rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/all.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    14739 2023-07-26 08:00:25.000000 pcalf-1.2.1/pcalf/datas/calcyanin.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/nterdb.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/datas/nterdb.ref.tsv
--rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-07-26 07:44:17.000000 pcalf-1.2.1/pcalf/datas/nterdb.tsv
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)      663 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       22 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/pcalf.egg-info/top_level.txt
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/
--rw-r--r--   0 mmillet    (501) staff       (20)  1158450 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb
--rw-r--r--   0 mmillet    (501) staff       (20)  1182597 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/Report.ipynb
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/report/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      156 2023-07-26 13:36:26.000000 pcalf-1.2.1/pcalf/report/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    17732 2023-07-26 13:36:26.000000 pcalf-1.2.1/pcalf/report/__pycache__/render.cpython-39.pyc
--rw-r--r--   0 mmillet    (501) staff       (20)    79976 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/pcalf.svg
--rw-r--r--   0 mmillet    (501) staff       (20)    25860 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/render.py
--rw-r--r--   0 mmillet    (501) staff       (20)    71713 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.css
--rw-r--r--   0 mmillet    (501) staff       (20)    19121 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.html
--rw-r--r--   0 mmillet    (501) staff       (20)    23654 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/report/template.js
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/
--rw-r--r--   0 mmillet    (501) staff       (20)    10244 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/.DS_Store
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/
--rw-r--r--   0 mmillet    (501) staff       (20)    34112 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     1715 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/Snakefile
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 13:14:00.000000 pcalf-1.2.1/pcalf/workflow/annotate/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      618 2023-07-26 12:15:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/config/config.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/biopython_1.79.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      135 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/checkm.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      230 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:41.000000 pcalf-1.2.1/pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     8241 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/checkm.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     4509 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk.smk
--rw-r--r--   0 mmillet    (501) staff       (20)    14816 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk
--rw-r--r--   0 mmillet    (501) staff       (20)      981 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/ncbi_metadatas.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     9235 2023-07-26 13:53:19.000000 pcalf-1.2.1/pcalf/workflow/annotate/rules/pcalf.smk
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     8201 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/annotate/scripts/ncbi_metadatas.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/
--rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      741 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/Snakefile
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/__pycache__/
--rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 12:47:01.000000 pcalf-1.2.1/pcalf/workflow/datasets/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      169 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/config/config.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/biopython_1.79.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:43.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/ncbi_dataset_14.14.0.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      199 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/ngd.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      141 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/prodigal-2.6.yaml
--rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/envs/seqkit.yaml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     4348 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/download.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     4721 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/fetch.smk
--rw-r--r--   0 mmillet    (501) staff       (20)     3557 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/rules/translate.smk
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/.DS_Store
--rw-r--r--   0 mmillet    (501) staff       (20)     3085 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/datas.py
--rw-r--r--   0 mmillet    (501) staff       (20)     4227 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/fallback.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1161 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py
--rw-r--r--   0 mmillet    (501) staff       (20)     4845 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/get_ncbi_reports.py
--rwxr-xr-x   0 mmillet    (501) staff       (20)     6473 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/gimme_taxa.py
--rwxr-xr-x   0 mmillet    (501) staff       (20)     1464 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1193 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/taxid_children.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1515 2023-07-24 14:02:32.000000 pcalf-1.2.1/pcalf/workflow/datasets/scripts/utils.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     3856 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:06:20.000000 pcalf-1.2.1/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        6 2023-07-26 13:59:45.000000 pcalf-1.2.1/pcalf.egg-info/top_level.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-07-24 14:02:32.000000 pcalf-1.2.1/pyproject.toml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-07-26 13:59:45.000000 pcalf-1.2.1/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)    12734 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf
--rw-r--r--   0 mmillet    (501) staff       (20)     8656 2023-07-26 12:20:10.000000 pcalf-1.2.1/scripts/pcalf-annotate-workflow
--rw-r--r--   0 mmillet    (501) staff       (20)     4197 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf-datasets-workflow
--rw-r--r--   0 mmillet    (501) staff       (20)     1330 2023-07-24 14:02:32.000000 pcalf-1.2.1/scripts/pcalf-report
--rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-07-26 13:59:45.000000 pcalf-1.2.1/setup.cfg
--rw-r--r--   0 mmillet    (501) staff       (20)     1205 2023-07-26 13:59:22.000000 pcalf-1.2.1/setup.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/
+-rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-07-24 14:02:32.000000 pcalf-1.2.2/LICENSE.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       44 2023-07-24 14:02:32.000000 pcalf-1.2.2/MANIFEST.in
+-rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-08-03 08:53:18.000000 pcalf-1.2.2/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     8049 2023-07-26 13:16:48.000000 pcalf-1.2.2/README.md
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      149 2023-07-24 14:09:01.000000 pcalf-1.2.2/pcalf/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/core/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8938 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/core/PcalfDB.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     2246 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/core/PcalfSnake.py
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/core/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/core/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)     9566 2023-07-26 13:14:00.000000 pcalf-1.2.2/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     2243 2023-07-26 12:47:00.000000 pcalf-1.2.2/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:09:01.000000 pcalf-1.2.2/pcalf/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     7822 2023-07-26 09:03:50.000000 pcalf-1.2.2/pcalf/core/__pycache__/biohmm.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    15626 2023-07-26 13:19:23.000000 pcalf-1.2.2/pcalf/core/__pycache__/bioseq.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     1063 2023-07-24 14:09:02.000000 pcalf-1.2.2/pcalf/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    18499 2023-07-26 13:19:22.000000 pcalf-1.2.2/pcalf/core/__pycache__/search.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)     8930 2023-07-26 09:01:06.000000 pcalf-1.2.2/pcalf/core/biohmm.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    17629 2023-07-26 12:34:35.000000 pcalf-1.2.2/pcalf/core/bioseq.py
+-rw-r--r--   0 mmillet    (501) staff       (20)      993 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/core/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     5167 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/core/pcalf_db_scheme.sql
+-rw-r--r--   0 mmillet    (501) staff       (20)    31420 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/core/search.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/datas/
+-rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly1.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly1.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly2.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly2.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/Gly3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/GlyX3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/GlyX3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/datas/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      155 2023-07-24 14:09:01.000000 pcalf-1.2.2/pcalf/datas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)      495 2023-07-26 07:22:49.000000 pcalf-1.2.2/pcalf/datas/accession.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/all.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    14739 2023-07-26 08:00:25.000000 pcalf-1.2.2/pcalf/datas/calcyanin.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/nterdb.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/datas/nterdb.ref.tsv
+-rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-07-26 07:44:17.000000 pcalf-1.2.2/pcalf/datas/nterdb.tsv
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8021 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)      663 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       22 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/pcalf.egg-info/top_level.txt
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/report/
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/report/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)  1158450 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)  1182597 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/Report.ipynb
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/report/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      156 2023-07-26 13:36:26.000000 pcalf-1.2.2/pcalf/report/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    17732 2023-07-26 13:36:26.000000 pcalf-1.2.2/pcalf/report/__pycache__/render.cpython-39.pyc
+-rw-r--r--   0 mmillet    (501) staff       (20)    79976 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/pcalf.svg
+-rw-r--r--   0 mmillet    (501) staff       (20)    25860 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/render.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    71713 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/template.css
+-rw-r--r--   0 mmillet    (501) staff       (20)    19121 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/template.html
+-rw-r--r--   0 mmillet    (501) staff       (20)    23654 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/report/template.js
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/
+-rw-r--r--   0 mmillet    (501) staff       (20)    10244 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/.DS_Store
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/.ipynb_checkpoints/
+-rw-r--r--   0 mmillet    (501) staff       (20)    34112 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     1447 2023-08-01 10:55:41.000000 pcalf-1.2.2/pcalf/workflow/annotate/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 13:14:00.000000 pcalf-1.2.2/pcalf/workflow/annotate/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      593 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/workflow/annotate/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      135 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/checkm.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      230 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:41.000000 pcalf-1.2.2/pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     7159 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/checkm.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     3510 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/gtdbtk.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     1088 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/ncbi_metadatas.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     9107 2023-08-03 08:51:16.000000 pcalf-1.2.2/pcalf/workflow/annotate/rules/pcalf.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/annotate/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/scripts/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     8201 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/annotate/scripts/ncbi_metadatas.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8196 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      741 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/Snakefile
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/__pycache__/
+-rw-r--r--   0 mmillet    (501) staff       (20)      167 2023-07-26 12:47:01.000000 pcalf-1.2.2/pcalf/workflow/datasets/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/config/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/config/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      169 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/config/config.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)      129 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/biopython_1.79.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      232 2023-07-26 13:16:43.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/ncbi_dataset_14.14.0.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      199 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/ngd.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      141 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/prodigal-2.6.yaml
+-rw-r--r--   0 mmillet    (501) staff       (20)      154 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/envs/seqkit.yaml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/rules/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/rules/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     4348 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/rules/download.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     4720 2023-07-28 06:08:19.000000 pcalf-1.2.2/pcalf/workflow/datasets/rules/fetch.smk
+-rw-r--r--   0 mmillet    (501) staff       (20)     3557 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/rules/translate.smk
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     6148 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/.DS_Store
+-rw-r--r--   0 mmillet    (501) staff       (20)     3085 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/datas.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4227 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/fallback.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1161 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     4845 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/get_ncbi_reports.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     6473 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/gimme_taxa.py
+-rwxr-xr-x   0 mmillet    (501) staff       (20)     1464 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1193 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/taxid_children.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1515 2023-07-24 14:02:32.000000 pcalf-1.2.2/pcalf/workflow/datasets/scripts/utils.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     8515 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     3806 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-07-24 14:06:20.000000 pcalf-1.2.2/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)      133 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        6 2023-08-03 08:53:17.000000 pcalf-1.2.2/pcalf.egg-info/top_level.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-07-24 14:02:32.000000 pcalf-1.2.2/pyproject.toml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-08-03 08:53:18.000000 pcalf-1.2.2/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)     9671 2023-08-03 08:51:16.000000 pcalf-1.2.2/scripts/pcalf
+-rw-r--r--   0 mmillet    (501) staff       (20)     9937 2023-08-03 08:51:16.000000 pcalf-1.2.2/scripts/pcalf-annotate-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     4197 2023-07-24 14:02:32.000000 pcalf-1.2.2/scripts/pcalf-datasets-workflow
+-rw-r--r--   0 mmillet    (501) staff       (20)     1330 2023-07-24 14:02:32.000000 pcalf-1.2.2/scripts/pcalf-report
+-rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-08-03 08:53:18.000000 pcalf-1.2.2/setup.cfg
+-rw-r--r--   0 mmillet    (501) staff       (20)     1206 2023-08-03 08:52:30.000000 pcalf-1.2.2/setup.py
```

### Comparing `pcalf-1.2.1/LICENSE.txt` & `pcalf-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/PKG-INFO` & `pcalf-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 1.2.1
+Version: 1.2.2
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcalf-1.2.1/README.md` & `pcalf-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/.DS_Store` & `pcalf-1.2.2/pcalf/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/PcalfDB.py` & `pcalf-1.2.2/pcalf/core/PcalfDB.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/PcalfSnake.py` & `pcalf-1.2.2/pcalf/core/PcalfSnake.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/PcalfDB.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/PcalfSnake.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/biohmm.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/biohmm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/bioseq.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/bioseq.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/log.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/log.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/__pycache__/search.cpython-39.pyc` & `pcalf-1.2.2/pcalf/core/__pycache__/search.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/biohmm.py` & `pcalf-1.2.2/pcalf/core/biohmm.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/bioseq.py` & `pcalf-1.2.2/pcalf/core/bioseq.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/log.py` & `pcalf-1.2.2/pcalf/core/log.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/pcalf_db_scheme.sql` & `pcalf-1.2.2/pcalf/core/pcalf_db_scheme.sql`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/core/search.py` & `pcalf-1.2.2/pcalf/core/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import os
 import logging
 import tempfile
 import concurrent
 import concurrent.futures
 import multiprocessing
-
+import yaml
 import pandas as pd
 from shutil import which
 
 import pyhmmer
 import tqdm
 
 from Bio.SeqFeature import SeqFeature, FeatureLocation
@@ -469,14 +469,89 @@
         features_table,['GlyX3_HMM_Profile'])
     glyzip_evalue_threshold, glyzip_coverage_threshold = get_coverage_and_evalue_threshold(
         features_table,['Gly1_HMM_Profile','Gly2_HMM_Profile','Gly3_HMM_Profile'])
 
     return (glyx3_evalue_threshold, glyx3_coverage_threshold, glyzip_evalue_threshold, glyzip_coverage_threshold)
 
 
+def dump_iteration(
+        res_dir,
+        sequences,
+        glyx3,
+        gly1,
+        gly2,
+        gly3,
+        nter
+        ):    
+    logging.info("Dumping HMMs.") 
+    hmmdir = os.path.join(res_dir,"HMM")
+    os.makedirs(hmmdir,exist_ok=True)
+    glyx3.hmm.write(open(hmmdir + "/Glyx3.hmm","wb"))
+    gly1.hmm.write(open(hmmdir + "/Gly1.hmm","wb"))
+    gly2.hmm.write(open(hmmdir + "/Gly2.hmm","wb"))
+    gly3.hmm.write(open(hmmdir + "/Gly3.hmm","wb"))
+
+    logging.info("Dumping MSAs.")
+    msadir = os.path.join(res_dir,"MSA")    
+    os.makedirs(msadir,exist_ok=True)
+    glyx3.msa.write(open(msadir+"/Glyx3.msa.fa","wb"),format="afa")
+    gly1.msa.write(open(msadir+"/Gly1.msa.fa","wb"),format="afa")
+    gly2.msa.write(open(msadir+"/Gly2.msa.fa","wb"),format="afa")
+    gly3.msa.write(open(msadir+"/Gly3.msa.fa","wb"),format="afa")
+    
+    logging.info("Dumping N-ter table.")
+    with open(res_dir+"/N-ter-DB.tsv","w") as nterout:
+        for nterid, n in nter.items():
+            nterout.write("{}\t{}\t{}\n".format(n[0],nterid,n[1]))
+
+    logging.info("Writing feature table.")
+    features = sequences.to_feature_table()
+    features.to_csv(res_dir + "/pcalf.features.tsv",sep="\t",header=True,index=True)
+    logging.info("Writing hits table")
+    hits = sequences.to_hits_table()
+    hits.to_csv(res_dir + "/pcalf.hits.tsv",sep="\t",header=True,index=True)
+
+    logging.info("Making summary.")
+    summary_datas = []
+    for idx, seq_features_df in features.groupby(["sequence_id","sequence_src"]):
+        sequence = idx[0]
+        sequence_src = idx[1]
+        cterom = ",".join(
+                        list(
+                            seq_features_df[seq_features_df.feature_id.isin(["Gly1","Gly2","Gly3"]) ].sort_values("feature_start").feature_id
+                            )
+                )
+
+        nter_type = None
+        nter_neighbor = None 
+        if not seq_features_df[seq_features_df.feature_id == "N-ter" ].empty:
+            nter_type,nter_neighbor = "".join(set(
+                seq_features_df[seq_features_df.feature_id == "N-ter" ].feature_src
+            )).split("||")
+
+        summary_datas.append(
+            {
+                "sequence_accession":sequence,
+                "sequence_src": sequence_src,
+                "flag":decision_tree(nter_type,cterom),
+                "nter":nter_type,
+                "nter_neighbor": nter_neighbor,
+                "cter":cterom,
+                "sequence":str(sequences.get_seq_by_id(sequence).seq),
+                # "iteration":seq_per_iteration[sequence]
+            }
+        )
+    if summary_datas:
+        df = pd.DataFrame(summary_datas).set_index("sequence_accession")
+    else:
+        df = pd.DataFrame(columns=["sequence_accession","sequence_src","flag","nter","nter_neighbor","cter","sequence"]).set_index("sequence_accession")
+    df.to_csv(res_dir + "/pcalf.summary.tsv",sep="\t",index=True,header=True)
+
+
+
 def pcalf(        
         fastas:list, 
         srcs:list,
         glyx3:Hmm, 
         gly1:Hmm, 
         gly2:Hmm, 
         gly3:Hmm,
@@ -547,14 +622,19 @@
         glyx3_evalue_threshold, auto_glyx3_e_value,
         glyx3_coverage_threshold, auto_glyx3_cov,
         glyzip_evalue_threshold,  auto_glyzip_e_value,
         glyzip_coverage_threshold, auto_glyzip_cov,
         nter_evalue_threshold, nter_coverage_threshold
     ))
 
+    thresholds = {
+        "glyx3":{"coverage":glyx3_coverage_threshold,"e-value":glyx3_evalue_threshold},
+        "glyzips":{"coverage":glyzip_coverage_threshold,"e-value":glyzip_evalue_threshold}
+        }
+
     for profile in [glyx3,gly1,gly2,gly3]:
         logging.info('{}:  Number of sequences = {}.'.format(
             profile.hmm.name.decode(),profile.hmm.nseq))
     
     logging.info("Dump Nter DB as fasta.")
     logging.debug("Number of sequences in the N-ter database at start : {}".format(len(nterdb)))
     nterfa = tempfile.NamedTemporaryFile(mode="w+")
@@ -582,39 +662,37 @@
         glyx3_evalue_threshold,  
         glyx3_coverage_threshold,  
         glyzip_evalue_threshold,
         glyzip_coverage_threshold,
         nter_coverage_threshold, 
         nter_evalue_threshold) 
     
-
-   
     new_calc = 0
     new_seq = 0
     valid_calcyanin = Sequences() 
     if sequences.sequences:            
         for seq in sequences.sequences:        
             if seq.get_feature("GlyX3" ):
                 new_seq += 1           
                 nter = ",".join([f.features[0].qualifiers["src"].split("|")[0] for f in  seq.get_feature("N-ter")])
                 cter = ",".join([f.features[0].id for f in seq.get_feature("Gly1" )+
                                     seq.get_feature("Gly2" )+
                                     seq.get_feature("Gly3" )])
                 flag = decision_tree(nter,cter)
+                seq.flag = flag
                 if flag == "Calcyanin with known N-ter" or flag == "Calcyanin with new N-ter":
                     new_calc += 1 
                     valid_calcyanin.sequences.append(seq)
             
 
         logging.info("New sequences with a match against GlyX3 [+{}]".format(new_seq))                    
-        logging.info("New calcyanin [+{}] ! :)".format(new_calc))                            
-        
-        logging.info("Updating HMM profiles and N-ter DB.")
-        
+        logging.info("New calcyanin [+{}] ! :)".format(new_calc))                                    
+        logging.info("Updating HMM profiles and N-ter DB.")        
         glyx3features = valid_calcyanin.get_feature("GlyX3")
+        
         if glyx3features:  
             logging.info("Updating GlyX3")
             glyx3 = update_hmm(glyx3features,glyx3,is_update_iterative)
 
             
         gly1features = valid_calcyanin.get_feature("Gly1")        
         if gly1features:    
@@ -645,42 +723,65 @@
                     )
                 else:
                     logging.debug("Already in DB ... {} has 100% identity with {} which is already in the N-ter DB.".format(                            
                         nf.id,
                         src,
                     ))                     
             logging.info("Number of sequences in the N-ter database after update : {}".format(len(nterdb)))                    
-    return sequences, glyx3 , gly1, gly2, gly3 , nterdb 
+    return sequences, glyx3, gly1, gly2, gly3, nterdb , thresholds
           
 
 
-def iterative_pcalf(*args,**kwargs):
+def run_pcalf(*args,**kwargs):
     ite = 0
+    thresholds_by_ite = {} 
     max_ite = kwargs.get('max_iteration')
+    res_dir = kwargs.get('res_dir')
     logging.info('Iterative search enable [max-iteration: {}]'.format(max_ite))
     keep_going = True
     fastas,names,glyx3,gly1,gly2,gly3,nterdb = args
     glyx3_initial_size = glyx3.hmm.nseq
-    while keep_going:
+    
+    while keep_going:        
         keep_going = False
         # do 
-        new_sequences, glyx3 , gly1, gly2, gly3 , nterdb  = pcalf(
+        ite_seqs, glyx3 , gly1, gly2, gly3 , nterdb , thresholds  = pcalf(
             fastas,names,glyx3,gly1,gly2,gly3,nterdb,**kwargs)
+        thresholds_by_ite["iteration_{}".format(ite)] = thresholds
         if glyx3.hmm.nseq > glyx3_initial_size:
             keep_going = True
             glyx3_initial_size = glyx3.hmm.nseq
+            dump_iteration(os.path.join(res_dir,'iterations','iteration_{}'.format(ite)),                
+                ite_seqs,
+                glyx3,
+                gly1,
+                gly2,
+                gly3,
+                nterdb
+            )
 
-    ite+=1
-    logging.info('{}/{} iterations done.'.format(ite,max_ite))
-    if ite==max_ite:
-        keep_going = False
+        ite+=1
+        logging.info('{}/{} iterations done.'.format(ite,max_ite))
+        if ite==max_ite:
+            keep_going = False
     logging.info('Converged (i.e , no new sequence detected) in {} iterations [max-iteration: {}]'.format(ite,max_ite))
-    return new_sequences, glyx3 , gly1, gly2, gly3 , nterdb
-
-
+    dump_iteration(
+        res_dir, 
+        ite_seqs,
+        glyx3,
+        gly1,
+        gly2,
+        gly3,
+        nterdb
+    )
+    logging.info('Last iteration results saved under {}'.format(res_dir))
+    thresholds_file_path = os.path.join(res_dir,'thresholds.yaml')
+    yaml.dump(thresholds_by_ite,open(thresholds_file_path ,'w') )
+    logging.info('Thresholds used for each iteration stored at : {}'.format(thresholds_file_path))
+    return ite_seqs, glyx3 , gly1, gly2, gly3 , nterdb
 
 def decision_tree(nter , cter):
     """give a flag to a calcyanin based on its C-ter modular organization and its N-ter."""
     if re.search("Gly1,Gly2,Gly3",cter):
         if nter in ["CoBaHMA-type","Y-type","X-type","Z-type"]:
             flag = "Calcyanin with known N-ter"
         else:
```

### Comparing `pcalf-1.2.1/pcalf/datas/Gly1.hmm` & `pcalf-1.2.2/pcalf/datas/Gly1.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/Gly1.msa.fa` & `pcalf-1.2.2/pcalf/datas/Gly1.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/Gly2.hmm` & `pcalf-1.2.2/pcalf/datas/Gly2.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/Gly2.msa.fa` & `pcalf-1.2.2/pcalf/datas/Gly2.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/Gly3.hmm` & `pcalf-1.2.2/pcalf/datas/Gly3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/Gly3.msa.fa` & `pcalf-1.2.2/pcalf/datas/Gly3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/GlyX3.hmm` & `pcalf-1.2.2/pcalf/datas/GlyX3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/GlyX3.msa.fa` & `pcalf-1.2.2/pcalf/datas/GlyX3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/all.hmm` & `pcalf-1.2.2/pcalf/datas/all.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/calcyanin.fasta` & `pcalf-1.2.2/pcalf/datas/calcyanin.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/nterdb.fasta` & `pcalf-1.2.2/pcalf/datas/nterdb.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/nterdb.ref.tsv` & `pcalf-1.2.2/pcalf/datas/nterdb.ref.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/datas/nterdb.tsv` & `pcalf-1.2.2/pcalf/datas/nterdb.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/pcalf.egg-info/PKG-INFO` & `pcalf-1.2.2/pcalf/pcalf.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/pcalf.egg-info/SOURCES.txt` & `pcalf-1.2.2/pcalf/pcalf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb` & `pcalf-1.2.2/pcalf/report/.ipynb_checkpoints/Report-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/Report.ipynb` & `pcalf-1.2.2/pcalf/report/Report.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/__pycache__/render.cpython-39.pyc` & `pcalf-1.2.2/pcalf/report/__pycache__/render.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/pcalf.svg` & `pcalf-1.2.2/pcalf/report/pcalf.svg`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/render.py` & `pcalf-1.2.2/pcalf/report/render.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/template.css` & `pcalf-1.2.2/pcalf/report/template.css`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/template.html` & `pcalf-1.2.2/pcalf/report/template.html`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/report/template.js` & `pcalf-1.2.2/pcalf/report/template.js`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb` & `pcalf-1.2.2/pcalf/workflow/.ipynb_checkpoints/Report-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/annotate/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/Snakefile` & `pcalf-1.2.2/pcalf/workflow/annotate/Snakefile`

 * *Files 14% similar despite different names*

```diff
@@ -35,19 +35,14 @@
         os.path.join(RESDIR , "ncbi-datas" , "ncbi_metadatas.tsv"),        
     ]
     
     # optional files depending on the value of QUICK
     if not QUICK:
         files.append(os.path.join(RESDIR,"checkm-res","checkm.done"))
         files.append(os.path.join(RESDIR,"gtdbtk-res","gtdbtk.done"))
-    #else:
-    #    files.append(os.path.join(RESDIR,"checkm-res","checkm.quick.done"))
-    #    files.append(os.path.join(RESDIR,"gtdbtk-res","gtdbtk.quick.done"))
-        #files.append(os.path.join(RESDIR , "gtdbtk-res","gtdbtk.ar53.bac120.summary.clean.tsv"))
-    
     return files
 
 include: "rules/pcalf.smk"
 include: "rules/checkm.smk"
 include: "rules/gtdbtk.smk"
 include: "rules/ncbi_metadatas.smk"
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/config/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/annotate/config/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/config/config.yaml` & `pcalf-1.2.2/pcalf/workflow/annotate/config/config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,12 +26,11 @@
   gly2_msa: null
   gly3_msa: null
   nterdb: null
   glyx3-evalue: null
   glyx3-coverage: null
   glyzip-evalue: null
   glyzip-coverage: null
-  iterative-search: True
   iterative-update: True
   max-iteration: 3
   Z: 10000 
   domZ: 10000
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/envs/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/annotate/envs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/rules/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/annotate/rules/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/rules/checkm.smk` & `pcalf-1.2.2/pcalf/workflow/annotate/rules/checkm.smk`

 * *Files 12% similar despite different names*

```diff
@@ -44,64 +44,26 @@
  'Contamination',
  'Strain heterogeneity']
 
 TAXCOLS = ['Bin Id',
  '# unique markers (of 43)',
   '# multi-copy',
    'Taxonomy']
-
-
-
-# rule cm_empty_checkm_tables:
-#     output:
-#         taxo   = temp(os.path.join(RESDIR , "checkm-res","tables","checkM_taxonomy.tsv")),
-#         stats  = temp(os.path.join(RESDIR , "checkm-res","tables","checkM_statistics.tsv")),
-#         fstats = temp(os.path.join(RESDIR , "checkm-res","tables","checkM_statistics_full.tsv")),
-#     params:
-#         genomes = INPUT
-#     run:
-#         import pandas as pd
-#         tdf = pd.DataFrame(
-#             columns = TAXCOLS[1:],
-#             index = list(params.genomes.keys())
-#             )
-#         tdf.index.name = TAXCOLS[0]
-#         tdf.to_csv(str(output.taxo),sep="\t",header=True)
-
-#         sdf = pd.DataFrame(
-#             columns = STATSCOLS[1:],
-#             index = list(params.genomes.keys())
-#             )
-#         sdf.index.name = STATSCOLS[0]
-#         sdf.to_csv(str(output.stats),sep="\t",header=True)
-
-#         fsdf = pd.DataFrame(
-#             columns = FULLSTATSCOLS[1:],
-#             index = list(params.genomes.keys())
-#             )
-#         fsdf.index.name = FULLSTATSCOLS[0]
-#         fsdf.to_csv(str(output.fstats),sep="\t",header=True)
-
-
-# rule cm_target_quick_checkm:
-#     output:
-#         touch(temp(os.path.join(RESDIR,"checkm-res","checkm.quick.done")))
-#     input:
-#         rules.cm_empty_checkm_tables.output
     
         
 rule cm_target_checkm:
     output:
         temp(os.path.join(RESDIR,"checkm-res","checkm.done")),
     input:
         expand(os.path.join(RESDIR , "checkm-res","tables","checkM_{table}.tsv"),table=["taxonomy","statistics_full","statistics"]),
     params:
         tmp = os.path.join(RESDIR , "checkm-res", "tmp"),
     shell:
-        'rm -r {params.tmp} && touch {output}'
+        'touch {output}'
+        #'rm -r {params.tmp} && 
 
 def aggregate_batches_checkm(wildcards):    
     return expand(
         os.path.join(RESDIR , "checkm-res", "tmp","{batch}",checkm_res,"checkM_{{table}}.tsv"),
         batch=GENOMESBATCH.keys()
     )
 
@@ -168,72 +130,81 @@
         "-f {output.tsv} "                  # output filename
         "-t {threads} "
         "{params.markerfile} "              # <marker file>
         "{params.checkm_dir} "              # <output folder>
         "&>> {log} "
 
 
-def get_bins(wildcards):
-    return expand(
-        os.path.join(RESDIR , "checkm-res", "tmp", 'bins', '{batch}', '{bin}.fna'),
-        batch=wildcards.batch , bin = list(GENOMESBATCH[wildcards.batch].keys()) 
-    )
-    
+def get_extension_from_file(wildcards,input):
+    with open(str(input)) as f:
+        return "."+os.path.basename(f.read().strip()).split('.')[-1]
+
 rule cm_CHECKM_lineage_wf:
     """ Main checkM rule.
         Compute CheckM on a given batch of bins.
     """
     output:
         tsv = os.path.join(RESDIR , "checkm-res", "tmp", "{batch}","lineage_wf","checkM_statistics.tsv"),
-    input:
-        # Function that returns the locations of genomes associated with {batch}        
-        get_bins,
+    input:             
+        os.path.join(RESDIR , "checkm-res", "tmp", 'bins', '{batch}', 'batch.tsv'),
     conda: 
         os.path.join(".." , "envs" , "checkm.yaml")
     resources:
         mem= 16000 if config["config-genomes"]["low_memory"] else 50000,
         mem_mb= 20000 if config["config-genomes"]["low_memory"] else 70000,
         # time= 24:00:00, # time limit for each job
         nodes= 1,
         cpus_per_task = 10 if config["config-genomes"]["low_memory"] else  15 ,           
     threads: 
         10
     params:            
         checkm_dir = lambda wildcards, output: os.path.dirname(output.tsv),
         checkm_data = config["config-genomes"]["CheckM_data"],
-        batch_dir = lambda wildcards, input: os.path.dirname(input[0]),
         low_memory = "--reduced_tree" if config["config-genomes"]["low_memory"] else "",
-        #tmp = "--tmpdir %s" % RESDIR , "checkm-res", "tmp" if RESDIR , "checkm-res", "tmp" else "",
+        tmp = os.path.join(RESDIR , "checkm-res", "tmp", '{batch}', 'tmp' ),
+        ext = lambda wildcards,input: get_extension_from_file(wildcards,input),
     log:
         os.path.join(RESDIR , "checkm-res", 'logs', "{batch}", checkm_res , "lineage_wf.log")
     benchmark:
         os.path.join(RESDIR , "checkm-res" , "benchmarks","lineage","{batch}.txt") 
     shell:
+        #"mkdir -p {params.tmp}; "
         "echo {params.checkm_data}; " #export LC_ALL=C ; 
         "checkm data setRoot {params.checkm_data} &>> {log}; "
         "checkm lineage_wf "
         "--tab_table "          # output as a tab-separated file
         "-f {output.tsv} "      # filename for the output
         "-t {threads} "
-        "{params.low_memory} "
-        "-x fna "               # extension of the bin files
-        "{params.batch_dir}/ "  # (input) directory containing the bin files
+        "{params.low_memory} "        
+        "-x {params.ext} "               # extension of the bin files
+        "{input} "  
         "{params.checkm_dir} "  # (output) directory where to store the results
-        "&>> {log} "
+        "&>> {log}; "
+        
+
+
+# rule cm_bins_into_batches:
+#     """ Gunzip a `fasta.gz` into the appropriate batch directory. """
+#     output:
+#         temp(os.path.join(RESDIR , "checkm-res", "tmp", 'bins', '{batch}', '{bin}.fna'))
+#     input:
+#         lambda wildcards: GENOMESBATCH[wildcards.batch][wildcards.bin],
+#     params:
+#         cmd = lambda wildcards,input: "gunzip -c " if str(input).endswith('.gz') else "cat ",
+#     threads: 
+#         1 
+#     shell:
+#         "{params.cmd} {input} > {output}"
 
-def get_genome_file_for_checkm(wildcards):
-    return glob.glob(
-        os.path.join(RESDIR,"datas","assemblies", "ncbi_dataset", wildcards.bin, "GC*_genomic.fna.gz" )
-        )[0]
 
 rule cm_bins_into_batches:
-    """ Gunzip a `fasta.gz` into the appropriate batch directory. """
     output:
-        temp(os.path.join(RESDIR , "checkm-res", "tmp", 'bins', '{batch}', '{bin}.fna'))
-    input:
-        lambda wildcards: GENOMESBATCH[wildcards.batch][wildcards.bin],
+        os.path.join(RESDIR , "checkm-res", "tmp", 'bins', '{batch}', 'batch.tsv')
     params:
-        cmd = lambda wildcards,input: "gunzip -c " if str(input).endswith('.gz') else "cat ",
-    threads: 
-        1 
-    shell:
-        "{params.cmd} {input} > {output}"
+        batch = GENOMESBATCH[wildcards.batch],
+    run:
+        batch_genomes = params.batch[str(wildcards.batch)]      
+        with open(str(output),'w') as fh:
+            for label,genome_path in batch_genomes.items():                
+                fh.write('{}\t{}\n'.format(
+                    label,genome_path
+                ))
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/rules/gtdbtk.smk` & `pcalf-1.2.2/pcalf/workflow/annotate/rules/gtdbtk.smk`

 * *Files 24% similar despite different names*

```diff
@@ -17,115 +17,95 @@
  'msa_percent',
  'translation_table',
  'red_value',
  'warnings']
 
 
 
-# rule gm_empty_gtdbtk_summary:
-#     output:
-#         temp(os.path.join(RESDIR , "gtdbtk-res","gtdbtk.ar53.bac120.summary.clean.tsv")),
-#     params:
-#         genomes = INPUT
-#     run:
-#         import pandas as pd
-#         df = pd.DataFrame(
-#             columns = GTDBSUMMARYCOLS[1:],
-#             index = list(params.genomes.keys())            
-#             )
-#         df.index.name = GTDBSUMMARYCOLS[0]        
-#         df.to_csv(str(output),sep="\t",header=True)
-                
-# rule gm_target_quick_gtdbtk:
-#     output:
-#         touch(temp(os.path.join(RESDIR,"gtdbtk-res","gtdbtk.quick.done")))
-#     input:
-#         rules.gm_empty_gtdbtk_summary.output
-
 rule gm_target_gtdbtk:
     output:
         touch(temp(os.path.join(RESDIR,"gtdbtk-res","gtdbtk.done")))
     input:
         os.path.join(RESDIR, "gtdbtk-res","gtdbtk.ar53.bac120.summary.clean.tsv"),
     
 rule gm_GTDBTK_clean_table:
     output:
         os.path.join(RESDIR , "gtdbtk-res","gtdbtk.ar53.bac120.summary.clean.tsv")
     input:
-        os.path.join(RESDIR , "gtdbtk-res","gtdbtk.ar53.bac120.summary.tsv")
-    run:
+        expand(
+            os.path.join(RESDIR , "gtdbtk-res", "{batch}", "gtdbtk.ar53.bac120.summary.tsv")
+            ,batch = GENOMESBATCH.keys())
+    run:        
         import os
         import pandas as pd
-        print(os.stat(str(input)).st_size)
-        print(str(input))
-        df = pd.read_csv(str(input),sep="\t",header=0,index_col=None)   
-        print(df)
-        if os.stat(str(input)).st_size != 0:
-            df = pd.read_csv(str(input),sep="\t",header=0,index_col=None)   
-            print(df)     
-            df.user_genome = df.user_genome.str.replace("USER_","")
-            print(df)
-            df.to_csv(str(output),sep="\t",header=True,index=False)
-        else:
-            open(str(output),'w').close()
+        dfs = []
+        for f in input:
+            if os.stat(str(f)).st_size != 0:
+                t = pd.read_csv(str(f),sep='\t',header=0)
+                dfs.append(t)    
+        df = pd.DataFrame()
+        if dfs:
+            df = pd.concat(dfs,axis=0)            
+        df.to_csv(str(output),index=False,header=True,sep='\t')
 
 
 rule gm_concatenate_archaea_and_bacteria_results:
     output:
-        os.path.join(RESDIR, "gtdbtk-res", "gtdbtk.ar53.bac120.summary.tsv")                                            
+        os.path.join(RESDIR, "gtdbtk-res", "{batch}", "gtdbtk.ar53.bac120.summary.tsv")                                            
     input:
-        bac = os.path.join(RESDIR, "gtdbtk-res", "gtdbtk.bac120.summary.tsv"),
-        ar  = os.path.join(RESDIR, "gtdbtk-res", "gtdbtk.ar53.summary.tsv"  ),                         
+        bac = os.path.join(RESDIR, "gtdbtk-res", "{batch}", "gtdbtk.bac120.summary.tsv"),
+        ar  = os.path.join(RESDIR, "gtdbtk-res", "{batch}", "gtdbtk.ar53.summary.tsv"  ),                         
     run:
+        import os
         import pandas as pd
-        bac = pd.DataFrame()
-        if os.stat(str(input.bac)).st_size != 0:
-            bac = pd.read_csv(str(input.bac),sep='\t',header=0)
-        arc = pd.DataFrame()
-        if os.stat(str(input.ar)).st_size != 0:
-            arc = pd.read_csv(str(input.ar),sep='\t',header=0)
-
-        pd.concat([bac,arc]).to_csv(str(output),index=False,header=True,sep='\t')
-        # SILENT ERROR ON CLUSTER ????? 
-        #"cat {input} | grep -m 1 user_genome > {output}; " # grep header from input files, either input.bac and input.ar can be empty
-        #"tail -q -n +2 {input} >> {output} "
-        # "cat {input.bac} "                # keep header from first input
-        # "<(tail -q -n +2 {input.ar}) "    # remove header from other input
-        # "> {output} "
+        dfs = []
+        for f in input:
+            if os.stat(str(f)).st_size != 0:
+                t = pd.read_csv(str(f),sep='\t',header=0)
+                dfs.append(t)    
+        df = pd.DataFrame()
+        if dfs:
+            df = pd.concat(dfs,axis=0)
+            df.user_genome = df.user_genome.str.replace("USER_","")
+        df.to_csv(str(output),index=False,header=True,sep='\t')
+
 
 
 rule gm_gtdbtk_classify_wf:
     output:
-        os.path.join(RESDIR , "gtdbtk-res",  "gtdbtk.ar53.summary.tsv"),        
-        os.path.join(RESDIR , "gtdbtk-res",  "gtdbtk.bac120.summary.tsv"),
+        os.path.join(RESDIR , "gtdbtk-res", "{batch}", "gtdbtk.ar53.summary.tsv"),        
+        os.path.join(RESDIR , "gtdbtk-res", "{batch}", "gtdbtk.bac120.summary.tsv"),
     input:
-        os.path.join(RESDIR , "gtdbtk-res", "batchfile.tsv"),
+        os.path.join(RESDIR , "gtdbtk-res", "{batch}", "batchfile.tsv"),
     conda: 
         os.path.join(".." , "envs" , "gtdbtk_2.1.yaml")
     params:
-        outdir = os.path.join(RESDIR , "gtdbtk-res"),
+        outdir = os.path.join(RESDIR , "gtdbtk-res", "{batch}"),
         gtdbtk_data = config["config-genomes"]["GTDB"],
     threads:
         15
     shell:
         "export GTDBTK_DATA_PATH={params.gtdbtk_data}; "
         "gtdbtk classify_wf "
         "--mash_db {params.gtdbtk_data} "
         "--batchfile {input} "
         "--out_dir {params.outdir} "
         "--cpus {threads} --debug && "
         "touch {output}"
 
 
+#def get_batch(wildcards):
+
+
 rule gm_gtdbtk_batchfile:
     output:
-        os.path.join(RESDIR , "gtdbtk-res", "batchfile.tsv")
+        os.path.join(RESDIR , "gtdbtk-res", "{batch}", "batchfile.tsv")
     params:
-        input_datas = INPUT
+        batch = lambda wildcards: GENOMESBATCH[wildcards.batch],
     run: 
         with open(str(output),'w') as fh:
-            for gid, files in params.input_datas.items():
+            for gid, file in params.batch.items():
                 fh.write("{}\tUSER_{}\n".format(                    
-                    files["genome"],
+                    file,
                     gid
                 ))
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/rules/ncbi_metadatas.smk` & `pcalf-1.2.2/pcalf/workflow/annotate/rules/ncbi_metadatas.smk`

 * *Files 11% similar despite different names*

```diff
@@ -21,9 +21,11 @@
     """
     output:
         os.path.join( RESDIR,"ncbi-datas","accession.txt" )     
     params:
         INPUT    
     run:        
         with open(str(output), 'w' ) as fh:
-            for k in INPUT.keys():                
-                fh.write("{}\n".format(k))                
+            for k in INPUT.keys():  
+                if k.startswith('GCA_') or k.startswith('GCF_'):
+                    k = "_".join(k.split('_')[0:2])
+                    fh.write("{}\n".format(k))
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/rules/pcalf.smk` & `pcalf-1.2.2/pcalf/workflow/annotate/rules/pcalf.smk`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             elif v=="11":
                 partial = "5',3'"
             else:
                 pass
     return "_".join(seqid.replace('>','').split("_")[:-1]) , start, stop, strand, partial, pseudo, "Prodigal prediction"
 
 
-rule ccya:
+rule pm_CCYA:
     output:
         os.path.join(RESDIR , "pcalf" , "ccyA.summary.tsv" ),
     input:
         os.path.join(RESDIR , "pcalf" , "pcalf.summary.tsv" ),
         os.path.join(RESDIR , "cds_fna_input.tsv"),        
     run:
         files = {}
@@ -148,15 +148,15 @@
         os.path.join(RESDIR , "pcalf" , "N-ter-DB.tsv"),
     run:
         import pandas as pd
         df = pd.read_csv(str(input),sep="\t",header=None)
         df.columns = ["nter","sequence_id","sequence"]
         df.to_csv(str(output),sep="\t", header=True,index = False)
 
-rule pm_pcalf:
+rule pm_PCALF:
     output:
         os.path.join(RESDIR , "pcalf" , "pcalf.summary.tsv" ),
         os.path.join(RESDIR , "pcalf" , "pcalf.features.tsv"),
         temp(os.path.join(RESDIR , "pcalf" , "N-ter-DB.tsv")),
         expand(
             os.path.join(RESDIR , "pcalf" ,"HMM","{hmm}.hmm"),
             hmm = ["Gly1","Gly2","Gly3","Glyx3"]
@@ -174,17 +174,16 @@
         gly2   = "--gly2-msa {}".format(config["config-ccya"]["gly2_msa"]) if config["config-ccya"]["gly2_msa"] else "",
         gly3   = "--gly3-msa {}".format(config["config-ccya"]["gly3_msa"]) if config["config-ccya"]["gly3_msa"] else "",
         nter   = "--nterdb {}".format(config["config-ccya"]["nterdb"]) if config["config-ccya"]["nterdb"] else "",
         evalue = "--glyx3-evalue {}".format(config["config-ccya"]["glyx3-evalue"]) if config["config-ccya"]["glyx3-evalue"] else "",
         coverage = "--glyx3-coverage {}".format(config["config-ccya"]["glyx3-coverage"]) if config["config-ccya"]["glyx3-coverage"] else "",
         glyzip_evalue = "--glyzip-evalue {}".format(config["config-ccya"]["glyzip-evalue"]) if config["config-ccya"]["glyzip-evalue"] else "",
         glyzip_coverage = "--glyzip-coverage {}".format(config["config-ccya"]["glyzip-coverage"]) if config["config-ccya"]["glyzip-coverage"] else "",
-        maxite = config["config-ccya"]['max-iteration'],
-        iterative_search = '--iterative-search' if config["config-ccya"]['iterative-search'] else '',
-        iterative_update = '--iterative-search' if config["config-ccya"]['iterative-update'] else '',
+        maxite = config["config-ccya"]['max-iteration'],        
+        iterative_update = '--iterative-update' if config["config-ccya"]['iterative-update'] else '',
         Z = "-Z {}".format(config["config-ccya"]["Z"]) if config["config-ccya"]["Z"] else "",
         domZ = "--domZ {}".format(config["config-ccya"]["domZ"]) if config["config-ccya"]["domZ"] else "",
     log:
         os.path.join(RESDIR , "logs" , "pcalf.log"),
     resources:        
         mem_mb= 1000,        
         nodes= 1, 
@@ -201,15 +200,14 @@
         "{params.gly3} "
         "{params.nter} "
         "--log {log} "
         "{params.evalue} "
         "{params.coverage} "
         "{params.glyzip_evalue} "
         "{params.glyzip_coverage} "
-        "{params.iterative_search} "
         "{params.iterative_update} "
         "--max-iteration {params.maxite} "
         "{params.Z} "
         "{params.domZ} " 
     
 def get_cds(wildcards):
     cds = []
```

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/scripts/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/annotate/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/annotate/scripts/ncbi_metadatas.py` & `pcalf-1.2.2/pcalf/workflow/annotate/scripts/ncbi_metadatas.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/Snakefile` & `pcalf-1.2.2/pcalf/workflow/datasets/Snakefile`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/config/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/datasets/config/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/envs/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/datasets/envs/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/rules/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/datasets/rules/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/rules/download.smk` & `pcalf-1.2.2/pcalf/workflow/datasets/rules/download.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/rules/fetch.smk` & `pcalf-1.2.2/pcalf/workflow/datasets/rules/fetch.smk`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     input:
         get_accession,
     shell:
         "cat {input} | sort | uniq > {output}"
 
 
 # GET ACCESSION FROM TAXID
-
 rule dm_ncbi_aggregate_accession_from_ncbi_cli_taxid:
     output:
         os.path.join(RESDIR,"tmp","accession.cli.txt"),
     input:
         expand(os.path.join(RESDIR,"tmp","taxids", "taxid_{taxid}",'accession_from_taxid_cmdline.tsv'),
             taxid=config["taxid"]),
     shell:
```

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/rules/translate.smk` & `pcalf-1.2.2/pcalf/workflow/datasets/rules/translate.smk`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/.DS_Store` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/datas.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/datas.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/fallback.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/fallback.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/filter_accession_on_taxid.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/get_ncbi_reports.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/get_ncbi_reports.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/gimme_taxa.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/gimme_taxa.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/log.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/log.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/taxid_children.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/taxid_children.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf/workflow/datasets/scripts/utils.py` & `pcalf-1.2.2/pcalf/workflow/datasets/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/pcalf.egg-info/PKG-INFO` & `pcalf-1.2.2/pcalf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 1.2.1
+Version: 1.2.2
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcalf-1.2.1/pcalf.egg-info/SOURCES.txt` & `pcalf-1.2.2/pcalf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 pcalf/workflow/annotate/envs/biopython_1.79.yaml
 pcalf/workflow/annotate/envs/checkm.yaml
 pcalf/workflow/annotate/envs/gtdbtk_2.1.yaml
 pcalf/workflow/annotate/envs/ncbi_dataset_14.14.0.yaml
 pcalf/workflow/annotate/rules/.DS_Store
 pcalf/workflow/annotate/rules/checkm.smk
 pcalf/workflow/annotate/rules/gtdbtk.smk
-pcalf/workflow/annotate/rules/gtdbtk_by_batch.smk
 pcalf/workflow/annotate/rules/ncbi_metadatas.smk
 pcalf/workflow/annotate/rules/pcalf.smk
 pcalf/workflow/annotate/scripts/.DS_Store
 pcalf/workflow/annotate/scripts/ncbi_metadatas.py
 pcalf/workflow/datasets/.DS_Store
 pcalf/workflow/datasets/Snakefile
 pcalf/workflow/datasets/__init__.py
```

### Comparing `pcalf-1.2.1/scripts/pcalf` & `pcalf-1.2.2/scripts/pcalf`

 * *Files 26% similar despite different names*

```diff
@@ -30,17 +30,14 @@
     parser.add_argument('-i','--input', dest='input', 
                         type = str, default=None,
                         help="Either a fasta file [gzip supported] or a tabular file with one file \"designation\tfile path\" per line.")
                                   
     parser.add_argument('-o', dest='res_dir', type=str, required=True,
                         help='Output directory. pcalf will ouput several files including updated HMMs and MSAs, a feature table and a summary.')   
 
-    parser.add_argument('--iterative-search', action="store_true",
-                        help="If set, searches will be done with updated profiles until convergence or --max-iteration is reached . ")
-
     parser.add_argument('--max-iteration', default=4,
                         help="Max iteration to be done if iterative-search enable. (default: %(default)s) ")                        
 
     parser.add_argument('--iterative-update', action="store_true",
                         help="If set, HMM profiles will be updated by aligning one sequence by one sequence. ")
 
     parser.add_argument('--glyx3-msa', dest = 'glyx3_msa', 
@@ -198,21 +195,18 @@
     
     # Initital number of sequences.
     _glyx3_nseq = glyx3.hmm.nseq
     _gly1_nseq = gly1.hmm.nseq
     _gly2_nseq = gly2.hmm.nseq
     _gly3_nseq = gly3.hmm.nseq
 
-    if args.iterative_search:
-        pcalf_func = search.iterative_pcalf
-    else:
-        pcalf_func = search.pcalf
+
 
     logger.info("Start search.")
-    calseq , u_glyx3 , u_gly1, u_gly2 , u_gly3 , u_nter = pcalf_func(
+    calseq , u_glyx3 , u_gly1, u_gly2 , u_gly3 , u_nter = search.run_pcalf(
         fastas,
         names,
         glyx3,
         gly1,
         gly2,
         gly3,
         nterdb, 
@@ -221,87 +215,28 @@
         glyx3_evalue_threshold=args.glyx3_evalue_threshold,  
         glyx3_coverage_threshold=args.glyx3_coverage_threshold,  
         glyzip_evalue_threshold= args.glyzip_e_evalue,
         glyzip_coverage_threshold = args.glyzip_coverage,
         nter_coverage_threshold = args.nter_coverage, 
         nter_evalue_threshold  =  args.nter_evalue,
         is_update_iterative=args.iterative_update,        
-        max_iteration=args.max_iteration
+        max_iteration=args.max_iteration,
+        res_dir = res_dir
     )
    
     logger.info("The search is over.")
 
     logger.info("# N_seqs within Glyx3 HMM : {} [+{}]".format(
         u_glyx3.hmm.nseq, u_glyx3.hmm.nseq -  _glyx3_nseq))
     logger.info("# N_seqs within Gly1 HMM : {} [+{}]".format(
         u_gly1.hmm.nseq, u_gly1.hmm.nseq - _gly1_nseq))
     logger.info("# N_seqs within Gly2 HMM : {} [+{}]".format(
         u_gly2.hmm.nseq, u_gly2.hmm.nseq - _gly2_nseq))
     logger.info("# N_seqs within Gly3 HMM : {} [+{}]".format(
         u_gly3.hmm.nseq, u_gly3.hmm.nseq - _gly3_nseq))
     
-    logger.info("Dumping HMMs.") 
-    hmmdir = os.path.join(res_dir,"HMM")
-    os.makedirs(hmmdir,exist_ok=True)
-    u_glyx3.hmm.write(open(hmmdir + "/Glyx3.hmm","wb"))
-    u_gly1.hmm.write(open(hmmdir + "/Gly1.hmm","wb"))
-    u_gly2.hmm.write(open(hmmdir + "/Gly2.hmm","wb"))
-    u_gly3.hmm.write(open(hmmdir + "/Gly3.hmm","wb"))
-
-    logger.info("Dumping MSAs.")
-    msadir = os.path.join(res_dir,"MSA")    
-    os.makedirs(msadir,exist_ok=True)
-    u_glyx3.msa.write(open(msadir+"/Glyx3.msa.fa","wb"),format="afa")
-    u_gly1.msa.write(open(msadir+"/Gly1.msa.fa","wb"),format="afa")
-    u_gly2.msa.write(open(msadir+"/Gly2.msa.fa","wb"),format="afa")
-    u_gly3.msa.write(open(msadir+"/Gly3.msa.fa","wb"),format="afa")
-    
-    logger.info("Dumping N-ter table.")
-    with open(res_dir+"/N-ter-DB.tsv","w") as nterout:
-        for nterid, n in u_nter.items():
-            nterout.write("{}\t{}\t{}\n".format(n[0],nterid,n[1]))
-
-    logger.info("Writing feature table.")
-    features = calseq.to_feature_table()
-    features.to_csv(res_dir + "/pcalf.features.tsv",sep="\t",header=True,index=True)
-    logger.info("Writing hits table")
-    hits = calseq.to_hits_table()
-    hits.to_csv(res_dir + "/pcalf.hits.tsv",sep="\t",header=True,index=True)
-
-    logger.info("Making summary.")
-    summary_datas = []
-    for idx, seq_features_df in features.groupby(["sequence_id","sequence_src"]):
-        sequence = idx[0]
-        sequence_src = idx[1]
-        cterom = ",".join(
-                        list(
-                            seq_features_df[seq_features_df.feature_id.isin(["Gly1","Gly2","Gly3"]) ].sort_values("feature_start").feature_id
-                            )
-                )
-
-        nter_type = None
-        nter_neighbor = None 
-        if not seq_features_df[seq_features_df.feature_id == "N-ter" ].empty:
-            nter_type,nter_neighbor = "".join(set(
-                seq_features_df[seq_features_df.feature_id == "N-ter" ].feature_src
-            )).split("||")
-
-        summary_datas.append(
-            {
-                "sequence_accession":sequence,
-                "sequence_src": sequence_src,
-                "flag":search.decision_tree(nter_type,cterom),
-                "nter":nter_type,
-                "nter_neighbor": nter_neighbor,
-                "cter":cterom,
-                "sequence":str(calseq.get_seq_by_id(sequence).seq),
-                # "iteration":seq_per_iteration[sequence]
-            }
-        )
-    if summary_datas:
-        df = pd.DataFrame(summary_datas).set_index("sequence_accession")
-    else:
-        df = pd.DataFrame(columns=["sequence_accession","sequence_src","flag","nter","nter_neighbor","cter","sequence"]).set_index("sequence_accession")
-    df.to_csv(res_dir + "/pcalf.summary.tsv",sep="\t",index=True,header=True)
+    ##
+
+   
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pcalf-1.2.1/scripts/pcalf-annotate-workflow` & `pcalf-1.2.2/scripts/pcalf-annotate-workflow`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 def get_args():
     parser = argparse.ArgumentParser(
         description="""
 
     pcalf-annotate
     Annotate genomes using pcalf, GTDB-TK, CheckM and ncbi-datasets CLI.
-
     """,
         formatter_class= argparse.RawTextHelpFormatter
     )
     parser.add_argument('-i', '--input', required=True , type=str , 
             help = "Yaml file containing path to genome, cds_faa and cds_fna, see README.md for details.")  
        
     parser.add_argument('--db', type=None , 
@@ -48,23 +47,46 @@
 
     parser.add_argument("--gtdb", default=None , type=str , 
             help = "path to GTDB database. [None]")
     
     parser.add_argument("--checkm", default=None , type=str , 
             help = "path to checkm datas. [None]")
 
+    parser.add_argument("-z", "--batch-size", default=1500 , type=int , 
+            help = "Batch size for CheckM and GTDBTK. [1500]")
+
     parser.add_argument('-q', '--quick', default=False, action="store_true", 
             help = "If set CheckM and GTDB-TK steps will not be run [False]")
 
     parser.add_argument('--force', action="store_true", 
            help= "Use this flag if you want to resume jobs from a specific instance. [False]" )
     
     parser.add_argument('--original', action="store_true", 
             help = "Use original HMMs and N-ter files for pcalf. [False]")
 
+    parser.add_argument('--glyx3-msa', dest = 'glyx3_msa', 
+                        default = None,
+                        help='Path to GlyX3 msa (default: %(default)s). A weighted HMM will be built from it.' )
+
+    parser.add_argument('--gly1-msa', dest = 'gly1_msa', 
+                        default = None, 
+                        help='Path to GlyZip1 msa (default: %(default)s). A weighted HMM will be built from it.' )
+
+    parser.add_argument('--gly2-msa', dest = 'gly2_msa', 
+                        default = None,
+                        help='path to GlyZip2 msa (default: %(default)s). A weighted HMM will be built from it.')
+
+    parser.add_argument('--gly3-msa', dest = 'gly3_msa', 
+                        default = None,
+                        help='path to GlyZip3 msa (default: %(default)s). A weighted HMM will be built from it.')    
+
+    parser.add_argument('--nter', dest = 'nter', 
+                        default = None,
+                        help='path to N-ter file (default: %(default)s).')    
+
     parser.add_argument("--debug", action="store_true")
 
     parser.add_argument('--snakargs', type=str, 
               default="--printshellcmds -j{} --use-conda".format(multiprocessing.cpu_count()),
               help='Snakemake arguments.')
 
     args = parser.parse_args()
@@ -108,18 +130,17 @@
      # Load DB if provided  else init one.
     dbfile = os.path.join(outdir,"pcalf.db")
     if os.path.exists(dbfile) and args.force:
         os.remove(dbfile)    
     
     logger.debug("DB file is : {}".format(dbfile))
     db = PcalfDB.PcalfDB(dbfile)    
-    glyx3 , gly1 , gly2, gly3 , nter = None, None, None, None, None
+    glyx3 , gly1 , gly2, gly3 , nter = args.glyx3_msa, args.gly1_msa, args.gly2_msa, args.gly3_msa , args.nter
 
-    if args.db: #db file provided        
-        
+    if args.db: #db file provided            
         logger.info("MSAs from {} will be used.".format(args.db))  
         externaldb = PcalfDB.PcalfDB(args.db)    
 
         if not externaldb.is_schema_valid():
             logger.error("Current database schema is different from the schema of the database you provide.")
             exit(-1)
 
@@ -149,14 +170,15 @@
     if not args.quick:
         if not args.checkm or not args.gtdb or not os.path.isdir(args.checkm) or not os.path.isdir(args.gtdb):
             logger.error("GTDB and checkm datas should be specified. If you want to skip this part of the analysis use the --quick flag.")
             exit(-1)
 
     annotate_module.config["config-genomes"]["CheckM_data"] = args.checkm
     annotate_module.config["config-genomes"]["GTDB"] =  args.gtdb
+    annotate_module.config["config-genomes"]["batch_size"] =  args.batch_size
     
     annotate_module.config["config-ccya"]["glyx3_msa"] = glyx3
     annotate_module.config["config-ccya"]["gly1_msa"]  = gly1
     annotate_module.config["config-ccya"]["gly2_msa"]  = gly2
     annotate_module.config["config-ccya"]["gly3_msa"]  = gly3
     annotate_module.config["config-ccya"]["nterdb"]    = nter
```

### Comparing `pcalf-1.2.1/scripts/pcalf-datasets-workflow` & `pcalf-1.2.2/scripts/pcalf-datasets-workflow`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/scripts/pcalf-report` & `pcalf-1.2.2/scripts/pcalf-report`

 * *Files identical despite different names*

### Comparing `pcalf-1.2.1/setup.py` & `pcalf-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pcalf',
-    version='1.2.1',
+    version='1.2.2',
     description='Search calcyanin in a set of amino acid sequences',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/K2SOHIGH/pcalf',
     author='Maxime Millet',
     author_email='maxime.luc.millet@gmail.com',
     license='MIT',
@@ -33,8 +33,8 @@
     ],
     python_requires = ">=3.9",
     packages = find_packages(),
     # package_dir = {"": "pcalf"},
     include_package_data=True,
     scripts = [script for script in glob.glob("scripts/*") if not os.path.basename(script).startswith("_") ],
     zip_safe=False
-)
+)
```

