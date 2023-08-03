# Comparing `tmp/chromatinhd-0.0.18.tar.gz` & `tmp/chromatinhd-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromatinhd-0.0.18.tar", last modified: Sat Jul 22 10:24:12 2023, max compression
+gzip compressed data, was "chromatinhd-0.0.19.tar", last modified: Thu Aug  3 08:46:52 2023, max compression
```

## Comparing `chromatinhd-0.0.18.tar` & `chromatinhd-0.0.19.tar`

### file list

```diff
@@ -1,209 +1,223 @@
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/.github/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/.github/workflows/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      539 2023-07-22 10:00:10.000000 chromatinhd-0.0.18/.github/workflows/ci.yml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3298 2023-07-21 17:12:01.000000 chromatinhd-0.0.18/.gitignore
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      120 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/.pre-commit-config.yaml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1070 2023-07-22 10:00:10.000000 chromatinhd-0.0.18/LICENSE.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/PKG-INFO
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      284 2023-07-22 10:00:10.000000 chromatinhd-0.0.18/README.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2134 2023-07-22 10:00:10.000000 chromatinhd-0.0.18/_setup.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/docs/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/override/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      196 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/override/main.html
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2523 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/index.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      925 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/docs/source/index.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       28 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/jupytext.toml
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/quickstart/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1170 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/quickstart/0_install.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5643 2023-07-22 07:37:54.000000 chromatinhd-0.0.18/docs/source/quickstart/1_data.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5762 2023-07-22 07:37:54.000000 chromatinhd-0.0.18/docs/source/quickstart/2_pred.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3195 2023-07-22 07:37:54.000000 chromatinhd-0.0.18/docs/source/quickstart/3_diff.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/reference/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      179 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/reference/data.md
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/reference/index.md
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   167512 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/favicon.ai
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2336 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/static/favicon.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   220360 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/static/logo.ai
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9528 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/static/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/docs/source/static/models/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/diff/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/diff/1x/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7684 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/diff/1x/logo.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   973869 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/diff/logo.pdf
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/dime/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   221105 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/dime/logo.pdf
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4068 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/dime/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/pred/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/pred/1x/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1621 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/pred/1x/logo.png
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   153226 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/pred/logo.pdf
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/static/models/time/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   219145 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/time/logo.pdf
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3954 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/docs/source/static/models/time/logo.png
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/docs/source/stylesheets/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      846 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/docs/source/stylesheets/extra.css
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1131 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/mkdocs.yml
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1554 2023-07-22 10:22:42.000000 chromatinhd-0.0.18/pyproject.toml
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/scripts/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      262 2023-07-22 10:24:08.000000 chromatinhd-0.0.18/scripts/build.sh
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16878 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/scripts/setup_data_tiny.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1186 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/scripts/test.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       38 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/setup.cfg
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/src/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/src/chromatinhd/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      625 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/src/chromatinhd/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/src/chromatinhd/biomart/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       83 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/biomart/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       92 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/biomart/cache.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5301 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/biomart/dataset.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3561 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/biomart/tss.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      378 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/clustering/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/clustering/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1069 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/data/clustering/clustering.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/src/chromatinhd/data/examples/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2046327 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4403 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2614194 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/folds/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/folds/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1645 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/folds/folds.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/fragments/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       51 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/fragments/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7247 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/data/fragments/fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/genotype/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       31 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/genotype/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      146 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/genotype/genotype.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/motifscan/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       74 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/motifscan/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2392 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/motifscan/motifscan.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      528 2023-01-31 18:45:51.000000 chromatinhd-0.0.18/src/chromatinhd/data/motifscan/motiftrack.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1641 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/regions.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/data/transcriptome/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2022-12-09 09:27:27.000000 chromatinhd-0.0.18/src/chromatinhd/data/transcriptome/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4877 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/data/transcriptome/transcriptome.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2389 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/embedding.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8811 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/flow.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.924239 chromatinhd-0.0.18/src/chromatinhd/grid/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       47 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/grid/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1630 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/grid/broken.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    13895 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/grid/grid.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/loaders/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4314 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/chunkfragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/loaders/extraction/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5044 2022-12-15 11:33:47.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/extraction/fragments.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18790 2023-01-10 08:03:37.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/extraction/motifs.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10212 2023-01-31 18:34:46.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/fragmentmotif.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10565 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/fragments.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3733 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/minibatching.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1930 2023-01-09 14:53:04.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/peakcounts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8365 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/pool.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      374 2022-12-02 07:47:23.000000 chromatinhd-0.0.18/src/chromatinhd/loaders/setup.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2022-12-13 10:48:55.000000 chromatinhd-0.0.18/src/chromatinhd/loss.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1291 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/src/chromatinhd/models/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      132 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16611 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/differential.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/enrichment/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/enrichment/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18467 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/enrichment/enrichment.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/interpret/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/interpret/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5245 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/interpret/genepositional.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      150 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      924 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/clustering.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1016 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/clustering_cuts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4821 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/cuts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/fragments_helpers.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3231 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/minibatches.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    22901 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/cutnf.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    12040 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/spline.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       45 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9280 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/cubic.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3460 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/linear.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5788 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/quadratic.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14633 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5598 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/differential.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3183 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/differential_expression.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/diff/trainer/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/trainer/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3588 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/diff/trainer/trainer.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       84 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3261 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/censorers.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/filter.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8759 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/genemultiwindow.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7202 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/genepairwindow.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      182 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/cuts.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5133 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/fragments.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/fragments_helpers.pyx
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7051 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/minibatches.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      571 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/transcriptome.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/transcriptome_fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       23 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/model/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    21849 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/model/additive.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      117 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1434 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/copredictivity.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1593 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/effect.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7880 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/predictivity.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/models/pred/trainer/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/trainer/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4701 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/models/pred/trainer/trainer.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1126 2022-12-23 16:16:31.000000 chromatinhd-0.0.18/src/chromatinhd/optim.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11353 2023-02-14 20:01:54.000000 chromatinhd-0.0.18/src/chromatinhd/peakcounts.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/plot/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      102 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/src/chromatinhd/plot/__init__.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.928239 chromatinhd-0.0.18/src/chromatinhd/plot/genome/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/plot/genome/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11346 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/src/chromatinhd/plot/genome/genes.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2400 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/plot/matshow45.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1312 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/plot/patch.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1925 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/plot/quasirandom.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2297 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/src/chromatinhd/plot/tickers.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6568 2022-12-03 11:44:55.000000 chromatinhd-0.0.18/src/chromatinhd/sparse.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4716 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/train.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/src/chromatinhd/utils/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4452 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/__init__.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1395 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/ansi.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      966 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/ecdf.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      213 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/numpy.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2341 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/testing.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1255 2023-07-21 17:11:57.000000 chromatinhd-0.0.18/src/chromatinhd/utils/torch.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.920239 chromatinhd-0.0.18/src/chromatinhd.egg-info/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-07-22 10:24:12.000000 chromatinhd-0.0.18/src/chromatinhd.egg-info/PKG-INFO
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5694 2023-07-22 10:24:12.000000 chromatinhd-0.0.18/src/chromatinhd.egg-info/SOURCES.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        1 2023-07-22 10:24:12.000000 chromatinhd-0.0.18/src/chromatinhd.egg-info/dependency_links.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      260 2023-07-22 10:24:12.000000 chromatinhd-0.0.18/src/chromatinhd.egg-info/requires.txt
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       12 2023-07-22 10:24:12.000000 chromatinhd-0.0.18/src/chromatinhd.egg-info/top_level.txt
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/tests/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2074 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/tests/conftest.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/tests/models/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/tests/models/diff/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/tests/models/diff/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      508 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/tests/models/diff/loader/test_clustering_cuts.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/tests/models/diff/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      307 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/tests/models/diff/model/test_cutnf.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.916239 chromatinhd-0.0.18/tests/models/pred/
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/tests/models/pred/loader/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      533 2023-07-22 09:14:17.000000 chromatinhd-0.0.18/tests/models/pred/loader/test_transcriptome_fragments.py
-drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 10:24:12.932239 chromatinhd-0.0.18/tests/models/pred/model/
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      310 2023-07-22 07:01:56.000000 chromatinhd-0.0.18/tests/models/pred/model/test_additive.py
--rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      480 2023-01-31 18:34:46.000000 chromatinhd-0.0.18/tests/test_loss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/.github/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/.github/workflows/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      674 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/.github/workflows/ci.yml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3298 2023-07-21 17:12:01.000000 chromatinhd-0.0.19/.gitignore
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      120 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/.pre-commit-config.yaml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1070 2023-07-22 10:00:10.000000 chromatinhd-0.0.19/LICENSE.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/PKG-INFO
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      284 2023-07-22 10:00:10.000000 chromatinhd-0.0.19/README.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/override/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      196 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/override/main.html
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2523 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/index.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      925 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/docs/source/index.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       28 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/jupytext.toml
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/quickstart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1170 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/quickstart/0_install.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5643 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/1_data.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5762 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/2_pred.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3195 2023-07-22 07:37:54.000000 chromatinhd-0.0.19/docs/source/quickstart/3_diff.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/data/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       42 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/clustering.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/fragments.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/regions.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       34 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/data/transcriptome.md
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/reference/index.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/source/reference/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/reference/models/pred/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/reference/models/pred/plot.md
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   167512 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/favicon.ai
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2336 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/favicon.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   220360 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/logo.ai
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9528 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/docs/source/static/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/docs/source/static/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/diff/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/diff/1x/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7684 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/diff/1x/logo.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   973869 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/diff/logo.pdf
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/dime/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   221105 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/dime/logo.pdf
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4068 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/dime/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/pred/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/pred/1x/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1621 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/pred/1x/logo.png
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   153226 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/pred/logo.pdf
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/static/models/time/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)   219145 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/time/logo.pdf
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3954 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/docs/source/static/models/time/logo.png
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/docs/source/stylesheets/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      375 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/stylesheets/extra-reference.css
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      847 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/docs/source/stylesheets/extra.css
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1270 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/mkdocs.yml
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1616 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/pyproject.toml
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/scripts/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      415 2023-08-03 08:46:41.000000 chromatinhd-0.0.19/scripts/build.sh
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16878 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/scripts/setup_data_tiny.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1186 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/scripts/test.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       38 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/setup.cfg
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/src/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      661 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/biomart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      101 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       92 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/cache.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5785 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/dataset.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3611 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/biomart/tss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      378 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/clustering/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/clustering/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1069 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/data/clustering/clustering.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.279798 chromatinhd-0.0.19/src/chromatinhd/data/examples/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2046327 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4403 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)  2614194 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/folds/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/folds/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3670 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/folds/folds.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/fragments/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       51 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/fragments/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7344 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/fragments/fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/genotype/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       31 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/genotype/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      146 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/genotype/genotype.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       74 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2392 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motifscan.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      528 2023-01-31 18:45:51.000000 chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motiftrack.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       35 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11269 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/peakcounts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2179 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/regions.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       40 2022-12-09 09:27:27.000000 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4781 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/transcriptome.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      238 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/device.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2430 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/embedding.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9539 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/flow.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/grid/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       47 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/grid/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1729 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/grid/broken.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14406 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/grid/grid.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/loaders/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4314 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/chunkfragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5044 2022-12-15 11:33:47.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/fragments.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18790 2023-01-10 08:03:37.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/motifs.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10212 2023-01-31 18:34:46.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/fragmentmotif.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    10589 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/fragments.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3733 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/minibatching.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1930 2023-01-09 14:53:04.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/peakcounts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8390 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/pool.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      374 2022-12-02 07:47:23.000000 chromatinhd-0.0.19/src/chromatinhd/loaders/setup.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2022-12-13 10:48:55.000000 chromatinhd-0.0.19/src/chromatinhd/loss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1291 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/models/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      132 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    16611 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/differential.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    18467 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/enrichment.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5245 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/genepositional.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      150 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      924 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1016 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering_cuts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4821 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/cuts.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/fragments_helpers.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3231 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/minibatches.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       20 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    23535 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/cutnf.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    12040 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/spline.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       45 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     9280 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/cubic.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3460 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/linear.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5788 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/quadratic.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    14633 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5598 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3183 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential_expression.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.291798 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3588 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/trainer.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       84 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      147 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3261 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/censorers.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/filter.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8982 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genemultiwindow.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     7202 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genepairwindow.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      182 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     5133 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1399 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments_helpers.pyx
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     3255 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/minibatches.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      571 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1087 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome_fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       23 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    20929 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/across.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    21570 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/additive.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      338 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/model/loss.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      183 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1581 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/copredictivity.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1593 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/effect.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     8120 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/predictivity.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       29 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4701 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/trainer.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1200 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/optim.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/plot/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      102 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/__init__.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/plot/genome/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       25 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/genome/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)    11346 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/genome/genes.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2400 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/matshow45.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1312 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/patch.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1925 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/plot/quasirandom.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2297 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/src/chromatinhd/plot/tickers.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6499 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/sparse.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4716 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/train.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/src/chromatinhd/utils/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     4452 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/__init__.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1395 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/ansi.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      966 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/ecdf.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      269 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/utils/numpy.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2341 2023-07-21 17:11:57.000000 chromatinhd-0.0.19/src/chromatinhd/utils/testing.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     1240 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/src/chromatinhd/utils/torch.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.287798 chromatinhd-0.0.19/src/chromatinhd.egg-info/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      860 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/PKG-INFO
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     6084 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/SOURCES.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)        1 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/dependency_links.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      260 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/requires.txt
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)       12 2023-08-03 08:46:52.000000 chromatinhd-0.0.19/src/chromatinhd.egg-info/top_level.txt
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/biomart/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      165 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/tests/biomart/conftest.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      463 2023-08-03 08:46:11.000000 chromatinhd-0.0.19/tests/biomart/tss_test.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)     2074 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/tests/conftest.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/diff/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/diff/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      508 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/tests/models/diff/loader/test_clustering_cuts.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/diff/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      307 2023-07-22 07:01:56.000000 chromatinhd-0.0.19/tests/models/diff/model/test_cutnf.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.283798 chromatinhd-0.0.19/tests/models/pred/
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/pred/loader/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      533 2023-07-22 09:14:17.000000 chromatinhd-0.0.19/tests/models/pred/loader/test_transcriptome_fragments.py
+drwxr-xr-x   0 wsaelens (231941) peak_free_atac  (1006)        0 2023-08-03 08:46:52.295798 chromatinhd-0.0.19/tests/models/pred/model/
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      310 2023-08-02 13:32:25.000000 chromatinhd-0.0.19/tests/models/pred/model/test_additive.py
+-rw-r--r--   0 wsaelens (231941) peak_free_atac  (1006)      480 2023-01-31 18:34:46.000000 chromatinhd-0.0.19/tests/test_loss.py
```

### Comparing `chromatinhd-0.0.18/.gitignore` & `chromatinhd-0.0.19/.gitignore`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/LICENSE.md` & `chromatinhd-0.0.19/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/PKG-INFO` & `chromatinhd-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromatinhd
-Version: 0.0.18
+Version: 0.0.19
 Summary: High-definition modeling of (single-cell) chromatin + transcriptomics data
 Author-email: Wouter Saelens <wouter.saelens@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/DeplanckeLab/ChromatinHD
 Project-URL: Bug Tracker, https://github.com/DeplanckeLab/ChromatinHD/issues
 Keywords: bioinformatics,chromatin accessibility,transcriptomics
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.18 Summary: High-
+Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.19 Summary: High-
 definition modeling of (single-cell) chromatin + transcriptomics data Author-
 email: Wouter Saelens
 saelens@gmail.com> License: MIT Project-URL: Homepage, https://github.com/
 DeplanckeLab/ChromatinHD Project-URL: Bug Tracker, https://github.com/
 DeplanckeLab/ChromatinHD/issues Keywords: bioinformatics,chromatin
 accessibility,transcriptomics Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `chromatinhd-0.0.18/_setup.py` & `chromatinhd-0.0.19/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,69 @@
