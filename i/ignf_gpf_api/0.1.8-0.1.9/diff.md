# Comparing `tmp/ignf_gpf_api-0.1.8.tar.gz` & `tmp/ignf_gpf_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignf_gpf_api-0.1.8.tar", last modified: Fri Apr 21 17:10:34 2023, max compression
+gzip compressed data, was "ignf_gpf_api-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ignf_gpf_api-0.1.8.tar` & `ignf_gpf_api-0.1.9.tar`

### file list

```diff
@@ -1,198 +1,214 @@
--rw-r--r--   0        0        0     1400 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/ci-dev.yml
--rw-r--r--   0        0        0     1394 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/ci-prod.yml
--rw-r--r--   0        0        0      844 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0     1881 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.gitignore
--rw-r--r--   0        0        0    23461 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.pylintrc
--rw-r--r--   0        0        0      200 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.pypirc
--rw-r--r--   0        0        0     1981 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/.vscode/settings.json
--rw-r--r--   0        0        0    35149 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/LICENSE
--rw-r--r--   0        0        0      122 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0      415 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/README.md
--rwxr-xr-x   0        0        0      510 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/check.sh
--rw-r--r--   0        0        0     1956 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/Dockerfile
--rw-r--r--   0        0        0      671 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/README.md
--rw-r--r--   0        0        0      244 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/config/apache/website.conf
--rw-r--r--   0        0        0      291 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docker/docker-compose.yml
--rw-r--r--   0        0        0       42 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/.gitignore
--rw-r--r--   0        0        0     3083 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/comme-executable.md
--rw-r--r--   0        0        0       34 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/comme-module.md
--rw-r--r--   0        0        0     4133 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/configuration.md
--rw-r--r--   0        0        0    23974 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/configuration_details.md
--rw-r--r--   0        0        0      358 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/custom.css
--rw-r--r--   0        0        0     3577 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/development.md
--rw-r--r--   0        0        0    12108 2023-04-21 17:10:28.523663 ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.excalidraw
--rw-r--r--   0        0        0   241521 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.png
--rw-r--r--   0        0        0     1223 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/index.md
--rw-r--r--   0        0        0      115 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/auth.md
--rw-r--r--   0        0        0      234 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/io.md
--rw-r--r--   0        0        0      302 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/store.md
--rw-r--r--   0        0        0       60 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow.md
--rw-r--r--   0        0        0      290 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow/action.md
--rw-r--r--   0        0        0      340 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/reference/workflow/resolver.md
--rw-r--r--   0        0        0     5356 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/tutoriel_1_archive.md
--rw-r--r--   0        0        0     4551 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/tutoriel_2_flux_vecteur.md
--rw-r--r--   0        0        0     4171 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/upload_descriptor.md
--rw-r--r--   0        0        0       12 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/docs/workflow.md
--rw-r--r--   0        0        0      687 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/Errors.py
--rw-r--r--   0        0        0       82 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/__init__.py
--rw-r--r--   0        0        0    15799 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/__main__.py
--rw-r--r--   0        0        0     8997 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/default.ini
--rw-r--r--   0        0        0     2247 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json
--rw-r--r--   0        0        0     3001 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/workflow.json
--rw-r--r--   0        0        0      285 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON.md5
--rwxr-xr-x   0        0        0        5 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2297 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
--rwxr-xr-x   0        0        0      449 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
--rw-r--r--   0        0        0   430828 2023-04-21 17:10:28.527663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
--rw-r--r--   0        0        0      588 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
--rw-r--r--   0        0        0      529 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json
--rw-r--r--   0        0        0       57 2023-04-21 17:10:28.531663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON.md5
--rw-r--r--   0        0        0   991843 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
--rw-r--r--   0        0        0      525 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json
--rw-r--r--   0        0        0     4798 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/archive-generic.jsonc
--rw-r--r--   0        0        0     8404 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/wfs-generic.jsonc
--rw-r--r--   0        0        0     5790 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Authentifier.py
--rw-r--r--   0        0        0      270 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Errors.py
--rw-r--r--   0        0        0     1493 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Token.py
--rw-r--r--   0        0        0       46 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/auth/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/FileHelper.py
--rw-r--r--   0        0        0     6947 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/JsonHelper.py
--rw-r--r--   0        0        0      916 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/PrintLogHelper.py
--rw-r--r--   0        0        0       59 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/helper/__init__.py
--rw-r--r--   0        0        0    11135 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/ApiRequester.py
--rw-r--r--   0        0        0      607 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Color.py
--rw-r--r--   0        0        0     5018 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Config.py
--rw-r--r--   0        0        0     5310 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Dataset.py
--rw-r--r--   0        0        0     4037 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/DescriptorFileReader.py
--rw-r--r--   0        0        0     7308 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/Errors.py
--rw-r--r--   0        0        0     2752 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/JsonConverter.py
--rw-r--r--   0        0        0     4379 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/OutputManager.py
--rw-r--r--   0        0        0       47 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/io/__init__.py
--rw-r--r--   0        0        0      793 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/SingleInstance.py
--rw-r--r--   0        0        0      637 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/Singleton.py
--rw-r--r--   0        0        0       33 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/__init__.py
--rw-r--r--   0        0        0        1 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/py.typed
--rw-r--r--   0        0        0      218 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Check.py
--rw-r--r--   0        0        0     1025 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/CheckExecution.py
--rw-r--r--   0        0        0     1947 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Configuration.py
--rw-r--r--   0        0        0     2002 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Endpoint.py
--rw-r--r--   0        0        0      179 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Errors.py
--rw-r--r--   0        0        0      608 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Offering.py
--rw-r--r--   0        0        0      227 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Processing.py
--rw-r--r--   0        0        0     2378 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/ProcessingExecution.py
--rw-r--r--   0        0        0    11618 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoreEntity.py
--rw-r--r--   0        0        0      699 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoredData.py
--rw-r--r--   0        0        0     7653 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/Upload.py
--rw-r--r--   0        0        0       57 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/__init__.py
--rw-r--r--   0        0        0     2397 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CommentInterface.py
--rw-r--r--   0        0        0     1047 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CsfInterface.py
--rw-r--r--   0        0        0      768 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/EventInterface.py
--rw-r--r--   0        0        0      789 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/FullEditInterface.py
--rw-r--r--   0        0        0      831 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/PartialEditInterface.py
--rw-r--r--   0        0        0     2014 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/SharingInterface.py
--rw-r--r--   0        0        0     2255 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/TagInterface.py
--rw-r--r--   0        0        0       88 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/__init__.py
--rw-r--r--   0        0        0      204 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Errors.py
--rw-r--r--   0        0        0    14121 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Workflow.py
--rw-r--r--   0        0        0       40 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/__init__.py
--rw-r--r--   0        0        0     4424 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ActionAbstract.py
--rw-r--r--   0        0        0     5031 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ConfigurationAction.py
--rw-r--r--   0        0        0     4304 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/OfferingAction.py
--rw-r--r--   0        0        0    15865 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py
--rw-r--r--   0        0        0    11298 2023-04-21 17:10:28.535663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/UploadAction.py
--rw-r--r--   0        0        0       72 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/__init__.py
--rw-r--r--   0        0        0      802 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/AbstractResolver.py
--rw-r--r--   0        0        0     1271 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/DictResolver.py
--rw-r--r--   0        0        0     4333 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/Errors.py
--rw-r--r--   0        0        0     5295 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/FileResolver.py
--rw-r--r--   0        0        0     3469 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/GlobalResolver.py
--rw-r--r--   0        0        0     3489 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py
--rw-r--r--   0        0        0     1462 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/UserResolver.py
--rw-r--r--   0        0        0      110 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/mkdocs.yml
--rw-r--r--   0        0        0     1280 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      956 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/ErrorsTestCase.py
--rw-r--r--   0        0        0     1735 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/GpfTestCase.py
--rw-r--r--   0        0        0     3366 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/MainTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      336 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_authentifier.ini
--rw-r--r--   0        0        0      308 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_overload.ini
--rw-r--r--   0        0        0      313 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_requester.ini
--rw-r--r--   0        0        0       40 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_upload.ini
--rw-r--r--   0        0        0       69 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_conf/test_value_type.ini
--rw-r--r--   0        0        0      460 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
--rw-r--r--   0        0        0      341 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
--rw-r--r--   0        0        0        5 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2023-04-21 17:10:28.539663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
--rw-r--r--   0        0        0       11 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
--rw-r--r--   0        0        0        5 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2023-04-21 17:10:28.547663 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
--rw-r--r--   0        0        0     2659 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_data/workflows/bad-workflow.jsonc
--rw-r--r--   0        0        0       53 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/FileHelper/md5.txt
--rw-r--r--   0        0        0       78 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_not_parsable.json
--rw-r--r--   0        0        0       52 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_not_valid.json
--rw-r--r--   0        0        0      108 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/json_parsable.json
--rw-r--r--   0        0        0      563 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema.json
--rw-r--r--   0        0        0      485 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema_invalid.json
--rw-r--r--   0        0        0       23 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/dict.json
--rw-r--r--   0        0        0       21 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/list.json
--rw-r--r--   0        0        0        2 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/not-valid.json
--rw-r--r--   0        0        0       31 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/_test/workflow/resolver/FileResolver/text.txt
--rw-r--r--   0        0        0     7383 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/auth/AuthentifierTestCase.py
--rw-r--r--   0        0        0     1183 2023-04-21 17:10:28.555662 ignf_gpf_api-0.1.8/tests/auth/TokenTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/auth/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/FileHelperTestCase.py
--rw-r--r--   0        0        0     9959 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/JsonHelperTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/helper/__init__.py
--rw-r--r--   0        0        0    13575 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ApiRequesterTestCase.py
--rw-r--r--   0        0        0     3595 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ConfigTestCase.py
--rw-r--r--   0        0        0     2218 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/DatasetTestCase.py
--rw-r--r--   0        0        0     1716 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/DescriptorFileReaderTestCase.py
--rw-r--r--   0        0        0     1974 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/ErrorsTestCase.py
--rw-r--r--   0        0        0     1198 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/JsonConverterTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/io/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/CheckExecutionTestCase.py
--rw-r--r--   0        0        0     2855 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ConfigurationTestCase.py
--rw-r--r--   0        0        0     3487 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/EndpointTestCase.py
--rw-r--r--   0        0        0     1144 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ErrorsTestCase.py
--rw-r--r--   0        0        0     1504 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/EventInterfaceTestCase.py
--rw-r--r--   0        0        0     3865 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/ProcessingExecutionTestCase.py
--rw-r--r--   0        0        0    18439 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/StoreEntityTestCase.py
--rw-r--r--   0        0        0    11477 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/UploadTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/__init__.py
--rw-r--r--   0        0        0     4538 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/CommentInterfaceTestCase.py
--rw-r--r--   0        0        0     2532 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/CsfInterfaceTestCase.py
--rw-r--r--   0        0        0     1699 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/FullEditInterfaceTestCase.py
--rw-r--r--   0        0        0     1745 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/PartialEditInterfaceTestCase.py
--rw-r--r--   0        0        0     3585 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/SharingInterfaceTestCase.py
--rw-r--r--   0        0        0     3600 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/TagInterfaceTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/store/interface/__init__.py
--rw-r--r--   0        0        0    14646 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/WorkflowTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/__init__.py
--rw-r--r--   0        0        0     3100 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ActionAbstractTestCase.py
--rw-r--r--   0        0        0     5384 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ConfigurationActionTestCase.py
--rw-r--r--   0        0        0     7133 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/OfferingActionTestCase.py
--rw-r--r--   0        0        0    16012 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/ProcessingExecutionActionTestCase.py
--rw-r--r--   0        0        0    19409 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/UploadActionTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/action/__init__.py
--rw-r--r--   0        0        0     1116 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/DictResolverTestCase.py
--rw-r--r--   0        0        0     4492 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/FileResolverTestCase.py
--rw-r--r--   0        0        0     2492 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/GlobalResolverTestCase.py
--rw-r--r--   0        0        0     6705 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/StoreEntityResolverTestCase.py
--rw-r--r--   0        0        0     2225 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/UserResolverTestCase.py
--rw-r--r--   0        0        0        0 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/tests/workflow/resolver/__init__.py
--rw-r--r--   0        0        0   116760 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/classes.png
--rw-r--r--   0        0        0     9175 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/classes.uxf
--rw-r--r--   0        0        0    43510 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/interfaces.png
--rw-r--r--   0        0        0     7059 2023-04-21 17:10:28.559663 ignf_gpf_api-0.1.8/uml/interfaces.uxf
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 ignf_gpf_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1400 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.github/workflows/ci-dev.yml
+-rw-r--r--   0        0        0     1394 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.github/workflows/ci-prod.yml
+-rw-r--r--   0        0        0      844 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0     1961 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.gitignore
+-rw-r--r--   0        0        0    23461 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.pylintrc
+-rw-r--r--   0        0        0      200 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.pypirc
+-rw-r--r--   0        0        0     2279 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/.vscode/settings.json
+-rw-r--r--   0        0        0    35149 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/LICENSE
+-rw-r--r--   0        0        0      122 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0      415 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/README.md
+-rwxr-xr-x   0        0        0      653 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/check.sh
+-rw-r--r--   0        0        0     1956 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docker/Dockerfile
+-rw-r--r--   0        0        0      671 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docker/README.md
+-rw-r--r--   0        0        0      244 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docker/config/apache/website.conf
+-rw-r--r--   0        0        0      291 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docker/docker-compose.yml
+-rw-r--r--   0        0        0       42 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/.gitignore
+-rw-r--r--   0        0        0     4130 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/comme-executable.md
+-rw-r--r--   0        0        0       34 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/comme-module.md
+-rw-r--r--   0        0        0     4133 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/configuration.md
+-rw-r--r--   0        0        0    23974 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/configuration_details.md
+-rw-r--r--   0        0        0      358 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/custom.css
+-rw-r--r--   0        0        0     4351 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/development.md
+-rw-r--r--   0        0        0    12108 2023-07-10 11:39:19.051128 ignf_gpf_api-0.1.9/docs/images/index__utilisation_module.excalidraw
+-rw-r--r--   0        0        0   241521 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/images/index__utilisation_module.png
+-rw-r--r--   0        0        0     1223 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/index.md
+-rw-r--r--   0        0        0      115 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/auth.md
+-rw-r--r--   0        0        0      298 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/io.md
+-rw-r--r--   0        0        0      302 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/store.md
+-rw-r--r--   0        0        0       60 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/workflow.md
+-rw-r--r--   0        0        0      290 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/workflow/action.md
+-rw-r--r--   0        0        0      340 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/reference/workflow/resolver.md
+-rw-r--r--   0        0        0     5356 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/tutoriel_1_archive.md
+-rw-r--r--   0        0        0     6730 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/tutoriel_2_flux_vecteur.md
+-rw-r--r--   0        0        0     5197 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/tutoriel_3_flux_raster.md
+-rw-r--r--   0        0        0     4171 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/upload_descriptor.md
+-rw-r--r--   0        0        0       12 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/docs/workflow.md
+-rw-r--r--   0        0        0      687 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/Errors.py
+-rw-r--r--   0        0        0       82 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/__init__.py
+-rw-r--r--   0        0        0    16718 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/__main__.py
+-rw-r--r--   0        0        0     9192 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/default.ini
+-rw-r--r--   0        0        0     2183 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json
+-rw-r--r--   0        0        0     3001 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/json_schemas/workflow.json
+-rw-r--r--   0        0        0      255 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON.md5
+-rwxr-xr-x   0        0        0        5 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2297 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
+-rwxr-xr-x   0        0        0      655 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
+-rw-r--r--   0        0        0   430828 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      588 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
+-rw-r--r--   0        0        0     4003 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON_style.sld
+-rw-r--r--   0        0        0      529 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json
+-rw-r--r--   0        0        0       52 2023-07-10 11:39:19.055128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON.md5
+-rw-r--r--   0        0        0   991843 2023-07-10 11:39:19.063128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
+-rw-r--r--   0        0        0      525 2023-07-10 11:39:19.063128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json
+-rw-r--r--   0        0        0     4391 2023-07-10 11:39:19.063128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
+-rw-r--r--   0        0        0      411 2023-07-10 11:39:19.063128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
+-rw-r--r--   0        0        0   368640 2023-07-10 11:39:19.063128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
+-rw-r--r--   0        0        0   676357 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
+-rw-r--r--   0        0        0       84 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
+-rw-r--r--   0        0        0     1731 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
+-rw-r--r--   0        0        0     4836 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/archive-generic.jsonc
+-rw-r--r--   0        0        0     9481 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/generic-raster_gpf.jsonc
+-rw-r--r--   0        0        0    13499 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/generic_joincache.jsonc
+-rw-r--r--   0        0        0    10970 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/generic_moissonnage.jsonc
+-rw-r--r--   0        0        0    10143 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/generique-maj-bdd_gpf.jsonc
+-rw-r--r--   0        0        0    15069 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/wfs-generic.jsonc
+-rw-r--r--   0        0        0     7603 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/auth/Authentifier.py
+-rw-r--r--   0        0        0      270 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/auth/Errors.py
+-rw-r--r--   0        0        0     1493 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/auth/Token.py
+-rw-r--r--   0        0        0       46 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/auth/__init__.py
+-rw-r--r--   0        0        0     2585 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/helper/FileHelper.py
+-rw-r--r--   0        0        0     6947 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/helper/JsonHelper.py
+-rw-r--r--   0        0        0      916 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/helper/PrintLogHelper.py
+-rw-r--r--   0        0        0       59 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/helper/__init__.py
+-rw-r--r--   0        0        0    11417 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/ApiRequester.py
+-rw-r--r--   0        0        0      607 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/Color.py
+-rw-r--r--   0        0        0     5683 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/Config.py
+-rw-r--r--   0        0        0     5310 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/Dataset.py
+-rw-r--r--   0        0        0     4041 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/DescriptorFileReader.py
+-rw-r--r--   0        0        0     7308 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/Errors.py
+-rw-r--r--   0        0        0     2764 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/JsonConverter.py
+-rw-r--r--   0        0        0     4379 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/OutputManager.py
+-rw-r--r--   0        0        0       47 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/io/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/pattern/SingleInstance.py
+-rw-r--r--   0        0        0      637 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/pattern/Singleton.py
+-rw-r--r--   0        0        0       33 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/pattern/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/py.typed
+-rw-r--r--   0        0        0      218 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Check.py
+-rw-r--r--   0        0        0     1337 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/CheckExecution.py
+-rw-r--r--   0        0        0     1947 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Configuration.py
+-rw-r--r--   0        0        0     2350 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Datastore.py
+-rw-r--r--   0        0        0     2002 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Endpoint.py
+-rw-r--r--   0        0        0      179 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Errors.py
+-rw-r--r--   0        0        0      608 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Offering.py
+-rw-r--r--   0        0        0      227 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Processing.py
+-rw-r--r--   0        0        0     2690 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/ProcessingExecution.py
+-rw-r--r--   0        0        0     1176 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Static.py
+-rw-r--r--   0        0        0    11554 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/StoreEntity.py
+-rw-r--r--   0        0        0      699 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/StoredData.py
+-rw-r--r--   0        0        0     7661 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/Upload.py
+-rw-r--r--   0        0        0      211 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/User.py
+-rw-r--r--   0        0        0       57 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/__init__.py
+-rw-r--r--   0        0        0     2397 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/CommentInterface.py
+-rw-r--r--   0        0        0     1047 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/CsfInterface.py
+-rw-r--r--   0        0        0      768 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/EventInterface.py
+-rw-r--r--   0        0        0      789 2023-07-10 11:39:19.067128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/FullEditInterface.py
+-rw-r--r--   0        0        0      831 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/PartialEditInterface.py
+-rw-r--r--   0        0        0     2014 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/SharingInterface.py
+-rw-r--r--   0        0        0     2255 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/TagInterface.py
+-rw-r--r--   0        0        0       88 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/Errors.py
+-rw-r--r--   0        0        0    14116 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/Workflow.py
+-rw-r--r--   0        0        0       40 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/__init__.py
+-rw-r--r--   0        0        0     5134 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ActionAbstract.py
+-rw-r--r--   0        0        0     5031 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ConfigurationAction.py
+-rw-r--r--   0        0        0     4660 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/OfferingAction.py
+-rw-r--r--   0        0        0    16013 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py
+-rw-r--r--   0        0        0    14407 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/UploadAction.py
+-rw-r--r--   0        0        0       72 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/__init__.py
+-rw-r--r--   0        0        0      802 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/AbstractResolver.py
+-rw-r--r--   0        0        0     1271 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/DictResolver.py
+-rw-r--r--   0        0        0     4333 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/Errors.py
+-rw-r--r--   0        0        0     5300 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/FileResolver.py
+-rw-r--r--   0        0        0     3473 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/GlobalResolver.py
+-rw-r--r--   0        0        0     3671 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py
+-rw-r--r--   0        0        0     1462 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/UserResolver.py
+-rw-r--r--   0        0        0      110 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/mkdocs.yml
+-rw-r--r--   0        0        0     1293 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      956 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1735 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/GpfTestCase.py
+-rw-r--r--   0        0        0     3366 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/MainTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_conf/test_authentifier.ini
+-rw-r--r--   0        0        0      308 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_conf/test_overload.ini
+-rw-r--r--   0        0        0      313 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_conf/test_requester.ini
+-rw-r--r--   0        0        0       40 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_conf/test_upload.ini
+-rw-r--r--   0        0        0       69 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_conf/test_value_type.ini
+-rw-r--r--   0        0        0      460 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
+-rw-r--r--   0        0        0      305 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
+-rw-r--r--   0        0        0        5 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2023-07-10 11:39:19.071128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
+-rw-r--r--   0        0        0       11 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
+-rw-r--r--   0        0        0        5 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2023-07-10 11:39:19.079128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
+-rw-r--r--   0        0        0     2659 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_data/workflows/bad-workflow.jsonc
+-rw-r--r--   0        0        0       53 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_test/helper/FileHelper/md5.txt
+-rw-r--r--   0        0        0       78 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/json_not_parsable.json
+-rw-r--r--   0        0        0       52 2023-07-10 11:39:19.087128 ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/json_not_valid.json
+-rw-r--r--   0        0        0      108 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/json_parsable.json
+-rw-r--r--   0        0        0      563 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/schema.json
+-rw-r--r--   0        0        0      485 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/schema_invalid.json
+-rw-r--r--   0        0        0       23 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/workflow/resolver/FileResolver/dict.json
+-rw-r--r--   0        0        0       21 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/workflow/resolver/FileResolver/list.json
+-rw-r--r--   0        0        0        2 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/workflow/resolver/FileResolver/not-valid.json
+-rw-r--r--   0        0        0       31 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/_test/workflow/resolver/FileResolver/text.txt
+-rw-r--r--   0        0        0     7398 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/auth/AuthentifierTestCase.py
+-rw-r--r--   0        0        0     1183 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/auth/TokenTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/auth/__init__.py
+-rw-r--r--   0        0        0     1056 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/helper/FileHelperTestCase.py
+-rw-r--r--   0        0        0     9959 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/helper/JsonHelperTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/helper/__init__.py
+-rw-r--r--   0        0        0    13575 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/ApiRequesterTestCase.py
+-rw-r--r--   0        0        0     3595 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/ConfigTestCase.py
+-rw-r--r--   0        0        0     2213 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/DatasetTestCase.py
+-rw-r--r--   0        0        0     1716 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/DescriptorFileReaderTestCase.py
+-rw-r--r--   0        0        0     1974 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1198 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/JsonConverterTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/io/__init__.py
+-rw-r--r--   0        0        0     1777 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/CheckExecutionTestCase.py
+-rw-r--r--   0        0        0     2855 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/ConfigurationTestCase.py
+-rw-r--r--   0        0        0     4124 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/DatastoreTestCase.py
+-rw-r--r--   0        0        0     3487 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/EndpointTestCase.py
+-rw-r--r--   0        0        0     1144 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1504 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/EventInterfaceTestCase.py
+-rw-r--r--   0        0        0     4215 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/ProcessingExecutionTestCase.py
+-rw-r--r--   0        0        0    18421 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/StoreEntityTestCase.py
+-rw-r--r--   0        0        0    11477 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/UploadTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/__init__.py
+-rw-r--r--   0        0        0     4538 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/CommentInterfaceTestCase.py
+-rw-r--r--   0        0        0     2532 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/CsfInterfaceTestCase.py
+-rw-r--r--   0        0        0     1699 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/FullEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     1745 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/PartialEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     3585 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/SharingInterfaceTestCase.py
+-rw-r--r--   0        0        0     3600 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/TagInterfaceTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/store/interface/__init__.py
+-rw-r--r--   0        0        0    14646 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/WorkflowTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/__init__.py
+-rw-r--r--   0        0        0     3347 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/ActionAbstractTestCase.py
+-rw-r--r--   0        0        0     5384 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/ConfigurationActionTestCase.py
+-rw-r--r--   0        0        0     8112 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/OfferingActionTestCase.py
+-rw-r--r--   0        0        0    16731 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/ProcessingExecutionActionTestCase.py
+-rw-r--r--   0        0        0    21477 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/UploadActionTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/action/__init__.py
+-rw-r--r--   0        0        0     1116 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/DictResolverTestCase.py
+-rw-r--r--   0        0        0     4492 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/FileResolverTestCase.py
+-rw-r--r--   0        0        0     3034 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/GlobalResolverTestCase.py
+-rw-r--r--   0        0        0     8243 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/StoreEntityResolverTestCase.py
+-rw-r--r--   0        0        0     2225 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/UserResolverTestCase.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/tests/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0   116760 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/uml/classes.png
+-rw-r--r--   0        0        0     9175 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/uml/classes.uxf
+-rw-r--r--   0        0        0    43510 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/uml/interfaces.png
+-rw-r--r--   0        0        0     7059 2023-07-10 11:39:19.091129 ignf_gpf_api-0.1.9/uml/interfaces.uxf
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 ignf_gpf_api-0.1.9/PKG-INFO
```

