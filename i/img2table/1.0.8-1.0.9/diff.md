# Comparing `tmp/img2table-1.0.8.tar.gz` & `tmp/img2table-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-1.0.8.tar", last modified: Mon Jul 31 11:14:16 2023, max compression
+gzip compressed data, was "img2table-1.0.9.tar", last modified: Thu Aug  3 11:42:23 2023, max compression
```

## Comparing `img2table-1.0.8.tar` & `img2table-1.0.9.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 11:12:00.000000 img2table-1.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 11:12:00.000000 img2table-1.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 11:12:00.000000 img2table-1.0.8/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 11:12:00.000000 img2table-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-31 11:12:00.000000 img2table-1.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-07-31 11:14:16.000000 img2table-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-31 11:12:00.000000 img2table-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 11:12:00.000000 img2table-1.0.8/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/examples/data/borderless/
--rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/borderless/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/borderless/2.png
--rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/borderless/3.png
--rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/borderless/4.png
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/borderless.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-31 11:12:00.000000 img2table-1.0.8/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 11:12:00.000000 img2table-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 11:12:00.000000 img2table-1.0.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 11:12:00.000000 img2table-1.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 11:12:00.000000 img2table-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-31 11:14:16.000000 img2table-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 11:12:00.000000 img2table-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/easyocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/coherency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-31 11:12:00.000000 img2table-1.0.8/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 11:14:16.000000 img2table-1.0.8/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/easyocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/easyocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/easyocr/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/easyocr/test_data/ocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/easyocr/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/easyocr/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/easyocr/test_easyocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)  3446838 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_coherency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_rows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:14:16.000000 img2table-1.0.8/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-31 11:12:00.000000 img2table-1.0.8/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.922782 img2table-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.786770 img2table-1.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-03 11:39:26.000000 img2table-1.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.786770 img2table-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-03 11:39:26.000000 img2table-1.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 11:39:26.000000 img2table-1.0.9/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 11:39:26.000000 img2table-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 11:39:26.000000 img2table-1.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-08-03 11:42:23.922782 img2table-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-08-03 11:39:26.000000 img2table-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-03 11:39:26.000000 img2table-1.0.9/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.790770 img2table-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.798771 img2table-1.0.9/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.802771 img2table-1.0.9/examples/data/borderless/
+-rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/borderless/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/borderless/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/borderless/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/borderless/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/borderless.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 11:39:26.000000 img2table-1.0.9/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 11:39:26.000000 img2table-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 11:39:26.000000 img2table-1.0.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-03 11:39:26.000000 img2table-1.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 11:39:26.000000 img2table-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-03 11:42:23.922782 img2table-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-03 11:39:26.000000 img2table-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.766768 img2table-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.802771 img2table-1.0.9/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.806771 img2table-1.0.9/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.806771 img2table-1.0.9/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.814772 img2table-1.0.9/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.814772 img2table-1.0.9/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.818772 img2table-1.0.9/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.818772 img2table-1.0.9/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.818772 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.822773 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.822773 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.826773 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.826773 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.830773 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.830773 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.830773 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.834774 img2table-1.0.9/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 11:39:26.000000 img2table-1.0.9/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.806771 img2table-1.0.9/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 11:42:23.000000 img2table-1.0.9/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.834774 img2table-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.838774 img2table-1.0.9/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.838774 img2table-1.0.9/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.838774 img2table-1.0.9/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.838774 img2table-1.0.9/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.842774 img2table-1.0.9/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.842774 img2table-1.0.9/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.846775 img2table-1.0.9/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.850775 img2table-1.0.9/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.850775 img2table-1.0.9/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.850775 img2table-1.0.9/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.854776 img2table-1.0.9/tests/ocr/easyocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/easyocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.854776 img2table-1.0.9/tests/ocr/easyocr/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/easyocr/test_data/ocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/easyocr/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/easyocr/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/easyocr/test_easyocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.854776 img2table-1.0.9/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.858776 img2table-1.0.9/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.858776 img2table-1.0.9/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.858776 img2table-1.0.9/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.858776 img2table-1.0.9/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.862776 img2table-1.0.9/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.862776 img2table-1.0.9/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.866777 img2table-1.0.9/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.866777 img2table-1.0.9/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.866777 img2table-1.0.9/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.866777 img2table-1.0.9/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.870777 img2table-1.0.9/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.870777 img2table-1.0.9/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.870777 img2table-1.0.9/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.870777 img2table-1.0.9/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.874777 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.878778 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.878778 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.878778 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.882778 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.886778 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.886778 img2table-1.0.9/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.886778 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.886778 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.890779 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.890779 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.894779 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.894779 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3446838 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.910781 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_coherency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.914781 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.914781 img2table-1.0.9/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.918781 img2table-1.0.9/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:42:23.922782 img2table-1.0.9/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-03 11:39:26.000000 img2table-1.0.9/tests/tables/processing/text/test_titles.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `img2table-1.0.8/LICENSE.txt` & `img2table-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/Makefile` & `img2table-1.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/PKG-INFO` & `img2table-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.8
+Version: 1.0.9
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -198,16 +198,14 @@
         
         ```bash
         # Example of installation with CUDA 11.8
         pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
         pip install paddleocr img2table
         ```
         
-        
-        *Released in version 0.0.13*
         <br>
         </details>
         
         
         <details>
         <summary>EasyOCR<a name="easyocr"></a></summary>
         <br>
@@ -223,15 +221,14 @@
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : list, optional, default <code>["en"]</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
         ></dl>
         
-        *Released in version 0.1.2*
         <br>
         </details>
         
         <details>
         <summary>Google Vision<a name="vision"></a></summary>
         <br>
         
@@ -333,15 +330,15 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
         >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
-        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
+        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted <b>on top of</b> bordered tables.</dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
         <b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
         
         *Borderless table extraction released in version 0.0.14*
@@ -457,14 +454,14 @@
         </ul>
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.12
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
 Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.8 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.9 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -81,23 +81,23 @@
 >
 >
 
 NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
 gpu has to be installed by the user manually as stated in this issue. ```bash #
 Example of installation with CUDA 11.8 pip install paddlepaddle-
 gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
-stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
+stable.html pip install paddleocr img2table ```
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.1.2*
+
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
@@ -180,10 +180,10 @@
       background. Effectiveness can not be guaranteed on other type of
       documents.
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
+:: OS Independent Requires-Python: >=3.8, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
 Provides-Extra: paddle Provides-Extra: easyocr
```