-# Get version
-import re
+[build-system]
+requires = [ "setuptools>=41", "wheel", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
 
+[tool.setuptools-git-versioning]
+enabled = true
+
+[project]
 name = "chromatinhd"
+authors = [
+    {name = "Wouter Saelens", email = "wouter.saelens@gmail.com"},
+]
+description = "High-definition modeling of (single-cell) chromatin + transcriptomics data"
+requires-python = ">=3.8"
+keywords = ["bioinformatics", "chromatin accessibility", "transcriptomics"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+]
+dependencies = [
+    "torch",  # --extra-index-url https://download.pytorch.org/whl/cu113
+    "torch-scatter", # --find-links https://data.pyg.org/whl/torch-1.12.1+cu113.html
+    "scanpy",
+    "matplotlib",
+    "numpy",
+    "seaborn",
+    "Cython",
+    "fisher",
+    "diskcache",
+    "appdirs",
+    "xarray",
+    "pysam",
+]
+dynamic = ["version", "readme"]
+license = {text = "MIT"}
+
+[project.urls]
+"Homepage" = "https://github.com/DeplanckeLab/ChromatinHD"
+"Bug Tracker" = "https://github.com/DeplanckeLab/ChromatinHD/issues"
+
+[tool.setuptools.dynamic]
+readme = {file = "README.md", content-type = "text/markdown"}
+
+[project.optional-dependencies]
+dev = [
+    "pre-commit",
+    "pytest",
+    "coverage",
+    "black",
+    "pylint",
+    "jupytext",
+    "pytest",
+    "statsmodels",
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings[python]",
+    "mkdocs-jupyter",
+    "mike",
+    "cairosvg",  # for mkdocs social
+    "pillow",  # for mkdocs social
+    "setuptools_scm"
+    # "faiss-cpu",
+]
 
-import setuptools
+[tool.setuptools_scm]
 
-VERSIONFILE = "src/" + name + "/_version.py"
-verstrline = open(VERSIONFILE, "rt").read()
-VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
-mo = re.search(VSRE, verstrline, re.M)
-if mo:
-    version = mo.group(1)
-else:
-    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
-
-# get long description
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name=name,
-    version=version,
-    author="Wouter Saelens",
-    author_email="wouter.saelens@gmail.com",
-    description="Modeling of chromatin + transcriptomics data",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/DeplanckeLab/ChromatinHD",
-    packages=setuptools.find_packages("src"),
-    package_dir={"": "src"},
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.8",
-    install_requires=[
-        "torch",  # --extra-index-url https://download.pytorch.org/whl/cu113
-        "torch-scatter",
-        # "torch==1.12.1",  # --extra-index-url https://download.pytorch.org/whl/cu113
-        # "torch-scatter",  # --find-links https://data.pyg.org/whl/torch-1.12.1+cu113.html
-        "scanpy",
-        "matplotlib",
-        "numpy",
-        "seaborn",
-        "Cython",
-        "fisher",
-        "diskcache",
-        "appdirs",
-        "xarray",
-        "pysam",
-    ],
-    extras_require={
-        "full": [],
-        "dev": [
-            "pre-commit",
-            "pytest",
-            "coverage",
-            "black",
-            "pylint",
-            "jupytext",
-            "pytest",
-            "statsmodels",
-            "mkdocs",
-            "mkdocs-material",
-            "mkdocstrings[python]",
-            "mkdocs-jupyter",
-            "mike",
-            "cairosvg",  # for mkdocs social
-            "pillow",  # for mkdocs social
-            # "faiss-cpu",
-        ],
-        "eqtl": ["cyvcf2", "xarray"],
-    },
-)
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore",
+]
```

### Comparing `chromatinhd-0.0.18/docs/source/index.md` & `chromatinhd-0.0.19/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/index.py` & `chromatinhd-0.0.19/docs/source/index.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/quickstart/0_install.py` & `chromatinhd-0.0.19/docs/source/quickstart/0_install.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/quickstart/1_data.py` & `chromatinhd-0.0.19/docs/source/quickstart/1_data.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/quickstart/2_pred.py` & `chromatinhd-0.0.19/docs/source/quickstart/2_pred.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/quickstart/3_diff.py` & `chromatinhd-0.0.19/docs/source/quickstart/3_diff.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/favicon.ai` & `chromatinhd-0.0.19/docs/source/static/favicon.ai`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/favicon.png` & `chromatinhd-0.0.19/docs/source/static/favicon.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/logo.ai` & `chromatinhd-0.0.19/docs/source/static/logo.ai`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/logo.png` & `chromatinhd-0.0.19/docs/source/static/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/diff/1x/logo.png` & `chromatinhd-0.0.19/docs/source/static/models/diff/1x/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/diff/logo.pdf` & `chromatinhd-0.0.19/docs/source/static/models/diff/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/dime/logo.pdf` & `chromatinhd-0.0.19/docs/source/static/models/dime/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/dime/logo.png` & `chromatinhd-0.0.19/docs/source/static/models/dime/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/pred/1x/logo.png` & `chromatinhd-0.0.19/docs/source/static/models/pred/1x/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/pred/logo.pdf` & `chromatinhd-0.0.19/docs/source/static/models/pred/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/time/logo.pdf` & `chromatinhd-0.0.19/docs/source/static/models/time/logo.pdf`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/static/models/time/logo.png` & `chromatinhd-0.0.19/docs/source/static/models/time/logo.png`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/docs/source/stylesheets/extra.css` & `chromatinhd-0.0.19/docs/source/stylesheets/extra.css`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 .jupyter-wrapper .jp-InputArea-editor {
     border-left: 2px green solid !important;
 }
 
 /* remove the cell toolbar with ugly tags */
 .jupyter-wrapper .celltoolbar {
     display: none !important;
-}
+}
```

