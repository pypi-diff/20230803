# Comparing `tmp/hdx_python_api-6.0.6.tar.gz` & `tmp/hdx_python_api-6.0.7.tar.gz`

## Comparing `hdx_python_api-6.0.6.tar` & `hdx_python_api-6.0.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    44094 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/main.md
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/api/locations.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   112315 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     6263 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    27463 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/conftest.py
--rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49390 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    47090 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/workingexample/run.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/LICENSE
--rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/README.md
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/pyproject.toml
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4978 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    44094 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/main.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24988 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4540 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/api/locations.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   112338 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9458 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     6883 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28580 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11098 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    27610 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4532 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7679 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15005 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9686 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22495 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3863 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169336 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13842 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      367 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      221 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1534 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842238 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48523 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38434 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45085 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/conftest.py
+-rwxr-xr-x   0        0        0    34761 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49390 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    75535 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11869 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0        0        0    19578 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    47292 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19114 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23055 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    63710 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21181 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116076 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5650 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/workingexample/run.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/LICENSE
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/README.md
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hdx_python_api-6.0.7/PKG-INFO
```

### Comparing `hdx_python_api-6.0.6/CONTRIBUTING.md` & `hdx_python_api-6.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/requirements.txt` & `hdx_python_api-6.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/.config/pre-commit-config.yaml` & `hdx_python_api-6.0.7/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/.github/workflows/publish.yaml` & `hdx_python_api-6.0.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.0.7/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/documentation/main.md` & `hdx_python_api-6.0.7/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.0.7/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/api/configuration.py` & `hdx_python_api-6.0.7/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.0.7/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/api/locations.py` & `hdx_python_api-6.0.7/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/dataset.py` & `hdx_python_api-6.0.7/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
         if scriptinfo:
             del kwargs["updated_by_script"]
         else:
             scriptinfo = self.configuration.get_user_agent()
         # No need to output timezone info here so no need to use now_utc()
         self.data[
             "updated_by_script"
-        ] = f"{scriptinfo} ({datetime.utcnow().isoformat()})"
+        ] = f"{scriptinfo} ({datetime.utcnow().isoformat(timespec='microseconds')})"
         batch = kwargs.get("batch")
         if batch:
             if not is_valid_uuid(batch):
                 raise HDXError(f"{batch} is not a valid UUID!")
             self.data["batch"] = batch
             del kwargs["batch"]
             if "batch_mode" not in kwargs:
```

### Comparing `hdx_python_api-6.0.6/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.0.7/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/date_helper.py` & `hdx_python_api-6.0.7/src/hdx/data/date_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,51 +6,63 @@
 
 from hdx.utilities.dateparse import now_utc, parse_date
 
 
 class DateHelper:
     @staticmethod
     def get_hdx_date(
-        date: Union[datetime, str], ignore_timeinfo: bool, max=False
+        date: Union[datetime, str],
+        ignore_timeinfo: bool,
+        include_microseconds=False,
+        max=False,
     ):
         """Get an HDX date as a string from a datetime.datetime object.
 
         Args:
             date (Union[datetime, str]): Date as datetime or string
             ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
+            include_microseconds (bool): Include microsconds. Defaults to False.
 
         Returns:
             str: HDX date as a string
         """
         if ignore_timeinfo:
             timezone_handling = 0
         else:
             timezone_handling = 3
 
         if isinstance(date, str):
-            date = parse_date(date, timezone_handling=timezone_handling)
+            date = parse_date(
+                date,
+                timezone_handling=timezone_handling,
+                include_microseconds=include_microseconds,
+            )
 
         if ignore_timeinfo:
             if max:
                 date = date.replace(
                     hour=23,
                     minute=59,
                     second=59,
-                    microsecond=0,
-                    tzinfo=None,
+                    microsecond=999999,
                 )
             else:
                 date = date.replace(
-                    hour=0, minute=0, second=0, microsecond=0, tzinfo=None
+                    hour=0,
+                    minute=0,
+                    second=0,
+                    microsecond=0,
                 )
         else:
-            date = date.astimezone(timezone.utc).replace(
-                microsecond=0, tzinfo=None
-            )
-        return date.isoformat()
+            date = date.astimezone(timezone.utc)
+        if include_microseconds:
+            timespec = "microseconds"
+        else:
+            timespec = "seconds"
+        return date.replace(tzinfo=None).isoformat(timespec=timespec)
 
     @staticmethod
     def get_reference_period_info(
         hdx_reference_period: Dict,
         date_format: Optional[str] = None,
         today: datetime = now_utc(),
     ) -> Dict:
@@ -89,16 +101,16 @@
                 ongoing = True
             else:
                 enddate = parse_date(enddate, max_time=True)
                 ongoing = False
             result["startdate"] = startdate
             result["enddate"] = enddate
             if date_format is None:
-                startdate_str = startdate.isoformat()
-                enddate_str = enddate.isoformat()
+                startdate_str = startdate.isoformat(timespec="seconds")
+                enddate_str = enddate.isoformat(timespec="seconds")
             else:
                 startdate_str = startdate.strftime(date_format)
                 enddate_str = enddate.strftime(date_format)
             result["startdate_str"] = startdate_str
             result["enddate_str"] = enddate_str
             result["ongoing"] = ongoing
         return result