### Comparing `img2table-1.0.8/README.md` & `img2table-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,14 @@
 
 ```bash
 # Example of installation with CUDA 11.8
 pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
 pip install paddleocr img2table
 ```
 
-
-*Released in version 0.0.13*
 <br>
 </details>
 
 
 <details>
 <summary>EasyOCR<a name="easyocr"></a></summary>
 <br>
@@ -216,15 +214,14 @@
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>lang : list, optional, default <code>["en"]</code></dt>
 >    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
 ></dl>
 
-*Released in version 0.1.2*
 <br>
 </details>
 
 <details>
 <summary>Google Vision<a name="vision"></a></summary>
 <br>
 
@@ -326,15 +323,15 @@
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
 >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
 >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
->    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
+>    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted <b>on top of</b> bordered tables.</dd>
 >    <dt>min_confidence : int, optional, default <code>50</code></dt>
 >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
 ></dl>
 
 <b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
 
 *Borderless table extraction released in version 0.0.14*
```

#### html2text {}

```diff
@@ -77,23 +77,23 @@
 >
 >
 
 NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
 gpu has to be installed by the user manually as stated in this issue. ```bash #
 Example of installation with CUDA 11.8 pip install paddlepaddle-
 gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
-stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
+stable.html pip install paddleocr img2table ```
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.1.2*
+
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
```

### Comparing `img2table-1.0.8/examples/Basic_usage.ipynb` & `img2table-1.0.9/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/Implicit_rows.ipynb` & `img2table-1.0.9/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/borderless.ipynb` & `img2table-1.0.9/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/borderless/1.png` & `img2table-1.0.9/examples/data/borderless/1.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/borderless/2.png` & `img2table-1.0.9/examples/data/borderless/2.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/borderless/3.png` & `img2table-1.0.9/examples/data/borderless/3.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/borderless/4.png` & `img2table-1.0.9/examples/data/borderless/4.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/borderless.jpg` & `img2table-1.0.9/examples/data/borderless.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/implicit.png` & `img2table-1.0.9/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/tables.pdf` & `img2table-1.0.9/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/tables.png` & `img2table-1.0.9/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/data/tables.xlsx` & `img2table-1.0.9/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/examples/utils.py` & `img2table-1.0.9/examples/utils.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/setup.cfg` & `img2table-1.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = img2table
 author = Xavier Canton
 summary = img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 license = MIT
 description_file = README.md
 description_content_type = text/markdown
 home_page = https://github.com/xavctn/img2table
-python_requires = >=3.7, <3.12
+python_requires = >=3.8, <3.12
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = src/
@@ -24,14 +24,15 @@
 azure = 
 	azure-cognitiveservices-vision-computervision
 paddle = 
 	paddlepaddle==2.4.2:python_version<'3.11'
 	paddleocr>=2.0.6:python_version<'3.11'
 easyocr = 
 	easyocr>=1.7.0
+	pillow<10
 
 [pbr]
 skip_authors = True
 skip_changelog = True
 skip_reno = True
 
 [egg_info]
```

### Comparing `img2table-1.0.8/src/img2table/__init__.py` & `img2table-1.0.9/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/document/base/__init__.py` & `img2table-1.0.9/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/document/base/rotation.py` & `img2table-1.0.9/src/img2table/document/base/rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,25 +80,25 @@
 
     # Compute slopes and angles
     df_angles = (df_cross.with_columns(((pl.col('y1') - pl.col('y1_right')) / (pl.col('x1') - pl.col('x1_right'))
                                         ).round(3).alias('slope'))
                  .with_columns((pl.col('slope').arctan() * 180 / np.pi).alias('angle'))
                  .with_columns(pl.when(pl.col('angle').abs() <= 45)
                                .then(pl.col('angle'))
-                               .otherwise(pl.min(pl.col('angle') + 90, 90 - pl.col('angle')) * -pl.col('angle').sign())
+                               .otherwise(pl.min_horizontal(pl.col('angle') + 90, 90 - pl.col('angle')) * -pl.col('angle').sign())
                                .alias('angle')
                                )
                  )
 
     # Get n most represented angles
     most_likely_angles = (df_angles.groupby('angle')
                           .count()
                           .sort(by=['count', pl.col('angle').abs()], descending=[True, False])
                           .limit(n_max)
-                          .collect(streaming=True)
+                          .collect()
                           .to_dicts()
                           )
 
     if most_likely_angles:
         if most_likely_angles[0].get('angle') == 0:
             return [0]
         else:
```

### Comparing `img2table-1.0.8/src/img2table/document/image.py` & `img2table-1.0.9/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/document/pdf.py` & `img2table-1.0.9/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/aws_textract.py` & `img2table-1.0.9/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/azure.py` & `img2table-1.0.9/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/base.py` & `img2table-1.0.9/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/data.py` & `img2table-1.0.9/src/img2table/ocr/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 
         # Compute coordinates of intersection
         df_words = (df_words.with_columns([pl.lit(bbox[0]).alias('x1_bbox'),
                                            pl.lit(bbox[1]).alias('y1_bbox'),
                                            pl.lit(bbox[2]).alias('x2_bbox'),
                                            pl.lit(bbox[3]).alias('y2_bbox')]
                                           )
-                    .with_columns([pl.max([pl.col('x1'), pl.col('x1_bbox')]).alias('x_left'),
-                                   pl.max([pl.col('y1'), pl.col('y1_bbox')]).alias('y_top'),
-                                   pl.min([pl.col('x2'), pl.col('x2_bbox')]).alias('x_right'),
-                                   pl.min([pl.col('y2'), pl.col('y2_bbox')]).alias('y_bottom'),
+                    .with_columns([pl.max_horizontal(['x1', 'x1_bbox']).alias('x_left'),
+                                   pl.max_horizontal(['y1', 'y1_bbox']).alias('y_top'),
+                                   pl.min_horizontal(['x2', 'x2_bbox']).alias('x_right'),
+                                   pl.min_horizontal(['y2', 'y2_bbox']).alias('y_bottom'),
                                    ])
                     )
 
         # Filter where intersection is not empty
         df_intersection = (df_words.filter(pl.col("x_right") > pl.col("x_left"))
                            .filter(pl.col("y_bottom") > pl.col("y_top"))
                            )
@@ -76,90 +76,87 @@
                                 pl.col('y2').max(),
                                 pl.col('value').alias('value')])
                           .sort([pl.col("y1"), pl.col("x1")])
                           )
 
         # Concatenate all rows
         text_lines = (df_text_parent.select(pl.col('value'))
-                      .collect(streaming=True)
+                      .collect()
                       .get_column('value')
                       .to_list()
                       )
 
         return "\n".join([" ".join(line).strip() for line in text_lines]).strip() or None
 
     def get_text_table(self, table: Table, page_number: int = None, min_confidence: int = 50) -> Table:
         """
         Identify text located in Table object
         :param table: Table object
         :param page_number: page number of the cell
         :param min_confidence: minimum confidence in order to include a word, from 0 (worst) to 99 (best)
         :return: table with content set on all cells
         """