### Comparing `chromatinhd-0.0.18/mkdocs.yml` & `chromatinhd-0.0.19/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
   - mkdocstrings:
       handlers:
         python:
           import:
           - https://docs.python-requests.org/en/master/objects.inv
           options:
             docstring_style: google
+            heading_level: 2
+            inheritance_diagram: True
+            show_root_heading: True
   - mike
   - search
   - mkdocs-jupyter:
       include: ["*.ipynb"] # Default: ["*.py", "*.ipynb"]
       remove_tag_config:
         remove_input_tags:
           - hide_code
@@ -43,8 +46,9 @@
   - admonition
   - pymdownx.details
   - pymdownx.superfences
   - attr_list
   - md_in_html
   - pymdownx.details
 extra_css:
-  - stylesheets/extra.css
+  - stylesheets/extra.css
+  - stylesheets/extra-reference.css
```

### Comparing `chromatinhd-0.0.18/scripts/setup_data_tiny.py` & `chromatinhd-0.0.19/scripts/setup_data_tiny.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/scripts/test.py` & `chromatinhd-0.0.19/scripts/test.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/__init__.py` & `chromatinhd-0.0.19/src/chromatinhd/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .device import default_device
 from .utils import get_git_root, get_output, get_code, save, Unpickler, load
 from . import sparse
 from . import utils
 from . import flow
 from . import grid
 from . import plot
 from . import data
@@ -29,8 +30,8 @@
     "loss",
     "embedding",
     "optim",
     "grid",
     "biomart",
     "models",
     "plot",
-]
+]
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/biomart/dataset.py` & `chromatinhd-0.0.19/src/chromatinhd/biomart/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import pandas as pd
 import io
 from .cache import cache
 import xml.etree.cElementTree as ET
 
 
 def get_datasets(
-    mart="ENSEMBL_MART_ENSEMBL", baseurl="http://www.ensembl.org/biomart/martservice?"
-):
+    mart:str="ENSEMBL_MART_ENSEMBL", baseurl:str="http://www.ensembl.org/biomart/martservice?"
+) -> pd.DataFrame:
+    """
+    List all datasets available within a mart and baseurl
+    """
     url = f"{baseurl}type=datasets&requestid=biomaRt&mart={mart}"
     if url in cache:
         attributes = cache[url]
     else:
         response = requests.get(url)
         datasets = pd.read_table(
             io.StringIO(response.text),
@@ -59,14 +62,17 @@
         mart="ENSEMBL_MART_ENSEMBL",
     ):
         self.name = name
         self.mart = mart
         self.baseurl = baseurl
 
     def list_attributes(self):
+        """
+        List all attributes available in a dataset
+        """
         url = f"{self.baseurl}type=attributes&dataset={self.name}&mart={self.mart}"
 
         if url in cache:
             attributes = cache[url]
         else:
             response = requests.get(url)
             attributes = pd.read_table(
@@ -83,14 +89,17 @@
                     "alternative_attribute",
                 ],
             ).set_index("attribute")
             cache[url] = attributes
         return attributes
 
     def list_filters(self):