### Comparing `ignf_gpf_api-0.1.8/.github/workflows/ci-dev.yml` & `ignf_gpf_api-0.1.9/.github/workflows/ci-dev.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/.github/workflows/ci-prod.yml` & `ignf_gpf_api-0.1.9/.github/workflows/ci-prod.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/.github/workflows/code-quality.yml` & `ignf_gpf_api-0.1.9/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/.gitignore` & `ignf_gpf_api-0.1.9/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -127,10 +127,16 @@
 
 # Pyre type checker
 .pyre/
 
 # Fichier de config personnel
 config.ini
 config_*.ini
+config-*.ini
 test.ini
+
+# Fichier python de test
 test.py
 test_*.py
+/*_dataset_*
+/*.jsonc
+/dpsg2023-06-00043
```

### Comparing `ignf_gpf_api-0.1.8/.pylintrc` & `ignf_gpf_api-0.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/.vscode/settings.json` & `ignf_gpf_api-0.1.9/.vscode/settings.json`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 {
     "cSpell.words": [
+        "autorefs",
         "bbox",
         "dateutil",
         "EPSG",
+        "fontawesome",
         "Géoplateforme",
+        "GEOSERVER",
         "geotuileur",
         "ignf",
+        "inlinehilite",
         "insee",
         "isoparse",
         "jsonschema",
+        "linenums",
         "mkapi",
         "mkdocs",
+        "mkdocstrings",
         "mypy",
         "parsables",
         "pathes",
         "pathlib",
+        "processings",
         "pylint",
         "pylintrc",
+        "pymdownx",
+        "pyotp",
         "pypi",
         "pypirc",
         "rcfile",
         "recupere",
         "requêtage",
         "setuptools",
         "sharings",
         "sidc",
+        "superfences",
         "testpypi",
         "tippecanoe",
+        "totp",
+        "unicode",
         "UNPUBLISHING",
         "venv",
         "virtualenv",
         "WMTS",
         "workdir"
     ],
     // On définit la docstring de base comme étant celle de google
@@ -73,8 +85,9 @@
         "-s",
         "./tests",
         "-p",
         "*TestCase.py"
     ],
     "python.testing.pytestEnabled": false,
     "python.testing.unittestEnabled": true,
+    "pylint.importStrategy": "fromEnvironment",
 }
```

### Comparing `ignf_gpf_api-0.1.8/LICENSE` & `ignf_gpf_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docker/Dockerfile` & `ignf_gpf_api-0.1.9/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docker/README.md` & `ignf_gpf_api-0.1.9/docker/README.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/comme-executable.md` & `ignf_gpf_api-0.1.9/docs/comme-executable.md`

 * *Files 27% similar despite different names*

```diff
@@ -18,14 +18,49 @@
 
 Cela devrait renvoyer :
 
 ``` txt
 Authentification réussie.
 ```
 
+## Mes datastores
+
+Dans la configuration, vous devez indiquer l'identifiant du datastore à utiliser.
+
+Si vous ne le connaissez pas, il est possible de lister les communautés auxquelles vous participez et, pour chacune d'elle, le datastore qui lui est associé.
+
+Commande pour lister les communautés auxquelles vous appartenez :
+
+```sh
+python -m ignf_gpf_api me
+```
+
+Cela devrait renvoyer :
+
+```
+Vos informations :
+  * email : prenom.nom@me.io
+  * nom : Prénom Nom
+  * votre id : 100000000000000000000024
+
+Vous êtes membre de 1 communauté(s) :
+
+  * communauté « Bac à sable » :
+      - id de la communauté : 200000000000000000000024
+      - id du datastore : 300000000000000000000024
+      - nom technique : bac-a-sable
+      - droits : community, uploads, processings, datastore, stored_data, broadcast
+```
+
+Dans cet exemple, l'identifiant du datastore à utiliser est `300000000000000000000024`.
+
+!!! warning "Attention"
+
+    Cela ne fonctionnera que si les autres paramètres (nom d'utilisateur, mot de passe et urls) sont corrects.
+
 
 ## Afficher toute la configuration
 
 Vous pouvez afficher toute la configuration via une commande. Cela peut vous permettre d'avoir une liste exhaustive des paramètres disponibles et de vérifier que votre fichier de configuration a bien le dernier mot sur les paramètres à utiliser.
 
 Affichez la configuration :
```

### Comparing `ignf_gpf_api-0.1.8/docs/configuration.md` & `ignf_gpf_api-0.1.9/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/configuration_details.md` & `ignf_gpf_api-0.1.9/docs/configuration_details.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/development.md` & `ignf_gpf_api-0.1.9/docs/development.md`

 * *Files 16% similar despite different names*

```diff
@@ -95,23 +95,39 @@
   - Config().om.debug("message")
   - Config().om.info("message")
   - Config().om.warning("message")
   - Config().om.error("message")
   - Config().om.critical("message")
 - Configuration centralisée via la classe Config()​ (cf. [Utilisation comme module Python](comme-module.md))
 
+## Déploiement des version dev et prod sur PyPI
 
-## Publication sur PyPI
+### Mise à jour des branches prod et dev
 
-La publication du package sur PyPI est automatique sur Github après la [création d'une release](https://github.com/ignf-sidc/ignf-gpf-api/releases/new) :
+Pour effectuer un déploiment de la librairie ignf-gpf-api, il faut d'abord modifier le numéro de version dans le fichier __init__.py dans le dossier ignf_gpf_api/ignf_gpf_api/ .
+
+Puis il faut résoudre ou faire les pull request entre dev et prod en fonction de l'avancement du projet pour avoir des branches dev et prod à jour.
+
+```py
+__version__ = <x.y.z>
+```
+
+### Création de la (pre)-release
+
+Pour publier une nouvelle version, qui va être ensuite publiée comme librairie sur PyPi, il faut [créer une (pre)-release](https://github.com/ignf-sidc/ignf-gpf-api/releases/new) :
 * créez une release de test sur la branche **dev** versionnée selon le modèle `tx.y.z` (ex : t1.2.3) pour déployer une nouvelle version du module en test ;
 * créez une release sur la branche **prod** versionnée selon le modèle `vx.y.z` (ex : v1.2.3) pour déployer une nouvelle version du module en production ;
 
-Si besoin, voici les commandes pour l'effectuer à la main :
+### Publication sur PyPI
+
+La publication du package sur PyPI est automatique sur Github grâce aux actions [CI Dev](https://github.com/ignf-sidc/ignf-gpf-api/actions/workflows/ci-dev.yml) et [CI Prod](https://github.com/ignf-sidc/ignf-gpf-api/actions/workflows/ci-prod.yml) :
 
+
+Si besoin, voici les commandes pour l'effectuer à la main :
+ 
 ```sh
 export FLIT_PASSWORD=<token>
 ```
 
 Publication sur TestPyPI :
 
 ```sh
```

### Comparing `ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.excalidraw` & `ignf_gpf_api-0.1.9/docs/images/index__utilisation_module.excalidraw`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/images/index__utilisation_module.png` & `ignf_gpf_api-0.1.9/docs/images/index__utilisation_module.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/index.md` & `ignf_gpf_api-0.1.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/tutoriel_1_archive.md` & `ignf_gpf_api-0.1.9/docs/tutoriel_1_archive.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/docs/tutoriel_2_flux_vecteur.md` & `ignf_gpf_api-0.1.9/docs/tutoriel_3_flux_raster.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,125 @@
-# Tutoriel 2 : publier un flux vecteur
+# Tutoriel 3 : publier un flux raster
 
-La Géoplateforme permet d'héberger des flux vecteur pour permettre à vos utilisateur de les télécharger/utiliser.
+La Géoplateforme permet d'héberger des flux raster pour permettre à vos utilisateur de les télécharger/utiliser.
 
-Pour cela, vous devez téléverser des données « vecteur » sur lesquelles la Géoplateforme va effectuer des traitements.
+Pour cela, vous devez téléverser des données « raster » sur lesquelles la Géoplateforme va effectuer des traitements.
 
 Pour commencer, nous vous conseillons de suivre ce tutoriel qui vous permet de manipuler des données déjà existantes. Vous pouvez ensuite adapter chaque étape pour livrer vos données.
 
 ## Définition de la configuration
 
 Suivez la page [configuration](configuration.md) pour définir le fichier de configuration.
 
 ## Récupération du jeu de données
 
-Le jeu de données « 1_dataset_vector » contient des données vecteur à téléverser.
+Le jeu de données « 1_dataset_raster » contient des données raster à téléverser.
 
 Récupérez les données en lançant la commande :
 
 ```sh
-python -m ignf_gpf_api dataset -n 1_dataset_vector
+python -m ignf_gpf_api dataset -n 4_dataset_raster_gpf
 ```
 
-Observez la structure des données :
+Observez la structure du fichier :
 
-```
-1_dataset_vector/
-├── CANTON
-│   ├── CANTON.cpg
-│   ├── CANTON.dbf
-│   ├── CANTON.prj
-│   ├── CANTON.shp
-│   └── CANTON.shx
-├── CANTON.md5
-└── upload_descriptor.json
+```text
+4_dataset_raster_gpf/
+├── test
+│   ├── 977-2018-0510-1979-U20N-0M50-E100.jp2
+│   ├── 977-2018-0510-1979-U20N-0M50-E100.tab
+│   ├── 977-2018-0510-1980-U20N-0M50-E100.jp2
+│   ├── 977-2018-0510-1980-U20N-0M50-E100.tab
+│   ├── 977-2018-0510-1981-U20N-0M50-E100.jp2
+│   ├── 977-2018-0510-1981-U20N-0M50-E100.tab
+│   ├── 977-2018-0510-1982-U20N-0M50-E100.jp2
+│   └── 977-2018-0510-1982-U20N-0M50-E100.tab
+├── test.md5
+└── upload_descriptor.jsonc
 ```
 
-Les données que la Géoplateforme va traiter sont situées dans le dossier `CANTON`.
-Le fichier `CANTON.md5` permettra de valider les données téléversées côté Géoplateforme.
+Les données que la Géoplateforme va traiter sont situées dans le dossier `test`.
+Le fichier `test.md5` permettra de valider les données téléversées côté Géoplateforme.
 
 Enfin, le fichier `upload_descriptor.json` permet de décrire la livraison à effectuer.
 
-
 ## Fichier descripteur de livraison
 
-Ouvrez le fichier pour avoir plus de détails.
+Ouvrez le fichier `upload_descriptor.json` pour avoir plus de détails.
 
 Il est composé d'une liste de `datasets` représentant chacun une livraison distincte.
 
 Chaque dataset contient :
 
 * la liste des dossiers à téléverser ;
 * les informations de la livraison à créer (nom, description, srs et type) ;
-* les commentaires et les tags à ajouter à la livraison.
+* les commentaires et les tags à ajouter à la livraison. (Memo : les commentaires ne sont pas encore supporter par la version actuel de la gpf)
 
 ## Livraison des données
 
 Livrer les données en indiquant le chemin du fichier descripteur au programme :
 
 ```sh
-python -m ignf_gpf_api upload -f 1_dataset_vector/upload_descriptor.json
+python -m ignf_gpf_api upload -f 4_dataset_raster_gpf/upload_descriptor.jsonc
 ```
 
-Le programme doit vous indiquer que le transfert est en cours, puis qu'il attend la fin des vérifications côté API avant de conclure que tout est bon.
+Le programme doit vous indiquer que le transfert est en cours, puis qu'il attend la fin des vérification côté API avant de conclure que tout est bon. (Memo : cette partie est assez longue du à des problèmes de performance côté Wordline. Le problème a déjà été remonté.)
 
 ## Workflow
 
 Une fois les données livrées, il faut traiter les données avant de les publier (c'est à dire effectuer un (ou plusieurs) géo-traitement(s),
 puis configurer un géo-service et le rendre accessible).
 
-Ces étapes sont décrites grâce à un workflow.
+Ces étapes sont décrites grâces à un workflow.
 
 Vous pouvez récupérer un workflow d'exemple grâce à la commande suivante :
 
 ```sh
-python -m ignf_gpf_api workflow -n wfs-generic.jsonc
+python -m ignf_gpf_api workflow -n generic-raster_gpf.jsonc
 ```
 
 Ouvrez le fichier. Vous trouverez plus de détails dans la [documentation sur les workflows](workflow.md), mais vous pouvez dès à présent voir que le workflow est composé de 4 étapes. Il faudra lancer une commande pour chacune d'elles.
 
 ```mermaid
 ---
-title: Workflow de publication de données vecteur en pyramide WFS
+title: Workflow de publication de données Rasteur en WMS et WMST
 ---
 %% doc mermaid ici https://mermaid-js.github.io/mermaid/#/flowchart?id=flowcharts-basic-syntax
 flowchart TD
-    A("upload") -->|mise-en-base| B("donnée stockée : BDD")
-    B -->|création-pyramide| C(donnée stockée : pyramide)
-    C -->|configuration-wfs| D(configuration)
-    D -->|publication-wfs| E(offre)
+    A("upload") -->|pyramide| B("pyramide rasteur")
+    B -->|configuration-WMST| C("configuration WMST")
+    C -->|publication-WMST| D("offre WMST")
+    B -->|configuration-WMS| E("configuration WMS")
+    E -->|publication-WMS| F("offre WMS")
 ```
 
 ## Traitement et publication
 
-Le workflow « wfs-generic » permet de passer de la livraison à un flux WFS servant la donnée. Il comporte 4 étapes :
+Le workflow « wms-generic » permet de passer de la livraison à un flux WMS servant la donnée. Il comporte les étapes suivantes:
 
-* `mise-en-base` : mise en base des données vecteur livrées ;
-* `création-pyramide` : création de la pyramide de vecteur pour l'utilisation dans un flux ;
-* `configuration-wfs` : configuration d'un service de flux WFS permettant d'utiliser les données vecteur ;
-* `publication-wfs` : publication du service de flux WFS sur le bon endpoint.
+* `pyramide` : création d'une pyramide avec les données en uploader
+* `configuration-WMST` : configuration d'un service de flux WMST à partir de la pyramide ;
+* `publication-WMST` : publication du service de flux WMST sur le bon endpoint.
+* `configuration-WMS` : configuration d'un service de flux WMS à partir de la pyramide ;
+* `publication-WMS` : publication du service de flux WMS sur le bon endpoint.
 
-Lancez les 4 commandes suivantes pour exécuter les 4 étapes :
+La partie WMST et WMS sont indépendante : Il n'y a pas besoin
+
+Les commandes à lancé sont les suivantes :
 
 ```sh
-python -m ignf_gpf_api workflow -f wfs-generic.jsonc -s mise-en-base
-python -m ignf_gpf_api workflow -f wfs-generic.jsonc -s création-pyramide
-python -m ignf_gpf_api workflow -f wfs-generic.jsonc -s configuration-wfs
-python -m ignf_gpf_api workflow -f wfs-generic.jsonc -s publication-wfs
+python -m ignf_gpf_api workflow -f generic-raster_gpf.jsonc -s pyramide
+# partie publication WMST
+python -m ignf_gpf_api workflow -f generic-raster_gpf.jsonc -s configuration-WMST
+python -m ignf_gpf_api workflow -f generic-raster_gpf.jsonc -s publication-WMST
+# partie publication WMS
+python -m ignf_gpf_api workflow -f generic-raster_gpf.jsonc -s configuration-WMS
+python -m ignf_gpf_api workflow -f generic-raster_gpf.jsonc -s publication-WMS
 ```
 
-Les deux premières commandes ne doivent pas être instantanées : un traitement est effectué et les logs doivent vous être remontés.
+La première commandes ne doit pas être instantanée : un traitement est effectué et les logs doivent vous être remontés.
 
 Le deux traitements suivants sont instantanés. A la fin, vous devez voir s'afficher un lien.
 
 Exemple :
 
-```
-INFO - Offre créée : Offering(id=62c708e72246434ac40ee3ad)
-   - download|https://geoservices-geotuileur.ccs-ign-plage.ccs.cegedim.cloud/download/plage/
-```
-
-Suivez le lien indiqué pour retrouver le flux WFS.
-
-Vous pouvez alors utiliser le flux.
+//TODO faire l'exemple récupération lien données WMS
```

### Comparing `ignf_gpf_api-0.1.8/docs/upload_descriptor.md` & `ignf_gpf_api-0.1.9/docs/upload_descriptor.md`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/Errors.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/__main__.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from ignf_gpf_api.workflow.resolver.GlobalResolver import GlobalResolver
 from ignf_gpf_api.workflow.resolver.StoreEntityResolver import StoreEntityResolver
 from ignf_gpf_api.workflow.action.UploadAction import UploadAction
 from ignf_gpf_api.io.Config import Config
 from ignf_gpf_api.io.DescriptorFileReader import DescriptorFileReader
 from ignf_gpf_api.store.Upload import Upload
 from ignf_gpf_api.store.StoreEntity import StoreEntity
+from ignf_gpf_api.store.ProcessingExecution import ProcessingExecution
+from ignf_gpf_api.store.User import User
 from ignf_gpf_api.workflow.resolver.UserResolver import UserResolver
 
 
 def main() -> None:
     """Fonction d'entrée."""
     # Résolution des paramètres utilisateurs
     o_args = parse_args()
@@ -50,14 +52,17 @@
         config(o_args)
     elif o_args.task == "upload":
         upload(o_args)
     elif o_args.task == "dataset":
         dataset(o_args)
     elif o_args.task == "workflow":
         workflow(o_args)
+    elif o_args.task == "me":
+        o_user = User.api_get("me")
+        print(o_user.to_json(indent=4))
 
 
 def parse_args(args: Optional[Sequence[str]] = None) -> argparse.Namespace:
     """Parse les paramètres utilisateurs.
 
     Args:
         args (Optional[Sequence[str]], optional): paramètres à parser, si None sys.argv utilisé.
@@ -94,14 +99,16 @@
     o_parser_auth.add_argument("--folder", "-f", type=str, default=None, help="Dossier où enregistrer le dataset")
     # Parser pour workflow
     o_parser_auth = o_sub_parsers.add_parser("workflow", help="Workflow")
     o_parser_auth.add_argument("--file", "-f", type=str, default=None, help="Chemin du fichier à utiliser OU chemin où extraire le dataset")
     o_parser_auth.add_argument("--name", "-n", type=str, default=None, help="Nom du workflow à extraire")
     o_parser_auth.add_argument("--step", "-s", type=str, default=None, help="Étape du workflow à lancer")
     o_parser_auth.add_argument("--behavior", "-b", type=str, default=None, help="Action à effectuer si l'exécution de traitement existe déjà")
+    # Parser pour me
+    o_parser_auth = o_sub_parsers.add_parser("me", help="me")
     return o_parser.parse_args(args)
 
 
 def auth(o_args: argparse.Namespace) -> None:
     """Authentifie l'utilisateur et retourne les informations de connexion demandées.
     Si aucune information est demandée, confirme juste la bonne authentification.
 
@@ -123,27 +130,31 @@
     o_response = ApiRequester().route_request("me_get")
     # Formatage
     d_info = o_response.json()
     # Info de base
     l_texts = [
         "Vos informations :",
         f"  * email : {d_info['email']}",
-        f"  * nom : {d_info['first_name']} {d_info['last_name']}",
+        f"  * nom : {d_info.get('first_name')} {d_info.get('last_name')}",
         f"  * votre id : {d_info['_id']}",
     ]
     # Gestion des communautés
     if not d_info["communities_member"]:
         l_texts.append("Vous n'êtes membre d'aucune communauté.")
     else:
         l_cm = d_info["communities_member"]
         l_texts.append("")
         l_texts.append(f"Vous êtes membre de {len(l_cm)} communauté(s) :")
         for d_cm in l_cm:
             d_community = d_cm["community"]
-            l_rights = [k.replace("_rights", "") for k, v in d_cm["rights"].items() if v is True]
+            print(d_cm["rights"])
+            if isinstance(d_cm["rights"], dict):
+                l_rights = [k.replace("_rights", "") for k, v in d_cm["rights"].items() if v is True]
+            else:
+                l_rights = d_cm["rights"]
             s_rights = ", ".join(l_rights)
             l_texts.append("")
             l_texts.append(f"  * communauté « {d_community['name']} » :")
             l_texts.append(f"      - id de la communauté : {d_community['_id']}")
             l_texts.append(f"      - id du datastore : {d_community['datastore']}")
             l_texts.append(f"      - nom technique : {d_community['technical_name']}")
             l_texts.append(f"      - droits : {s_rights}")
@@ -307,15 +318,26 @@
             GlobalResolver().add_resolver(StoreEntityResolver("store_entity"))
             GlobalResolver().add_resolver(UserResolver("user"))
             # le comportement
             s_behavior = str(o_args.behavior).upper() if o_args.behavior is not None else None
             # on reset l'afficheur de log
             PrintLogHelper.reset()
             # et on lance l'étape en précisant l'afficheur de log et le comportement
-            o_workflow.run_step(o_args.step, lambda processing_execution: PrintLogHelper.print(processing_execution.api_logs()), behavior=s_behavior)
+            def callback_run_step(processing_execution: ProcessingExecution) -> None:
+                """fonction callback pour l'affichage des logs lors du suivi d'un traitement
+
+                Args:
+                    processing_execution (ProcessingExecution): processing exécution en cours
+                """
+                try:
+                    PrintLogHelper.print(processing_execution.api_logs())
+                except Exception:
+                    PrintLogHelper.print("Logs indisponibles pour le moment...")
+
+            o_workflow.run_step(o_args.step, callback_run_step, behavior=s_behavior)
     else:
         l_children: List[str] = []
         for p_child in p_root.iterdir():
             if p_child.is_file():
                 l_children.append(p_child.name)
         print("Jeux de données disponibles :\n   * {}".format("\n   * ".join(l_children)))
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/default.ini` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/default.ini`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,32 @@
 # DEBUG, INFO, WARNING, ERROR, CRITICAL
 log_level=INFO
 
 
 [store_authentification]
 ############################### Paramétrage de l'authentification via KeyCloak ###############################
 token_url=https://qlf-iam-gpf.ign.fr/auth/realms/master/protocol/openid-connect/token
+http_proxy=
+https_proxy=
+grant_type=password
+client_secret=
+client_id=CLIENT_ID_TO_MODIFY
 login=LOGIN_TO_MODIFY
 password=PASSWORD_TO_MODIFY
-client_id=CLIENT_ID_TO_MODIFY
+totp_key=
 # En cas d'échec lors de l'authentification : max nb_attempts tentatives, sec_between_attempt secondes entre chacune d'entre elles
 nb_attempts=5
 sec_between_attempt=1
 
 
 [store_api]
 ############################### Paramètres de l'API Entrepôt ###############################
 root_url=https://api-qualification.ccs-ign-plage.ccs.cegedim.cloud/api/v1
+http_proxy=
+https_proxy=
 datastore=DATASTORE_ID_TO_MODIFY
 root_datastore=${store_api:root_url}/datastores/${store_api:datastore}
 # En cas d'échec lors du requêtage : max nb_attempts tentatives, sec_between_attempt secondes entre chacune d'entre elles
 nb_attempts=5
 sec_between_attempt=1
 # Nb max d'éléments à récupérer en cas de listing
 nb_limit=10
@@ -119,14 +126,17 @@
 
 # CheckExecution
 check_execution_list=${routing:check_list}/executions
 check_execution_get=${routing:check_execution_list}/{check_execution}
 check_execution_delete=${routing:check_execution_list}/{check_execution}
 check_execution_logs=${routing:check_execution_get}/logs
 
+# fichiers static
+static_list=${store_api:root_datastore}/statics
+
 
 [upload]
 ############################### Contrainte d'unicité à la création d'une livraison ###############################
 # Contrainte d'unicité définie par un ensemble de propriétés ET de tags (laisser vide si aucune). Les propriétés
 # d'une même ligne sont séparées par un point-virgule
 # Exemple :
 # pour définir une unicité sur les attributs "name", "srs" et le tag "livraison"
@@ -134,17 +144,17 @@
 uniqueness_constraint_infos=name
 uniqueness_constraint_tags=
 # Comportement du programmesi une livraison existe déjà (sur la base de la contrainte d'unicité)
 #   - DELETE : tente de supprimer la livraison existante et de la recréer,
 #   - CONTINUE : le programme reprend le transfert
 #   - STOP : le programme affiche uniquement un message et s'arrête
 behavior_if_exists=STOP
-md5_pattern={md5_key}  data/{file_path}
-push_data_file_key=filename
-push_md5_file_key=filename
+md5_pattern={md5_key}  {file_path}
+push_data_file_key=file
+push_md5_file_key=file
 nb_sec_between_check_updates=10
 check_message_pattern=Vérifications : {nb_asked} en attente, {nb_in_progress} en cours, {nb_failed} en échec, {nb_passed} en succès
 status_open=OPEN
 status_close=CLOSE
 
 [processing_execution]
 nb_sec_between_check_updates=10
@@ -182,16 +192,16 @@
 #   - groupe filter_tags : filtre sur une entité entrepôt exploitant ses tags
 
 # Filtre de store_entity à partir des propriétés
 filter_infos = ((\s*)INFOS(\s*)\((?P<filter_infos>.*?)\)(\s*))?
 # Filtre de store_entity à partir des tags
 filter_tags = ((\s*)TAGS(\s*)\((?P<filter_tags>.*?)\)(\s*))?
 filter = ((\s*)\[${filter_infos},?${filter_tags}\])
-store_entity_regex=(?P<entity_type>(upload|stored_data|processing_execution|offering|processing|configuration|endpoint))\.(?P<selected_field_type>(tags|infos))\.(?P<selected_field>\w*)${filter}
-global_regex=(?P<param>{(?P<resolver_name>[a-z_]+)\.(?P<to_solve>.*)})
+store_entity_regex=(?P<entity_type>(upload|stored_data|processing_execution|offering|processing|configuration|endpoint|static|datastore))\.(?P<selected_field_type>(tags|infos))\.(?P<selected_field>\w*)${filter}
+global_regex=(?P<param>(\["|{"?)(?P<resolver_name>[a-z_]+)(\.|":"|",")(?P<to_solve>[^"]*)("\]|"?}))
 file_regex=(?P<resolver_type>str|list|dict)\((?P<resolver_file>.*)\)
 
 
 [json_converter]
 # Pattern de convertion des types Python en str
 datetime_pattern = %Y-%m-%dT%H:%M:%S
 date_pattern = %Y-%m-%d
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/json_schemas/upload_descriptor_file.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999984929591049%*

 * *Differences: {"'properties'": "{'datasets': {'items': {'properties': {'upload_infos': {'properties': {'srs': "*

 * *                 "{delete: ['pattern']}}}}}}}"}*

```diff
@@ -24,15 +24,14 @@
                             "description": {
                                 "type": "string"
                             },
                             "name": {
                                 "type": "string"
                             },
                             "srs": {
-                                "pattern": "^EPSG:[0-9]{4,5}$",
                                 "type": "string"
                             },
                             "type": {
                                 "enum": [
                                     "RASTER",
                                     "VECTOR",
                                     "ARCHIVE"
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_conf/json_schemas/workflow.json` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_conf/json_schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/1_dataset_vector/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/2_dataset_archive/CANTON/CANTON.zip`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/datasets/2_dataset_archive/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/archive-generic.jsonc` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/archive-generic.jsonc`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             "intégration-archive-livrée": {
                 "actions": [
                     {
                         // On crée une exécution de traitement
                         "type": "processing-execution",
                         "body_parameters": {
                             // On récupère l'id du traitement nommé "Intégration d'archives livrées"
-                            "processing": "{store_entity.processing.infos._id [INFOS(name=Intégration d'archives livrées)]}",
+                            "processing": "{store_entity.processing.infos._id [INFOS(name=archive)]}",
                             "inputs": {
                                 "upload": [
                                     // On récupère l'id de la Livraison associée grâce à son nom
                                     "{store_entity.upload.infos._id [INFOS(name=EXAMPLE_DATASET_ARCHIVE)]}"
                                 ]
                             },
                             "output": {
@@ -48,15 +48,16 @@
                             "layer_name": "{user.last_name}__archive",
                             "type_infos": {
                                 "title": "Couche Canton du tutoriel",
                                 "abstract": "Exemple d'archive à télécharger",
                                 "used_data": [
                                     {
                                         // On récupère l'id de la Donnée Stockée créée à l'étape précédente grâce à son nom et l'un de ses tags
-                                        "stored_data": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__Archive), TAGS(tuto=oui)]}"
+                                        "stored_data": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__Archive), TAGS(tuto=oui)]}",
+                                        "sub_name": "archive"
                                     }
                                 ]
                             }
                         },
                         // Liste des commentaires ajoutés à la Configuration
                         "comments": [
                             "Tutoriel de mise à disposition d'archive"
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/_data/workflows/wfs-generic.jsonc` & `ignf_gpf_api-0.1.9/ignf_gpf_api/_data/workflows/generique-maj-bdd_gpf.jsonc`

 * *Files 19% similar despite different names*

```diff
@@ -1,157 +1,185 @@
 {
     "workflow": {
         "steps": {
             // Étape n°1 : Mise en base de vecteurs livrés
-            "mise-en-base": {
+            "mise-en-base-1": {
                 "actions": [
                     {
                         // On crée une exécution de traitement
                         "type": "processing-execution",
                         "body_parameters": {
                             // On récupère l'id du traitement nommé "Intégration de données vecteur livrées en base"
                             "processing": "{store_entity.processing.infos._id [INFOS(name=Intégration de données vecteur livrées en base)]}",
                             "inputs": {
                                 "upload": [
                                     // On récupère l'id de la Livraison associée grâce à son nom
-                                    "{store_entity.upload.infos._id [INFOS(name=EXAMPLE_DATASET_ARCHIVE)]}"
+                                    "{store_entity.upload.infos._id [INFOS(name=EXAMPLE_DATASET_MAJ_BDD_1)]}"
                                 ]
                             },
                             "output": {
                                 "stored_data": {
-                                    // On crée une nouvelle Donnée Stockée nommée "UserLastName_Base_intermédiaire"
-                                    "name": "{user.last_name}__Base_intermédiaire"
+                                    // On crée une nouvelle Donnée Stockée nommée "UserLastName__tuto_base_maj"
+                                    "name": "{user.last_name}__tuto_base_maj",
+                                    "storage_type": "POSTGRESQL"
                                 }
                             },
                             "parameters": {}
                         },
                         // Liste des commentaires ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "comments": [
-                            "Tutoriel de mise en place d'une pyramide vecteur : création base intermédiaire"
+                            "Tutoriel mise à jour d'une BDD : création base"
                         ],
                         // Liste des tags ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "tags": {
                             "tuto": "oui",
                             "temp": "oui"
                         }
                     }
                 ],
+                // Pour Bag donc pas besoin pour tester la gpf
                 "parents": []
             },
-            // Étape n°2 : création de la pyramide vecteur
-            "création-pyramide": {
+            // Étape n°2 : configuration d'un flux WMS
+            "configuration-wms": {
+                "actions": [
+                    {
+                        "type": "configuration",
+                        "body_parameters": {
+                            "type": "WMS-VECTOR",
+                            "name": "{user.last_name}__tuto_base_maj_WMS",
+                            "layer_name": "{user.last_name}__tuto_base_maj_WMS",
+                            "type_infos": {
+                                "title": "{user.last_name} -- Donnée tutoriel mise à jour BDD",
+                                "abstract": "Exemple de flux à visualiser pour la MAJ des BDD",
+                                "keywords": [
+                                    "Tutoriel"
+                                ],
+                                // base potentiellement vide ou au future plus étendu : on met la BBOX obligatoirement
+                                "bbox": {
+                                  "west": -175,
+                                  "south": -75,
+                                  "east": 175,
+                                  "north": 85
+                                },                            
+                                "used_data": [
+                                    // C'est un flux simple : on n'utilise qu'une seule donnée du niveau 5 au niveau 18
+                                    {
+                                        "relations": [
+                                            {
+                                                "name": "installation_autorisation",// TODO : à compléter selon donné en entrée
+                                                // ficher de style livré comme ficher statique avec comme "name" : "Style pour les installations"
+                                                "style": "{store_entity.static.infos._id [INFOS(name=Style pour les installations)]}"
+                                            }
+                                        ],
+                                        // On récupère l'id de la Donnée Stockée créée à l'étape précédente grâce à son nom, son type et l'un de ses tags
+                                        "stored_data": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__tuto_base_maj)]}"
+                                    }
+                                ]
+                            }
+                        },
+                        // Liste des commentaires ajoutés à la Configuration
+                        "comments": [
+                            "Tutoriel mise à jour d'une BDD : configuration du flux wms"
+                        ],
+                        // Liste des tags ajoutés à la Configuration
+                        "tags": {
+                            "tuto": "oui",
+                            "temp": "oui"
+                        }
+                    }
+                ],
+                "parents": ["mise-en-base-1"]
+            },
+            // Étape n°3 : publication du flux WMS
+            "publication-wms": {
+                "actions": [
+                    {
+                        "type": "offering",
+                        "url_parameters": {
+                            // On récupère l'id de la Configuration créée à l'étape précédente grâce à son nom et l'un de ses tags
+                            "configuration": "{store_entity.configuration.infos._id [INFOS(name={user.last_name}__Flux_vecteur_WMS)]}"
+                        },
+                        "body_parameters": {
+                            "visibility": "PRIVATE",
+                            // Endpoint de type WMS
+                            "endpoint": "{store_entity.endpoint.infos._id [INFOS(type=WMS-VECTOR)]}"
+                        }
+                    }
+                ],
+                "parents": ["configuration-wms"]
+            },
+            // Étape n°4 : mise à jour de la base 2é livraison
+            "mise-en-base-2": {
                 "actions": [
                     {
                         // On crée une exécution de traitement
                         "type": "processing-execution",
                         "body_parameters": {
-                            // On récupère l'id du traitement nommé "Création d'une pyramide vecteur"
-                            "processing": "{store_entity.processing.infos._id [INFOS(name=Création d'une pyramide vecteur)]}",
+                            // On récupère l'id du traitement nommé "Intégration de données vecteur livrées en base"
+                            "processing": "{store_entity.processing.infos._id [INFOS(name=Intégration de données vecteur livrées en base)]}",
                             "inputs": {
-                                "stored_data": [
-                                    // On récupère l'id de la Donnée Stockée créée à l'étape précédente grâce à son nom, son type et l'un de ses tags
-                                    "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__Base_intermédiaire, type=VECTOR-DB) TAGS(tuto=oui)]}"
+                                "upload": [
+                                    // On récupère l'id de la Livraison associée grâce à son nom
+                                    "{store_entity.upload.infos._id [INFOS(name=EXAMPLE_DATASET_MAJ_BDD_2)]}"
                                 ]
                             },
                             "output": {
                                 "stored_data": {
-                                    // On crée une nouvelle Donnée Stockée nommée "UserLastName__Pyramide_vecteur"
-                                    "name": "{user.last_name}__Pyramide_vecteur"
+                                    // On met a jour la livraison avec les données de la 2é livraison
+                                    "id": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__tuto_base_maj)]}"
                                 }
                             },
-                            "parameters": {
-                                // Tile Matrix Set à utiliser
-                                "tms": "PM",
-                                // Niveau du bas
-                                "bottom_level": "18",
-                                // Niveau du haut
-                                "top_level": "5",
-                                // Tables à utiliser, sur quels niveaux et avec quels attributs
-                                "composition": [
-                                    {
-                                        "table": "canton",
-                                        "bottom_level": "18",
-                                        "top_level": "5",
-                                        "attributes": "id,insee_dep,insee_reg,insee_can"
-                                    }
-                                ],
-                                // BBOX : on veut conserver toute l'emprise, donc on laisse vide
-                                //"bbox": [], // A COMPLETER
-                                // Options de généralisation tippecanoe (par défaut: "-al -ap")
-                                "tippecanoe_options": "-S10"
-                            }
+                            "parameters": {}
                         },
                         // Liste des commentaires ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "comments": [
-                            "Tutoriel de mise en place d'une pyramide vecteur : création pyramide vecteur à publier"
+                            "Tutoriel mise à jour d'une BDD : 2é livraison"
                         ],
                         // Liste des tags ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "tags": {
                             "tuto": "oui",
-                            "temp": "non"
+                            "temp": "oui"
                         }
                     }
                 ],
-                "parents": [
-                    "mise-en-base"
-                ]
+                "parents": ["publication-wms"]
             },
-            // Étape n°3 : configuration d'un flux WFS
-            "configuration-wfs": {
+            // Étape n°5 : mise à jour de la base 3é livraison
+            "mise-en-base-3": {
                 "actions": [
                     {
-                        "type": "configuration",
+                        // On crée une exécution de traitement
+                        "type": "processing-execution",
                         "body_parameters": {
-                            "type": "WMTS-TMS",
-                            "name": "{user.last_name}__Flux_vecteur",
-                            "layer_name": "{user.last_name}__flux_vecteur",
-                            "type_infos": {
-                                "title": "Couche Canton du tutoriel",
-                                "abstract": "Exemple de flux à visualiser",
-                                "used_data": [
-                                    // C'est un flux simple : on n'utilise qu'une seule donnée du niveau 5 au niveau 18
-                                    {
-                                        // On récupère l'id de la Donnée Stockée créée à l'étape précédente grâce à son nom, son type et l'un de ses tags
-                                        "stored_data": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__Pyramide_vecteur, type=ROK4-PYRAMID-VECTOR), TAGS(tuto=oui)]}",
-                                        "bottom_level": "18",
-                                        "top_level": "5"
-                                    }
+                            // On récupère l'id du traitement nommé "Intégration de données vecteur livrées en base"
+                            "processing": "{store_entity.processing.infos._id [INFOS(name=Intégration de données vecteur livrées en base)]}",
+                            "inputs": {
+                                "upload": [
+                                    // On récupère l'id de la Livraison associée grâce à son nom
+                                    "{store_entity.upload.infos._id [INFOS(name=EXAMPLE_DATASET_MAJ_BDD_3)]}"
                                 ]
-                            }
+                            },
+                            "output": {
+                                "stored_data": {
+                                    // On met a jour la livraison avec les données de la 2é livraison
+                                    "id": "{store_entity.stored_data.infos._id [INFOS(name={user.last_name}__tuto_base_maj)]}"
+                                }
+                            },
+                            "parameters": {}
                         },
-                        // Liste des commentaires ajoutés à la Configuration
+                        // Liste des commentaires ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "comments": [
-                            "Tutoriel de mise en place d'une pyramide vecteur : configuration de la pyramide"
+                            "Tutoriel mise à jour d'une BDD : 3é livraison"
                         ],
-                        // Liste des tags ajoutés à la Configuration
+                        // Liste des tags ajoutés à la Donnée Stockée en sortie de l'exécution du traitement
                         "tags": {
-                            "tuto": "oui"
-                        }
-                    }
-                ],
-                "parents": [
-                    "création-pyramide"
-                ]
-            },
-            // Étape n°4 : publication du flux WFS millésimé
-            "publication-wfs": {
-                "actions": [
-                    {
-                        "type": "offering",
-                        "url_parameters": {
-                            // On récupère l'id de la Configuration créée à l'étape précédente grâce à son nom et l'un de ses tags
-                            "configuration": "{store_entity.configuration.infos._id [INFOS(name={user.last_name}__Flux_vecteur), TAGS(tuto=oui)]}"
-                        },
-                        "body_parameters": {
-                            "visibility": "PRIVATE",
-                            // Endpoint de type WMTS-TMS (id trouvé en récupérant les informations de l'entrepôt)
-                            "endpoint": "6220b50fb579ed7b9ad7f4ae"
+                            "tuto": "oui",
+                            "temp": "oui"
                         }
                     }
                 ],
-                "parents": [
-                    "configuration-wfs"
-                ]
+                "parents": ["mise-en-base-2"]
             }
         }
     }
 }
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Authentifier.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/auth/Authentifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import traceback
 from http import HTTPStatus
 from typing import Dict, Optional
 import requests
+import pyotp
 
 from ignf_gpf_api.pattern.Singleton import Singleton
 from ignf_gpf_api.auth.Token import Token
 from ignf_gpf_api.auth.Errors import AuthentificationError
 from ignf_gpf_api.io.Config import Config
 
 
@@ -21,48 +22,83 @@
         __nb_attempts (int): nombre de tentatives possibles en cas de problème rencontré pendant la récupération du jeton
         __sec_between_attempt (int): nombre de secondes entre deux tentatives en cas de problème rencontré pendant la récupération du jeton
         __last_token (Token): sauvegarde du dernier jeton récupéré (pour éviter de multiples requêtes au serveur KeyCloak)
     """
 
     def __init__(self) -> None:
         # Sauvegarde de la conf comme attributs d'instance
-        self.__token_url: str = Config().get("store_authentification", "token_url")
-        self.__login: str = Config().get("store_authentification", "login")
-        self.__password: str = Config().get("store_authentification", "password")
-        self.__client_id: str = Config().get("store_authentification", "client_id")
+        self.__token_url: str = Config().get_str("store_authentification", "token_url")
         self.__nb_attempts: int = Config().get_int("store_authentification", "nb_attempts")
         self.__sec_between_attempt: int = Config().get_int("store_authentification", "sec_between_attempt")
+        self.__request_params = self.__get_request_params()
+        # Gestion TOTP
+        self.__totp: Optional[pyotp.TOTP] = None
+        s_totp_key: Optional[str] = Config().get("store_authentification", "totp_key")
+        if s_totp_key:
+            self.__totp = pyotp.TOTP(s_totp_key)
+        # Récupération des paramètres du proxy
+        self.__proxy = {
+            "http": Config().get_str("store_authentification", "http_proxy"),
+            "https": Config().get_str("store_authentification", "https_proxy"),
+        }
         # Permettra la sauvegarde du dernier jeton récupéré (pour éviter de multiples requêtes au serveur KeyCloak)
         self.__last_token: Optional[Token] = None
 
+    def __get_request_params(self) -> Dict[str, str]:
+        """Lit la config, la compile et renvoie un dictionnaire contenant les prams de connection.
+
+        Raises:
+            AuthentificationError: levée si type d'authentification inconnu
+
+        Returns:
+            Dict[str, str]: params de connection
+        """
+        # Récupération du type d'authentification
+        s_grant_type = Config().get_str("store_authentification", "grant_type")
+        d_params = {"grant_type": s_grant_type}
+        # Completion selon le type
+        if s_grant_type == "password":
+            d_params["username"] = Config().get_str("store_authentification", "login")
+            d_params["password"] = Config().get_str("store_authentification", "password")
+            d_params["client_id"] = Config().get_str("store_authentification", "client_id")
+            s_client_secret = Config().get_str("store_authentification", "client_secret")
+            if s_client_secret is not None:
+                d_params["client_secret"] = s_client_secret
+        elif s_grant_type == "client_credentials":
+            d_params["client_id"] = Config().get_str("store_authentification", "client_id")
+            d_params["client_secret"] = Config().get_str("store_authentification", "client_secret")
+        else:
+            raise AuthentificationError(f"Type d'authentification « {s_grant_type} » inconnue. Vérifiez le paramétrage 'store_authentification.grant_type'.")
+        return d_params
+
     def __request_new_token(self, nb_attempts: int) -> None:
         """Récupère un nouveau jeton de zéro et le sauvegarde.
 
         En cas de problème pendant la récupération, essaie `nb_attempts` fois en attendant `__sec_between_attempt` secondes entre plusieurs tentatives.
 
         Args:
             nb_attempts (int): Nombre de tentatives en cas d'échec
 
         Raises:
             Exception: liée à la requête http, levée si la récupération de jeton au bout de `nb_attempts` tentatives
         """
         o_response = None
         try:
+            # Préparation données d'authentification
+            d_data = self.__request_params.copy()
+            if self.__totp:
+                d_data["totp"] = self.__totp.now()
             # Requête KeyCloak de récupération du jeton
             o_response = requests.post(
                 self.__token_url,
-                data={
-                    "grant_type": "password",
-                    "username": self.__login,
-                    "password": self.__password,
-                    "client_id": self.__client_id,
-                },
+                data=d_data,
                 headers={
                     "content-type": "application/x-www-form-urlencoded",
                 },
+                proxies=self.__proxy,
             )
             if o_response.status_code == HTTPStatus.OK:
                 self.__last_token = Token(o_response.json())
             else:
                 raise requests.exceptions.HTTPError(f"Code retour authentification KeyCloak = {o_response.status_code}")
 
         except Exception as e_error:
@@ -93,15 +129,15 @@
             return self.__last_token.get_access_string()
         except Exception as e_error:
             s_error_message = f"La récupération du jeton d'authentification a échoué après {self.__nb_attempts} tentatives"
             Config().om.error(s_error_message)
             raise AuthentificationError(s_error_message) from e_error
 
     def get_http_header(self, json_content_type: bool = False) -> Dict[str, str]:
-        """Renvoie une entête HTTP d'authentification à destination du KeyCloak et consommable par une requête via le module requests.
+        """Renvoie une entête HTTP d'authentification à destination de KeyCloak et consommable par une requête via le module requests.
 
         Args:
             json_content_type (bool): indique si le `content-type` `application/json` doit être spécifié
 
         Returns:
             Dictionnaire de la forme : `{"Authorization": "Bearer <JETON>", "content-type":"application/json"}`
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/auth/Token.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/auth/Token.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/FileHelper.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/helper/FileHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/JsonHelper.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/helper/JsonHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/helper/PrintLogHelper.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/helper/PrintLogHelper.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/ApiRequester.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/ApiRequester.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,21 +20,26 @@
 
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     PATCH = "PATCH"
     DELETE = "DELETE"
 
-    regex_content_range = re.compile(Config().get("store_api", "regex_content_range"))
+    regex_content_range = re.compile(Config().get_str("store_api", "regex_content_range"))
 
     def __init__(self) -> None:
         # Récupération du convertisseur Json
         self.__jsonConverter = JsonConverter()
         self.__nb_attempts = Config().get_int("store_api", "nb_attempts")
         self.__sec_between_attempt = Config().get_int("store_api", "sec_between_attempt")
+        # Récupération des paramètres du proxy
+        self.__proxy = {
+            "http": Config().get_str("store_api", "http_proxy"),
+            "https": Config().get_str("store_api", "https_proxy"),
+        }
 
     def route_request(
         self,
         route_name: str,
         route_params: Optional[Dict[str, Any]] = None,
         method: str = "GET",
         params: Optional[Dict[str, Any]] = None,
@@ -97,14 +102,16 @@
             params (Optional[Dict[str, Any]], optional): paramètres de la requête (ajouté à l'url)
             data (Optional[Union[Dict[str, Any], List[Any]]], optional): contenue de la requête (ajouté au corp)
             files (Optional[Dict[str, Tuple[Any]]], optional): fichiers à envoyer
 
         Returns:
             réponse si succès
         """
+        Config().om.debug(f"url_request({url}, {method}, {params}, {data})")
+
         i_nb_attempts = 0
         while True:
             i_nb_attempts += 1
             try:
                 # On fait la requête
                 return self.__url_request(url, method, params=params, data=data, files=files)
             except NotFoundError as e_error:
@@ -167,22 +174,20 @@
             params (Optional[Dict[str, Any]], optional): paramètres.
             data (Optional[Union[Dict[str, Any], List[Any]]], optional): données.
             files (Optional[Dict[str, Tuple[Any]]], optional): fichiers.
 
         Returns:
             réponse si succès
         """
-        d_proxies = {
-            "http": None,
-            "https": None,
-        }
+        Config().om.debug(f"__url_request({url}, {method}, {params}, {data})")
+
         # Définition du header
         d_headers = Authentifier().get_http_header(json_content_type=files is None)
         # Execution de la requête
-        r = requests.request(url=url, params=params, json=data, method=method, headers=d_headers, proxies=d_proxies, files=files)  # type:ignore
+        r = requests.request(url=url, params=params, json=data, method=method, headers=d_headers, proxies=self.__proxy, files=files)
 
         # Vérification du résultat...
         if r.status_code >= 200 and r.status_code < 300:
             # Si c'est ok, on renvoie la réponse
             return r
         if r.status_code == 500:
             # Erreur interne (pas de retour)
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Color.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/Color.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Config.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/Config.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from ignf_gpf_api.pattern.Singleton import Singleton
 from ignf_gpf_api.io.OutputManager import OutputManager
 from ignf_gpf_api.io.Errors import ConfigReaderError
 
 
 class Config(metaclass=Singleton):
-    """Classe singleton de gestion de la configuration.
-
+    """Lit le fichier de configuration (classe Singleton).
     Attributes:
         __config_parser (configparser): ConfigParser
         __ini_file_path (string): Chemin vers le fichier de configuration BaGI
     """
 
     conf_dir_path = Path(__file__).parent.parent.absolute() / "_conf"
     data_dir_path = Path(__file__).parent.parent.absolute() / "_data"
@@ -33,15 +32,16 @@
             raise ConfigReaderError("Fichier de configuration par défaut {ConfigReader.ini_file_path} non trouvé.")
 
         self.__config_parser: configparser.ConfigParser = configparser.ConfigParser(interpolation=configparser.ExtendedInterpolation())
         with Config.ini_file_path.open(encoding="UTF-8") as f_ini:
             self.__config_parser.read_file(f_ini)
 
         # Définition du niveau de log pour l'OutputManager par défaut
-        self.__output_manager.set_log_level(self.get("logging", "log_level"))
+        s_level: str = self.get_str("logging", "log_level", "INFO")
+        self.__output_manager.set_log_level(s_level)
 
     def set_output_manager(self, output_manager: Any) -> None:
         self.__output_manager = output_manager
 
     @property
     def om(self) -> OutputManager:
         return self.__output_manager
@@ -64,24 +64,40 @@
         """Retourne le config_parser.
 
         Returns:
             le config parser
         """
         return self.__config_parser
 
-    def get(self, section: str, option: str, fallback: Optional[str] = None) -> str:
+    def get(self, section: str, option: str, fallback: Optional[str] = None) -> Optional[str]:
         """Récupère la valeur associée au paramètre demandé.
 
         Args:
             section (str): section du paramètre
             option (str): option du paramètre
             fallback (Optional[str], optional): valeur par défaut.
 
         Returns:
-            la valeur du paramètre
+            Optional[str]: la valeur du paramètre
+        """
+        s_value: Optional[str] = self.__config_parser.get(section, option, fallback=fallback)
+        if s_value == "":
+            return None
+        return s_value
+
+    def get_str(self, section: str, option: str, fallback: Optional[str] = None) -> str:
+        """Récupère la valeur du paramètre demandé.
+
+        Args:
+            section (str): section du paramètre
+            option (str): option du paramètre
+            fallback (Optional[str], optional): valeur par défaut. Defaults to None.
+
+        Returns:
+            Optional[str]: la valeur du paramètre
         """
         return self.__config_parser.get(section, option, fallback=fallback)  # type: ignore
 
     def get_int(self, section: str, option: str, fallback: Optional[int] = None) -> int:
         """Récupère la valeur associée au paramètre demandé, convertie en `int`.
 
         Args:
@@ -122,8 +138,8 @@
 
     def get_temp(self) -> Path:
         """Récupère le chemin racine du dossier temporaire à utiliser.
 
         Returns:
             chemin racine du dossier temporaire à utiliser
         """
-        return Path(self.get("miscellaneous", "tmp_workdir"))
+        return Path(self.get_str("miscellaneous", "tmp_workdir"))
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Dataset.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/Dataset.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/DescriptorFileReader.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/DescriptorFileReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.__descriptor_dict: Optional[Dict[Any, Any]] = None
         self.__datasets: List[Dataset] = []
         self.__parent_folder = descriptor_file_path.parent.absolute()
         # Ouverture du fichier descripteur de livraison
         self.__descriptor_dict = JsonHelper.load(descriptor_file_path, file_not_found_pattern="Fichier descripteur de livraison {json_path} non trouvé.")
 
         # Ouverture du schéma JSON à respecter
-        p_schema_file_path = Config.conf_dir_path / Config().get("json_schemas", "descriptor_file")
+        p_schema_file_path = Config.conf_dir_path / Config().get_str("json_schemas", "descriptor_file")
         d_schema = JsonHelper.load(p_schema_file_path, file_not_found_pattern="Schéma de fichier descriptif de livraison {json_path} non trouvé. Contactez le support.")
 
         # Valide le fichier descriptif
         JsonHelper.validate_object(
             self.__descriptor_dict,
             d_schema,
             "Fichier descriptif de livraison {json_path} non valide.",
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/Errors.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/JsonConverter.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/JsonConverter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 class JsonConverter(metaclass=Singleton):
     """Classe de conversion des objects python en json. Le but est de convertir
     les objets qui ne sont pas nativement gérés par Python comme les dates."""
 
     def __init__(self) -> None:
         """initialisation : liste des routes et adresse site"""
         # Stockage en attributs de classe des patterns
-        self.__datetime_pattern = Config().get("json_converter", "datetime_pattern")
-        self.__date_pattern = Config().get("json_converter", "date_pattern")
-        self.__time_pattern = Config().get("json_converter", "time_pattern")
+        self.__datetime_pattern = Config().get_str("json_converter", "datetime_pattern")
+        self.__date_pattern = Config().get_str("json_converter", "date_pattern")
+        self.__time_pattern = Config().get_str("json_converter", "time_pattern")
 
     def dumps(self, data: Dict[Any, Any]) -> str:
         """Cette fonction permet de convertir les classes python en string JSON.
         Pour le moment, sont traitées les dates, times, et datetimes.
         On utilise un "converter" spécialisé.
 
         Args:
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/io/OutputManager.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/io/OutputManager.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/SingleInstance.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/pattern/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/pattern/Singleton.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/pattern/Singleton.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Configuration.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/Configuration.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Endpoint.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/Endpoint.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Offering.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/Offering.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/ProcessingExecution.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/ProcessingExecution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+import json
 from typing import Optional
 
 from ignf_gpf_api.store.StoreEntity import StoreEntity
 from ignf_gpf_api.store.interface.CsfInterface import CsfInterface
 from ignf_gpf_api.io.ApiRequester import ApiRequester
 
 
@@ -33,14 +34,22 @@
         s_route = f"{self._entity_name}_logs"
         # Requête "get"
         o_response = ApiRequester().route_request(
             s_route,
             route_params={self._entity_name: self.id},
         )
         s_log = o_response.text
+        try:
+            if s_log in ["", "[]"]:
+                return ""
+            # les logs sont retourné sous forme de liste on tente le passage de liste à un texte propre.
+            l_log = json.loads(s_log)
+            s_log = "\n".join(l_log)
+        except Exception:
+            pass
         # on renvoie les logs
         return s_log
 
     def api_launch(self) -> None:
         """Lance l'exécution du traitement sur l'API."""
         # Génération du nom de la route
         s_route = f"{self._entity_name}_launch"
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoreEntity.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/StoreEntity.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,16 +120,15 @@
         i_limit = Config().get_int("store_api", "nb_limit")
 
         # Gestion des paramètres nuls
         infos_filter = infos_filter if infos_filter is not None else {}
         tags_filter = tags_filter if tags_filter is not None else {}
 
         # Fusion des filtres sur les attributs et les tags
-        d_params: Dict[str, Any] = infos_filter if infos_filter is not None else {}
-        d_params["tags[]"] = [f"{k}={v}" for k, v in tags_filter.items()]
+        d_params: Dict[str, Any] = {**infos_filter, **{f"tags[{k}]": v for k, v in tags_filter.items()}}
 
         # Génération du nom de la route
         s_route = f"{cls._entity_name}_list"
 
         # Liste pour stocker les entités
         l_entities: List[T] = []
 
@@ -264,20 +263,19 @@
         # Affichage à destination d'un utilisateur.
         # On affiche l'id et le nom si possible.
 
         # Liste pour stocker les infos à afficher
         l_infos = []
         # Ajout de l'id
         l_infos.append(f"id={self.id}")
-        # Ajout du nom si possible
-        if "name" in self._store_api_dict:
-            l_infos.append(f"name={self['name']}")
-        # Ajout du layer_name si possible
-        if "layer_name" in self._store_api_dict:
-            l_infos.append(f"layer_name={self['layer_name']}")
+        # Ajout de certains attributs si possible
+        l_attributes = ["name", "layer_name", "technical_name"]
+        for s_attribut in l_attributes:
+            if s_attribut in self._store_api_dict:
+                l_infos.append(f"{s_attribut}={self[s_attribut]}")
         # Retour
         return f"{self.__class__.__name__}({', '.join(l_infos)})"
 
     def __repr__(self) -> str:
         # Affichage à destination d'un développeur.
         # Pour le moment, pas de différence avec __str__
         return str(self)
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/StoredData.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/StoredData.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/Upload.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/Upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Args:
             file_path: chemin local vers le fichier à envoyer
             api_path: chemin distant du dossier où déposer le fichier
         """
         # Génération du nom de la route
         s_route = f"{self._entity_name}_push_data"
         # Récupération du nom de la clé pour le fichier
-        s_file_key = Config().get("upload", "push_data_file_key")
+        s_file_key = Config().get_str("upload", "push_data_file_key")
 
         # Ouverture du fichier et remplissage du tuple de fichier
         with file_path.open("rb") as o_file_binary:
             o_tuple_file = (file_path.name, o_file_binary)
             o_dict_files = {s_file_key: o_tuple_file}
             # Requête
             ApiRequester().route_request(
@@ -84,15 +84,15 @@
 
         Args:
             file_path: chemin local vers le fichier à envoyer
         """
         # Génération du nom de la route
         s_route = f"{self._entity_name}_push_md5"
         # Récupération du nom de la clé pour le fichier
-        s_file_key = Config().get("upload", "push_md5_file_key")
+        s_file_key = Config().get_str("upload", "push_md5_file_key")
 
         # Ouverture du fichier et remplissage du tuple de fichier
         with file_path.open("rb") as o_file_binary:
             o_tuple_file = (file_path.name, o_file_binary)
             o_dict_files = {s_file_key: o_tuple_file}
             # Requête
             ApiRequester().route_request(
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CommentInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/CommentInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/CsfInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/CsfInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/EventInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/EventInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/FullEditInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/FullEditInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/PartialEditInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/PartialEditInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/SharingInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/SharingInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/store/interface/TagInterface.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/store/interface/TagInterface.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/Workflow.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/Workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         # Récupération de l'étape dans la définition de workflow
         d_step_definition = self.__get_step_definition(step_name)
         # initialisation des actions parentes
         o_parent_action: Optional[ActionAbstract] = None
         # Pour chaque action définie dans le workflow, instanciation de l'objet Action puis création sur l'entrepôt
         for d_action_raw in d_step_definition["actions"]:
             # création de l'action
-            o_action = Workflow.generate(f"{step_name}", d_action_raw, o_parent_action, behavior)
+            o_action = Workflow.generate(step_name, d_action_raw, o_parent_action, behavior)
             # résolution
             o_action.resolve()
             # exécution de l'action
             Config().om.info(f"Exécution de l'action '{o_action.workflow_context}-{o_action.index}'...")
             o_action.run()
             # on attend la fin de l'exécution si besoin
             if isinstance(o_action, ProcessingExecutionAction):
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ActionAbstract.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ActionAbstract.py`

 * *Files 16% similar despite different names*

```diff
@@ -84,20 +84,38 @@
             infos (Dict[str, Any]): paramètres d'attributs pour la création de l'entité
             tags (Dict[str, Any]): paramètres de tags pour la création de l'entité
 
         Returns:
             critère de filtres sur les infos et les tags
         """
         # On liste les filtres sur les informations (uniqueness_constraint_infos)
-        l_attributes = Config().get(config_key, "uniqueness_constraint_infos").split(";")
+        l_attributes = Config().get_str(config_key, "uniqueness_constraint_infos", "").split(";")
         d_infos = {}
         for s_infos in l_attributes:
             if s_infos != "":
                 d_infos[s_infos] = infos.get(s_infos, None)
         # On liste les filtres sur les tags (uniqueness_constraint_tags)
-        l_tags = Config().get(config_key, "uniqueness_constraint_tags").split(";")
+        l_tags = Config().get_str(config_key, "uniqueness_constraint_tags", "").split(";")
         d_tags = {}
         for s_tag in l_tags:
             if s_tag != "":
                 d_tags[s_tag] = tags[s_tag]
         # On peut maintenant renvoyer les filtres
         return d_infos, d_tags
+
+    ##############################################################
+    # Fonctions de représentation
+    ##############################################################
+    def __str__(self) -> str:
+        # Affichage à destination d'un utilisateur.
+        # On affiche l'id et le nom si possible.
+
+        # Liste pour stocker les infos à afficher
+        l_infos = []
+        # Ajout de l'id
+        l_infos.append(f"workflow={self.workflow_context}")
+        return f"{self.__class__.__name__}({', '.join(l_infos)})"
+
+    def __repr__(self) -> str:
+        # Affichage à destination d'un développeur.
+        # Pour le moment, pas de différence avec __str__
+        return str(self)
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ConfigurationAction.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/OfferingAction.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/OfferingAction.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,21 @@
         # Ajout de l'Offering
         self.__create_offering()
         # Affichage
         o_offering = self.offering
         if o_offering is not None:
             # Récupération des liens
             o_offering.api_update()
-            s_urls = "\n   - ".join(o_offering["urls"])
-            Config().om.info(f"Offre créée : {self.__offering}\n   - {s_urls}")
+            if len(o_offering["urls"]) > 0 and isinstance(o_offering["urls"][0], dict):
+                # si les url sont récupérées sous forme de dict on affiche l'url uniquement
+                s_urls = "\n   - ".join([d_url["url"] for d_url in o_offering["urls"]])
+            else:
+                # si les url sont récupérées sous forme de liste
+                s_urls = "\n   - ".join(o_offering["urls"])
+            Config().om.info(f"Offre créée : {self.__offering}\n{s_urls}")
         Config().om.info("Création d'une offre : terminé")
 
     def __create_offering(self) -> None:
         """Création de l'Offering sur l'API à partir des paramètres de définition de l'action."""
         o_offering = self.find_offering()
         if o_offering is not None:
             self.__offering = o_offering
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/ProcessingExecutionAction.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def __init__(self, workflow_context: str, definition_dict: Dict[str, Any], parent_action: Optional["ActionAbstract"] = None, behavior: Optional[str] = None) -> None:
         super().__init__(workflow_context, definition_dict, parent_action)
         # Autres attributs
         self.__processing_execution: Optional[ProcessingExecution] = None
         self.__upload: Optional[Upload] = None
         self.__stored_data: Optional[StoredData] = None
-        self.__behavior: str = behavior if behavior is not None else Config().get("processing_execution", "behavior_if_exists")
+        self.__behavior: str = behavior if behavior is not None else Config().get_str("processing_execution", "behavior_if_exists")
 
     def run(self) -> None:
         Config().om.info("Création d'une exécution de traitement et complétion de l'entité en sortie...")
         # Création de l'exécution du traitement (attributs processing_execution et Upload/StoredData défini)
         self.__create_processing_execution()
         # Ajout des tags sur l'Upload ou la StoredData
         self.__add_tags()
@@ -64,20 +64,14 @@
             if o_stored_data is not None:
                 # Comportement d'arrêt du programme
                 if self.__behavior == self.BEHAVIOR_STOP:
                     raise GpfApiError(f"Impossible de créer l’exécution de traitement, une donnée stockée en sortie équivalente {o_stored_data} existe déjà.")
                 # Comportement de suppression des entités détectées
                 if self.__behavior == self.BEHAVIOR_DELETE:
                     Config().om.warning(f"Une donnée stockée équivalente à {o_stored_data} va être supprimée puis recréée.")
-                    Config().om.warning("Si une exécution de traitement liée à la donnée équivalente existe, elle sera supprimée.")
-                    # Récupération des traitements qui ont créé la donnée stockée équivalente
-                    l_process = ProcessingExecution.api_list(infos_filter={"output_stored_data": o_stored_data.id})
-                    for o_process in l_process:
-                        # Suppression du traitement
-                        o_process.api_delete()
                     # Suppression de la donnée stockée
                     o_stored_data.api_delete()
                     # création de la ProcessingExecution
                     self.__processing_execution = ProcessingExecution.api_create(self.definition_dict["body_parameters"])
                     d_info = self.__processing_execution.get_store_properties()["output"]
                 # Comportements non supportés
                 else:
@@ -259,7 +253,22 @@
         if "upload" in d_output:
             d_el = self.definition_dict["body_parameters"]["output"]["upload"]
         elif "stored_data" in d_output:
             d_el = self.definition_dict["body_parameters"]["output"]["stored_data"]
         else:
             return False
         return "name" in d_el
+
+    ##############################################################
+    # Fonctions de représentation
+    ##############################################################
+    def __str__(self) -> str:
+        # Affichage à destination d'un utilisateur.
+        # On affiche l'id et le nom si possible.
+
+        # Liste pour stocker les infos à afficher
+        l_infos = []
+        # Ajout de l'id
+        l_infos.append(f"workflow={self.workflow_context}")
+        if self.processing_execution:
+            l_infos.append(f"processing_execution={self.processing_execution.id}")
+        return f"{self.__class__.__name__}({', '.join(l_infos)})"
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/action/UploadAction.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/action/UploadAction.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     BEHAVIOR_DELETE = "DELETE"
     BEHAVIOR_CONTINUE = "CONTINUE"
 
     def __init__(self, dataset: Dataset, behavior: Optional[str] = None) -> None:
         self.__dataset: Dataset = dataset
         self.__upload: Optional[Upload] = None
         # On suit le comportement donnée en paramètre ou à défaut celui de la config
-        self.__behavior: str = behavior if behavior is not None else Config().get("upload", "behavior_if_exists")
+        self.__behavior: str = behavior if behavior is not None else Config().get_str("upload", "behavior_if_exists")
 
     def run(self) -> Upload:
         """Crée la livraison décrite dans le dataset et livre les données avant de
         retourner la livraison créée.
 
         Returns:
             livraison créée
@@ -79,15 +79,15 @@
                 # Sinon on continue avec cet upload pour le compléter (behavior == CONTINUE)
                 # cas livraison fermé : on plante
                 if not o_upload.is_open():
                     raise GpfApiError(f"Impossible de continuer, la livraison {o_upload} est fermée.")
                 Config().om.info(f"Livraison identique {o_upload} trouvée, le programme va la reprendre et la compléter.")
                 self.__upload = o_upload
         else:
-            # Si le livraison est nulle, on en crée une nouvelle (on utilise les champs de "upload_infos" du dataset)
+            # Si la livraison est nulle, on en crée une nouvelle (on utilise les champs de "upload_infos" du dataset)
             self.__upload = Upload.api_create(self.__dataset.upload_infos)
             Config().om.info(f"Livraison {self.__upload['name']} créée avec succès.")
 
     def __add_tags(self) -> None:
         """Ajoute les tags."""
         if self.__upload is not None and self.__dataset.tags is not None:
             Config().om.info(f"Livraison {self.__upload['name']} : ajout des {len(self.__dataset.tags)} tags...")
@@ -99,28 +99,71 @@
         if self.__upload is not None:
             Config().om.info(f"Livraison {self.__upload['name']} : ajout des {len(self.__dataset.comments)} commentaires...")
             for s_comment in self.__dataset.comments:
                 self.__upload.api_add_comment({"text": s_comment})
             Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.comments)} commentaires ont été ajoutés avec succès.")
 
     def __push_data_files(self) -> None:
-        """Téléverse les fichiers de données."""
+        """Téléverse les fichiers de données (listés dans le dataset)."""
         if self.__upload is not None:
-            Config().om.info(f"Livraison {self.__upload['name']} : téléversement des {len(self.__dataset.data_files)} fichiers de données...")
+            # Liste les fichiers déjà téléversés sur l'entrepôt et récupère leur taille
+            Config().om.info(f"Livraison {self.__upload['name']} : récupération de l'arborescence des données déjà téléversées...")
+            l_arborescence = self.__upload.api_tree()
+            d_destination_taille = UploadAction.parse_tree(l_arborescence)
+
             for p_file_path, s_api_path in self.__dataset.data_files.items():
+                # Regarde si le fichier du dataset est déjà dans la liste des fichiers téléversés sur l'entrepôt
+                # NB: sur l'entrepôt, tous les fichiers "data" sont dans le dossier parent "data" TODO vérifier que c'est toujours le cas !
+                s_data_api_path = f"{s_api_path}/{p_file_path.name}"
+                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}...")
+                if s_data_api_path in d_destination_taille:
+                    # le fichier est déjà livré, on check sa taille :
+                    if d_destination_taille[s_data_api_path] == p_file_path.stat().st_size:
+                        # le fichier a été complètement téléversé. On passe au fichier suivant.
+                        Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: déjà livré")
+                        continue
+
+                    # le fichier n'a pas été téléversé en totalité.
+                    # Si le mode "Append" n'est pas disponible sur le serveur, il faut supprimer le fichier à moitié téléversé.
+                    # Sinon il faudra reprendre le téléversement (!)
+                    self.__upload.api_delete_data_file(s_data_api_path)
+
+                # sinon, on doit livrer le fichier
                 self.__upload.api_push_data_file(p_file_path, s_api_path)
-            Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.data_files)} fichiers de données ont été téléversés avec succès.")
+                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: terminé")
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.data_files)} fichiers de données ont été ajoutés avec succès.")
 
     def __push_md5_files(self) -> None:
-        """Téléverse les fichiers de clefs."""
+        """Téléverse les fichiers de clefs (listés dans le dataset)."""
         if self.__upload is not None:
-            Config().om.info(f"Livraison {self.__upload['name']} : téléversement des {len(self.__dataset.md5_files)} fichiers de clefs...")
+            # Liste les fichiers md5 téléversés sur l'entrepôt et récupère leur taille
+            l_arborescence = self.__upload.api_tree()
+            d_destination_taille = UploadAction.parse_tree(l_arborescence)
+
             for p_file_path in self.__dataset.md5_files:
+                # Regarde si le fichier du dataset est déjà dans la liste des fichiers téléversés sur l'entrepôt
+                # NB: sur l'entrepot, tous les fichiers md5 sont à la racine
+                s_api_path = p_file_path.name
+                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}...")
+                if s_api_path in d_destination_taille:
+                    # le fichier est déjà livré, on check sa taille :
+                    if d_destination_taille[s_api_path] == p_file_path.stat().st_size:
+                        # le fichier a été complètement téléversé. On passe au fichier suivant.
+                        Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}: déjà livré")
+                        continue
+
+                    # le fichier n'a pas été téléversé en totalité.
+                    # Si le mode "Append" n'est pas disponible sur le serveur, il faut supprimer le fichier à moitié téléversé.
+                    # Sinon il faudra reprendre le téléversement (!)
+                    self.__upload.api_delete_data_file(s_api_path)
+
+                # sinon, on doit livrer le fichier
                 self.__upload.api_push_md5_file(p_file_path)
-            Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.md5_files)} fichiers de clefs ont été téléversés avec succès.")
+                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}: terminé")
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.md5_files)} fichiers md5 ont été ajoutés avec succès.")
 
     def __close(self) -> None:
         """Ferme la livraison."""
         if self.__upload is not None:
             Config().om.info(f"Livraison {self.__upload['name']} : fermeture de la livraison...")
             self.__upload.api_close()
             Config().om.info(f"Livraison {self.__upload['name']} : livraison fermée avec succès. La livraison va maintenant être vérifiée par la Géoplateforme.")
@@ -157,15 +200,15 @@
             upload (Upload): Livraison à monitorer
             callback (Optional[Callable[[str], None]]): fonction de callback à exécuter avec le message de suivi.
 
         Returns:
             True si toutes les vérifications sont ok, sinon False
         """
         i_nb_sec_between_check = Config().get_int("upload", "nb_sec_between_check_updates")
-        s_check_message_pattern = Config().get("upload", "check_message_pattern")
+        s_check_message_pattern = Config().get_str("upload", "check_message_pattern")
         b_success: Optional[bool] = None
         Config().om.info(f"Monitoring des vérifications toutes les {i_nb_sec_between_check} secondes...")
         while b_success is None:
             # On récupère les vérifications
             d_checks = upload.api_list_checks()
             # On peut déterminer b_success s'il n'y en a plus en attente et en cours
             if len(d_checks["asked"]) == len(d_checks["in_progress"]) == 0:
@@ -208,18 +251,18 @@
         for d_element in tree:
             # On complète le chemin
             if prefix != "":
                 s_chemin = f"{prefix}/{d_element['name']}"
             else:
                 s_chemin = str(d_element["name"])
             # Fichier ou dossier ?
-            if d_element["type"] == "file":
+            if d_element["type"].lower() == "file":
                 # Fichier, on l'ajoute à notre dictionnaire
                 d_files[s_chemin] = int(d_element["size"])
-            elif d_element["type"] == "directory":
+            elif d_element["type"].lower() == "directory":
                 # Dossier, on itère dessus avec le nom du dossier comme préfixe
                 d_sub_files = UploadAction.parse_tree(d_element["children"], prefix=s_chemin)
                 # On fusionne ces fichiers à notre dict principal
                 d_files = {**d_files, **d_sub_files}
             else:
                 raise GpfApiError(f"Type d'élément rencontré dans l'arborescence '{d_element['type']}' non géré. Contacter le support.")
         return d_files
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/AbstractResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/AbstractResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/DictResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/DictResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/Errors.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/Errors.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/FileResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/FileResolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         Contenu du fichier `list.json` :
 
         ```json
         ["valeur 1", "valeur 2"]
         ```
 
-        Chaîne à remplacer : `{"values": "{file.str(list.json)"]}`
+        Chaîne à remplacer : `{"values": "{file.list(list.json)"]}`
 
         Résultat : `{"values": ["valeur 1", "valeur 2"]}`
 
 
     Fichier de clé-valeur :
 
         Contenu du fichier `dict.json` :
@@ -53,15 +53,15 @@
 
         Résultat : `{"parameters": {"k1":"v1", "k2":"v2"}}`
 
     Attributes:
         __name (str): nom de code du resolver
     """
 
-    _file_regex = re.compile(Config().get("workflow_resolution_regex", "file_regex"))
+    _file_regex = re.compile(Config().get_str("workflow_resolution_regex", "file_regex"))
 
     def __resolve_str(self, string_to_solve: str, s_path: str) -> str:
         """fonction privé qui se charge d'extraire une string d'un fichier texte
            on valide que le contenu est bien un texte
         Args:
             string_to_solve (str): chaîne à résoudre
             s_path (str): string du path du fichier à ouvrir
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/GlobalResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/GlobalResolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class GlobalResolver(metaclass=Singleton):
     """Classe permettant de résoudre une action en appelant les tous résolveurs listés.
 
     Attributes:
         __resolvers (Dict[str, AbstractResolver]): association nom du résolveur / résolveur.
     """
 
-    _regex: Pattern[str] = re.compile(Config().get("workflow_resolution_regex", "global_regex"))
+    _regex: Pattern[str] = re.compile(Config().get_str("workflow_resolution_regex", "global_regex"))
     _solved_strings: Dict[str, str] = {}
 
     def __init__(self) -> None:
         """Constructeur."""
         self.__resolvers: Dict[str, AbstractResolver] = {}
 
     def add_resolver(self, resolver: AbstractResolver) -> None:
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/StoreEntityResolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from ignf_gpf_api.store.StoredData import StoredData
 from ignf_gpf_api.store.StoreEntity import StoreEntity
 from ignf_gpf_api.store.Configuration import Configuration
 from ignf_gpf_api.store.ProcessingExecution import ProcessingExecution
 from ignf_gpf_api.store.Offering import Offering
 from ignf_gpf_api.store.Upload import Upload
 from ignf_gpf_api.store.Endpoint import Endpoint
+from ignf_gpf_api.store.Static import Static
+from ignf_gpf_api.store.Datastore import Datastore
 from ignf_gpf_api.io.Config import Config
 
 
 class StoreEntityResolver(AbstractResolver):
     """Classe permettant de résoudre des paramètres faisant référence à une entité.
 
     Attributes:
@@ -27,24 +29,26 @@
         Upload.entity_name(): Upload,
         Processing.entity_name(): Processing,
         StoredData.entity_name(): StoredData,
         Configuration.entity_name(): Configuration,
         Offering.entity_name(): Offering,
         ProcessingExecution.entity_name(): ProcessingExecution,
         Endpoint.entity_name(): Endpoint,
+        Static.entity_name(): Static,
+        Datastore.entity_name(): Datastore,
     }
 
     def __init__(self, name: str) -> None:
         """À l'instanciation, le résolveur est nommé selon ce qui est indiqué dans la Config.
 
         Args:
             name (str): nom du résolveur
         """
         super().__init__(name)
-        self.__regex: Pattern[str] = re.compile(Config().get("workflow_resolution_regex", "store_entity_regex"))
+        self.__regex: Pattern[str] = re.compile(Config().get_str("workflow_resolution_regex", "store_entity_regex"))
 
     def resolve(self, string_to_solve: str) -> str:
         # On parse la chaîne à résoudre
         o_result = self.regex.search(string_to_solve)
         if o_result is None:
             raise ResolverError(self.name, string_to_solve)
         d_groups = o_result.groupdict()
```

### Comparing `ignf_gpf_api-0.1.8/ignf_gpf_api/workflow/resolver/UserResolver.py` & `ignf_gpf_api-0.1.9/ignf_gpf_api/workflow/resolver/UserResolver.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/mkdocs.yml` & `ignf_gpf_api-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/pyproject.toml` & `ignf_gpf_api-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "types-requests",
     "jsonschema",
     "jsonc-parser",
     "toml",
     "types-toml",
     "python-dateutil",
     "types-python-dateutil",
+    "pyotp",
 ]
 
 [project.optional-dependencies]
 test = [
     "black<23",
     "pylint==2.17",
     "mypy==0.950",
```

### Comparing `ignf_gpf_api-0.1.8/tests/ErrorsTestCase.py` & `ignf_gpf_api-0.1.9/tests/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/GpfTestCase.py` & `ignf_gpf_api-0.1.9/tests/GpfTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/MainTestCase.py` & `ignf_gpf_api-0.1.9/tests/MainTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json` & `ignf_gpf_api-0.1.9/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf` & `ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp` & `ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx` & `ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json` & `ignf_gpf_api-0.1.9/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_data/workflows/bad-workflow.jsonc` & `ignf_gpf_api-0.1.9/tests/_data/workflows/bad-workflow.jsonc`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/_test/helper/JsonHelper/schema.json` & `ignf_gpf_api-0.1.9/tests/_test/helper/JsonHelper/schema.json`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/auth/AuthentifierTestCase.py` & `ignf_gpf_api-0.1.9/tests/auth/AuthentifierTestCase.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             # On a dû faire une requête
             self.assertEqual(o_mock.call_count, 1, "o_mock.call_count == 1")
             # Vérifications sur l'historique (enfin ici y'a une requête...)
             o_history = o_mock.request_history
             # Requête 1 : vérification du type
             self.assertEqual(o_history[0].method.lower(), "post", "method == post")
             # Requête 1 : vérification du text
-            s_text = "grant_type=password&username=TEST_LOGIN&password=TEST_PASSWORD&client_id=TEST_CLIENT_ID"
+            s_text = "grant_type=password&username=TEST_LOGIN&password=TEST_PASSWORD&client_id=TEST_CLIENT_ID&client_secret="
             self.assertEqual(o_history[0].text, s_text, "check text")
 
     def test_get_access_token_string_2_attempts(self) -> None:
         """Vérifie le bon fonctionnement de get_access_token_string si plusieurs tentatives."""
         # On mock...
         with requests_mock.Mocker() as o_mock:
             # Deux erreurs puis une authentification réussie
```

### Comparing `ignf_gpf_api-0.1.8/tests/auth/TokenTestCase.py` & `ignf_gpf_api-0.1.9/tests/auth/TokenTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/helper/FileHelperTestCase.py` & `ignf_gpf_api-0.1.9/tests/helper/FileHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/helper/JsonHelperTestCase.py` & `ignf_gpf_api-0.1.9/tests/helper/JsonHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/io/ApiRequesterTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/ApiRequesterTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/io/ConfigTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/ConfigTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/io/DatasetTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/DatasetTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,9 +44,9 @@
             },
         )
         self.assertEqual(o_dataset.md5_files, [p_root / "CANTON.md5"])
         self.assertTrue(p_md5.exists(), "CANTON.md5 n'existe pas")
         s_data_md5 = p_md5.read_text(encoding="UTF-8")
         for p_file in o_dataset.data_files:
             s_md5 = FileHelper.md5_hash(p_file)
-            s_line = f"{s_md5}  data/{p_file.relative_to(p_root)}"
+            s_line = f"{s_md5}  {p_file.relative_to(p_root)}"
             self.assertIn(s_line, s_data_md5)
```

### Comparing `ignf_gpf_api-0.1.8/tests/io/DescriptorFileReaderTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/DescriptorFileReaderTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/io/ErrorsTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/io/JsonConverterTestCase.py` & `ignf_gpf_api-0.1.9/tests/io/JsonConverterTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/ConfigurationTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/ConfigurationTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/EndpointTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/EndpointTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/ErrorsTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/EventInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/EventInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/ProcessingExecutionTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/ProcessingExecutionTestCase.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,37 @@
 
     cmd : python3 -m unittest -b tests.store.ProcessingExecutionTestCase
     """
 
     def test_api_logs(self) -> None:
         """Vérifie le bon fonctionnement de api_logs."""
         s_data = "2022/05/18 14:29:25       INFO §USER§ Envoi du signal de début de l'exécution à l'API.\n2022/05/18 14:29:25       INFO §USER§ Signal transmis avec succès."
-        # Instanciation d'une fausse réponse HTTP
-        o_response = GpfTestCase.get_response(text=s_data)
-        # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
-        with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
-            # on appelle la fonction à tester : api_logs
-            o_processing_execution = ProcessingExecution({"_id": "id_entité"})
-            s_data_recupere = o_processing_execution.api_logs()
+        l_rep = [
+            {"data": s_data, "rep": s_data},
+            {"data": "", "rep": ""},
+            {"data": "[]", "rep": ""},
+            {"data": '["log1", "log2", " log \\"complexe\\""]', "rep": 'log1\nlog2\n log "complexe"'},
+        ]
+
+        for d_rep in l_rep:
+            # Instanciation d'une fausse réponse HTTP
+            o_response = GpfTestCase.get_response(text=d_rep["data"])
+            # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
+            with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
+                # on appelle la fonction à tester : api_logs
+                o_processing_execution = ProcessingExecution({"_id": "id_entité"})
+                s_data_recupere = o_processing_execution.api_logs()
 
-            # on vérifie que route_request est appelé correctement
-            o_mock_request.assert_called_once_with(
-                "processing_execution_logs",
-                route_params={"processing_execution": "id_entité"},
-            )
-            # on vérifie la similitude des données retournées
-            self.assertEqual(s_data, s_data_recupere)
+                # on vérifie que route_request est appelé correctement
+                o_mock_request.assert_called_once_with(
+                    "processing_execution_logs",
+                    route_params={"processing_execution": "id_entité"},
+                )
+                # on vérifie la similitude des données retournées
+                self.assertEqual(d_rep["rep"], s_data_recupere)
 
     def test_api_launch(self) -> None:
         """Vérifie le bon fonctionnement de api_launch."""
         # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
         with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
             # on appelle la fonction à tester : api_launch
             o_processing_execution = ProcessingExecution({"_id": "id_entité"})
```

### Comparing `ignf_gpf_api-0.1.8/tests/store/StoreEntityTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/StoreEntityTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
             # Vérification sur o_mock_request
             # Fonction appelée 3 fois
             self.assertEqual(o_mock_request.call_count, 2)
             # Paramètres ok, avec pages de 1 à 2
             self.assertListEqual(
                 o_mock_request.call_args_list,
                 [
-                    call("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 1, "limit": 10}),
-                    call("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 2, "limit": 10}),
+                    call("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 1, "limit": 10}),
+                    call("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 2, "limit": 10}),
                 ],
             )
             # Vérifications sur l_entities
             self.assertIsInstance(l_entities, list)
             self.assertEqual(len(l_entities), 12)
             for i, o_entity in enumerate(l_entities, start=1):
                 self.assertIsInstance(o_entity, StoreEntity)
@@ -169,15 +169,15 @@
             # Vérification sur o_mock_request
             # Fonction appelée 1 fois
             self.assertEqual(o_mock_request.call_count, 1)
             # Paramètres ok, avec page 1 uniquement
             self.assertListEqual(
                 o_mock_request.call_args_list,
                 [
-                    call("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 1, "limit": 10}),
+                    call("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 1, "limit": 10}),
                 ],
             )
             # Vérifications sur l_entities
             self.assertIsInstance(l_entities, list)
             self.assertEqual(len(l_entities), 10)
             for i, o_entity in enumerate(l_entities, start=1):
                 self.assertIsInstance(o_entity, StoreEntity)
@@ -190,45 +190,45 @@
         # On a une réponse renvoyant 2 entités et indiquant qu'il y a 2 entités au total
         o_response = GpfTestCase.get_response(json=[{"_id": "1"}, {"_id": "2"}], headers={"Content-Range": "1-2/2"})
         # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons param
         with patch.object(ApiRequester(), "route_request", return_value=o_response) as o_mock_request:
             # On effectue le listing d'une entité
             l_entities = StoreEntity.api_list(infos_filter={"k_info": "v_info"}, tags_filter={"k_tag": "v_tag"})
             # Vérification sur o_mock_request
-            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 1, "limit": 10})
+            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 1, "limit": 10})
             # Vérifications sur l_entities
             self.assertIsInstance(l_entities, list)
             self.assertEqual(len(l_entities), 2)
             for i, o_entity in enumerate(l_entities, start=1):
                 self.assertIsInstance(o_entity, StoreEntity)
                 self.assertEqual(o_entity.id, str(i))
 
         # On a une réponse renvoyant 2 entités et sans Content-Range
         o_response = GpfTestCase.get_response(json=[{"_id": "1"}, {"_id": "2"}])
         # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons param
         with patch.object(ApiRequester(), "route_request", return_value=o_response) as o_mock_request:
             # On effectue le listing d'une entité
             l_entities = StoreEntity.api_list(infos_filter={"k_info": "v_info"}, tags_filter={"k_tag": "v_tag"})
             # Vérification sur o_mock_request
-            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 1, "limit": 10})
+            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 1, "limit": 10})
             # Vérifications sur l_entities
             self.assertIsInstance(l_entities, list)
             self.assertEqual(len(l_entities), 2)
             for i, o_entity in enumerate(l_entities, start=1):
                 self.assertIsInstance(o_entity, StoreEntity)
                 self.assertEqual(o_entity.id, str(i))
 
         # On a une réponse renvoyant 2 entités et avec un content-range non parsable
         o_response = GpfTestCase.get_response(json=[{"_id": "1"}, {"_id": "2"}], headers={"Content-Range": "non_parsable"})
         # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons param
         with patch.object(ApiRequester(), "route_request", return_value=o_response) as o_mock_request:
             # On effectue le listing d'une entité
             l_entities = StoreEntity.api_list(infos_filter={"k_info": "v_info"}, tags_filter={"k_tag": "v_tag"})
             # Vérification sur o_mock_request
-            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[]": ["k_tag=v_tag"], "page": 1, "limit": 10})
+            o_mock_request.assert_called_once_with("store_entity_list", params={"k_info": "v_info", "tags[k_tag]": "v_tag", "page": 1, "limit": 10})
             # Vérifications sur l_entities
             self.assertIsInstance(l_entities, list)
             self.assertEqual(len(l_entities), 2)
             for i, o_entity in enumerate(l_entities, start=1):
                 self.assertIsInstance(o_entity, StoreEntity)
                 self.assertEqual(o_entity.id, str(i))
```

### Comparing `ignf_gpf_api-0.1.8/tests/store/UploadTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/UploadTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/CommentInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/CommentInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/CsfInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/CsfInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/FullEditInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/FullEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/PartialEditInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/PartialEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/SharingInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/SharingInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/store/interface/TagInterfaceTestCase.py` & `ignf_gpf_api-0.1.9/tests/store/interface/TagInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/WorkflowTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/WorkflowTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         # On teste le workflow archive-generic.jsonc
         o_workflow_1 = Workflow.open_workflow(p_workflows / "archive-generic.jsonc")
         self.assertEqual(o_workflow_1.name, "archive-generic.jsonc")
         self.assertEqual(len(o_workflow_1.steps), 3)
         # On teste le workflow wfs-generic.jsonc
         o_workflow_2 = Workflow.open_workflow(p_workflows / "wfs-generic.jsonc", "wfs generic")
         self.assertEqual(o_workflow_2.name, "wfs generic")
-        self.assertEqual(len(o_workflow_2.steps), 4)
+        self.assertEqual(len(o_workflow_2.steps), 8)
         # On teste un fichier inexistant
         with self.assertRaises(GpfApiError) as o_arc:
             Workflow.open_workflow(Path("pas_là.json"))
         self.assertEqual(o_arc.exception.message, "Le fichier de workflow pas_là.json est introuvable. Contactez le support.")
 
     def test_validate(self) -> None:
         """Test de la fonction validate."""
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/action/ActionAbstractTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/action/ActionAbstractTestCase.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,26 @@
             o_mock_resolve.assert_called_once_with(str(json.dumps(d_definition, indent=4)))
 
     def test_get_filters(self) -> None:
         """Test de get_filters."""
         d_info_full = {"info_1": "val_1", "info_2": "val_2", "info_3": "val_3"}
         d_tags_full = {"tag_1": "val_1", "tag_2": "val_2", "tag_3": "val_3"}
         # On mock la fonction Config.get
-        with patch.object(Config(), "get", side_effect=["info_1;info_2", "tag_3"]) as o_mock_get:
+        with patch.object(Config(), "get_str", side_effect=["info_1;info_2", "tag_3"]) as o_mock_get:
             # Appel
             d_infos, d_tags = ActionAbstract.get_filters("config_key", d_info_full, d_tags_full)
             # Vérifications
             # Fonction appelée 2 fois
             self.assertEqual(o_mock_get.call_count, 2)
             # Pour récupère la liste des infos à filter
-            o_mock_get.assert_any_call("config_key", "uniqueness_constraint_infos")
+            o_mock_get.assert_any_call("config_key", "uniqueness_constraint_infos", "")
             # Pour récupère la liste des tags à filter
-            o_mock_get.assert_any_call("config_key", "uniqueness_constraint_tags")
+            o_mock_get.assert_any_call("config_key", "uniqueness_constraint_tags", "")
             # Vérifications critères conservés
             self.assertDictEqual(d_infos, {"info_1": "val_1", "info_2": "val_2"})
             self.assertDictEqual(d_tags, {"tag_3": "val_3"})
+
+    def test_str(self) -> None:
+        """test de __str__"""
+        d_definition = {"test": "val"}
+        o_action = ConcreteAction("nom", d_definition, None)
+        self.assertEqual("ConcreteAction(workflow=nom)", str(o_action))
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/action/ConfigurationActionTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/action/ConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/action/OfferingActionTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/action/OfferingActionTestCase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from unittest.mock import patch, MagicMock
+from typing import Any
 
 from ignf_gpf_api.store.Offering import Offering
 from ignf_gpf_api.store.Configuration import Configuration
 from ignf_gpf_api.workflow.action.OfferingAction import OfferingAction
 
 from tests.GpfTestCase import GpfTestCase
 
@@ -48,26 +49,55 @@
         """test de run quand l'offre à créer existe"""
         # Instanciation de OfferingAction
         o_offering_action = self.__get_offering_action()
 
         # mock de offering
         o_mock_offering = MagicMock()
         o_mock_offering.api_launch.return_value = None
-        o_mock_offering.__getitem__.return_value = "getitem"
 
-        with patch.object(o_offering_action, "find_offering", return_value=o_mock_offering) as o_mock_offering_action_list_offering:
-            with patch.object(Offering, "api_create", return_value=None) as o_mock_offering_api_create:
-                # on lance l'exécution de run
-                o_offering_action.run()
+        def side_effect_dict(arg: str) -> Any:
+            """side_effect pour récupération des élément de offering, gestion du cas des url qui sont dans un dictionnaire
 
-                # test de l'appel à OfferingAction.find_offering
-                o_mock_offering_action_list_offering.assert_called_once()
+            Args:
+                arg (str): clef à affiché
 
-                # test de l'appel à Offering.api_create
-                o_mock_offering_api_create.assert_not_called()
+            Returns:
+                Any: valeur de retour
+            """
+            if arg == "urls":
+                return [{"url": "http://1"}, {"url": "http://2"}]
+            return "getitem"
+
+        def side_effect_text(arg: str) -> Any:
+            """side_effect pour récupération des élément de offering, gestion du cas des url qui sont donné directement
+
+            Args:
+                arg (str): clef à affiché
+
+            Returns:
+                Any: valeur de retour
+            """
+            if arg == "urls":
+                return ["http://1", "http://2"]
+            return "getitem"
+
+        for f_effect in [side_effect_dict, side_effect_text]:
+
+            o_mock_offering.__getitem__.side_effect = f_effect
+
+            with patch.object(o_offering_action, "find_offering", return_value=o_mock_offering) as o_mock_offering_action_list_offering:
+                with patch.object(Offering, "api_create", return_value=None) as o_mock_offering_api_create:
+                    # on lance l'exécution de run
+                    o_offering_action.run()
+
+                    # test de l'appel à OfferingAction.find_offering
+                    o_mock_offering_action_list_offering.assert_called_once()
+
+                    # test de l'appel à Offering.api_create
+                    o_mock_offering_api_create.assert_not_called()
 
     def test_find_offering_exists_and_ok(self) -> None:
         """Test de find_offering quand une offering est trouvée et que le endpoint correspond."""
         # Instanciation de OfferingAction
         o_offering_action = self.__get_offering_action()
 
         # mock de Offering
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/action/ProcessingExecutionActionTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/action/ProcessingExecutionActionTestCase.py`

 * *Files 3% similar despite different names*

```diff
@@ -324,7 +324,19 @@
         for s_output in ["upload", "stored_data"]:
             for b_new in [True, False]:
                 d_output = {"name": "new"} if b_new else {"_id": "ancien"}
                 d_definition_dict: Dict[str, Any] = {"body_parameters":{"output":{s_output:d_output}}}
                 # initialisation de ProcessingExecutionAction
                 o_pea = ProcessingExecutionAction("contexte", d_definition_dict)
                 self.assertEqual(o_pea.output_new_entity, b_new)
+
+
+    def test_str(self) -> None:
+        """test de __str__"""
+        d_definition = {"_id": "ancien"}
+        # test sans processing execution
+        o_action = ProcessingExecutionAction("nom", d_definition)
+        self.assertEqual("ProcessingExecutionAction(workflow=nom)", str(o_action))
+        # test avec processing execution
+        with patch('ignf_gpf_api.workflow.action.ProcessingExecutionAction.ProcessingExecutionAction.processing_execution', new_callable=PropertyMock) as o_mock_processing_execution:
+            o_mock_processing_execution.return_value = MagicMock(id='test uuid')
+            self.assertEqual("ProcessingExecutionAction(workflow=nom, processing_execution=test uuid)", str(o_action))
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/action/UploadActionTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/action/UploadActionTestCase.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 from ignf_gpf_api.io.Config import Config
 from ignf_gpf_api.Errors import GpfApiError
 from tests.GpfTestCase import GpfTestCase
 
 # pylint:disable=too-many-arguments
 # pylint:disable=too-many-locals
 # pylint:disable=too-many-branches
+# pylint:disable=dangerous-default-value
+# pylint:disable=too-many-statements
 # pylint:disable=protected-access
 # fmt: off
 # (on désactive le formatage en attendant Python 3.10 et la possibilité de mettre des parenthèses pour gérer le multi with proprement)
 
 
 class UploadActionTestCase(GpfTestCase):
     """Tests UploadAction class.
 
     cmd : python3 -m unittest -b tests.workflow.action.UploadActionTestCase
     """
 
+    # constante afin de savoir si un fichier téléversé est entièrement téléversé ou pas.
+    SIZE_OK = 10000
     @classmethod
     def setUpClass(cls) -> None:
         """fonction lancée une fois avant tous les tests de la classe"""
         super().setUpClass()
         # On détruit le Singleton Config
         Config._instance = None
         # On charge une config spéciale pour les tests d'upload
@@ -74,29 +78,34 @@
         run_fail: bool,
         data_files: Dict[Path, str],
         md5_files: List[Path],
         upload_infos: Dict[str, Any],
         tags: Dict[str, str],
         comments: List[str],
         message_exception: Optional[str] = None,
+        files_on_api: Dict[str, int] = {},
+        nb_data_files_on_api_ok: int = 0,
+        nb_md5_files_on_api_ok: int = 0,
     ) -> None:
         """Lance le test UploadAction.run selon un cas de figure. Faire varier les paramètres permet de jouer sur le cas testé.
-
         Args:
             behavior (Optional[str]): mode lorsque la livraison existe déjà
             return_value_find_upload (Optional[Upload]): liste des upload retourné par le mock de Upload.api_list
             api_create (bool): vérification de l'exécution de Upload.api_create (True => api_create exécuté; False => api_create non exécuté)
             api_delete (bool): vérification de l'exécution de Upload.api_delete (True => api_delete exécuté; False => api_delete non exécuté)
             run_fail (bool): vérification de l'exécution avec erreur de UploadAction.run (True => run plant; False => run s'exécute sans erreur)
             data_files (Dict[Path, str]): fichiers de données
-            md5_files (List[Path]): fichier de md5
-            upload_infos (Dict[str, Any]): information de la livraison
-            tags (Dict[str, str]): tag à ajouté à la livraison
-            comments (List[str]): commentaire à ajouté à la livraison
+            md5_files (List[Path]): fichiers de md5
+            upload_infos (Dict[str, Any]): informations de la livraison
+            tags (Dict[str, str]): tags à ajouter à la livraison
+            comments (List[str]): commentaires à ajouter à la livraison
             message_exception (Optional[str]): si run_fail==True le message d'erreur attendu
+            files_on_api (Dict[str, int]): liste des fichiers déjà livrés sur l'API et leur taille (SIZE_OK si ok)
+            nb_data_files_on_api_ok (int): nombre fichiers de données déjà livrés sur l'API et à ne pas re-livrer
+            nb_md5_files_on_api_ok (int): nombre fichiers de clé déjà livrés sur l'API et à ne pas re-livrer
         """
 
         def create(d_dict: Dict[str, Any]) -> Upload:
             print("new creation")
             d_dict["status"] = "OPEN"
             return Upload(d_dict)
 
@@ -115,17 +124,22 @@
             patch.object(Upload, "api_create", wraps=create) as o_mock_api_create, \
             patch.object(Upload, "api_close", MagicMock()) as o_mock_close, \
             patch.object(Upload, "api_delete", MagicMock()) as o_mock_api_delete, \
             patch.object(Upload, "api_add_tags", MagicMock()) as o_mock_api_add_tags, \
             patch.object(Upload, "api_add_comment", MagicMock()) as o_mock_api_add_comment, \
             patch.object(Upload, "api_push_data_file", MagicMock()) as o_mock_api_push_data_file, \
             patch.object(Upload, "api_push_md5_file", MagicMock()) as o_mock_api_push_md5_file, \
+            patch.object(Upload, "api_tree", MagicMock()) as o_mock_api_tree, \
+            patch.object(UploadAction, "parse_tree", return_value=files_on_api) as o_mock_parse_tree, \
             patch.object(Upload, "api_update", return_value=None), \
+            patch.object(Path, "stat") as o_mock_path_stat, \
             patch.object(Config, "get", wraps=config_get) \
         :
+            # Mock de la fonction stat
+            o_mock_path_stat.return_value.st_size = self.SIZE_OK
             # création du dataset
             o_mock_dataset = MagicMock()
             o_mock_dataset.data_files = data_files
             o_mock_dataset.md5_files = md5_files
             o_mock_dataset.upload_infos = upload_infos
             o_mock_dataset.tags = tags
             o_mock_dataset.comments = comments
@@ -142,45 +156,51 @@
             o_mock_find_upload.assert_called_once_with()
 
             # vérif de o_mock_api_create
             if api_create:
                 o_mock_api_create.assert_called_once_with(upload_infos)
             else:
                 o_mock_api_create.assert_not_called()
-
             # vérif de o_mock_api_delete
             if api_delete:
                 o_mock_api_delete.assert_called_once_with()
             else:
                 o_mock_api_delete.assert_not_called()
-
             # vérif de o_mock_api_add_tags
             if tags is not None:
                 o_mock_api_add_tags.assert_called_once_with(tags)
             else:
                 o_mock_api_add_tags.assert_not_called()
-
             # vérif de o_mock_api_add_comment
             if comments is not None:
-                assert o_mock_api_add_comment.call_count == len(comments)
+                self.assertEqual(o_mock_api_add_comment.call_count, len(comments))
                 for s_comment in comments:
                     o_mock_api_add_comment.assert_any_call({"text": s_comment})
             else:
                 o_mock_api_add_comment.assert_not_called()
-
             # vérif de o_mock_api_push_data_file
-            assert o_mock_api_push_data_file.call_count == len(data_files)
+            # appelée une fois par fichiers à livrer moins le nb de fichiers déjà livrés
+            self.assertEqual(o_mock_api_push_data_file.call_count, len(data_files) - nb_data_files_on_api_ok)
+            # appelée selon le Path des fichiers à livrer
             for p_file_path, s_api_path in data_files.items():
-                o_mock_api_push_data_file.assert_any_call(p_file_path, s_api_path)
-
+                # S'il ne sont pas déjà livrés et avec la bonne taille
+                if files_on_api.get(f"data/{s_api_path}") != self.SIZE_OK:
+                    o_mock_api_push_data_file.assert_any_call(p_file_path, s_api_path)
             # vérif de o_mock_api_push_md5_file
-            assert o_mock_api_push_md5_file.call_count == len(md5_files)
+            # appelée une fois par fichiers à livrer moins le nb de fichiers déjà livrés
+            self.assertEqual(o_mock_api_push_md5_file.call_count, len(md5_files) - nb_md5_files_on_api_ok)
+            # appelée selon le Path des fichiers à livrer
             for p_file_path in md5_files:
-                o_mock_api_push_md5_file.assert_any_call(p_file_path)
-
+                # S'il ne sont pas déjà livrés et avec la bonne taille
+                if files_on_api.get(p_file_path.name) != self.SIZE_OK:
+                    o_mock_api_push_md5_file.assert_any_call(p_file_path)
+            # vérif de o_mock_api_tree (appelée par UploadAction.__push_data_files et UploadAction.__push_md5_files)
+            self.assertEqual(o_mock_api_tree.call_count, 2)
+            # vérif de o_mock_parse_tree (appelée par UploadAction.__push_data_files et UploadAction.__push_md5_files)
+            self.assertEqual(o_mock_parse_tree.call_count, 2)
             # vérif de o_mock_close
             o_mock_close.assert_called_once_with()
 
     def test_run(self) -> None:
         """Lance le test de UploadAction.run selon plusieurs cas de figures."""
         self.run_args(
             behavior=None,
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/resolver/DictResolverTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/resolver/DictResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/resolver/FileResolverTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/resolver/FileResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/resolver/GlobalResolverTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/resolver/GlobalResolverTestCase.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     localization = {
         "Jacques_country": "France",
         "Jacques_city": "Paris",
         "Jacques_street": "Champs-Elysée",
         "John_country": "England",
         "John_city": "London",
         "John_street": "rue_Londres",
+        "city": ["Paris", "London"],
+        "store": {"Paris": "Champs-Elysée", "London": "rue_Londres"},
     }
     profession = {
         "chef": "Jacques",
         "sailor": "John",
     }
 
     @classmethod
@@ -39,14 +41,18 @@
         self.assertTrue("localization" in GlobalResolver().resolvers)
         self.assertTrue("profession" in GlobalResolver().resolvers)
 
     def test_resolve(self) -> None:
         """Vérifie le bon fonctionnement de la fonction resolve."""
         # Cas simples : une seule résolution
         self.assertEqual(GlobalResolver().resolve("{localization.Jacques_country}"), "France")
+        self.assertEqual(GlobalResolver().resolve('{"localization":"Jacques_country"}'), "France")
+        self.assertEqual(GlobalResolver().resolve('["localization","Jacques_country"]'), "France")
+        self.assertEqual(GlobalResolver().resolve('{"localization":"store"}'), "{'Paris': 'Champs-Elysée', 'London': 'rue_Londres'}")
+        self.assertEqual(GlobalResolver().resolve('["localization","city"]'), "['Paris', 'London']")
         self.assertEqual(GlobalResolver().resolve("{profession.sailor}"), "John")
         # Cas avancés : deux résolutions l'une dans l'autre
         self.assertEqual(GlobalResolver().resolve("{localization.{profession.sailor}_country}"), "England")
         self.assertEqual(GlobalResolver().resolve("{localization.{profession.chef}_city}"), "Paris")
         # Cas erreur :
         with self.assertRaises(ResolverNotFoundError) as o_arc:
             GlobalResolver().resolve("{resolver_not_found.foo}")
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/resolver/StoreEntityResolverTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/resolver/StoreEntityResolverTestCase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 from unittest.mock import patch
-from ignf_gpf_api.store.Endpoint import Endpoint
 
+from ignf_gpf_api.store.Endpoint import Endpoint
 from ignf_gpf_api.store.StoreEntity import StoreEntity
 from ignf_gpf_api.store.Upload import Upload
-
+from ignf_gpf_api.store.Datastore import Datastore
 from ignf_gpf_api.workflow.resolver.Errors import NoEntityFoundError, ResolverError
 from ignf_gpf_api.workflow.resolver.StoreEntityResolver import StoreEntityResolver
 
 from tests.GpfTestCase import GpfTestCase
 
 
 class StoreEntityResolverTestCase(GpfTestCase):
@@ -110,7 +110,33 @@
             s_to_solve = "endpoint.tags.k_tag [INFOS(type=ARCHIVE)]"
             with self.assertRaises(ResolverError) as o_arc:
                 o_store_entity_resolver.resolve("endpoint.tags.k_tag [INFOS(type=ARCHIVE)]")
             # Vérification erreur
             self.assertEqual(o_arc.exception.message, f"Erreur du résolveur 'store_entity' avec la chaîne '{s_to_solve}'.")
             # Vérifications o_mock_api_list
             o_mock_api_list.assert_called_once_with(infos_filter={"type": "ARCHIVE"}, tags_filter={}, page=1)
+
+    def test_resolve_datastore(self) -> None:
+        """Vérifie le bon fonctionnement de la fonction resolve pour un store.
+        On peut utiliser `name` pour filter sur le `name` et sur le `technical_name`.
+        """
+
+        o_store_entity_resolver = StoreEntityResolver("store_entity")
+        l_entities = [
+            Datastore({"_id": "1", "name": "Datastore 1", "technical_name": "ds1"}),
+        ]
+
+        # On mock la fonction api_list, on veut vérifier qu'elle est appelée avec les bons param
+        with patch.object(Datastore, "api_list", return_value=l_entities) as o_mock_api_list:
+            s_result = o_store_entity_resolver.resolve("datastore.infos._id [INFOS(name=ds1)]")
+            # Vérifications o_mock_api_list
+            o_mock_api_list.assert_called_once_with(infos_filter={"name": "ds1"}, tags_filter={}, page=1)
+            # Vérification id récupérée
+            self.assertEqual(s_result, "1")
+
+        # On mock la fonction api_list, on veut vérifier qu'elle est appelée avec les bons param
+        with patch.object(Datastore, "api_list", return_value=l_entities) as o_mock_api_list:
+            s_result = o_store_entity_resolver.resolve("datastore.infos._id [INFOS(name=Datastore 1)]")
+            # Vérifications o_mock_api_list
+            o_mock_api_list.assert_called_once_with(infos_filter={"name": "Datastore 1"}, tags_filter={}, page=1)
+            # Vérification id récupérée
+            self.assertEqual(s_result, "1")
```

### Comparing `ignf_gpf_api-0.1.8/tests/workflow/resolver/UserResolverTestCase.py` & `ignf_gpf_api-0.1.9/tests/workflow/resolver/UserResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/uml/classes.png` & `ignf_gpf_api-0.1.9/uml/classes.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/uml/classes.uxf` & `ignf_gpf_api-0.1.9/uml/classes.uxf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/uml/interfaces.png` & `ignf_gpf_api-0.1.9/uml/interfaces.png`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/uml/interfaces.uxf` & `ignf_gpf_api-0.1.9/uml/interfaces.uxf`

 * *Files identical despite different names*

### Comparing `ignf_gpf_api-0.1.8/PKG-INFO` & `ignf_gpf_api-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignf_gpf_api
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python API to simplify the use of the GPF HTTPS API.
 Author-email: Valentin Sasyan <valentin.sasyan@ign.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,14 +13,15 @@
 Requires-Dist: types-requests
 Requires-Dist: jsonschema
 Requires-Dist: jsonc-parser
 Requires-Dist: toml
 Requires-Dist: types-toml
 Requires-Dist: python-dateutil
 Requires-Dist: types-python-dateutil
+Requires-Dist: pyotp
 Requires-Dist: mkdocs-material==9.* ; extra == "doc"
 Requires-Dist: mkdocstrings[python] ; extra == "doc"
 Requires-Dist: black<23 ; extra == "test"
 Requires-Dist: pylint==2.17 ; extra == "test"
 Requires-Dist: mypy==0.950 ; extra == "test"
 Requires-Dist: requests_mock ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
```