-        try:
-            # Filter dataframe on relevant page
-            df_words = self.df.filter(pl.col('class') == "ocrx_word")
-            if page_number:
-                df_words = df_words.filter(pl.col('page') == page_number)
-            # Filter dataframe on relevant words
-            df_words = df_words.filter(pl.col('value').is_not_null() & (pl.col('confidence') >= min_confidence))
-
-            # Create dataframe containing all coordinates of Cell objects
-            list_cells = [{"row": id_row, "col": id_col, "x1_w": cell.x1, "x2_w": cell.x2, "y1_w": cell.y1, "y2_w": cell.y2}
-                          for id_row, row in enumerate(table.items)
-                          for id_col, cell in enumerate(row.items)]
-            df_cells = pl.LazyFrame(data=list_cells)
-
-            # Cartesian product between two dataframes
-            df_word_cells = df_words.join(other=df_cells, how="cross")
-
-            # Compute coordinates of intersection
-            df_word_cells = df_word_cells.with_columns([pl.max([pl.col('x1'), pl.col('x1_w')]).alias('x_left'),
-                                                        pl.max([pl.col('y1'), pl.col('y1_w')]).alias('y_top'),
-                                                        pl.min([pl.col('x2'), pl.col('x2_w')]).alias('x_right'),
-                                                        pl.min([pl.col('y2'), pl.col('y2_w')]).alias('y_bottom'),
-                                                        ])
-
-            # Filter where intersection is not empty
-            df_intersection = (df_word_cells.filter(pl.col("x_right") > pl.col("x_left"))
-                               .filter(pl.col("y_bottom") > pl.col("y_top"))
-                               )
-
-            # Compute area of word bbox and intersection
-            df_areas = (df_intersection.with_columns([
-                ((pl.col('x2') - pl.col('x1')) * (pl.col('y2') - pl.col('y1'))).alias('w_area'),
-                ((pl.col('x_right') - pl.col('x_left')) * (pl.col('y_bottom') - pl.col('y_top'))).alias('int_area')
-            ])
-            )
-
-            # Filter on words where its bbox is contained in area
-            df_words_contained = df_areas.filter(pl.col('int_area') / pl.col('w_area') >= 0.75)
-
-            # Group text by parent
-            df_text_parent = (df_words_contained
-                              .groupby(['row', 'col', 'parent'])
-                              .agg([pl.col('x1').min(),
-                                    pl.col('x2').max(),
-                                    pl.col('y1').min(),
-                                    pl.col('y2').max(),
-                                    pl.col('value').apply(lambda x: ' '.join(x), return_dtype=str).alias('value')])
-                              .sort([pl.col("row"), pl.col("col"), pl.col('y1'), pl.col('x1')])
-                              .groupby(['row', 'col'])
-                              .agg(pl.col('value').apply(lambda x: '\n'.join(x).strip(), return_dtype=str).alias('text'))
-                              )
-
-            # Implement found values to table cells content
-            for rec in df_text_parent.collect(streaming=True).to_dicts():
-                table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
-
-            return table
-        except pl.PolarsPanicError:
-            return table
+        # Filter dataframe on relevant page
+        df_words = self.df.filter(pl.col('class') == "ocrx_word")
+        if page_number:
+            df_words = df_words.filter(pl.col('page') == page_number)
+        # Filter dataframe on relevant words
+        df_words = df_words.filter(pl.col('value').is_not_null() & (pl.col('confidence') >= min_confidence))
+
+        # Create dataframe containing all coordinates of Cell objects
+        list_cells = [{"row": id_row, "col": id_col, "x1_w": cell.x1, "x2_w": cell.x2, "y1_w": cell.y1, "y2_w": cell.y2}
+                      for id_row, row in enumerate(table.items)
+                      for id_col, cell in enumerate(row.items)]
+        df_cells = pl.LazyFrame(data=list_cells)
+
+        # Cartesian product between two dataframes
+        df_word_cells = df_words.join(other=df_cells, how="cross")
+
+        # Compute coordinates of intersection
+        df_word_cells = df_word_cells.with_columns([pl.max_horizontal(['x1', 'x1_w']).alias('x_left'),
+                                                    pl.max_horizontal(['y1', 'y1_w']).alias('y_top'),
+                                                    pl.min_horizontal(['x2', 'x2_w']).alias('x_right'),
+                                                    pl.min_horizontal(['y2', 'y2_w']).alias('y_bottom'),
+                                                    ])
+
+        # Filter where intersection is not empty
+        df_intersection = (df_word_cells.filter(pl.col("x_right") > pl.col("x_left"))
+                           .filter(pl.col("y_bottom") > pl.col("y_top"))
+                           )
+
+        # Compute area of word bbox and intersection
+        df_areas = (df_intersection.with_columns([
+            ((pl.col('x2') - pl.col('x1')) * (pl.col('y2') - pl.col('y1'))).alias('w_area'),
+            ((pl.col('x_right') - pl.col('x_left')) * (pl.col('y_bottom') - pl.col('y_top'))).alias('int_area')
+        ])
+        )
+
+        # Filter on words where its bbox is contained in area
+        df_words_contained = df_areas.filter(pl.col('int_area') / pl.col('w_area') >= 0.75)
+
+        # Group text by parent
+        df_text_parent = (df_words_contained
+                          .groupby(['row', 'col', 'parent'])
+                          .agg([pl.col('x1').min(),
+                                pl.col('x2').max(),
+                                pl.col('y1').min(),
+                                pl.col('y2').max(),
+                                pl.col('value').apply(lambda x: ' '.join(x), return_dtype=str).alias('value')])
+                          .sort([pl.col("row"), pl.col("col"), pl.col('y1'), pl.col('x1')])
+                          .groupby(['row', 'col'])
+                          .agg(pl.col('value').apply(lambda x: '\n'.join(x).strip(), return_dtype=str).alias('text'))
+                          )
+
+        # Implement found values to table cells content
+        for rec in df_text_parent.collect().to_dicts():
+            table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
+
+        return table
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             try:
-                assert self.df.collect(streaming=True).sort(by=['id']).frame_equal(other.df.collect(streaming=True).sort(by=['id']))
+                assert self.df.collect().sort(by=['id']).frame_equal(other.df.collect().sort(by=['id']))
                 return True
             except AssertionError:
                 return False
         return False
