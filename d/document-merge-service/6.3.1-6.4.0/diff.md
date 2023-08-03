# Comparing `tmp/document_merge_service-6.3.1.tar.gz` & `tmp/document_merge_service-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.3.1.tar", max compression
+gzip compressed data, was "document_merge_service-6.4.0.tar", max compression
```

## Comparing `document_merge_service-6.3.1.tar` & `document_merge_service-6.4.0.tar`

### file list

```diff
@@ -1,71 +1,75 @@
--rw-r--r--   0        0        0    12161 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/LICENSE
--rw-r--r--   0        0        0     2243 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/README.md
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3232 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-07-31 12:45:30.726650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9772 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1354 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0    30689 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/__snapshots__/test_template.ambr
--rw-r--r--   0        0        0     2357 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25634 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0      597 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8938 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3555 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/pyproject.toml
--rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.3.1/PKG-INFO
+-rw-r--r--   0        0        0    12390 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/LICENSE
+-rw-r--r--   0        0        0     2522 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3232 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0     4750 2023-08-03 10:13:53.349800 document_merge_service-6.4.0/document_merge_service/api/data/invalid-template.xlsx
+-rw-r--r--   0        0        0  1127936 2023-08-03 10:13:53.353800 document_merge_service-6.4.0/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-08-03 10:13:53.353800 document_merge_service-6.4.0/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0    10589 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/odt-template.odt
+-rw-r--r--   0        0        0       22 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9772 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0      815 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/file_converter.py
+-rw-r--r--   0        0        0     2841 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1354 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4995 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2357 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1004 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_convert.py
+-rw-r--r--   0        0        0     1963 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25634 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0      597 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      460 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3769 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8938 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-08-03 10:13:53.357800 document_merge_service-6.4.0/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3555 2023-08-03 10:13:53.361800 document_merge_service-6.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 document_merge_service-6.4.0/PKG-INFO
```

### Comparing `document_merge_service-6.3.1/CHANGELOG.md` & `document_merge_service-6.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 6.4.0 (03 August 2023)
+### Feature
+* Allow conversion of docx and odt files to pdf using a new convert endpoint ([`e00e49e`](https://github.com/adfinis/document-merge-service/commit/e00e49e210b17469457b76eccf306f17b40da43a))
+
 ## 6.3.1 (31 July 2023)
 ### Fix
 
 * **auth:** Don't run any authentication logic if auth is disabled ([`564b504`](https://github.com/adfinis/document-merge-service/commit/564b504be673f34677eb6736a3b26dbbfdd3d7ec))
 
 ## 6.3.0 (25 July 2023)
 ### Feature
```

### Comparing `document_merge_service-6.3.1/LICENSE` & `document_merge_service-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/README.md` & `document_merge_service-6.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Document Merge Service
 
 [![Build Status](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml/badge.svg)](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/adfinis/document-merge-service)
 [![License: GPL-3.0-or-later](https://img.shields.io/github/license/adfinis/document-merge-service)](https://spdx.org/licenses/GPL-3.0-or-later.html)
 
-A document template merge service providing an API to manage templates and merge them with given data.
+A document template merge service providing an API to manage templates and merge them with given data. It can also be used to convert Docx files to PDF.
 
 ## Installation
 
 **Requirements**
 
 - docker
 - docker-compose
@@ -50,14 +50,22 @@
 
 After uploading successfully, you can merge a template with the following call:
 
 ```bash
 curl -H "Content-Type: application/json" --data '{"data": {"test": "Test Input"}}' http://localhost:8000/api/v1/template/test-template/merge/ > output.docx
 ```
 
+### Converting a template
+To convert a standalone Docx file the following call can be used:
+
+```bash
+curl -X POST --form file=@my-test-file.docx --form target_format="pdf" http://localhost:8000/api/v1/convert > example.pdf
+```
+
+
 ## Further reading
 
 - [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
 - [Usage](USAGE.md) - How to use the DMS and it's features
 - [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
   contribution. Contributions are welcome!
```

### Comparing `document_merge_service-6.3.1/document_merge_service/api/authentication.py` & `document_merge_service-6.4.0/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/black.png` & `document_merge_service-6.4.0/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.4.0/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.4.0/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.4.0/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.4.0/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.4.0/document_merge_service/api/data/invalid-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/engines.py` & `document_merge_service-6.4.0/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/filters.py` & `document_merge_service-6.4.0/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/jinja.py` & `document_merge_service-6.4.0/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.4.0/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.4.0/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.4.0/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.4.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.4.0/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/models.py` & `document_merge_service-6.4.0/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/serializers.py` & `document_merge_service-6.4.0/document_merge_service/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,7 +133,17 @@
     )
     files = serializers.ListField(
         child=CustomFileField(write_only=True, allow_empty_file=False), required=False
     )
 
     class Meta:
         model = models.Template
+
+
+class ConvertSerializer(serializers.Serializer):
+    file = CustomFileField(required=True, allow_empty_file=False)
+    target_format = serializers.ChoiceField(
+        allow_null=False,
+        required=True,
+        choices=[("pdf", "PDF")],
+        help_text="The target format of the conversion. Currently only 'pdf' is supported.",
+    )
```

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/__snapshots__/test_template.ambr` & `document_merge_service-6.4.0/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.4.0/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/unoconv.py` & `document_merge_service-6.4.0/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/api/views.py` & `document_merge_service-6.4.0/document_merge_service/api/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import mimetypes
-from pathlib import Path
-from tempfile import NamedTemporaryFile
 
 import jinja2
-from django.conf import settings
 from django.http import HttpResponse
 from django.utils.encoding import smart_str
 from generic_permissions.permissions import PermissionViewMixin
 from generic_permissions.visibilities import VisibilityViewMixin
 from rest_framework import exceptions, viewsets
 from rest_framework.decorators import action
 from rest_framework.generics import RetrieveAPIView
+from rest_framework.views import APIView
 
 from . import engines, filters, models, serializers
-from .unoconv import Unoconv
+from .file_converter import FileConverter
 
 
 class TemplateView(VisibilityViewMixin, PermissionViewMixin, viewsets.ModelViewSet):
     queryset = models.Template.objects
     serializer_class = serializers.TemplateSerializer
     filterset_class = filters.TemplateFilterSet
     ordering_fields = ("slug", "description")
@@ -32,15 +30,14 @@
         template = self.get_object()
         engine = engines.get_engine(template.engine, template.template)
 
         content_type, _ = mimetypes.guess_type(template.template.name)
         response = HttpResponse(
             content_type=content_type or "application/force-download"
         )
-        extension = mimetypes.guess_extension(content_type)
 
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         data = serializer.data["data"]
         files = serializer.data.get("files")
 
@@ -54,32 +51,17 @@
             raise exceptions.ValidationError(
                 f"Placeholder from template not found in data: {exc}"
             )
 
         convert = serializer.data.get("convert")
 
         if convert:
-            dir = Path(settings.DATABASE_DIR, "tmp")
-            dir.mkdir(parents=True, exist_ok=True)
-            with NamedTemporaryFile("wb", dir=dir) as tmp:
-                tmp.write(response.content)
-                unoconv = Unoconv(
-                    pythonpath=settings.UNOCONV_PYTHON,
-                    unoconvpath=settings.UNOCONV_PATH,
-                )
-                result = unoconv.process(tmp.name, convert)
-            extension = convert
-            status = 500
-            if result.returncode == 0:
-                status = 200
-            response = HttpResponse(
-                content=result.stdout, status=status, content_type=result.content_type
-            )
+            response = FileConverter.convert(response.content, convert)
 
-        filename = f"{template.slug}.{extension}"
+        filename = f"{template.slug}.{convert}"
         response["Content-Disposition"] = f'attachment; filename="{filename}"'
         return response
 
 
 class DownloadTemplateView(RetrieveAPIView):
     queryset = models.Template.objects
     lookup_field = "pk"
@@ -94,7 +76,32 @@
         response = HttpResponse(content_type=content_type)
         response["Content-Disposition"] = 'attachment; filename="%s"' % smart_str(
             template.slug + extension
         )
         response["Content-Length"] = template.template.size
         response.write(template.template.read())
         return response
+
+
+class ConvertView(APIView):
+    def post(self, request, **kwargs):
+        serializer = serializers.ConvertSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+
+        file = serializer.data["file"]
+        target_format = serializer.data["target_format"]
+
+        content_type, foo = mimetypes.guess_type(file.name)
+
+        if content_type not in [
+            "application/vnd.oasis.opendocument.text",
+            "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
+        ]:
+            raise exceptions.ValidationError(
+                "Incorrect file format. Only docx and odt files are supported for conversion."
+            )
+
+        response = FileConverter.convert(file.read(), target_format)
+
+        filename = f"{file.name.split('.')[0]}.{target_format}"
+        response["Content-Disposition"] = f'attachment; filename="{filename}"'
+        return response
```

### Comparing `document_merge_service-6.3.1/document_merge_service/conftest.py` & `document_merge_service-6.4.0/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/sentry.py` & `document_merge_service-6.4.0/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/settings.py` & `document_merge_service-6.4.0/document_merge_service/settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/document_merge_service/tests/test_settings.py` & `document_merge_service-6.4.0/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.1/pyproject.toml` & `document_merge_service-6.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.3.1"
+version = "6.4.0"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
```

### Comparing `document_merge_service-6.3.1/PKG-INFO` & `document_merge_service-6.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.3.1
+Version: 6.4.0
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,15 +43,15 @@
 
 # Document Merge Service
 
 [![Build Status](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml/badge.svg)](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/adfinis/document-merge-service)
 [![License: GPL-3.0-or-later](https://img.shields.io/github/license/adfinis/document-merge-service)](https://spdx.org/licenses/GPL-3.0-or-later.html)
 
-A document template merge service providing an API to manage templates and merge them with given data.
+A document template merge service providing an API to manage templates and merge them with given data. It can also be used to convert Docx files to PDF.
 
 ## Installation
 
 **Requirements**
 
 - docker
 - docker-compose
@@ -93,14 +93,22 @@
 
 After uploading successfully, you can merge a template with the following call:
 
 ```bash
 curl -H "Content-Type: application/json" --data '{"data": {"test": "Test Input"}}' http://localhost:8000/api/v1/template/test-template/merge/ > output.docx
 ```
 
+### Converting a template
+To convert a standalone Docx file the following call can be used:
+
+```bash
+curl -X POST --form file=@my-test-file.docx --form target_format="pdf" http://localhost:8000/api/v1/convert > example.pdf
+```
+
+
 ## Further reading
 
 - [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
 - [Usage](USAGE.md) - How to use the DMS and it's features
 - [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
   contribution. Contributions are welcome!
```

