# Comparing `tmp/aaz-dev-1.5.2.tar.gz` & `tmp/aaz-dev-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaz-dev-1.5.2.tar", last modified: Wed Aug  2 05:09:46 2023, max compression
+gzip compressed data, was "aaz-dev-1.6.0.tar", last modified: Thu Aug  3 08:20:17 2023, max compression
```

## Comparing `aaz-dev-1.5.2.tar` & `aaz-dev-1.6.0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.695994 aaz-dev-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-08-02 05:07:11.000000 aaz-dev-1.5.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 05:07:11.000000 aaz-dev-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 05:07:11.000000 aaz-dev-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-02 05:09:46.695994 aaz-dev-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-02 05:07:11.000000 aaz-dev-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 05:09:46.695994 aaz-dev-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.639994 aaz-dev-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.647994 aaz-dev-1.5.2/src/aaz_dev/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.651994 aaz-dev-1.5.2/src/aaz_dev/app/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/app/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/app/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/app/url_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.651994 aaz-dev-1.5.2/src/aaz_dev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.651994 aaz-dev-1.5.2/src/aaz_dev/cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/api/az.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/api/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_arg_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_module_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    38422 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_operation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_selector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/controller/portal_cli_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/common/_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.655994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/command/
--rw-r--r--   0 runner    (1001) docker     (123)    31945 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/group/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.659994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/setup.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/cli/templates/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/command/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/api/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.663994 aaz-dev-1.5.2/src/aaz_dev/command/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41719 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/cfg_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/specs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    67823 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/workspace_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/controller/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.667994 aaz-dev-1.5.2/src/aaz_dev/command/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.671994 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26098 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http_response_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    36541 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_selector_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_subresource_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.671994 aaz-dev-1.5.2/src/aaz_dev/command/model/editor/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/editor/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.671994 aaz-dev-1.5.2/src/aaz_dev/command/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/specs/_command_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/model/specs/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.671994 aaz-dev-1.5.2/src/aaz_dev/command/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/command.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/group.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/resource_ref.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/command/templates/tree.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.671994 aaz-dev-1.5.2/src/aaz_dev/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.675994 aaz-dev-1.5.2/src/aaz_dev/swagger/api/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.675994 aaz-dev-1.5.2/src/aaz_dev/swagger/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/controller/command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/controller/specs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.675994 aaz-dev-1.5.2/src/aaz_dev/swagger/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.679994 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/cmd_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/path_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.683994 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_resource_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.683994 aaz-dev-1.5.2/src/aaz_dev/swagger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/swagger/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.683994 aaz-dev-1.5.2/src/aaz_dev/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-08-02 05:08:49.000000 aaz-dev-1.5.2/src/aaz_dev/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-02 05:08:49.000000 aaz-dev-1.5.2/src/aaz_dev/ui/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-02 05:08:49.000000 aaz-dev-1.5.2/src/aaz_dev/ui/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 05:08:49.000000 aaz-dev-1.5.2/src/aaz_dev/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 05:08:49.000000 aaz-dev-1.5.2/src/aaz_dev/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.647994 aaz-dev-1.5.2/src/aaz_dev/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.687994 aaz-dev-1.5.2/src/aaz_dev/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.691994 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   574621 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2235009 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   146625 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   473675 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-02 05:09:45.000000 aaz-dev-1.5.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.695994 aaz-dev-1.5.2/src/aaz_dev/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/error_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/portal_file_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/src/aaz_dev/utils/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:09:46.647994 aaz-dev-1.5.2/src/aaz_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 05:09:46.000000 aaz-dev-1.5.2/src/aaz_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-02 05:07:12.000000 aaz-dev-1.5.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.763133 aaz-dev-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-08-03 08:19:39.000000 aaz-dev-1.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-03 08:19:39.000000 aaz-dev-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-03 08:19:39.000000 aaz-dev-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-03 08:20:17.763133 aaz-dev-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-08-03 08:19:39.000000 aaz-dev-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:20:17.763133 aaz-dev-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.727132 aaz-dev-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.731132 aaz-dev-1.6.0/src/aaz_dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.735132 aaz-dev-1.6.0/src/aaz_dev/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/app/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/app/url_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.735132 aaz-dev-1.6.0/src/aaz_dev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.735132 aaz-dev-1.6.0/src/aaz_dev/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/api/az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/api/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.735132 aaz-dev-1.6.0/src/aaz_dev/cli/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_arg_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_operation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_selector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/controller/portal_cli_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.735132 aaz-dev-1.6.0/src/aaz_dev/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/common/_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/command/
+-rw-r--r--   0 runner    (1001) docker     (123)    31945 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.739132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/setup.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/cli/templates/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/command/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/api/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/command/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41719 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/cfg_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/specs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67823 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/workspace_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/controller/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.743132 aaz-dev-1.6.0/src/aaz_dev/command/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.747132 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26098 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36541 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_selector_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_subresource_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.747132 aaz-dev-1.6.0/src/aaz_dev/command/model/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/editor/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.747132 aaz-dev-1.6.0/src/aaz_dev/command/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/specs/_command_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/model/specs/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.751133 aaz-dev-1.6.0/src/aaz_dev/command/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/command.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/group.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/resource_ref.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/command/templates/tree.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.751133 aaz-dev-1.6.0/src/aaz_dev/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.751133 aaz-dev-1.6.0/src/aaz_dev/swagger/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.751133 aaz-dev-1.6.0/src/aaz_dev/swagger/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/controller/command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/controller/specs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.751133 aaz-dev-1.6.0/src/aaz_dev/swagger/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.755133 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/cmd_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.755133 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_resource_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.755133 aaz-dev-1.6.0/src/aaz_dev/swagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/swagger/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.755133 aaz-dev-1.6.0/src/aaz_dev/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-08-03 08:19:53.000000 aaz-dev-1.6.0/src/aaz_dev/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-03 08:19:53.000000 aaz-dev-1.6.0/src/aaz_dev/ui/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-03 08:19:53.000000 aaz-dev-1.6.0/src/aaz_dev/ui/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-03 08:19:53.000000 aaz-dev-1.6.0/src/aaz_dev/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 08:19:53.000000 aaz-dev-1.6.0/src/aaz_dev/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.731132 aaz-dev-1.6.0/src/aaz_dev/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.755133 aaz-dev-1.6.0/src/aaz_dev/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.759133 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   574621 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2235009 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   146625 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   473675 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-03 08:20:16.000000 aaz-dev-1.6.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.763133 aaz-dev-1.6.0/src/aaz_dev/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/error_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/portal_file_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/src/aaz_dev/utils/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:20:17.731132 aaz-dev-1.6.0/src/aaz_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 08:20:17.000000 aaz-dev-1.6.0/src/aaz_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 08:19:40.000000 aaz-dev-1.6.0/version.py
```

### Comparing `aaz-dev-1.5.2/HISTORY.rst` & `aaz-dev-1.6.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 Release History
 ===============
 