```

### Comparing `img2table-1.0.8/src/img2table/ocr/easyocr.py` & `img2table-1.0.9/src/img2table/ocr/easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/google_vision.py` & `img2table-1.0.9/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/paddle.py` & `img2table-1.0.9/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/pdf.py` & `img2table-1.0.9/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/ocr/tesseract.py` & `img2table-1.0.9/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/__init__.py` & `img2table-1.0.9/src/img2table/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/image.py` & `img2table-1.0.9/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/metrics.py` & `img2table-1.0.9/src/img2table/tables/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,34 +96,33 @@
 
     # Create contours dataframe
     df_contours = pl.LazyFrame(data=contours)
 
     # Cross join to get corresponding contours and filter on contours that corresponds horizontally
     df_h_cnts = (df_contours.join(df_contours, how='cross')
                  .filter(pl.col('id') != pl.col('id_right'))
-                 .filter(pl.min([pl.col('x2'), pl.col('x2_right')])
-                         - pl.max([pl.col('x1'), pl.col('x1_right')]) > 0)
+                 .filter(pl.min_horizontal(['x2', 'x2_right']) - pl.max_horizontal(['x1', 'x1_right']) > 0)
                  )
 
     # Get contour which is directly below
     df_cnts_below = (df_h_cnts.filter(pl.col('y1') < pl.col('y1_right'))
                      .sort(['id', 'y1_right'])
                      .with_columns(pl.lit(1).alias('ones'))
                      .with_columns(pl.col('ones').cumsum().over(["id"]).alias('rk'))
                      .filter(pl.col('rk') == 1)
                      )
 
-    if df_cnts_below.collect(streaming=True).height == 0:
+    if df_cnts_below.collect().height == 0:
         return None, [Cell(x1=c.get('x1'), y1=c.get('y1'), x2=c.get('x2'), y2=c.get('y2')) for c in contours]
 
     # Compute median vertical distance between contours
     median_v_dist = (df_cnts_below.with_columns(((pl.col('y1_right') + pl.col('y2_right')
                                                    - pl.col('y1') - pl.col('y2')) / 2).abs().alias('y_diff'))
                      .select(pl.median('y_diff'))
-                     .collect(streaming=True)
+                     .collect()
                      .to_dicts()
                      .pop()
                      .get('y_diff')
                      )
 
     return median_v_dist, [Cell(x1=c.get('x1'), y1=c.get('y1'), x2=c.get('x2'), y2=c.get('y2')) for c in contours]
```

### Comparing `img2table-1.0.8/src/img2table/tables/objects/__init__.py` & `img2table-1.0.9/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/objects/extraction.py` & `img2table-1.0.9/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/objects/line.py` & `img2table-1.0.9/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/objects/row.py` & `img2table-1.0.9/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/objects/table.py` & `img2table-1.0.9/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,26 +12,23 @@
 def get_cells(horizontal_lines: List[Line], vertical_lines: List[Line]) -> List[Cell]:
     """
     Identify cells from horizontal and vertical rows
     :param horizontal_lines: list of horizontal rows
     :param vertical_lines: list of vertical rows
     :return: list of all cells in image
     """
-    try:
-        # Create dataframe with cells from horizontal and vertical rows
-        df_cells = get_cells_dataframe(horizontal_lines=horizontal_lines,
-                                       vertical_lines=vertical_lines)
+    # Create dataframe with cells from horizontal and vertical rows
+    df_cells = get_cells_dataframe(horizontal_lines=horizontal_lines,
+                                   vertical_lines=vertical_lines)
 
-        # Handle case of empty cells
-        if df_cells.collect(streaming=True).height == 0:
-            return []
+    # Handle case of empty cells
+    if df_cells.collect().height == 0:
+        return []
 
-        # Deduplicate cells
-        df_cells_dedup = deduplicate_cells(df_cells=df_cells)
+    # Deduplicate cells
+    df_cells_dedup = deduplicate_cells(df_cells=df_cells)
 
-        # Convert to Cell objects
-        cells = [Cell(x1=row["x1"], x2=row["x2"], y1=row["y1"], y2=row["y2"])
-                 for row in df_cells_dedup.collect(streaming=True).to_dicts()]
+    # Convert to Cell objects
+    cells = [Cell(x1=row["x1"], x2=row["x2"], y1=row["y1"], y2=row["y2"])
+             for row in df_cells_dedup.collect().to_dicts()]
 
-        return cells
-    except pl.PolarsPanicError:
-        return []
+    return cells
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,35 +17,35 @@
                 )
 
     # Create copy of df_cells
     df_cells_cp = (df_cells.clone()
                    .rename({col: f"{col}_" for col in df_cells.columns})
                    )
 
-    if df_cells.collect(streaming=True).height == 0:
+    if df_cells.collect().height == 0:
         return df_cells
 
     # Cross join to get cells pairs and filter on right cells bigger than right cells
     df_cross_cells = (df_cells.clone()
                       .join(df_cells_cp, how='cross')
                       .filter(pl.col('index') != pl.col('index_'))
                       .filter(pl.col('area') <= pl.col('area_'))
                       )
 
     ### Compute indicator if the first cell is contained in second cell
     # Compute coordinates of intersection