+        """
+        List all filters available in a dataset
+        """
         url = f"{self.baseurl}type=filters&dataset={self.name}&mart={self.mart}"
 
         if url in cache:
             filters = cache[url]
         else:
             response = requests.get(url)
             filters = pd.read_table(
@@ -114,15 +123,18 @@
 
     def attribute(self, name, **kwargs):
         return Attribute(name, **kwargs)
 
     def filter(self, name, **kwargs):
         return Filter(name, **kwargs)
 
-    def get(self, attributes=[], filters=[]):
+    def get(self, attributes=[], filters=[]) -> pd.DataFrame:
+        """
+        Get the result with a given set of attributes and filters
+        """
         xml = ET.Element(
             "Query",
             virtualSchemaName="default",
             formatter="TSV",
             header="0",
             uniqueRows="0",
             datasetConfigVersion="0.6",
@@ -147,14 +159,17 @@
                 names=[attribute.name for attribute in attributes],
             )
             cache[url] = result
         return result
 
     @classmethod
     def from_genome(self, genome):
+        """
+        Get the biomart dataset given a particular genome name, e.g. GRCm38, GRCh38, GRCm39, mm10, hg19, ...
+        """
         if genome in ["mm10", "GRCm38"]:
             return Dataset(
                 "mmusculus_gene_ensembl",
                 "https://nov2020.archive.ensembl.org/biomart/martservice?",
                 "ENSEMBL_MART_ENSEMBL",
             )
         elif genome in ["hg19", "GRCh37"]:
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/biomart/tss.py` & `chromatinhd-0.0.19/src/chromatinhd/biomart/tss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 from .dataset import Dataset
 
 
 def get_canonical_transcripts(
     biomart_dataset: Dataset, gene_ids=None, chrom=None, start=None, end=None
 ):
+    """
+    Get all canonical transcripts
+    """
     filters = []
     if gene_ids is not None:
         filters.append(
             biomart_dataset.filter("ensembl_gene_id", value=",".join(gene_ids))
         )
     if chrom is not None:
         filters.append(
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/clustering/clustering.py` & `chromatinhd-0.0.19/src/chromatinhd/data/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz` & `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi` & `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/fragments.tsv.gz.tbi`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad` & `chromatinhd-0.0.19/src/chromatinhd/data/examples/pbmc10ktiny/transcriptome.h5ad`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/fragments/fragments.py` & `chromatinhd-0.0.19/src/chromatinhd/data/fragments/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pandas as pd
-import pickle
 
 from chromatinhd.flow import (
     Flow,
     StoredTorchInt32,
     Stored,
     StoredTorchInt64,
     TSV,
@@ -27,24 +26,25 @@
 
 class Fragments(Flow):
     """Fragments centered around a gene window"""
 
     regions = Linked("regions")
     """regions of the fragments"""
 
-    coordinates = StoredTorchInt64("coordinates")
+    coordinates: torch.Tensor = StoredTorchInt64("coordinates")
     """Coordinates of the fragments"""
 
-    mapping = StoredTorchInt64("mapping")
+    mapping: torch.Tensor = StoredTorchInt64("mapping")
     """Mapping of a fragment to a gene and a cell"""
 
-    cellxgene_indptr = StoredTorchInt64("cellxgene_indptr")
+    cellxgene_indptr: torch.Tensor = StoredTorchInt64("cellxgene_indptr")
     """Index pointers for each cellxgene combination"""
 
-    regions = Linked("regions")
+    regions: pd.DataFrame = Linked("regions")
+    """Dataframe containing chromosome, start, end and strand of each region"""
 
     def create_cellxgene_indptr(self):
         cellxgene = self.mapping[:, 0] * self.n_genes + self.mapping[:, 1]
 
         if not (cellxgene.diff() >= 0).all():
             raise ValueError(
                 "Fragments should be ordered by cell then gene (ascending)"
@@ -134,19 +134,19 @@
         overwrite=True,
     ):
         """
         Create a Fragments object from a tsv file
 
         Parameters:
             fragments_file:
-                fragments_file of the tsv file
+                Location of the `fragments.tsv` file created by e.g. CellRanger or sinto
             path:
-                folder in which the fragments object will be created
+                Folder in which the fragments data will be stored
             regions:
-                regions object
+                Regions object
         """
 
         if isinstance(fragments_file, str):
             fragments_file = pathlib.Path(fragments_file)
         if isinstance(path, str):
             path = pathlib.Path(path)
         if not fragments_file.exists():
@@ -155,22 +155,18 @@
             raise FileExistsError(f"Folder {path} already exists")
         path.mkdir(parents=True, exist_ok=True)
 
         # region information
         var = pd.DataFrame(index=regions.coordinates.index)
         var["ix"] = np.arange(var.shape[0])
 
-        n_genes = var.shape[0]
-
         # cell information
         obs["ix"] = np.arange(obs.shape[0])
         cell_to_cell_ix = obs["ix"].to_dict()
 
-        n_cells = obs.shape[0]
-
         # load fragments tabix
         import pysam
 
         fragments_tabix = pysam.TabixFile(str(fragments_file))
 
         coordinates_raw = []
         mapping_raw = []
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/motifscan/motifscan.py` & `chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motifscan.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/motifscan/motiftrack.py` & `chromatinhd-0.0.19/src/chromatinhd/data/motifscan/motiftrack.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/regions.py` & `chromatinhd-0.0.19/src/chromatinhd/data/regions.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,25 @@
     coordinates = TSV("coordinates", columns=["chrom", "start", "end"])
     window = Stored("window")
 
     @classmethod
     def from_canonical_transcripts(
         cls, canonical_transcripts: pd.DataFrame, window: np.ndarray, path: pathlib.Path
     ):
+        """
+        Create regions from a Dataframe of canonical transcripts, using a specified window around each transcription start site.
+
+        Parameters:
+            canonical_transcripts:
+                Dataframe of canonical transcripts, with columns chrom, start, end, strand, ensembl_transcript_id
+            window:
+                Window around each transcription start site. Should be a 2-element array, e.g. [-10000, 10000]
+            path:
+                Folder in which the fragments data will be stored
+        """
         regions = canonical_transcripts[
             ["chrom", "start", "end", "ensembl_transcript_id"]
         ].copy()
 
         regions["tss"] = [
             genes_row["start"] if genes_row["strand"] == +1 else genes_row["end"]
             for _, genes_row in canonical_transcripts.loc[regions.index].iterrows()
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/data/transcriptome/transcriptome.py` & `chromatinhd-0.0.19/src/chromatinhd/data/transcriptome/transcriptome.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,40 +32,41 @@
 
     @obs.setter
     def obs(self, value):
         value.index.name = "cell"
         value.to_csv(self.path / "obs.tsv", sep="\t")
         self._obs = value
 
-    _adata = None
-
-    @property
-    def adata(self):
-        if self._adata is None:
-            self._adata = pickle.load((self.path / "adata.pkl").open("rb"))
-        return self._adata
-
-    @adata.setter
-    def adata(self, value):
-        pickle.dump(value, (self.path / "adata.pkl").open("wb"))
-        self._adata = value
+    adata = Stored("adata")
+    """
+    Anndata object containing the transcriptome data.
+    """
 
     def gene_id(self, symbol):
+        """
+        Get the gene id for a given gene symbol.
+        """
         assert all(pd.Series(symbol).isin(self.var["symbol"])), set(
             pd.Series(symbol)[~pd.Series(symbol).isin(self.var["symbol"])]
         )
         return self.var.reset_index("gene").set_index("symbol").loc[symbol]["gene"]
 
     def symbol(self, gene_id):
+        """
+        Get the gene symbol for a given gene ID (e.g. Ensembl ID)
+        """
         assert all(pd.Series(gene_id).isin(self.var.index)), set(
             pd.Series(gene_id)[~pd.Series(gene_id).isin(self.var.index)]
         )
         return self.var.loc[gene_id]["symbol"]
 
     def gene_ix(self, symbol):
+        """
+        Get the gene index for a given gene symbol.
+        """
         self.var["ix"] = np.arange(self.var.shape[0])
         assert all(pd.Series(symbol).isin(self.var["symbol"])), set(
             pd.Series(symbol)[~pd.Series(symbol).isin(self.var["symbol"])]
         )
         return self.var.reset_index("gene").set_index("symbol").loc[symbol]["ix"]
 
     def create_X(self):
@@ -75,37 +76,32 @@
 
             X_scipy = scipy.sparse.csr_matrix(X_scipy)
         X = sparse.COOMatrix.from_scipy_csr(X_scipy)
         X.populate_mapping()
 
         self.X = X
 
-    _X = None
-
-    @property
-    def X(self):
-        if self._X is None:
-            self._X = Unpickler((self.path / "X.pkl").open("rb")).load()
-        return self._X
-
-    @X.setter
-    def X(self, value):
-        pickle.dump(value, (self.path / "X.pkl").open("wb"))
-        self._X = value
+    X = Stored("X")
 
     @classmethod
     def from_adata(cls, adata, path):
+        """
+        Create a Transcriptome object from an AnnData object.
+        """
         transcriptome = cls(path=path)
         transcriptome.adata = adata
         transcriptome.layers["X"] = adata.X
         transcriptome.var = adata.var
         transcriptome.obs = adata.obs
         return transcriptome
 
     layers = StoredDict("layers", Stored)
+    """
+    Dictionary of layers, such as raw, normalized and imputed data.
+    """
 
 
 class ClusterTranscriptome(Flow):
     var = Stored("var")
     obs = Stored("obs")
     adata = Stored("adata")
     X = Stored("X")
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/embedding.py` & `chromatinhd-0.0.19/src/chromatinhd/embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import torch
 import numpy as np
 
 
 class EmbeddingTensor(torch.nn.Embedding):
     """
-    Simple wrapper around torch.nn.Embedding which allows an embedding of any dimensions
+    Simple wrapper around torch.nn.Embedding which allows an embedding of any number of dimensions instead of just 1
 
     The actual tensor underyling this embedding can be accessed using
     `x.weight`, although this will have dimensions [num_embeddings, prod(embedding_dims)]
 
     To get the underlying tensor in the correct dimensions, you can use
-    `x.get_full_weight()`, which will have dimensions [num_embeddings, *embedding_dims]
-
-    To set the value of this parameter, without tracking gradients, use `x.data`
+    `x.data`, which will have dimensions [num_embeddings, *embedding_dims]. This can also be used to set the value.
     """
 
     def __init__(self, num_embeddings, embedding_dims, *args, **kwargs):
         if not isinstance(embedding_dims, tuple):
             embedding_dims = tuple(embedding_dims)
         if len(embedding_dims) == 0:
             embedding_dim = 1
@@ -51,16 +49,18 @@
         """
         The data of the parameter in dimensions [num_embeddings, *embedding_dims]
         """
         return self.get_full_weight().data
 
     @data.setter
     def data(self, value):
-        assert value.shape == self.weight.shape
-        self.weight.data = value
+        if value.ndim == 2:
+            self.weight.data = value
+        else:
+            self.weight.data = value.reshape(self.weight.data.shape)
 
     @property
     def shape(self):
         """
         The shape of the parameter, i.e. [num_embeddings, *embedding_dims]
         """
         return (self.weight.shape[0], *self.embedding_dims)
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/flow.py` & `chromatinhd-0.0.19/src/chromatinhd/flow.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import copy
 import json
 import importlib
 import shutil
 
 
 class Flow:
+    """
+    A folder on disk that can contain other folders or objects
+    """
+
     path: pathlib.Path
     default_name = None
 
     def __init__(self, path=None, folder=None, name=None, reset=False):
         if path is None:
             if folder is None:
                 raise ValueError("Either path or folder must be specified")
@@ -54,28 +58,41 @@
         return self.path / ".flow"
 
     def __repr__(self):
         return f'{self.__class__.__name__}("{self.path}")'
 
     @classmethod
     def from_path(cls, path):
+        """
+        Load a previously created flow from disk
+        """
         info = json.load(open(path / ".flow"))
 
         # load class
         module = importlib.import_module(info["module"])
         cls = getattr(module, info["class"])
 
         return cls(path=path)
 
     def reset(self):
+        """
+        Remove all files in this flow
+        """
         shutil.rmtree(self.path)
         self.path.mkdir(parents=True, exist_ok=True)
 
+    def __getstate__(self):
+        raise TypeError("This class cannot be pickled.")
+
 
 class Linked:
+    """
+    A link to another flow on disk
+    """
+
     def __init__(self, name):
         self.name = name
 
     def __get__(self, obj, type=None):
         if obj is not None:
             name = "_" + self.name
             if not hasattr(obj, name):
@@ -101,14 +118,18 @@
             else:
                 path.unlink()
         path.symlink_to(value.path.resolve())
         setattr(obj, name, value)
 
 
 class Stored:
+    """
+    A python object that is stored on disk using pickle
+    """
+
     def __init__(self, name, default=None):
         self.name = name
         self.default = default
 
     def get_path(self, folder):
         return folder / (self.name + ".pkl")
 
@@ -129,14 +150,18 @@
     def __set__(self, obj, value):
         name = "_" + self.name
         pickle.dump(value, self.get_path(obj.path).open("wb"))
         setattr(obj, name, value)
 
 
 class StoredTorchInt64(Stored):
+    """
+    A pytorch int64 tensor stored on disk
+    """
+
     def __get__(self, obj, type=None):
         if obj is not None:
             name = "_" + self.name
             if not hasattr(obj, name):
                 x = pickle.load(self.get_path(obj.path).open("rb"))
                 if not x.dtype is torch.int64:
                     x = x.to(torch.int64)
@@ -149,14 +174,18 @@
         value = value.to(torch.int64).contiguous()
         name = "_" + self.name
         pickle.dump(value, self.get_path(obj.path).open("wb"))
         setattr(obj, name, value)
 
 
 class StoredTorchInt32(Stored):
+    """
+    A pytorch int64 tensor stored on disk
+    """
+
     def __get__(self, obj, type=None):
         if obj is not None:
             name = "_" + self.name
             if not hasattr(obj, name):
                 x = pickle.load(self.get_path(obj.path).open("rb"))
                 if not x.dtype is torch.int32:
                     x = x.to(torch.int32)
@@ -169,14 +198,18 @@
         value = value.to(torch.int32).contiguous()
         name = "_" + self.name
         pickle.dump(value, self.get_path(obj.path).open("wb"))
         setattr(obj, name, value)
 
 
 class StoredNumpyInt64(Stored):
+    """
+    A numpy int64 tensor stored on disk
+    """
+
     def __get__(self, obj, type=None):
         if obj is not None:
             name = "_" + self.name
             if not hasattr(obj, name):
                 x = pickle.load(self.get_path(obj.path).open("rb"))
                 if not x.dtype is np.int64:
                     x = x.astype(np.int64)
@@ -189,14 +222,18 @@
         value = np.ascontiguousarray(value.astype(np.int64))
         name = "_" + self.name
         pickle.dump(value, self.get_path(obj.path).open("wb"))
         setattr(obj, name, value)
 
 
 class CompressedNumpy(Stored):
+    """
+    A compressed numpy array stored on disk
+    """
+
     dtype = np.float64
 
     def __get__(self, obj, type=None):
         if obj is not None:
             name = "_" + self.name
             if not hasattr(obj, name):
                 x = pickle.load(
@@ -223,14 +260,18 @@
 
 
 class CompressedNumpyInt64(CompressedNumpy):
     dtype = np.int64
 
 
 class TSV(Stored):
+    """
+    A pandas object stored on disk in tsv format
+    """
+
     def __init__(self, name, columns=None):
         super().__init__(name)
         self.columns = columns
 
     def get_path(self, folder):
         return folder / (self.name + ".tsv")
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/grid/broken.py` & `chromatinhd-0.0.19/src/chromatinhd/grid/broken.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from chromatinhd.grid.grid import Grid, Panel
 import numpy as np
 import pandas as pd
 import matplotlib as mpl
 
 
 class Broken(Grid):
+    """
+    A grid build from distinct "regions" that are using the same coordinate space
+    """
+
     def __init__(self, regions, width, gap=1, height=0.5, *args, **kwargs):
         super().__init__(padding_width=gap, *args, **kwargs)
 
         regions["width"] = regions["end"] - regions["start"]
         regions["ix"] = np.arange(len(regions))
 
         assert width > gap * (len(regions) - 1), "Width is not enough to contain gaps"
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/grid/grid.py` & `chromatinhd-0.0.19/src/chromatinhd/grid/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 active_fig = None
 
 
 class Element:
+    """
+    A basic element in a figure with a (top-left) position and dimensions
+    """
+
     pos = None
     dim = None
 
     @property
     def width(self):
         return self.dim[0]
 
     @property
     def height(self):
         return self.dim[1]
 
-
 TITLE_HEIGHT = 0.3
-
-# AXIS_WIDTH = 0.2
-# AXIS_HEIGHT = 0.2
-
 AXIS_WIDTH = AXIS_HEIGHT = 0.0
 
-
 class Ax(Element):
     ax2 = None
     insets = None
 
     def __init__(self, dim=None, pos=(0.0, 0.0)):
         global active_fig
         self.ax = mpl.figure.Axes(active_fig, [0, 0, 1, 1])
@@ -138,14 +136,18 @@
         super().__init__(dim=dim)
         self.label = label
         self.ax.set_axis_off()
         self.ax.text(0.5, 0.5, label, ha="center", va="center", size="large")
 
 
 class Wrap(Element):
+    """
+    Grid-like layout with a fixed number of columns that will automatically wrap panels in the next row
+    """
+
     title = None
 
     def __init__(
         self,
         ncol=6,
         padding_width=0.5,
         padding_height=None,
@@ -276,14 +278,18 @@
         if self.title is not None:
             self.title.dim = (width, self.title.dim[1])
 
         self.dim = (width, height)
 
 
 class Grid(Element):
+    """
+    Grid layout with a fixed number of columns and rows
+    """
+
     title = None
 
     def __init__(
         self,
         nrow=1,
         ncol=1,
         padding_width=0.5,
@@ -444,28 +450,39 @@
         self[row, column] = el
         if padding is not None:
             self.paddings_width[column] = padding
         return el
 
 
 class _Figure(mpl.figure.Figure):
+    """
+    Figure but with panel support
+    """
+
     main: Panel
 
     def __init__(self, main: Panel, *args, **kwargs):
         self.main = main
         global active_fig
         active_fig = self
         super().__init__(*args, **kwargs)
 
     def plot(self):
+        """
+        Align all panels within the figure
+        """
+
         self.main.align()
         self.set_size_inches(*self.main.dim)
         self.main.position(self)
 
     def set_tight_bounds(self):
+        """
+        Sets the bounds of the figure so that all elements are visible
+        """
         new_bounds = self.get_tightbbox().extents
         current_size = self.get_size_inches()
         new_size = new_bounds[2] - new_bounds[0], new_bounds[3] - new_bounds[1]
 
         self.set_figwidth(new_bounds[2] - new_bounds[0])
         self.set_figheight(new_bounds[3] - new_bounds[1])
 
@@ -486,8 +503,11 @@
                     ]
                 ).reshape((2, 2))
             )
             ax.set_position(new_bbox)
 
 
 def Figure(main, *args, **kwargs):
+    """
+    Create a figure with panel support
+    """
     return plt.figure(*args, main=main, **kwargs, FigureClass=_Figure)
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/chunkfragments.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/chunkfragments.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/extraction/fragments.pyx` & `chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/fragments.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/extraction/motifs.pyx` & `chromatinhd-0.0.19/src/chromatinhd/loaders/extraction/motifs.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/fragmentmotif.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/fragmentmotif.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/fragments.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 import numpy as np
 import pyximport
+from typing import List
 
 pyximport.install(
     reload_support=True,
     language_level=3,
     setup_args=dict(include_dirs=[np.get_include()]),
 )
 import chromatinhd.data.fragments
@@ -199,15 +200,15 @@
             n_total_genes=self.n_genes,
             **minibatch.items(),
         )
 
 
 @dataclasses.dataclass
 class FragmentsCountingResult(FragmentsResult):
-    n: list[torch.Tensor]
+    n: List[torch.Tensor]
 
 
 class FragmentsCounting:
     cellxgene_batch_size: int
 
     preloaded = False
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/minibatching.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/minibatching.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/peakcounts.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/peakcounts.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loaders/pool.py` & `chromatinhd-0.0.19/src/chromatinhd/loaders/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import copy
 import threading
 import numpy as np
 import time
+from typing import List
 
 
 class ThreadWithResult(threading.Thread):
     result = None
 
     def __init__(
         self,
         group=None,
         target=None,
         name=None,
         loader=None,
         args=(),
         kwargs={},
         *,
-        daemon=None
+        daemon=None,
     ):
         assert target is not None
         self.loader = loader
 
         def function():
             self.result = target(*args, **kwargs)
 
         super().__init__(group=group, target=function, name=name, daemon=daemon)
 
 
 class LoaderPool:
     tasks: list
     next_task_sets: list
     loaders_available: list
-    n_todo: list[int]
+    n_todo: List[int]
     shuffle_on_iter = False
 
     def __init__(
         self,
         loader_cls,
         loader_kwargs=None,
         n_workers=3,
@@ -191,15 +192,15 @@
 
     def __del__(self):
         self.terminate()
 
 
 class LoaderPool2:
     loaders_available: list
-    n_todo: list[int]
+    n_todo: List[int]
     shuffle_on_iter = False
 
     def __init__(
         self,
         loader_cls,
         loader_kwargs=None,
         n_workers=3,
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/loss.py` & `chromatinhd-0.0.19/src/chromatinhd/loss.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/__init__.py` & `chromatinhd-0.0.19/src/chromatinhd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/differential.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/differential.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/enrichment/enrichment.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/enrichment/enrichment.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/interpret/genepositional.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/interpret/genepositional.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/clustering.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/clustering_cuts.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/clustering_cuts.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/cuts.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/cuts.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/fragments_helpers.pyx` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/fragments_helpers.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/loader/minibatches.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/loader/minibatches.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/model/cutnf.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/cutnf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import torch
-import numpy as np
 import math
-import tqdm.auto as tqdm
+import pickle
+
+import numpy as np
+import torch
 import torch_scatter
+import tqdm.auto as tqdm
+import xarray as xr
+import pandas as pd
 
 from chromatinhd.embedding import EmbeddingTensor
-from . import spline
-from chromatinhd.models import HybridModel
-
 from chromatinhd.flow import Flow, Stored
-
+from chromatinhd.loaders import LoaderPool2
+from chromatinhd.models import HybridModel
+from chromatinhd.models.diff.loader.clustering_cuts import ClusteringCuts
 from chromatinhd.models.diff.loader.minibatches import Minibatcher
-from chromatinhd.models.diff.loader.clustering_cuts import (
-    ClusteringCuts,
-)
 from chromatinhd.models.diff.trainer import Trainer
-from chromatinhd.loaders import LoaderPool2
 from chromatinhd.optim import SparseDenseAdam
-
-import pickle
+from chromatinhd import default_device
+from chromatinhd.data.fragments import Fragments
+from chromatinhd.data.clustering import Clustering
+from chromatinhd.utils import crossing
+from .spline import DifferentialQuadraticSplineStack, TransformedDistribution
 
 
 class Decoder(torch.nn.Module):
     def __init__(
         self,
         n_latent,
         n_genes,
@@ -132,14 +134,18 @@
         return [*self.nn.parameters()]
 
     def parameters_sparse(self):
         return [self.rho_weight.weight]
 
 
 class Model(torch.nn.Module, HybridModel):
+    """
+    A ChromatinHD-diff model that models the probability density of observing a cut site between clusterings
+    """
+
     def __init__(
         self,
         fragments,
         clustering,
         nbins=(
             128,
             64,
@@ -155,16 +161,14 @@
     ):
         super().__init__()
 
         self.n_total_genes = fragments.n_genes
 
         self.n_clusters = clustering.n_clusters
 
-        from .spline import DifferentialQuadraticSplineStack, TransformedDistribution
-
         transform = DifferentialQuadraticSplineStack(
             nbins=nbins,
             n_genes=fragments.n_genes,
         )
         self.mixture = TransformedDistribution(transform)
         n_delta_mixture_components = sum(transform.split_deltas)
 
@@ -278,15 +282,21 @@
             clustering=data.clustering.onehot,
             genes_oi=data.minibatch.genes_oi_torch,
             local_gene_ix=data.cuts.local_gene_ix,
             local_cellxgene_ix=data.cuts.local_cellxgene_ix,
             localcellxgene_ix=data.cuts.localcellxgene_ix,
         )
 
-    def train_model(self, fragments, clustering, fold, device="cuda", n_epochs=30):
+    def train_model(
+        self, fragments, clustering, fold, device=default_device, n_epochs=30
+    ):
+        """
+        Trains the model
+        """
+
         # set up minibatchers and loaders
         minibatcher_train = Minibatcher(
             fold["cells_train"],
             range(fragments.n_genes),
             n_genes_step=500,
             n_cells_step=200,
         )
@@ -343,25 +353,33 @@
     ):
         return torch_scatter.segment_sum_coo(
             likelihood, local_cellxgene_ix, dim_size=n_cells * n_genes
         ).reshape((n_cells, n_genes))
 
     def get_prediction(
         self,
-        fragments,
-        clustering,
+        fragments: Fragments,
+        clustering: Clustering,
         cells=None,
         cell_ixs=None,
         genes=None,
         gene_ixs=None,
-        device="cuda",
-        return_raw=False,
+        device: str = default_device,
     ):
         """
         Returns the prediction of a dataset
+
+        Parameters:
+            fragments: Fragments object
+            clustering: Clustering object
+            cells: Cells to predict
+            cell_ixs: Cell indices to predict
+            genes: Genes to predict
+            gene_ixs: Gene indices to predict
+            device: Device to use
         """
         if cell_ixs is None:
             if cells is None:
                 cells = fragments.obs.index
             fragments.obs["ix"] = np.arange(len(fragments.obs))
             cell_ixs = fragments.obs.loc[cells]["ix"].values
         if cells is None:
@@ -443,19 +461,14 @@
                 )
                 .cpu()
                 .numpy()
             )
 
         self = self.to("cpu")
 
-        if return_raw:
-            return predicted, expected, n_fragments
-
-        import xarray as xr
-
         result = xr.Dataset(
             {
                 "likelihood_mixture": xr.DataArray(
                     likelihood_mixture,
                     dims=("cell", "gene"),
                     coords={"cell": cells, "gene": fragments.var.index},
                 ),
@@ -465,20 +478,20 @@
                     coords={"cell": cells, "gene": fragments.var.index},
                 ),
             }
         )
         return result
 
     def evaluate_pseudo(self, coordinates, clustering=None, gene_oi=None, gene_ix=None):
-        from chromatinhd.models.diff.loader.cuts import Result as CutsResult
-        from chromatinhd.models.diff.loader.minibatches import Minibatch
         from chromatinhd.models.diff.loader.clustering import Result as ClusteringResult
         from chromatinhd.models.diff.loader.clustering_cuts import (
             Result as ClusteringCutsResult,
         )
+        from chromatinhd.models.diff.loader.cuts import Result as CutsResult
+        from chromatinhd.models.diff.loader.minibatches import Minibatch
 
         device = coordinates.device
         if not torch.is_tensor(clustering):
             if clustering is None:
                 clustering = 0.0
             clustering = torch.ones((1, self.n_clusters), device=device) * clustering
 
@@ -540,17 +553,14 @@
         n_latent: int,
         device: torch.DeviceObjType = "cuda",
         how: str = "probs_diff_masked",
         prob_cutoff: float = None,
     ) -> np.ndarray:
         n_genes = self.rho_bias.shape[0]
 
-        import pandas as pd
-        from chromatinhd.utils import crossing
-
         self = self.to(device).eval()
 
         # create design for inference
         design_gene = pd.DataFrame({"gene_ix": np.arange(n_genes)})
         design_latent = pd.DataFrame({"active_latent": np.arange(n_latent)})
         design_coord = pd.DataFrame(
             {"coord": np.arange(window[0], window[1] + 1, step=25)}
@@ -647,14 +657,21 @@
         path = self.path / "models"
         path.mkdir(exist_ok=True)
         return path
 
     def train_models(
         self, fragments, clustering, folds, device="cuda", n_epochs=30, **kwargs
     ):
+        """
+        Trains the models
+
+        Parameters:
+            fragments:
+                Fragments object
+        """
         self.n_models = len(folds)
         for fold_ix, fold in [(fold_ix, fold) for fold_ix, fold in enumerate(folds)]:
             desired_outputs = [self.models_path / ("model_" + str(fold_ix) + ".pkl")]
             force = False
             if not all([desired_output.exists() for desired_output in desired_outputs]):
                 force = True
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/model/spline.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/spline.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/cubic.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/cubic.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/linear.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/linear.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/model/splines/quadratic.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/model/splines/quadratic.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/__init__.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/differential.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/plot/differential_expression.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/plot/differential_expression.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/diff/trainer/trainer.py` & `chromatinhd-0.0.19/src/chromatinhd/models/diff/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/censorers.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/censorers.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/genemultiwindow.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genemultiwindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,27 @@
     fdr = p_vals * len(p_vals) / ranked_p_values
     fdr[fdr > 1] = 1
 
     return fdr
 
 
 class GeneMultiWindow(chd.flow.Flow):
+    """
+    Interpret a *pred* model positionally by censoring windows of across multiple window sizes.
+    """
+
     design = chd.flow.Stored("design")
+    """
+    The design of the censoring windows.
+    """
 
     genes = chd.flow.Stored("genes", default=set)
+    """
+    The genes that have been scored.
+    """
 
     def score(
         self,
         fragments,
         transcriptome,
         models,
         folds,
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/interpret/genepairwindow.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/interpret/genepairwindow.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/fragments.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/fragments_helpers.pyx` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/fragments_helpers.pyx`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/transcriptome.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/loader/transcriptome_fragments.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/loader/transcriptome_fragments.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/model/additive.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/model/additive.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,15 @@
 from chromatinhd.models.pred.loader.transcriptome_fragments import (
     TranscriptomeFragments,
 )
 from chromatinhd.models.pred.trainer import Trainer
 from chromatinhd.loaders import LoaderPool2
 from chromatinhd.optim import SparseDenseAdam
 
-
-def paircor(x, y, dim=0, eps=0.1):
-    divisor = (y.std(dim) * x.std(dim)) + eps
-    cor = ((x - x.mean(dim, keepdims=True)) * (y - y.mean(dim, keepdims=True))).mean(
-        dim
-    ) / divisor
-    return cor
-
-
-def paircor_loss(x, y):
-    return -paircor(x, y).mean() * 100
-
-
-def gene_paircor_loss(x, y):
-    return -paircor(x, y) * 100
+from .loss import paircor, paircor_loss, gene_paircor_loss
 
 
 class SineEncoding(torch.nn.Module):
     def __init__(self, n_frequencies):
         super().__init__()
 
         self.register_buffer(
@@ -76,17 +62,16 @@
     def __init__(
         self,
         n_genes,
         n_frequencies=10,
         n_embedding_dimensions=5,
         nonlinear=True,
         dropout_rate=0.0,
-        **kwargs
+        **kwargs,
     ):
-
         self.n_embedding_dimensions = n_embedding_dimensions
 
         self.nonlinear = nonlinear
         self.dropout_rate = dropout_rate
 
         super().__init__(**kwargs)
 
@@ -229,15 +214,15 @@
         dummy=False,
         n_frequencies=50,
         reduce="sum",
         nonlinear=True,
         n_embedding_dimensions=10,
         dropout_rate=0.0,
         embedding_to_expression_initialization="default",
-        **kwargs
+        **kwargs,
     ):
         super().__init__()
 
         if dummy:
             self.fragment_embedder = FragmentEmbedderCounter()
         else:
             self.fragment_embedder = FragmentEmbedder(
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/copredictivity.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/copredictivity.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import chromatinhd.plot
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 class Copredictivity(chromatinhd.grid.Panel):
+    """
+    Plot co-predictivity of a gene.
+    """
+
     def __init__(self, plotdata, width):
         super().__init__((width, width / 2))
 
         norm = mpl.colors.CenteredNorm(0, np.abs(plotdata["cor"]).max())
         cmap = mpl.cm.RdBu_r
 
         chromatinhd.plot.matshow45(
@@ -36,9 +40,12 @@
             va="center",
         )
         panel_copredictivity_legend.ax.yaxis.set_ticks_position("left")
         panel_copredictivity_legend.ax.yaxis.set_label_position("left")
 
     @classmethod
     def from_genepairwindow(cls, genepairwindow, gene, width):
+        """
+        Plot co-predictivity of a gene using a GenePairWindow object.
+        """
         plotdata = genepairwindow.get_plotdata(gene).reset_index()
         return cls(plotdata, width)
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/effect.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/effect.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/plot/predictivity.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/plot/predictivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import chromatinhd.grid
 import matplotlib as mpl
 from chromatinhd.grid.broken import Broken, Panel
 import numpy as np
 
 
 class Predictivity(chromatinhd.grid.Panel):
+    """
+    Plot predictivity of a gene.
+    """
+
     def __init__(self, plotdata, window, width, show_accessibility=False):
         super().__init__((width, 0.5))
 
         plotdata["effect_sign"] = np.sign(plotdata["effect"])
         plotdata["segment"] = plotdata["effect_sign"].diff().ne(0).cumsum()
 
         ax = self.ax
@@ -97,14 +101,17 @@
         # vline at tss
         ax.axvline(0, color="#888888", lw=0.5, zorder=-1, dashes=(2, 2))
 
     @classmethod
     def from_genemultiwindow(
         cls, genemultiwindow, gene, width, show_accessibility=False
     ):
+        """
+        Plot predictivity of a specific gene using a GeneMultiWindow object
+        """
         plotdata = genemultiwindow.get_plotdata(gene).reset_index()
         window = np.array([plotdata["position"].min(), plotdata["position"].max()])
         return cls(plotdata, window, width, show_accessibility=show_accessibility)
 
 
 class Pileup(chromatinhd.grid.Panel):
     def __init__(self, plotdata, window, width):
@@ -143,14 +150,17 @@
         ax.axvline(0, color="#888888", lw=0.5, zorder=-1, dashes=(2, 2))
 
         ax.set_xticks([])
         ax.set_ylim(0)
 
     @classmethod
     def from_genemultiwindow(cls, genemultiwindow, gene, width):
+        """
+        Plot pileup of a specific gene using a GeneMultiWindow object
+        """
         plotdata = genemultiwindow.get_plotdata(gene).reset_index()
         window = np.array([plotdata["position"].min(), plotdata["position"].max()])
         return cls(plotdata, window, width)
 
 
 class PredictivityBroken(Broken):
     def __init__(
@@ -163,15 +173,15 @@
             gap=gap,
             *args,
             **kwargs,
         )
 
         ylim = plotdata["deltacor"].min() * 1.05
 
-        for ((region, region_info), (panel, ax)) in zip(
+        for (region, region_info), (panel, ax) in zip(
             regions.iterrows(), self.elements[0]
         ):
             plotdata_region = plotdata[
                 (plotdata["position"] >= region_info["start"])
                 & (plotdata["position"] <= region_info["end"])
             ]
 
@@ -207,15 +217,15 @@
 
 class LabelBroken(Broken):
     def __init__(self, regions, *args, **kwargs):
         super().__init__(regions=regions, height=0.00001, *args, **kwargs)
 
         assert len(self.elements[0]) == len(regions)
 
-        for ((region, region_info), (panel, ax)) in zip(
+        for (region, region_info), (panel, ax) in zip(
             regions.iterrows(), self.elements[0]
         ):
             ax.set_xlim(region_info["start"], region_info["end"])
             ax.set_xticks([])
             ax.set_ylim(0, 0.1)
             ax.set_yticks([])
             ax.spines.left.set_visible(False)
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/models/pred/trainer/trainer.py` & `chromatinhd-0.0.19/src/chromatinhd/models/pred/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/optim.py` & `chromatinhd-0.0.19/src/chromatinhd/optim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 
 import torch
 class SparseDenseAdam(torch.optim.Optimizer):
+    """
+    Optimize both sparse and densre parameters using ADAM
+    """
     def __init__(self, parameters_sparse, parameters_dense, lr = 1e-3, weight_decay = 0., **kwargs):
         if len(parameters_sparse) == 0:
             self.optimizer_sparse = None
         else:
             self.optimizer_sparse = torch.optim.SparseAdam(
                 parameters_sparse,
                 lr = lr,
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/peakcounts.py` & `chromatinhd-0.0.19/src/chromatinhd/data/peakcounts/peakcounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 import pandas as pd
 
 import scanpy as sc
 
 import collections
 import subprocess as sp
 import tqdm.auto as tqdm
-import pathlib
 import pickle
 
 from chromatinhd.flow import Flow
 
-htslib_folder = pathlib.Path("/data/peak_free_atac/software/htslib-1.16/")
-tabix_location = htslib_folder / "tabix"
-
 
 class PeakCounts(Flow):
     def create_adata(self, original_adata):
         adata = sc.AnnData(self.counts, obs=self.obs, var=self.var)
         adata.obsm["X_umap"] = original_adata.obsm["X_umap"]
         self.adata = adata
 
-    def count_peaks(self, fragments_location, cell_ids):
+    def count_peaks(self, fragments_location, cell_ids, tabix_location="tabix"):
         # extract unique peaks
         peaks = self.peaks
         unique_peak_ids = list(set(peaks["peak"]))
         peak_idxs = {peak_id: i for i, peak_id in enumerate(unique_peak_ids)}
 
         # create peaks file for tabix
         self.peaks_bed = peaks[["chrom", "start", "end"]]
@@ -281,15 +277,15 @@
 
         self.peaks = peaks
 
 
 class FragmentPeak(FullPeak):
     default_name = "fragment_peak"
 
-    def count_peaks(self, fragments_location, cell_ids):
+    def count_peaks(self, fragments_location, cell_ids, tabix_location="tabix"):
         # add ix to peaks
         peaks = self.peaks
         peaks["ix"] = np.arange(peaks.shape[0])
 
         # create peaks file for tabix
         peaks_bed = peaks[["chrom", "start", "end"]]
         self.peaks_bed = peaks_bed
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/plot/genome/genes.py` & `chromatinhd-0.0.19/src/chromatinhd/plot/genome/genes.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/plot/matshow45.py` & `chromatinhd-0.0.19/src/chromatinhd/plot/matshow45.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/plot/patch.py` & `chromatinhd-0.0.19/src/chromatinhd/plot/patch.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/plot/quasirandom.py` & `chromatinhd-0.0.19/src/chromatinhd/plot/quasirandom.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/plot/tickers.py` & `chromatinhd-0.0.19/src/chromatinhd/plot/tickers.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/sparse.py` & `chromatinhd-0.0.19/src/chromatinhd/sparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 @dataclass
 class COOMatrix(Sparse):
     """
     COOMatrix sparse matrix
 
-    This implementation mainly cachges the row_switch and mapping dictionaries, which speed up subsampling in the first (row) dimension
+    Additional CSR-like data can be stored to speed up subsampling
     """
 
     row: torch.tensor
     col: torch.tensor
     values: torch.tensor
     shape: torch.Size
     row_switch = None
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd/train.py` & `chromatinhd-0.0.19/src/chromatinhd/train.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/utils/__init__.py` & `chromatinhd-0.0.19/src/chromatinhd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/utils/ansi.py` & `chromatinhd-0.0.19/src/chromatinhd/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/utils/ecdf.py` & `chromatinhd-0.0.19/src/chromatinhd/utils/ecdf.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/utils/testing.py` & `chromatinhd-0.0.19/src/chromatinhd/utils/testing.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/src/chromatinhd/utils/torch.py` & `chromatinhd-0.0.19/src/chromatinhd/utils/torch.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,21 +19,18 @@
 
     indices = torch.searchsorted(xp.contiguous(), x.contiguous(), right=False) - 1
     indices = torch.clamp(indices, 0, a.shape[-1] - 1)
 
     return b.index_select(a.ndim - 1, indices)
 
 
-def indices_to_indptr(x, n):
+def indices_to_indptr(x:torch.Tensor, n:int) -> torch.Tensor:
     return torch.nn.functional.pad(
         torch.cumsum(torch.bincount(x, minlength=n), 0), (1, 0)
     )
 
+ind2ptr = indices_to_indptr
 
-def ind2ptr(x, minlength):
-    return torch.nn.functional.pad(
-        torch.cumsum(torch.bincount(x, minlength=minlength), 0), (1, 0)
-    )
-
-
-def ptr2ind(x):
+def indptr_to_indices(x:torch.Tensor) -> torch.Tensor:
     return torch.repeat_interleave(torch.arange(len(x) - 1), torch.diff(x))
+
+ptr2ind = indptr_to_indices
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd.egg-info/PKG-INFO` & `chromatinhd-0.0.19/src/chromatinhd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromatinhd
-Version: 0.0.18
+Version: 0.0.19
 Summary: High-definition modeling of (single-cell) chromatin + transcriptomics data
 Author-email: Wouter Saelens <wouter.saelens@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/DeplanckeLab/ChromatinHD
 Project-URL: Bug Tracker, https://github.com/DeplanckeLab/ChromatinHD/issues
 Keywords: bioinformatics,chromatin accessibility,transcriptomics
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.18 Summary: High-
+Metadata-Version: 2.1 Name: chromatinhd Version: 0.0.19 Summary: High-
 definition modeling of (single-cell) chromatin + transcriptomics data Author-
 email: Wouter Saelens
 saelens@gmail.com> License: MIT Project-URL: Homepage, https://github.com/
 DeplanckeLab/ChromatinHD Project-URL: Bug Tracker, https://github.com/
 DeplanckeLab/ChromatinHD/issues Keywords: bioinformatics,chromatin
 accessibility,transcriptomics Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `chromatinhd-0.0.18/src/chromatinhd.egg-info/SOURCES.txt` & `chromatinhd-0.0.19/src/chromatinhd.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE.md
 README.md
-_setup.py
 mkdocs.yml
 pyproject.toml
 .github/workflows/ci.yml
 docs/override/main.html
 docs/source/index.md
 docs/source/index.py
 docs/source/jupytext.toml
 docs/source/quickstart/0_install.py
 docs/source/quickstart/1_data.py
 docs/source/quickstart/2_pred.py
 docs/source/quickstart/3_diff.py
-docs/source/reference/data.md
 docs/source/reference/index.md
+docs/source/reference/data/clustering.md
+docs/source/reference/data/fragments.md
+docs/source/reference/data/regions.md
+docs/source/reference/data/transcriptome.md
+docs/source/reference/models/pred/plot.md
 docs/source/static/favicon.ai
 docs/source/static/favicon.png
 docs/source/static/logo.ai
 docs/source/static/logo.png
 docs/source/static/models/diff/logo.pdf
 docs/source/static/models/diff/1x/logo.png
 docs/source/static/models/dime/logo.pdf
 docs/source/static/models/dime/logo.png
 docs/source/static/models/pred/logo.pdf
 docs/source/static/models/pred/1x/logo.png
 docs/source/static/models/time/logo.pdf
 docs/source/static/models/time/logo.png
+docs/source/stylesheets/extra-reference.css
 docs/source/stylesheets/extra.css
 scripts/build.sh
 scripts/setup_data_tiny.py
 scripts/test.py
 src/chromatinhd/__init__.py
+src/chromatinhd/device.py
 src/chromatinhd/embedding.py
 src/chromatinhd/flow.py
 src/chromatinhd/loss.py
 src/chromatinhd/optim.py
-src/chromatinhd/peakcounts.py
 src/chromatinhd/sparse.py
 src/chromatinhd/train.py
 src/chromatinhd.egg-info/PKG-INFO
 src/chromatinhd.egg-info/SOURCES.txt
 src/chromatinhd.egg-info/dependency_links.txt
 src/chromatinhd.egg-info/requires.txt
 src/chromatinhd.egg-info/top_level.txt
@@ -61,14 +65,16 @@
 src/chromatinhd/data/fragments/__init__.py
 src/chromatinhd/data/fragments/fragments.py
 src/chromatinhd/data/genotype/__init__.py
 src/chromatinhd/data/genotype/genotype.py
 src/chromatinhd/data/motifscan/__init__.py
 src/chromatinhd/data/motifscan/motifscan.py
 src/chromatinhd/data/motifscan/motiftrack.py
+src/chromatinhd/data/peakcounts/__init__.py
+src/chromatinhd/data/peakcounts/peakcounts.py
 src/chromatinhd/data/transcriptome/__init__.py
 src/chromatinhd/data/transcriptome/transcriptome.py
 src/chromatinhd/grid/__init__.py
 src/chromatinhd/grid/broken.py
 src/chromatinhd/grid/grid.py
 src/chromatinhd/loaders/__init__.py
 src/chromatinhd/loaders/chunkfragments.py
@@ -108,22 +114,23 @@
 src/chromatinhd/models/pred/__init__.py
 src/chromatinhd/models/pred/interpret/__init__.py
 src/chromatinhd/models/pred/interpret/censorers.py
 src/chromatinhd/models/pred/interpret/filter.py
 src/chromatinhd/models/pred/interpret/genemultiwindow.py
 src/chromatinhd/models/pred/interpret/genepairwindow.py
 src/chromatinhd/models/pred/loader/__init__.py
-src/chromatinhd/models/pred/loader/cuts.py
 src/chromatinhd/models/pred/loader/fragments.py
 src/chromatinhd/models/pred/loader/fragments_helpers.pyx
 src/chromatinhd/models/pred/loader/minibatches.py
 src/chromatinhd/models/pred/loader/transcriptome.py
 src/chromatinhd/models/pred/loader/transcriptome_fragments.py
 src/chromatinhd/models/pred/model/__init__.py
+src/chromatinhd/models/pred/model/across.py
 src/chromatinhd/models/pred/model/additive.py
+src/chromatinhd/models/pred/model/loss.py
 src/chromatinhd/models/pred/plot/__init__.py
 src/chromatinhd/models/pred/plot/copredictivity.py
 src/chromatinhd/models/pred/plot/effect.py
 src/chromatinhd/models/pred/plot/predictivity.py
 src/chromatinhd/models/pred/trainer/__init__.py
 src/chromatinhd/models/pred/trainer/trainer.py
 src/chromatinhd/plot/__init__.py
@@ -137,11 +144,13 @@
 src/chromatinhd/utils/ansi.py
 src/chromatinhd/utils/ecdf.py
 src/chromatinhd/utils/numpy.py
 src/chromatinhd/utils/testing.py
 src/chromatinhd/utils/torch.py
 tests/conftest.py
 tests/test_loss.py
+tests/biomart/conftest.py
+tests/biomart/tss_test.py
 tests/models/diff/loader/test_clustering_cuts.py
 tests/models/diff/model/test_cutnf.py
 tests/models/pred/loader/test_transcriptome_fragments.py
 tests/models/pred/model/test_additive.py
```

### Comparing `chromatinhd-0.0.18/tests/conftest.py` & `chromatinhd-0.0.19/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chromatinhd-0.0.18/tests/models/pred/loader/test_transcriptome_fragments.py` & `chromatinhd-0.0.19/tests/models/pred/loader/test_transcriptome_fragments.py`

 * *Files identical despite different names*