+1.6.0
+++++++
+* Adding `profile_` prefix for azure stack profile in CLI aaz package (#274)
+
 1.5.2
 ++++++
 * Update docs for Command Usage and Testing (#270)
 * Fix bugs while command has no arguments (#271)
 * Add docs for subcommand generation (#272)
 
 1.5.1
```

### Comparing `aaz-dev-1.5.2/LICENSE` & `aaz-dev-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/PKG-INFO` & `aaz-dev-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.5.2
+Version: 1.6.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz-dev-1.5.2/README.md` & `aaz-dev-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/setup.py` & `aaz-dev-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/app/app.py` & `aaz-dev-1.6.0/src/aaz_dev/app/app.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/app/run.py` & `aaz-dev-1.6.0/src/aaz_dev/app/run.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/app/url_converters.py` & `aaz-dev-1.6.0/src/aaz_dev/app/url_converters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/api/_cmds.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/api/az.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/api/az.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/api/portal.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/api/portal.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_arg_group_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_arg_group_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_command_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_module_manager.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_module_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         lines = lines[:insert_after + 1] + insert_lines + lines[insert_after + 1:]
 
         yield file, '\n'.join(lines)
 
     def _load_view_profile(self, profile_name, aaz_path):
         profile = CLIViewProfile()
         profile.name = profile_name
-        profile_folder_name = profile_name.lower().replace('-', '_')
+        profile_folder_name = profile.profile_folder_name
         profile_path = os.path.join(aaz_path, profile_folder_name)
         if not os.path.exists(profile_path):
             return profile
         profile.command_groups = self._load_view_command_groups(path=profile_path)
         return profile
 
     def _load_view_command_groups(self, *names, path):
```

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_operation_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_operation_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,14 +876,15 @@
         for scopes in _iter_response_scopes_by_schema_base(s, s_name, s_scope_define, cmd_ctx):
             yield scopes
 
     for disc in discriminators:
         key_name = to_snack_case(disc.property)
         key_value = disc.value
         disc_name = f"disc_{to_snack_case(disc.value)}"
+
         disc_scope_define = f'{scope_define}.discriminate_by("{key_name}", "{key_value}")'
         for scopes in _iter_response_scopes_by_schema_base(disc, disc_name, disc_scope_define, cmd_ctx):
             yield scopes
 
 
 def render_schema(schema, cls_map, name):
     schema_kwargs = {}
```

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_output_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_output_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_profile_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_profile_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class AzProfileGenerator:
     """Used to generate atomic layer command group"""
 
     def __init__(self, aaz_folder, profile):
         self.aaz_folder = aaz_folder
         self.profile = profile
-        self.profile_folder_name = profile.name.lower().replace('-', '_')
+        self.profile_folder_name = profile.profile_folder_name
         self._removed_folders = set()
         self._removed_files = set()
         self._modified_files = {}
 
     def generate(self):
         # check aaz/__init__.py
         file_name = '__init__.py'
```

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/az_selector_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/az_selector_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/controller/portal_cli_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/controller/portal_cli_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_command.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_command_group.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/atomic/_help.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/atomic/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/common/_fields.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/common/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_command.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_command_group.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/model/view/_module.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/model/view/_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/__init__.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/_filters.py` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/extension/setup.py.j2` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/extension/setup.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/cli/templates/main/__init__.py.j2` & `aaz-dev-1.6.0/src/aaz_dev/cli/templates/main/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/api/_cmds.py` & `aaz-dev-1.6.0/src/aaz_dev/command/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/api/editor.py` & `aaz-dev-1.6.0/src/aaz_dev/command/api/editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/api/specs.py` & `aaz-dev-1.6.0/src/aaz_dev/command/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/controller/cfg_reader.py` & `aaz-dev-1.6.0/src/aaz_dev/command/controller/cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/controller/specs_manager.py` & `aaz-dev-1.6.0/src/aaz_dev/command/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/controller/workspace_cfg_editor.py` & `aaz-dev-1.6.0/src/aaz_dev/command/controller/workspace_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/controller/workspace_manager.py` & `aaz-dev-1.6.0/src/aaz_dev/command/controller/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/__init__.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg_builder.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_arg_group.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_arg_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_command.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_command_group.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_condition.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_condition.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_configuration.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_content.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_content.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_fields.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_format.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_help.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http_request_body.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http_request_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_http_response_body.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_http_response_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_create.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_create.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_delete.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_delete.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_instance_update.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_instance_update.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_operation.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_output.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_output.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_resource.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_schema.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_selector_index.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_selector_index.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_subresource_selector.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_subresource_selector.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/configuration/_xml.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/configuration/_xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/editor/_workspace.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/editor/_workspace.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/model/specs/_command_tree.py` & `aaz-dev-1.6.0/src/aaz_dev/command/model/specs/_command_tree.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/templates/__init__.py` & `aaz-dev-1.6.0/src/aaz_dev/command/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/templates/_filters.py` & `aaz-dev-1.6.0/src/aaz_dev/command/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/templates/command.md.j2` & `aaz-dev-1.6.0/src/aaz_dev/command/templates/command.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/command/templates/group.md.j2` & `aaz-dev-1.6.0/src/aaz_dev/command/templates/group.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/api/specs.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/controller/command_generator.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/controller/command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/controller/specs_manager.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/cmd_builder.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/contact.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/contact.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/fields.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/info.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/info.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/items.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/items.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/operation.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/parameter.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/path_item.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/path_item.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/reference.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/reference.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/response.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/response.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/schema.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/security_scheme.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/security_scheme.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/swagger.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/tag.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/tag.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/schema/xml.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/schema/xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_resource.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_resource_provider.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_resource_provider.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_module.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/model/specs/_utils.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/model/specs/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/swagger/utils/tools.py` & `aaz-dev-1.6.0/src/aaz_dev/swagger/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/asset-manifest.json` & `aaz-dev-1.6.0/src/aaz_dev/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/favicon.ico` & `aaz-dev-1.6.0/src/aaz_dev/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/index.html` & `aaz-dev-1.6.0/src/aaz_dev/ui/index.html`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/logo192.png` & `aaz-dev-1.6.0/src/aaz_dev/ui/logo192.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/logo512.png` & `aaz-dev-1.6.0/src/aaz_dev/ui/logo512.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js.map` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/main.1cbe9b1d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map` & `aaz-dev-1.6.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/config.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/config.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/error_format.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/error_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/exceptions.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/plane.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/plane.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/portal_file_schema.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/portal_file_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev/utils/stage.py` & `aaz-dev-1.6.0/src/aaz_dev/utils/stage.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.5.2/src/aaz_dev.egg-info/PKG-INFO` & `aaz-dev-1.6.0/src/aaz_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.5.2
+Version: 1.6.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz-dev-1.5.2/src/aaz_dev.egg-info/SOURCES.txt` & `aaz-dev-1.6.0/src/aaz_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