-    df_cross_cells = df_cross_cells.with_columns([pl.max([pl.col('x1'), pl.col('x1_')]).alias('x_left'),
-                                                  pl.max([pl.col('y1'), pl.col('y1_')]).alias('y_top'),
-                                                  pl.min([pl.col('x2'), pl.col('x2_')]).alias('x_right'),
-                                                  pl.min([pl.col('y2'), pl.col('y2_')]).alias('y_bottom'),
+    df_cross_cells = df_cross_cells.with_columns([pl.max_horizontal(['x1', 'x1_']).alias('x_left'),
+                                                  pl.max_horizontal(['y1', 'y1_']).alias('y_top'),
+                                                  pl.min_horizontal(['x2', 'x2_']).alias('x_right'),
+                                                  pl.min_horizontal(['y2', 'y2_']).alias('y_bottom'),
                                                   ])
 
     # Compute area of intersection
-    df_cross_cells = df_cross_cells.with_columns((pl.max([pl.col('x_right') - pl.col('x_left'), pl.lit(0)])
-                                                  * pl.max([pl.col('y_bottom') - pl.col('y_top'), pl.lit(0)])
+    df_cross_cells = df_cross_cells.with_columns((pl.max_horizontal([pl.col('x_right') - pl.col('x_left'), pl.lit(0)])
+                                                  * pl.max_horizontal([pl.col('y_bottom') - pl.col('y_top'), pl.lit(0)])
                                                   ).alias('int_area')
                                                  )
 
     # Create column indicating if left cell is contained in right cell
     df_cross_cells = df_cross_cells.with_columns(((pl.col('x_right') >= pl.col('x_left'))
                                                   & (pl.col('y_bottom') >= pl.col('y_top'))
                                                   & (pl.col('int_area') / pl.col('area') >= 0.9)
@@ -53,36 +53,36 @@
                                                  )
 
     ### Compute indicator if cells are adjacent
     # Compute intersections and horizontal / vertical differences
     df_cross_cells = (df_cross_cells
                       .with_columns([(pl.col('x_right') - pl.col('x_left')).alias('overlapping_x'),
                                      (pl.col('y_bottom') - pl.col('y_top')).alias('overlapping_y')])
-                      .with_columns(pl.min([(pl.col(_1) - pl.col(_2)).abs()
-                                            for _1, _2 in itertools.product(['x1', 'x2'], ['x1_', 'x2_'])]
-                                           ).alias('diff_x'))
-                      .with_columns(pl.min([(pl.col(_1) - pl.col(_2)).abs()
-                                            for _1, _2 in itertools.product(['y1', 'y2'], ['y1_', 'y2_'])]
-                                           ).alias('diff_y'))
+                      .with_columns(pl.min_horizontal([(pl.col(_1) - pl.col(_2)).abs()
+                                                       for _1, _2 in itertools.product(['x1', 'x2'], ['x1_', 'x2_'])]
+                                                      ).alias('diff_x'))
+                      .with_columns(pl.min_horizontal([(pl.col(_1) - pl.col(_2)).abs()
+                                                       for _1, _2 in itertools.product(['y1', 'y2'], ['y1_', 'y2_'])]
+                                                      ).alias('diff_y'))
                       )
 
     # Create column indicating if both cells are adjacent and  column indicating if the right cell is redundant with
     # the left cell
     condition_adjacent = (((pl.col("overlapping_y") > 5)
-                           & (pl.col("diff_x") / pl.max([pl.col("width"), pl.col("width_")]) <= 0.05))
+                           & (pl.col("diff_x") / pl.max_horizontal(["width", "width_"]) <= 0.05))
                           | ((pl.col("overlapping_x") > 5)
-                             & (pl.col("diff_y") / pl.max([pl.col("height"), pl.col("height_")]) <= 0.05))
+                             & (pl.col("diff_y") / pl.max_horizontal(["height", "height_"]) <= 0.05))
                           )
     df_cross_cells = (df_cross_cells.with_columns(condition_adjacent.alias('adjacent'))
                       .with_columns((pl.col('contained') & pl.col('adjacent')).alias('redundant'))
                       )
 
     # Get list of redundant cells and remove them from original cell dataframe
     redundant_cells = (df_cross_cells.filter(pl.col('redundant'))
-                       .collect(streaming=True)
+                       .collect()
                        .get_column('index_')
                        .unique()
                        .to_list()
                        )
     df_final_cells = (df_cells.with_row_count(name="cnt")
                       .filter(~pl.col('cnt').is_in(redundant_cells))
                       .drop('cnt')
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     # Create condition on horizontal correspondence in order to use both rows and filter on relevant combinations
     matching_condition = ((pl.col('l_corresponds') | pl.col('l_contained'))
                           & (pl.col('r_corresponds') | pl.col('r_contained')))
     cross_h_lines = cross_h_lines.filter(matching_condition)
 
     # Create cell bbox from horizontal rows
-    df_bbox = (cross_h_lines.select([pl.max([pl.col('x1'), pl.col('x1_')]).alias('x1_bbox'),
-                                     pl.min([pl.col('x2'), pl.col('x2_')]).alias('x2_bbox'),
+    df_bbox = (cross_h_lines.select([pl.max_horizontal(['x1', 'x1_']).alias('x1_bbox'),
+                                     pl.min_horizontal(['x2', 'x2_']).alias('x2_bbox'),
                                      pl.col('y1').alias("y1_bbox"),
                                      pl.col('y1_').alias('y2_bbox')]
                                     )
                .with_row_count(name="idx")
                )
 
     # Deduplicate on upper bound
@@ -79,27 +79,27 @@
     df_h_lines = pl.LazyFrame(data=[l.dict for l in horizontal_lines])
     df_v_lines = pl.LazyFrame(data=[l.dict for l in vertical_lines])
 
     # Identify potential cells bboxes from horizontal rows
     df_bbox = get_potential_cells_from_h_lines(df_h_lines=df_h_lines)
 
     # Cross join with vertical rows
-    df_bbox = df_bbox.with_columns(pl.max([(pl.col('x2_bbox') - pl.col('x1_bbox')) * 0.025,
-                                           pl.lit(5.0)]).round(0).alias('h_margin')
+    df_bbox = df_bbox.with_columns(pl.max_horizontal([(pl.col('x2_bbox') - pl.col('x1_bbox')) * 0.025,
+                                                      pl.lit(5.0)]).round(0).alias('h_margin')
                                    )
     df_bbox_v = df_bbox.join(df_v_lines, how='cross')
 
     # Check horizontal correspondence between cell and vertical rows
     horizontal_cond = ((pl.col("x1_bbox") - pl.col("h_margin") <= pl.col("x1"))
                        & (pl.col("x2_bbox") + pl.col("h_margin") >= pl.col("x1")))
     df_bbox_v = df_bbox_v.filter(horizontal_cond)
 
     # Check vertical overlapping
-    df_bbox_v = (df_bbox_v.with_columns((pl.min([pl.col('y2'), pl.col('y2_bbox')])
-                                         - pl.max([pl.col('y1'), pl.col('y1_bbox')])).alias('overlapping')
+    df_bbox_v = (df_bbox_v.with_columns((pl.min_horizontal(['y2', 'y2_bbox'])
+                                         - pl.max_horizontal(['y1', 'y1_bbox'])).alias('overlapping')
                                         )
                  .filter(pl.col('overlapping') / (pl.col('y2_bbox') - pl.col('y1_bbox')) >= 0.8)
                  )
 
     # Get all vertical delimiters by bbox
     df_bbox_delimiters = (df_bbox_v.sort(['idx', "x1_bbox", "x2_bbox", "y1_bbox", "y2_bbox", "x1"])
                           .groupby(['idx', "x1_bbox", "x2_bbox", "y1_bbox", "y2_bbox"])
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,52 +172,52 @@
     :param contours: list of image contours as cell objects
     :return: list of rows not intersecting with words
     """
     # Get contours dataframe
     df_cnts = pl.LazyFrame(data=[{"x1": c.x1, "y1": c.y1, "x2": c.x2, "y2": c.y2} for c in contours])
 
     # If there are no rows or no contours, do nothing
-    if len(lines) == 0 or df_cnts.collect(streaming=True).height == 0:
+    if len(lines) == 0 or df_cnts.collect().height == 0:
         return lines
 
     # Create dataframe containing rows
     df_lines = (pl.LazyFrame(data=[line.dict for line in lines])
-                .with_columns([pl.max([pl.col('width'), pl.col('height')]).alias('length'),
+                .with_columns([pl.max_horizontal([pl.col('width'), pl.col('height')]).alias('length'),
                                (pl.col('x1') == pl.col('x2')).alias('vertical')]
                               )
                 .with_row_count(name="line_id")
                 .rename({"x1": "x1_line", "x2": "x2_line", "y1": "y1_line", "y2": "y2_line"})
                 )
 
     # Merge both dataframes
     df_words_lines = df_cnts.join(df_lines, how='cross')
 
     # Compute intersection between contours bbox and rows
     # - vertical case
     vert_int = (
         (((pl.col('x1') + pl.col('x2')) / 2 - pl.col('x1_line')).abs() / (pl.col('x2') - pl.col('x1')) < 0.45)
-        * pl.max([(pl.min([pl.col('y2'), pl.col('y2_line')]) - pl.max([pl.col('y1'), pl.col('y1_line')])), pl.lit(0)])
+        * pl.max_horizontal([(pl.min_horizontal(['y2', 'y2_line']) - pl.max_horizontal(['y1', 'y1_line'])), pl.lit(0)])
     )
     # - horizontal case
     hor_int = (
         (((pl.col('y1') + pl.col('y2')) / 2 - pl.col('y1_line')).abs() / (pl.col('y2') - pl.col('y1')) < 0.33)
-        * pl.max([(pl.min([pl.col('x2'), pl.col('x2_line')]) - pl.max([pl.col('x1'), pl.col('x1_line')])), pl.lit(0)])
+        * pl.max_horizontal([(pl.min_horizontal(['x2', 'x2_line']) - pl.max_horizontal(['x1', 'x1_line'])), pl.lit(0)])
     )
     df_words_lines = df_words_lines.with_columns((pl.col('vertical') * vert_int
                                                   + (1 - pl.col('vertical')) * hor_int).alias('intersection')
                                                  )
 
     # Compute total intersection for each line
     df_inter = (df_words_lines.groupby(['line_id', 'length'])
                 .agg(pl.col('intersection').sum().alias('intersection'))
                 )
 
     # Identify rows that intersect contours
     intersecting_lines = (df_inter.filter(pl.col('intersection') / pl.col('length') > 0.25)
-                          .collect(streaming=True)
+                          .collect()
                           .get_column('line_id')
                           .to_list()
                           )
 
     return [line for idx, line in enumerate(lines) if idx not in intersecting_lines]
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,56 +13,52 @@
 def compute_table_median_row_sep(table: Table, contours: List[Cell]) -> Optional[float]:
     """
     Compute median row separation in table
     :param table: Table object
     :param contours: list of image contours as cell objects
     :return: median row separation
     """
-    try:
-        # Create dataframe with contours
-        list_elements = [{"id": idx, "x1": el.x1, "y1": el.y1, "x2": el.x2, "y2": el.y2}
-                         for idx, el in enumerate(contours)]
-        df_elements = pl.LazyFrame(data=list_elements)
-
-        # Filter on elements that are within the table
-        df_elements_table = df_elements.filter((pl.col('x1') >= table.x1) & (pl.col('x2') <= table.x2)
-                                               & (pl.col('y1') >= table.y1) & (pl.col('y2') <= table.y2))
-
-        # Cross join to get corresponding elements and filter on elements that corresponds horizontally
-        df_h_elms = (df_elements_table.join(df_elements_table, how='cross')
-                     .filter(pl.col('id') != pl.col('id_right'))
-                     .filter(pl.min([pl.col('x2'), pl.col('x2_right')])
-                             - pl.max([pl.col('x1'), pl.col('x1_right')]) > 0)
+    # Create dataframe with contours
+    list_elements = [{"id": idx, "x1": el.x1, "y1": el.y1, "x2": el.x2, "y2": el.y2}
+                     for idx, el in enumerate(contours)]
+    df_elements = pl.LazyFrame(data=list_elements)
+
+    # Filter on elements that are within the table
+    df_elements_table = df_elements.filter((pl.col('x1') >= table.x1) & (pl.col('x2') <= table.x2)
+                                           & (pl.col('y1') >= table.y1) & (pl.col('y2') <= table.y2))
+
+    # Cross join to get corresponding elements and filter on elements that corresponds horizontally
+    df_h_elms = (df_elements_table.join(df_elements_table, how='cross')
+                 .filter(pl.col('id') != pl.col('id_right'))
+                 .filter(pl.min_horizontal(['x2', 'x2_right']) - pl.max_horizontal(['x1', 'x1_right']) > 0)
+                 )
+
+    # Get element which is directly below
+    df_elms_below = (df_h_elms.filter(pl.col('y1') < pl.col('y1_right'))
+                     .sort(['id', 'y1_right'])
+                     .with_columns(pl.lit(1).alias('ones'))
+                     .with_columns(pl.col('ones').cumsum().over(["id"]).alias('rk'))
+                     .filter(pl.col('rk') == 1)
                      )
 
-        # Get element which is directly below
-        df_elms_below = (df_h_elms.filter(pl.col('y1') < pl.col('y1_right'))
-                         .sort(['id', 'y1_right'])
-                         .with_columns(pl.lit(1).alias('ones'))
-                         .with_columns(pl.col('ones').cumsum().over(["id"]).alias('rk'))
-                         .filter(pl.col('rk') == 1)
-                         )
-
-        if df_elms_below.collect(streaming=True).height == 0:
-            return None
-
-        # Compute median vertical distance between elements
-        median_v_dist = (df_elms_below.with_columns(((pl.col('y1_right') + pl.col('y2_right')
-                                                      - pl.col('y1') - pl.col('y2')) / 2).abs().alias('y_diff'))
-                         .select(pl.median('y_diff'))
-                         .collect(streaming=True)
-                         .to_dicts()
-                         .pop()
-                         .get('y_diff')
-                         )
-
-        return median_v_dist
-    except pl.PolarsPanicError:
+    if df_elms_below.collect().height == 0:
         return None
 
+    # Compute median vertical distance between elements
+    median_v_dist = (df_elms_below.with_columns(((pl.col('y1_right') + pl.col('y2_right')
+                                                  - pl.col('y1') - pl.col('y2')) / 2).abs().alias('y_diff'))
+                     .select(pl.median('y_diff'))
+                     .collect()
+                     .to_dicts()
+                     .pop()
+                     .get('y_diff')
+                     )
+
+    return median_v_dist
+
 
 def handle_implicit_rows_table(img: np.ndarray, table: Table, contours: List[Cell], margin: int = 5) -> Table:
     """
     Find implicit rows and update tables based on those
     :param img: image array
     :param table: Table object
     :param contours: list of image contours as cell objects
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-1.0.9/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/coherency.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,34 +22,33 @@
     list_elements = [{"id": idx, "x1": el.x1, "y1": el.y1, "x2": el.x2, "y2": el.y2}
                      for idx, el in enumerate(delimiter_group.elements)]
     df_elements = pl.LazyFrame(data=list_elements)
 
     # Cross join to get corresponding elements and filter on elements that corresponds horizontally
     df_h_elms = (df_elements.join(df_elements, how='cross')
                  .filter(pl.col('id') != pl.col('id_right'))
-                 .filter(pl.min([pl.col('x2'), pl.col('x2_right')])
-                         - pl.max([pl.col('x1'), pl.col('x1_right')]) > 0)
+                 .filter(pl.min_horizontal(['x2', 'x2_right']) - pl.max_horizontal(['x1', 'x1_right']) > 0)
                  )
 
     # Get element which is directly below
     df_elms_below = (df_h_elms.filter(pl.col('y1') < pl.col('y1_right'))
                      .sort(['id', 'y1_right'])
                      .with_columns(pl.lit(1).alias('ones'))
                      .with_columns(pl.col('ones').cumsum().over(["id"]).alias('rk'))
                      .filter(pl.col('rk') == 1)
                      )
 
-    if df_elms_below.collect(streaming=True).height == 0:
+    if df_elms_below.collect().height == 0:
         return None
 
     # Compute median vertical distance between elements
     median_v_dist = (df_elms_below.with_columns(((pl.col('y1_right') + pl.col('y2_right')
                                                   - pl.col('y1') - pl.col('y2')) / 2).abs().alias('y_diff'))
                      .select(pl.median('y_diff'))
-                     .collect(streaming=True)
+                     .collect()
                      .to_dicts()
                      .pop()
                      .get('y_diff')
                      )
 
     return median_v_dist
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-1.0.9/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/common.py` & `img2table-1.0.9/src/img2table/tables/processing/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     # Cross join
     df_cross = (df_cnt.join(df_cnt, how='cross')
                 .filter(pl.col('id') != pl.col('id_right'))
                 .filter(pl.col('area') <= pl.col('area_right'))
                 )
 
     # Compute intersection area between contours and identify if the smallest contour overlaps the largest one
-    x_left = pl.max(pl.col('x1'), pl.col('x1_right'))
-    x_right = pl.min(pl.col('x2'), pl.col('x2_right'))
-    y_top = pl.max(pl.col('y1'), pl.col('y1_right'))
-    y_bottom = pl.min(pl.col('y2'), pl.col('y2_right'))
-    intersection = pl.max(x_right - x_left, 0) * pl.max(y_bottom - y_top, 0)
+    x_left = pl.max_horizontal('x1', 'x1_right')
+    x_right = pl.min_horizontal('x2', 'x2_right')
+    y_top = pl.max_horizontal('y1', 'y1_right')
+    y_bottom = pl.min_horizontal('y2', 'y2_right')
+    intersection = pl.max_horizontal(x_right - x_left, 0) * pl.max_horizontal(y_bottom - y_top, 0)
 
     df_cross = (df_cross.with_columns(intersection.alias('intersection'))
                 .with_columns((pl.col('intersection') / pl.col('area') >= 0.25).alias('overlaps'))
                 )
 
     # Identify relevant contours: no contours is overlapping it
     deleted_contours = df_cross.filter(pl.col('overlaps')).select('id').unique()
@@ -74,23 +74,23 @@
                        pl.max('x2').alias('x2_overlap'),
                        pl.min('y1').alias('y1_overlap'),
                        pl.max('y2').alias('y2_overlap'))
                   )
 
     df_final = (df_cnt.join(deleted_contours, on="id", how="anti")
                 .join(df_overlap, on='id', how='left')
-                .select([pl.min(pl.col('x1'), pl.col('x1_overlap')).alias('x1'),
-                         pl.max(pl.col('x2'), pl.col('x2_overlap')).alias('x2'),
-                         pl.min(pl.col('y1'), pl.col('y1_overlap')).alias('y1'),
-                         pl.max(pl.col('y2'), pl.col('y2_overlap')).alias('y2'),
+                .select([pl.min_horizontal('x1', 'x1_overlap').alias('x1'),
+                         pl.max_horizontal('x2', 'x2_overlap').alias('x2'),
+                         pl.min_horizontal('y1', 'y1_overlap').alias('y1'),
+                         pl.max_horizontal('y2', 'y2_overlap').alias('y2'),
                          ])
                 )
 
     # Map results to cells
-    return [Cell(**d) for d in df_final.collect(streaming=True).to_dicts()]
+    return [Cell(**d) for d in df_final.collect().to_dicts()]
 
 
 def merge_contours(contours: List[Cell], vertically: Optional[bool] = True) -> List[Cell]:
     """
     Create merge contours by an axis
     :param contours: list of contours
     :param vertically: boolean indicating if contours are merged according to the vertical or horizontal axis
```

### Comparing `img2table-1.0.8/src/img2table/tables/processing/prepare_image.py` & `img2table-1.0.9/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table/tables/processing/text/titles.py` & `img2table-1.0.9/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/src/img2table.egg-info/PKG-INFO` & `img2table-1.0.9/src/img2table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.8
+Version: 1.0.9
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -198,16 +198,14 @@
         
         ```bash
         # Example of installation with CUDA 11.8
         pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
         pip install paddleocr img2table
         ```
         
-        
-        *Released in version 0.0.13*
         <br>
         </details>
         
         
         <details>
         <summary>EasyOCR<a name="easyocr"></a></summary>
         <br>
@@ -223,15 +221,14 @@
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : list, optional, default <code>["en"]</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
         ></dl>
         
-        *Released in version 0.1.2*
         <br>
         </details>
         
         <details>
         <summary>Google Vision<a name="vision"></a></summary>
         <br>
         
@@ -333,15 +330,15 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
         >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
-        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
+        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted <b>on top of</b> bordered tables.</dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
         <b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
         
         *Borderless table extraction released in version 0.0.14*
@@ -457,14 +454,14 @@
         </ul>
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.12
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
 Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.8 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.9 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -81,23 +81,23 @@
 >
 >
 
 NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
 gpu has to be installed by the user manually as stated in this issue. ```bash #
 Example of installation with CUDA 11.8 pip install paddlepaddle-
 gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
-stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
+stable.html pip install paddleocr img2table ```
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.1.2*
+
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
@@ -180,10 +180,10 @@
       background. Effectiveness can not be guaranteed on other type of
       documents.
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
+:: OS Independent Requires-Python: >=3.8, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
 Provides-Extra: paddle Provides-Extra: easyocr
```

### Comparing `img2table-1.0.8/src/img2table.egg-info/SOURCES.txt` & `img2table-1.0.9/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/_mock_data/azure.pkl` & `img2table-1.0.9/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/_mock_data/tesseract_hocr.html` & `img2table-1.0.9/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/_mock_data/textract.json` & `img2table-1.0.9/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/_mock_data/vision.json` & `img2table-1.0.9/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/_mock_data/vision.pkl` & `img2table-1.0.9/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/conftest.py` & `img2table-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/base/test_data/test.png` & `img2table-1.0.9/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/base/test_rotation.py` & `img2table-1.0.9/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/image/test_data/blank.png` & `img2table-1.0.9/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/image/test_data/dark.png` & `img2table-1.0.9/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/image/test_data/expected.xlsx` & `img2table-1.0.9/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/image/test_data/test.png` & `img2table-1.0.9/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/image/test_image.py` & `img2table-1.0.9/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/pdf/test_data/test.pdf` & `img2table-1.0.9/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/document/pdf/test_pdf.py` & `img2table-1.0.9/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-1.0.9/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/aws_textract/test_data/content.json` & `img2table-1.0.9/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/aws_textract/test_data/test.png` & `img2table-1.0.9/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/azure/test_azure.py` & `img2table-1.0.9/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/azure/test_data/test.png` & `img2table-1.0.9/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/data/test_data/expected_table.json` & `img2table-1.0.9/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/data/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/data/test_ocr_data.py` & `img2table-1.0.9/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/easyocr/test_data/ocr.json` & `img2table-1.0.9/tests/ocr/easyocr/test_data/ocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/easyocr/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/easyocr/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/easyocr/test_data/test.png` & `img2table-1.0.9/tests/ocr/easyocr/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/easyocr/test_easyocr.py` & `img2table-1.0.9/tests/ocr/easyocr/test_easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-1.0.9/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/google_vision/test_data/test.png` & `img2table-1.0.9/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/google_vision/test_google_vision.py` & `img2table-1.0.9/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/paddle/test_data/hocr.json` & `img2table-1.0.9/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/paddle/test_data/test.png` & `img2table-1.0.9/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/paddle/test_paddle.py` & `img2table-1.0.9/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/pdf/test_data/content.json` & `img2table-1.0.9/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/pdf/test_data/test.pdf` & `img2table-1.0.9/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-1.0.9/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-1.0.9/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/tesseract/test_data/test.png` & `img2table-1.0.9/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/ocr/tesseract/test_tesseract.py` & `img2table-1.0.9/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/image/test_data/blank.png` & `img2table-1.0.9/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/image/test_data/ocr.csv` & `img2table-1.0.9/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/image/test_data/test.png` & `img2table-1.0.9/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/image/test_image.py` & `img2table-1.0.9/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/image/test_metrics.py` & `img2table-1.0.9/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_data/expected_tables.json` & `img2table-1.0.9/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_data/ocr.csv` & `img2table-1.0.9/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_data/tables.json` & `img2table-1.0.9/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_extraction.py` & `img2table-1.0.9/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_line.py` & `img2table-1.0.9/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_row.py` & `img2table-1.0.9/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/objects/test_table.py` & `img2table-1.0.9/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/contours.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-1.0.9/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png` & `img2table-1.0.9/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_coherency.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_data/rows.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/rows/test_rows.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/rows/test_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_data/rows.json` & `img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-1.0.9/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/common/test_common.py` & `img2table-1.0.9/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/common/test_data/test.jpg` & `img2table-1.0.9/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-1.0.9/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/text/test_data/ocr.csv` & `img2table-1.0.9/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/text/test_data/table.json` & `img2table-1.0.9/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/text/test_data/test.jpg` & `img2table-1.0.9/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.8/tests/tables/processing/text/test_titles.py` & `img2table-1.0.9/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

