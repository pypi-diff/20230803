# Comparing `tmp/sefazetllib-0.1.42.tar.gz` & `tmp/sefazetllib-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.42.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.43.tar", max compression
```

## Comparing `sefazetllib-0.1.42.tar` & `sefazetllib-0.1.43.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10173 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/LICENSE
--rw-r--r--   0        0        0     3159 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/README.md
--rw-r--r--   0        0        0     2442 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/pyproject.toml
--rw-r--r--   0        0        0     1663 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/Builder.py
--rw-r--r--   0        0        0      135 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/__init__.py
--rw-r--r--   0        0        0     2338 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       52 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     8218 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0       36 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0      701 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     1986 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     3366 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2521 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2282 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0      274 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      949 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0       89 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      362 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      281 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1049 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      268 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      723 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0     4069 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/database/PostgreSQL.py
--rw-r--r--   0        0        0      134 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      259 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1793 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     4679 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      195 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      683 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2134 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     2386 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0     7601 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2194 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      229 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      573 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/transform/ColumnsToLowerCase.py
--rw-r--r--   0        0        0     1471 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4331 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      552 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0      270 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0       45 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      325 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      400 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      747 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      158 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0     2097 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      627 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      425 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      229 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     7729 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      383 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0      110 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     3551 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      185 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       76 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       52 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       88 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     6415 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      884 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      374 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      524 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3484 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1128 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0      986 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1142 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1110 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1595 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2086 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1074 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      935 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0       99 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      963 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1678 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       32 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-14 14:28:01.183135 sefazetllib-0.1.42/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 sefazetllib-0.1.42/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/LICENSE
+-rw-r--r--   0        0        0     3159 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/README.md
+-rw-r--r--   0        0        0     2442 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0     1663 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/Builder.py
+-rw-r--r--   0        0        0      135 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     2338 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       52 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     8218 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0       36 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0      701 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     1986 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     3366 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2521 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2282 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0      274 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      949 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0       89 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      362 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      281 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1049 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      268 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      723 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0     4140 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/database/PostgreSQL.py
+-rw-r--r--   0        0        0      134 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      259 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1793 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     4679 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      195 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      683 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2134 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     2386 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0     7601 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2194 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      229 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0      573 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/transform/ColumnsToLowerCase.py
+-rw-r--r--   0        0        0     1471 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4331 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      552 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0      270 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0       45 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      325 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      400 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      747 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      158 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0     2097 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      627 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      425 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      229 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     7729 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      383 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0      110 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     3551 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/config/__init__.py
+-rw-r--r--   0        0        0     1117 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/config/logging.py
+-rw-r--r--   0        0        0      185 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/errors/__init__.py
+-rw-r--r--   0        0        0       76 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/errors/method_not_implemented.py
+-rw-r--r--   0        0        0       52 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/errors/unsupported_file_extension.py
+-rw-r--r--   0        0        0       88 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/errors/variable_processing_error.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/generators/__init__.py
+-rw-r--r--   0        0        0     6415 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/generators/etl_generator.py
+-rw-r--r--   0        0        0      884 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/generators/generator.py
+-rw-r--r--   0        0        0      374 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/templates/etl_template
+-rw-r--r--   0        0        0        0 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/__init__.py
+-rw-r--r--   0        0        0      524 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/__init__.py
+-rw-r--r--   0        0        0     3484 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rw-r--r--   0        0        0     1128 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rw-r--r--   0        0        0      986 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rw-r--r--   0        0        0     1142 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rw-r--r--   0        0        0     1110 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rw-r--r--   0        0        0     1595 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rw-r--r--   0        0        0     2086 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rw-r--r--   0        0        0     1074 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rw-r--r--   0        0        0      935 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_variable.py
+-rw-r--r--   0        0        0       99 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/replace_template/__init__.py
+-rw-r--r--   0        0        0      963 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rw-r--r--   0        0        0     1678 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/usecases/replace_template/replace_template.py
+-rw-r--r--   0        0        0       32 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/utils/__init__.py
+-rw-r--r--   0        0        0     3631 2023-08-03 21:53:08.364954 sefazetllib-0.1.43/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 sefazetllib-0.1.43/PKG-INFO
```

### Comparing `sefazetllib-0.1.42/LICENSE` & `sefazetllib-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/README.md` & `sefazetllib-0.1.43/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/pyproject.toml` & `sefazetllib-0.1.43/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.42"
+version = "0.1.43"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
```

### Comparing `sefazetllib-0.1.42/sefazetllib/Builder.py` & `sefazetllib-0.1.43/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.43/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.43/sefazetllib/etl/ETL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.43/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.43/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.43/sefazetllib/extract/ExtractS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.43/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.43/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.43/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.43/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.43/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.43/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         schema = kwargs["schema"].lower()
         table = kwargs["table"].lower()
         self.conn.execute(text(f"TRUNCATE TABLE {schema}.{table}"))
         return
 
     def drop_constraints(self, **kwargs):
         table = kwargs["table"].lower()
+        schema = kwargs["schema"].lower()
         dependencies = [
             row._asdict()
             for row in self.conn.execute(
                 text(
                     f"""
         SELECT tc.table_schema,
             tc.constraint_name,
@@ -79,17 +80,17 @@
             ccu.table_schema AS foreign_table_schema,
             ccu.table_name AS foreign_table_name,
             ccu.column_name AS foreign_column_name
         FROM information_schema.table_constraints AS tc
             JOIN information_schema.key_column_usage AS kcu ON tc.constraint_name = kcu.constraint_name
             AND tc.table_schema = kcu.table_schema
             JOIN information_schema.constraint_column_usage AS ccu ON ccu.constraint_name = tc.constraint_name
-            AND ccu.table_schema = tc.table_schema
         WHERE tc.constraint_type = 'FOREIGN KEY'
             AND (tc.table_name = '{table}' OR ccu.table_name = '{table}')
+            AND (tc.table_schema = '{schema}' OR ccu.table_schema = '{schema}')
         """
                 )
             ).fetchall()
         ]
 
         alter_queries = [
             f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} DROP CONSTRAINT {dependencie['constraint_name']};"""
```

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.43/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/load/Load.py` & `sefazetllib-0.1.43/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.43/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.43/sefazetllib/load/LoadS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.43/sefazetllib/load/LoadSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/load/LoadStorage.py` & `sefazetllib-0.1.43/sefazetllib/load/LoadStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/transform/ColumnsToLowerCase.py` & `sefazetllib-0.1.43/sefazetllib/transform/ColumnsToLowerCase.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.43/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.43/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.43/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.43/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.43/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.43/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.43/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/__init__.py` & `sefazetllib-0.1.43/sefazetllibcli/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.43/sefazetllibcli/config/logging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.43/sefazetllibcli/generators/etl_generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.43/sefazetllibcli/generators/generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_imports_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_key_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_load_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_transforms_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_transforms_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/usecases/replace_template/replace_template.py` & `sefazetllib-0.1.43/sefazetllibcli/usecases/replace_template/replace_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.43/sefazetllibcli/utils/parse_etl.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.42/PKG-INFO` & `sefazetllib-0.1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.42
+Version: 0.1.43
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
```

