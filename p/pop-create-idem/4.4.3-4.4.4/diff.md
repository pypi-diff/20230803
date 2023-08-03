# Comparing `tmp/pop-create-idem-4.4.3.tar.gz` & `tmp/pop-create-idem-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-4.4.3.tar", last modified: Tue Aug  1 12:16:39 2023, max compression
+gzip compressed data, was "pop-create-idem-4.4.4.tar", last modified: Wed Aug  2 18:11:42 2023, max compression
```

## Comparing `pop-create-idem-4.4.3.tar` & `pop-create-idem-4.4.4.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5513 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4412 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8799 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     3989 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     3502 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/sls.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/cloudspec/customize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/customize/contracts/
--rw-r--r--   0 root         (0) root         (0)       32 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/customize/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2116 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/example.py
--rw-r--r--   0 root         (0) root         (0)     3756 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     6705 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3114 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/test.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2209 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     4216 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      451 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     5663 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     7937 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     4724 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6503 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     5055 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2715 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)     1338 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1398 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1831 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4032 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
--rw-r--r--   0 root         (0) root         (0)     1152 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1234 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
--rw-r--r--   0 root         (0) root         (0)      539 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1313 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
--rw-r--r--   0 root         (0) root         (0)     2223 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      819 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     3074 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
--rw-r--r--   0 root         (0) root         (0)      456 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2805 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.474303 pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.482304 pop-create-idem-4.4.3/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1204 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-01 12:16:38.000000 pop-create-idem-4.4.3/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 12:16:39.478304 pop-create-idem-4.4.3/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5513 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8423 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-01 12:16:39.000000 pop-create-idem-4.4.3/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-01 12:16:39.486304 pop-create-idem-4.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3304 2023-08-01 12:16:25.000000 pop-create-idem-4.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8799 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/sls.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/customize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/customize/contracts/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/customize/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/example.py
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/test.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6503 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      819 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.902600 pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 18:11:42.906600 pop-create-idem-4.4.4/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-02 18:11:42.000000 pop-create-idem-4.4.4/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 18:11:42.910600 pop-create-idem-4.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3304 2023-08-02 18:11:28.000000 pop-create-idem-4.4.4/setup.py
```

### Comparing `pop-create-idem-4.4.3/LICENSE` & `pop-create-idem-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/PKG-INFO` & `pop-create-idem-4.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.4.3
+Version: 4.4.4
 Summary: UNKNOWN
 Home-page: https://docs.idemproject.io/pop-create-idem/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/pop-create-idem
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/pop-create-idem/-/issues
@@ -154,11 +154,11 @@
 This command creates a new project with the boilerplate code needed to get started with each respective cloud provider.
 
 Next steps
 ++++++++++
 
 After you generate your Idem plugin:
 
-* Try the example Swagger petstore tutorial in the `tutorial` directory, which walks you through generating an Idem plugin with a Swagger specification.
-* Configure the plugin for your provider. See the `pop-create-idem` quickstart for instructions.
+* Configure the plugin for your provider. See the `quickstart <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/quickstart.html>`_ for instructions.
+* Try the example Swagger petstore tutorial `Auto-generate an Idem plugin from Swagger <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/swagger_example.html>`_, which walks you through generating an Idem plugin with a Swagger specification.
```

### Comparing `pop-create-idem-4.4.3/README.rst` & `pop-create-idem-4.4.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -127,9 +127,9 @@
 This command creates a new project with the boilerplate code needed to get started with each respective cloud provider.
 
 Next steps
 ++++++++++
 
 After you generate your Idem plugin:
 
-* Try the example Swagger petstore tutorial in the `tutorial` directory, which walks you through generating an Idem plugin with a Swagger specification.
-* Configure the plugin for your provider. See the `pop-create-idem` quickstart for instructions.
+* Configure the plugin for your provider. See the `quickstart <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/quickstart.html>`_ for instructions.
+* Try the example Swagger petstore tutorial `Auto-generate an Idem plugin from Swagger <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/swagger_example.html>`_, which walks you through generating an Idem plugin with a Swagger specification.
```

### Comparing `pop-create-idem-4.4.3/cloudspec/__init__.py` & `pop-create-idem-4.4.4/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/cloudspec/conf.py` & `pop-create-idem-4.4.4/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/sls.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/sls.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/init.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/example.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/example.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-4.4.4/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/conf.py` & `pop-create-idem-4.4.4/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/params.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-4.4.4/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/tool/format/case.py` & `pop-create-idem-4.4.4/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-4.4.4/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem/tool/gradle.py` & `pop-create-idem-4.4.4/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-4.4.4/pop_create_idem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.4.3
+Version: 4.4.4
 Summary: UNKNOWN
 Home-page: https://docs.idemproject.io/pop-create-idem/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/pop-create-idem
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/pop-create-idem/-/issues
@@ -154,11 +154,11 @@
 This command creates a new project with the boilerplate code needed to get started with each respective cloud provider.
 
 Next steps
 ++++++++++
 
 After you generate your Idem plugin:
 
-* Try the example Swagger petstore tutorial in the `tutorial` directory, which walks you through generating an Idem plugin with a Swagger specification.
-* Configure the plugin for your provider. See the `pop-create-idem` quickstart for instructions.
+* Configure the plugin for your provider. See the `quickstart <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/quickstart.html>`_ for instructions.
+* Try the example Swagger petstore tutorial `Auto-generate an Idem plugin from Swagger <https://docs.idemproject.io/pop-create-idem/en/latest/tutorial/swagger_example.html>`_, which walks you through generating an Idem plugin with a Swagger specification.
```

### Comparing `pop-create-idem-4.4.3/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-4.4.4/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.3/setup.py` & `pop-create-idem-4.4.4/setup.py`

 * *Files identical despite different names*