@@ -119,22 +131,31 @@
             enddate (Union[datetime, str, None]): Dataset end date. Defaults to None.
             ongoing (bool): True if ongoing, False if not. Defaults to False.
             ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
 
         Returns:
             str: HDX reference period
         """
-        startdate = cls.get_hdx_date(startdate, ignore_timeinfo)
+        startdate = cls.get_hdx_date(
+            startdate,
+            ignore_timeinfo=ignore_timeinfo,
+            include_microseconds=False,
+        )
         if ongoing:
             enddate = "*"
         else:
             if not enddate:
                 enddate = startdate
             else:
-                enddate = cls.get_hdx_date(enddate, ignore_timeinfo, max=True)
+                enddate = cls.get_hdx_date(
+                    enddate,
+                    ignore_timeinfo=ignore_timeinfo,
+                    include_microseconds=False,
+                    max=True,
+                )
         return f"[{startdate} TO {enddate}]"
 
     @classmethod
     def get_hdx_reference_period_from_years(
         cls,
         startyear: Union[str, int, Iterable],
         endyear: Union[str, int, None] = None,
```

### Comparing `hdx_python_api-6.0.6/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.0.7/src/hdx/data/filestore_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,9 +96,11 @@
         merge_two_dictionaries(resource, updated_resource)
         cls.resource_check_required_fields(
             resource, check_upload=True, **kwargs
         )
         if resource.get_file_to_upload():
             resource["url"] = cls.temporary_url
         if data_updated:
-            resource["last_modified"] = datetime.utcnow().isoformat()
+            resource["last_modified"] = datetime.utcnow().isoformat(
+                timespec="microseconds"
+            )
             resource.data_updated = False
```

### Comparing `hdx_python_api-6.0.6/src/hdx/data/hdxobject.py` & `hdx_python_api-6.0.7/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.0.7/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/organization.py` & `hdx_python_api-6.0.7/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/resource.py` & `hdx_python_api-6.0.7/src/hdx/data/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,17 @@
             data_updated (bool): If True, set last_modified to now. Defaults to False.
 
         Returns:
             None
         """
         data_updated = kwargs.pop("data_updated", self.data_updated)
         if data_updated and not self.file_to_upload:
-            self.old_data["last_modified"] = datetime.utcnow().isoformat()
+            self.old_data["last_modified"] = datetime.utcnow().isoformat(
+                timespec="microseconds"
+            )
             self.data_updated = False
             # old_data will be merged into data in the next step
         self._merge_hdx_update(
             "resource", "id", self._get_files(), True, **kwargs
         )
 
     def update_in_hdx(self, **kwargs: Any) -> None:
@@ -765,24 +767,26 @@
 
     def get_date_data_updated(self) -> datetime:
         """Get date resource data was updated
 
         Returns:
             datetime: Date resource data was updated
         """
-        return parse_date(self.data["last_modified"])
+        return parse_date(
+            self.data["last_modified"], include_microseconds=True
+        )
 
     def set_date_data_updated(
-        self, date: Union[datetime, str], ignore_timeinfo: bool = True
+        self, date: Union[datetime, str], ignore_timeinfo: bool = False
     ) -> None:
         """Set date resource data was updated
 
         Args:
             date (Union[datetime, str]): Date resource data was updated
-            ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to True.
+            ignore_timeinfo (bool): Ignore time and time zone of date. Defaults to False.
 
         Returns:
             None
         """
         self.data["last_modified"] = DateHelper.get_hdx_date(
-            date, ignore_timeinfo
+            date, ignore_timeinfo=ignore_timeinfo, include_microseconds=True
         )
```

### Comparing `hdx_python_api-6.0.6/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.0.7/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/resource_view.py` & `hdx_python_api-6.0.7/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/showcase.py` & `hdx_python_api-6.0.7/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/user.py` & `hdx_python_api-6.0.7/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/data/vocabulary.py` & `hdx_python_api-6.0.7/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.0.7/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.0.7/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/src/hdx/facades/simple.py` & `hdx_python_api-6.0.7/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.0.7/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.0.7/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.0.7/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.0.7/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/resource_formats.json` & `hdx_python_api-6.0.7/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.0.7/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/test_data.csv` & `hdx_python_api-6.0.7/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/test_data.zip` & `hdx_python_api-6.0.7/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.0.7/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.0.7/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.0.7/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.0.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.0.7/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.0.7/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.0.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.0.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.0.7/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/conftest.py` & `hdx_python_api-6.0.7/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.0.7/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/api/test_locations.py` & `hdx_python_api-6.0.7/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/__init__.py` & `hdx_python_api-6.0.7/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_organization.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_resource.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1015,12 +1015,21 @@
     def test_date_data_updated(self, configuration, read):
         resource = Resource.read_from_hdx(
             "74b74ae1-df0c-4716-829f-4f939a046811"
         )
         assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
         assert resource["name"] == "MyResource1"
         assert resource["package_id"] == "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d"
-        resource.set_date_data_updated("2020-03-02")
-        expected = "2020-03-02T00:00:00+00:00"
-        assert resource.get_date_data_updated().isoformat() == expected
-        resource.set_date_data_updated(parse_date("2020-03-02"))
-        assert resource.get_date_data_updated().isoformat() == expected
+        date = "2020-03-02 10:34:43.123456"
+        resource.set_date_data_updated(date)
+        expected = "2020-03-02T10:34:43.123456+00:00"
+        assert (
+            resource.get_date_data_updated().isoformat(timespec="microseconds")
+            == expected
+        )
+        resource.set_date_data_updated(
+            parse_date(date, include_microseconds=True)
+        )
+        assert (
+            resource.get_date_data_updated().isoformat(timespec="microseconds")
+            == expected
+        )
```

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_user.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.0.7/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/facades/__init__.py` & `hdx_python_api-6.0.7/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.0.7/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.0.7/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.0.7/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/workingexample/my_resource.xlsx` & `hdx_python_api-6.0.7/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/.gitignore` & `hdx_python_api-6.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/LICENSE` & `hdx_python_api-6.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/README.md` & `hdx_python_api-6.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/pyproject.toml` & `hdx_python_api-6.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.0.6/PKG-INFO` & `hdx_python_api-6.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.6
+Version: 6.0.7
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
```

