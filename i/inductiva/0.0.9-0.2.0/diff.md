# Comparing `tmp/inductiva-0.0.9.tar.gz` & `tmp/inductiva-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.0.9.tar", last modified: Fri Apr 14 13:02:50 2023, max compression
+gzip compressed data, was "inductiva-0.2.0.tar", last modified: Thu Aug  3 16:10:00 2023, max compression
```

## Comparing `inductiva-0.0.9.tar` & `inductiva-0.2.0.tar`

### file list

```diff
@@ -1,140 +1,381 @@
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-04-14 10:18:54.000000 inductiva-0.0.9/MANIFEST.in
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3650 2023-04-14 13:02:50.492152 inductiva-0.0.9/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3276 2023-04-14 13:02:29.000000 inductiva-0.0.9/README.md
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/api/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/api/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/api/methods.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/api_client.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/path_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/admin_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/admin_user_username_tasks.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_submit.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_kill.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_output.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/paths/task_task_id_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tag_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/apis/tags/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/admin_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/apis/tags/tasks_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/configuration.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/model/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/body_upload_task_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/http_validation_error.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/new_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/queue_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/task_request.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/task_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/model/validation_error.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/models/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/models/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/admin_user/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_submit/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_submit/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_submit/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_input/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_output/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/paths/task_task_id_status/get.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/rest.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/client/schemas.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva/core/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/core/cupy/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/cupy/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/cupy/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/math.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/core/slepc/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/slepc/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/slepc/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/core/test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      571 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/fluid_types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/post_processing/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/post_processing/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/post_processing/splishsplash.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1748 2023-04-14 13:02:29.000000 inductiva-0.0.9/inductiva/fluids/scenarios/_post_processing.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2670 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/dam_break.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7904 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/unit_box.obj
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8868 2023-04-14 11:29:18.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9181 2023-04-14 11:29:18.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/shapes.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/fluids/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/dualsphysics.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/openfoam.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/splishsplash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/swash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/fluids/simulators/xbeach.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/molecules/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/molecules/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/molecules/simulators/gromacs.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1353 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/scenarios.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/simulation/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/simulation/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/simulation/simulator.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.492152 inductiva-0.0.9/inductiva/utils/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/data.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2159 2023-04-14 11:15:16.000000 inductiva-0.0.9/inductiva/utils/files.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/files_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/flags.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/meta.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/misc.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/misc_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-04-14 10:18:54.000000 inductiva-0.0.9/inductiva/utils/templates.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14281 2023-04-14 13:02:29.000000 inductiva-0.0.9/inductiva/utils/visualization.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 13:02:50.488152 inductiva-0.0.9/inductiva.egg-info/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3650 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/SOURCES.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/dependency_links.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/requires.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-14 13:02:50.000000 inductiva-0.0.9/inductiva.egg-info/top_level.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-14 10:18:54.000000 inductiva-0.0.9/pyproject.toml
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-14 13:02:50.492152 inductiva-0.0.9/setup.cfg
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-14 10:18:54.000000 inductiva-0.0.9/setup.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.338693 inductiva-0.2.0/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11357 2023-07-18 09:32:07.000000 inductiva-0.2.0/LICENSE
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-07-18 09:32:07.000000 inductiva-0.2.0/MANIFEST.in
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11551 2023-08-03 16:10:00.338693 inductiva-0.2.0/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11155 2023-08-03 13:51:42.000000 inductiva-0.2.0/README.md
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      427 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/admin/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      231 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/admin/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3015 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/admin/executers.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1521 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/admin/tasks.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/api/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      248 2023-07-24 10:52:30.000000 inductiva-0.2.0/inductiva/api/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14580 2023-07-24 10:52:30.000000 inductiva-0.2.0/inductiva/api/methods.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/client/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60868 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/api_client.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/client/apis/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3203 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/apis/path_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/apis/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      111 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_user_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_users.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      128 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_users_username.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      139 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/admin_users_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/executers_pools.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      128 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/executers_register.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      210 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/gcp_instances.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      227 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/gcp_instances_group.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/gcp_instances_price.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       98 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_task_id.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/task_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      100 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      116 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      128 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      127 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      136 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id_output_list.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      127 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/paths/tasks_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      707 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/tag_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/apis/tags/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      383 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/tags/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      799 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/tags/admin_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      655 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/tags/executers_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      959 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/apis/tags/instance_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1183 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/apis/tags/tasks_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16772 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/configuration.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/model/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2854 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/body_upload_task_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2915 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/executer.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11560 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/client/model/executer_create.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5892 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/client/model/executer_id.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4027 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/model/file_info.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7078 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/g_cloud_executer.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6276 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/g_cloud_host_info.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3686 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/http_validation_error.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5927 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/inductiva_executer.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3250 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/inductiva_host_info.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3369 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/instance.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11935 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/client/model/instance_create.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15807 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/client/model/instance_group.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4162 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/new_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4206 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/model/output_archive_info.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4488 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/queue_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2791 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/resource_pool_id.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    20840 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6677 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task_request.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3469 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2225 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task_status_code.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    21455 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task_with_user_info.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    21449 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/task_with_username.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4542 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9100 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/client/model/user_create.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2829 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/username.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8447 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/model/validation_error.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/models/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1905 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/models/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1063 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/paths/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14835 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_user/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_user/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12793 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_user/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_user_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_user_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10491 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_user_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_users/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12836 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_users_username/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      331 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users_username/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10606 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users_username/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/admin_users_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      343 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14161 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/admin_users_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/executers_pools/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      321 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/executers_pools/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8005 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/executers_pools/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/executers_register/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/executers_register/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12745 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/executers_register/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/gcp_instances/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      317 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12703 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances/delete.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12775 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/gcp_instances_group/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances_group/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12786 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances_group/delete.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12853 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances_group/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/gcp_instances_price/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances_price/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12723 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/gcp_instances_price/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      299 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12094 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12945 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_task_id/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      315 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10596 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15372 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10641 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10603 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/task_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10540 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/task_task_id_status/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      301 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12094 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      315 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12945 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      317 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10596 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15372 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10641 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      331 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13737 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output_list/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output_list/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10574 2023-08-03 13:51:30.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_output_list/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      331 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10540 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/paths/tasks_task_id_status/get.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12104 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/rest.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103945 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/client/schemas.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/core/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/core/cupy/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/cupy/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/cupy/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/math.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/core/slepc/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/slepc/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/slepc/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/core/test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2095 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/design.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/fluids/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      666 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/fluid_types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/fluids/post_processing/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/post_processing/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/post_processing/splishsplash.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/fluids/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      481 2023-08-03 16:09:17.000000 inductiva-0.2.0/inductiva/fluids/scenarios/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1346 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/_post_processing.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.314693 inductiva-0.2.0/inductiva/fluids/scenarios/coastal_area/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      132 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/coastal_area/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13752 2023-08-03 16:09:17.000000 inductiva-0.2.0/inductiva/fluids/scenarios/coastal_area/coastal_area.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7874 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/coastal_area/output.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/scenarios/dam_break/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/dam_break/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2758 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/scenarios/dam_break/dam_break.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8645 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1378 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/unit_box.obj
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      218 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9862 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9181 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2177 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/output.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/scenarios/heat_sink/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      109 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/heat_sink/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6364 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/scenarios/heat_sink/heat_sink.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4136 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/heat_sink/output.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/scenarios/wind_tunnel/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/wind_tunnel/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11471 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/fluids/scenarios/wind_tunnel/post_processing.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8679 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/scenarios/wind_tunnel/wind_tunnel.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/shapes.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/fluids/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/fluids/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1143 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/simulators/dualsphysics.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1239 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/simulators/openfoam.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1105 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/simulators/splishsplash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1093 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/simulators/swash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1092 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/fluids/simulators/xbeach.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/generative/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:09:17.000000 inductiva-0.2.0/inductiva/generative/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10420 2023-08-03 16:09:17.000000 inductiva-0.2.0/inductiva/generative/diamond_square.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/molecules/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      148 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/molecules/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      189 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/scenarios/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/molecules/scenarios/md_water_box/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/molecules/scenarios/md_water_box/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5273 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/molecules/scenarios/md_water_box/md_water_box.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1637 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/scenarios/md_water_box/post_processing.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/molecules/scenarios/protein_solvation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/scenarios/protein_solvation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5973 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/scenarios/protein_solvation/post_processing.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5527 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/molecules/scenarios/protein_solvation/protein_solvation.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1375 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/molecules/scenarios/utils.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/molecules/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/molecules/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1120 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/molecules/simulators/gromacs.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1600 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/scenarios.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/simulation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/simulation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1527 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/simulation/simulator.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      195 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3086 2023-07-18 10:43:30.000000 inductiva-0.2.0/inductiva/tasks/methods.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1101 2023-08-03 13:51:42.000000 inductiva-0.2.0/inductiva/tasks/run_simulation.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9995 2023-08-03 16:09:17.000000 inductiva-0.2.0/inductiva/tasks/task.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/coastal_area/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/templates/coastal_area/swash/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1366 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/templates/coastal_area/swash/input.sws.jinja
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/heat_sink/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.318693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      304 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/commands.json
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fins/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1310 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fins/T
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      869 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fins/p
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fluid/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1347 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fluid/T
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1216 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fluid/U
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      871 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fluid/p
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      987 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/fluid/p_rgh
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/heater/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1101 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/heater/T
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      869 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/0/heater/p
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fins/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1243 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fins/thermophysicalProperties
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fluid/
+-rwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)     1029 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fluid/fvOptions
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      769 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fluid/g
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1316 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fluid/thermophysicalProperties
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      735 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/fluid/turbulenceProperties
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      769 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/g
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/heater/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1114 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/heater/fvOptions
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1243 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/heater/thermophysicalProperties
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      767 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/regionProperties
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/triSurface/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9243 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/triSurface/fluidHeaterFins.stl
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    55184 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/triSurface/interface_fluid.stl
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      522 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/constant/triSurface/interface_heater.stl
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000) 38295006 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/fluidHeaterFins.unv
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      874 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/parameters.jinja
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1162 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/blockMeshDict
+-rwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)      716 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/cellMaxFinT
+-rwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)      718 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/cellMaxHeaterT
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1971 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/controlDict
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      763 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/decomposeParDict
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fins/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1013 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fins/fvSchemes
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1037 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fins/fvSolution
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fluid/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1165 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fluid/fvSchemes
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1465 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fluid/fvSolution
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      745 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fvSchemes
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      703 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/fvSolution
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/heater/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1013 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/heater/fvSchemes
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1036 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/heater/fvSolution
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      757 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/meshQualityDict
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3016 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/snappyHexMeshDict
+-rwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)      953 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/volAvgFinTemperature
+-rwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)      957 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/heat_sink/openfoam/files/system/volAvgHeaterTemperature
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/md_water_box/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      786 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/commands.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      898 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/energy_minimization.mdp.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1343 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/positions_decorrelation.mdp
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1449 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/simulation.mdp.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      113 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/md_water_box/gromacs/topol.top
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/protein_solvation/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/protein_solvation/gromacs/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      920 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/templates/protein_solvation/gromacs/commands.json
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      847 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/protein_solvation/gromacs/energy_minimization.mdp.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      680 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/templates/protein_solvation/gromacs/ions.mdp
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1435 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/templates/protein_solvation/gromacs/simulation.mdp.jinja
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/wind_tunnel/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      692 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/commands.json.jinja
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1302 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/U.orig
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/include/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      531 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/include/fixedInlet
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      535 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/include/frontBackUpperPatches
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      644 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/include/initialConditions_template.openfoam.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1365 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/k
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1458 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/nut
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1344 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/omega
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1228 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/0/p
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/constant/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      745 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/constant/transportProperties
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      798 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/constant/turbulenceProperties
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.334693 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1885 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/blockMeshDict_template.openfoam.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1155 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/controlDict_template.openfoam.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      991 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/cuttingPlane
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      732 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/decomposeParDict_template.openfoam.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1249 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/forceCoeffs
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1249 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/fvSchemes
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1676 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/fvSolution
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      832 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/meshQualityDict
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9386 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/snappyHexMeshDict_template.openfoam.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1680 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/streamLines
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1003 2023-07-18 10:25:52.000000 inductiva-0.2.0/inductiva/templates/wind_tunnel/openfoam/files/system/surfaceFeaturesDict
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.338693 inductiva-0.2.0/inductiva/utils/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-07-21 09:12:23.000000 inductiva-0.2.0/inductiva/utils/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10504 2023-08-03 16:02:23.000000 inductiva-0.2.0/inductiva/utils/data.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2446 2023-07-24 10:52:30.000000 inductiva-0.2.0/inductiva/utils/files.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/utils/files_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/utils/flags.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/utils/meta.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      653 2023-08-03 16:02:23.000000 inductiva-0.2.0/inductiva/utils/misc.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-07-18 09:32:07.000000 inductiva-0.2.0/inductiva/utils/misc_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1097 2023-08-03 16:02:23.000000 inductiva-0.2.0/inductiva/utils/output_contents.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2036 2023-07-24 10:52:30.000000 inductiva-0.2.0/inductiva/utils/templates.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    19179 2023-08-02 15:22:37.000000 inductiva-0.2.0/inductiva/utils/visualization.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-08-03 16:10:00.310693 inductiva-0.2.0/inductiva.egg-info/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11551 2023-08-03 16:10:00.000000 inductiva-0.2.0/inductiva.egg-info/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14110 2023-08-03 16:10:00.000000 inductiva-0.2.0/inductiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-08-03 16:10:00.000000 inductiva-0.2.0/inductiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      235 2023-08-03 16:10:00.000000 inductiva-0.2.0/inductiva.egg-info/requires.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-08-03 16:10:00.000000 inductiva-0.2.0/inductiva.egg-info/top_level.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-07-18 09:32:07.000000 inductiva-0.2.0/pyproject.toml
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      877 2023-08-03 16:10:00.338693 inductiva-0.2.0/setup.cfg
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-07-18 09:32:07.000000 inductiva-0.2.0/setup.py
```

### Comparing `inductiva-0.0.9/inductiva/api/methods.py` & `inductiva-0.2.0/inductiva/api/methods.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,54 @@
 """Methods that interact with the lower-level inductiva-web-api-client.
 
 The relevant function for usage outside of this file is invoke_api().
 Check the demos directory for examples on how it is used.
 """
-import asyncio
-import json
 import os
 import pathlib
 import signal
 import time
 from contextlib import contextmanager
-from typing import Any, Dict, Optional, Type
-from urllib.parse import urlparse
+from typing import Any, Dict, List, Optional, Tuple, Type
+from uuid import UUID
 
-import websockets
 from absl import logging
 
 import inductiva
 from inductiva.client import ApiClient, ApiException, Configuration
 from inductiva.client.apis.tags.tasks_api import TasksApi
 from inductiva.client.models import (BodyUploadTaskInput, TaskRequest,
                                      TaskStatus)
 from inductiva.exceptions import RemoteExecutionError
 from inductiva.types import Path
 from inductiva.utils.data import (extract_output, get_validate_request_params,
                                   pack_input, unpack_output)
 from inductiva.utils.meta import get_method_name, get_type_annotations
+from inductiva import utils
+
+
+def validate_api_key(api_key: Optional[str]) -> Configuration:
+    """Validates the API key and returns API configuration"""
+    if inductiva.api_key is None:
+        raise ValueError(
+            "No API Key specified. "
+            "Set it in the code with \"inductiva.api_key = <YOUR_SECRET_KEY>\""
+            " or set the INDUCTIVA_API_KEY environment variable.")
+
+    api_config = Configuration(host=inductiva.api_url)
+    api_config.api_key["APIKeyHeader"] = api_key
+
+    return api_config
+
+
+def get_client() -> ApiClient:
+    """Returns an ApiClient instance."""
+    api_config = validate_api_key(inductiva.api_key)
+
+    return ApiClient(api_config)
 
 
 def submit_request(api_instance: TasksApi, request: TaskRequest) -> TaskStatus:
     """Submits a task request to the API.
 
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
@@ -48,62 +67,81 @@
 
     return api_response.body
 
 
 def upload_input(api_instance: TasksApi, task_id, original_params,
                  type_annotations):
     """Uploads the inputs of a given task to the API.
+
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
         task_id: ID of the task.
         original_params: Params of the request passed by the user.
         type_annotations: Annotations of the params' types.
     """
+    logging.info("Creating input archive...")
     input_zip_path = pack_input(
         params=original_params,
         type_annotations=type_annotations,
         zip_name=task_id,
     )
+    file_size = os.path.getsize(input_zip_path)
+    logging.info("Input archive created.")
+    logging.info("Input archive size: %s", utils.format_bytes(file_size))
 
-    logging.debug("Uploading input zip ...")
+    logging.info("Uploading input...")
     try:
         with open(input_zip_path, "rb") as zip_fp:
             _ = api_instance.upload_task_input(
                 path_params={"task_id": task_id},
                 body=BodyUploadTaskInput(file=zip_fp),
             )
     except ApiException as e:
         logging.exception(
             "Exception when calling TasksApi->upload_task_inputs: %s", e)
         raise e
 
+    logging.info("Input archive uploaded.")
+
     os.remove(input_zip_path)
 
 
-def download_output(api_instance: TasksApi, task_id):
+def download_output(
+        api_instance: TasksApi,
+        task_id,
+        output_dir: Optional[Path] = None) -> Tuple[List, pathlib.Path]:
     """Downloads the output of a given task from the API.
 
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
         task_id: ID of the task.
 
     Return:
-        Returns the path to the downloaded ZIP file.
+        Downloads and extracts the data to the client.
     """
+    logging.info("Downloading output...")
     try:
         api_response = api_instance.download_task_output(
             path_params={"task_id": task_id},
             stream=True,
         )
+        logging.info("Output downloaded.")
     except ApiException as e:
         raise e
 
     logging.debug("Downloaded output to %s", api_response.body.name)
 
-    return api_response.body.name
+    if output_dir is None:
+        output_dir = os.path.join(inductiva.output_dir, task_id)
+
+    logging.info("Extracting output ZIP file to \"%s\"...", output_dir)
+    result_list = extract_output(api_response.body.name, output_dir)
+    logging.info("Output extracted.")
+
+    return result_list, pathlib.Path(output_dir)
 
 
 def block_until_finish(api_instance: TasksApi, task_id: str) -> str:
     """Block until a task executing remotely finishes execution.
 
     Args:
         api_instance: Instance of TasksApi used to send necessary requests.
@@ -127,14 +165,25 @@
         task_id: ID of the task to kill.
    """
     logging.debug("Sending kill task request ...")
     api_instance.kill_task(path_params={"task_id": task_id},)
     logging.info("Task terminated.")
 
 
+def get_task_status(api_instance: TasksApi, task_id: str) -> TaskStatus:
+    """Check the status of a task."""
+
+    api_response = api_instance.get_task_status(
+        path_params={"task_id": task_id})
+
+    status = api_response.body["status"]
+
+    return status
+
+
 def block_until_status_is(api_instance: TasksApi,
                           task_id,
                           desired_status,
                           sleep_secs=0.5):
     """Block until the status of a task becomes the desired status.
 
     Args:
@@ -146,20 +195,15 @@
     Returns:
         Returns info related to the task, containing two fields,
     """
     prev_status = None
 
     while True:
         try:
-            api_response = \
-                api_instance.get_task_status(
-                    path_params={"task_id": task_id},
-                )
-
-            status = api_response.body["status"]
+            status = get_task_status(api_instance, task_id)
             logging.debug("Task status is %s", status)
         except ApiException as e:
             raise e
 
         if status != prev_status:
             if status == "submitted":
                 logging.info("Waiting for resources...")
@@ -168,15 +212,15 @@
 
         # If status reaches the desired status, then stop polling
         if status in desired_status:
             break
 
         time.sleep(sleep_secs)
 
-    return api_response.body["status"]
+    return status
 
 
 @contextmanager
 def blocking_task_context(api_instance: TasksApi, task_id):
     """Context to handle execution of a blocking task.
 
     The context handles exceptions and the SIGINT signal, issuing a request
@@ -208,35 +252,61 @@
         signal.signal(signal.SIGINT, original_sig)
 
 
 def invoke_api_from_fn_ptr(
     params,
     function_ptr,
     output_dir: Optional[Path] = None,
-    track_logs: bool = False,
+    resource_pool_id: Optional[UUID] = None,
 ):
     """Perform a task remotely defined by a function pointer."""
     type_annotations = get_type_annotations(function_ptr)
     method_name = get_method_name(function_ptr)
     return invoke_api(
         method_name,
         params,
         output_dir=output_dir,
         type_annotations=type_annotations,
         return_type=type_annotations["return"],
-        log_remote_execution=track_logs,
+        resource_pool_id=resource_pool_id,
+    )
+
+
+def submit_task(api_instance, task_request, params, type_annotations):
+    """Submit a task and send input files to the API."""
+
+    task = submit_request(
+        api_instance=api_instance,
+        request=task_request,
     )
 
+    task_id = task["id"]
+    logging.info("Task ID: %s", task_id)
+
+    with blocking_task_context(api_instance, task_id):
+        if task["status"] == "pending-input":
+
+            upload_input(
+                api_instance=api_instance,
+                original_params=params,
+                task_id=task_id,
+                type_annotations=type_annotations,
+            )
+
+            logging.info("Task request submitted.")
+
+    return task_id
+
 
 def invoke_api(method_name: str,
                params,
                type_annotations: Dict[Any, Type],
                output_dir: Optional[Path] = None,
                return_type: Type = pathlib.Path,
-               log_remote_execution: bool = False):
+               resource_pool_id: Optional[UUID] = None):
     """Perform a task remotely via Inductiva's Web API.
 
     Currently, the implementation handles the whole flow of the task execution,
     and blocks until the task finishes execution.
     The flow is summarized as follows:
         1. Transform request params into the params used to
         validate permission to execute the request.
@@ -258,142 +328,108 @@
         input_dir: Directory containing the input files to be uploaded.
         output_dir: Directory where to place the output files.
         return_type: Type of the return value of the task, for unpacking.
 
     Return:
         Returns the output of the task.
     """
-    if inductiva.api_key is None:
-        raise ValueError(
-            "No API Key specified. "
-            "Set it in the code with \"inductiva.api_key = <YOUR_SECRET_KEY>\""
-            " or set the INDUCTIVA_API_KEY environment variable.")
-
-    api_config = Configuration(host=inductiva.api_url)
-    api_config.api_key["APIKeyHeader"] = inductiva.api_key
+    api_config = validate_api_key(inductiva.api_key)
 
     request_params = get_validate_request_params(
         original_params=params,
         type_annotations=type_annotations,
     )
 
     task_request = TaskRequest(
         method=method_name,
         params=request_params,
+        resource_pool=resource_pool_id,
     )
 
     with ApiClient(api_config) as client:
         api_instance = TasksApi(client)
 
-        task = submit_request(
+        task_id = submit_task(api_instance, task_request, params,
+                              type_annotations)
+
+        block_until_status_is(
             api_instance=api_instance,
-            request=task_request,
+            task_id=task_id,
+            desired_status={"started"},
         )
-
-        task_id = task["id"]
+        logging.info("An executer has picked up the request")
+        logging.info("The requested task is being executed remotely")
 
         # While the task is executing, use a context manager that kills the
         # task if some exception or SIGINT is caught.
         with blocking_task_context(api_instance, task_id):
-            if task["status"] == "pending-input":
-                upload_input(
-                    api_instance=api_instance,
-                    original_params=params,
-                    task_id=task_id,
-                    type_annotations=type_annotations,
-                )
-
-            logging.info("Request submitted.")
-
-            block_until_status_is(
+            status = block_until_finish(
                 api_instance=api_instance,
                 task_id=task_id,
-                desired_status={"started"},
             )
-            logging.info("An executer has picked up the request.")
-            logging.info("The requested task is being executed remotely...")
-
-            if log_remote_execution:
-                status = asyncio.run(follow_task(task_id))
-            else:
-                status = block_until_finish(
-                    api_instance=api_instance,
-                    task_id=task_id,
-                )
 
             if status == "success":
                 logging.info("Task executed successfuly.")
             else:
                 logging.info("Task failed.")
 
-        logging.info("Downloading output...")
-        output_zip_path = download_output(
-            api_instance=api_instance,
-            task_id=task_id,
-        )
-        logging.info("Output downloaded.")
+        result_list = download_output(api_instance, task_id, output_dir)
 
-    if output_dir is None:
-        output_dir = os.path.join(inductiva.output_dir, task_id)
-
-    logging.info("Extracting output ZIP file to \"%s\"...", output_dir)
-    result_list = extract_output(output_zip_path, output_dir)
-    logging.info("Output extracted.")
-
-    if status == "failed":
-        raise RemoteExecutionError(f"""Remote execution failed.
-    Find more details in: \"{os.path.abspath(output_dir)}\".""")
+        if status == "failed":
+            raise RemoteExecutionError(f"""Remote execution failed.
+        Find more details in: \"{os.path.abspath(output_dir)}\".""")
 
     return unpack_output(result_list, output_dir, return_type)
 
 
-def run_simulation(
-    api_method_name: str,
-    input_dir: pathlib.Path,
-    output_dir: pathlib.Path,
-    params: Dict[str, Any],
-    log_remote_execution: bool = False,
-) -> pathlib.Path:
-
-    params = {
-        "sim_dir": input_dir,
-        **params,
-    }
-    type_annotations = {
-        "sim_dir": pathlib.Path,
-    }
+def invoke_async_api(method_name: str,
+                     params,
+                     type_annotations: Dict[Any, Type],
+                     resource_pool_id: Optional[UUID] = None) -> str:
+    """Perform a task asyc and remotely via Inductiva's Web API.
+
+    Submits a simulation async to the API and returns the task id.
+    The flow is similar to invoke_api, but it does not block until the task
+    is finished.
+    The flow is summarized as follows:
+        1. Transform request params into the params used to
+        validate permission to execute the request.
+        2. Submit task via the "POST task/submit" endpoint.
+            Note: HTTP status code 400 informs the requested method is invalid,
+                and HTTP status code 403 informs that the user is not authorized
+                to post such request.
+        3. If the status returned by the previous HTTP request is
+            "pending-input", ZIP inputs and send them via
+            "POST task/{task_id}/input".
+        4. Return task_id and leaves the simulation on the queue until resources
+            become available.
 
-    result = invoke_api(
-        api_method_name,
-        params,
-        type_annotations,
-        output_dir=output_dir,
-        return_type=pathlib.Path,
-        log_remote_execution=log_remote_execution,
-    )
+    Args:
+        request: Request sent to the API for validation.
+        input_dir: Directory containing the input files to be uploaded.
 
-    if not isinstance(result, pathlib.Path):
-        raise RuntimeError(f"Expected result to be a Path, got {type(result)}")
+    Return:
+        Returns the task id.
+    """
 
-    return result
+    api_config = validate_api_key(inductiva.api_key)
 
+    request_params = get_validate_request_params(
+        original_params=params,
+        type_annotations=type_annotations,
+    )
 
-async def follow_task(task_id: str) -> str:
-    parsed_url = urlparse(inductiva.api_url)
-    url = \
-        f"ws://{parsed_url.hostname}:{parsed_url.port}/" \
-        f"task/{task_id}/logs/tail"
+    task_request = TaskRequest(
+        method=method_name,
+        params=request_params,
+        resource_pool=resource_pool_id,
+    )
 
-    logging.debug("Following task logs at %s", url)
-    async with websockets.connect(url) as ws:
-        while True:
-            message = await ws.recv()
-            parsed_message = json.loads(message)
+    with ApiClient(api_config) as client:
+        api_instance = TasksApi(client)
 
-            if parsed_message["type"] == "update":
-                status = parsed_message["content"]
-                logging.debug("Task status update: %s", status)
+        task_id = submit_task(api_instance=api_instance,
+                              task_request=task_request,
+                              params=params,
+                              type_annotations=type_annotations)
 
-                return status
-            else:
-                new_line = parsed_message["content"]
-                print(new_line, end="")
+    return task_id
```

### Comparing `inductiva-0.0.9/inductiva/client/__init__.py` & `inductiva-0.2.0/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/client/api_client.py` & `inductiva-0.2.0/inductiva/client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,15 +846,15 @@
     @classmethod
     def __file_name_from_content_disposition(
             cls,
             content_disposition: typing.Optional[str]) -> typing.Optional[str]:
         if content_disposition is None:
             return None
         match = cls.__filename_content_disposition_pattern.search(
-            content_disposition)
+                content_disposition)
         if not match:
             return None
         return match.group(1)
 
     def __deserialize_application_octet_stream(
         self, response: urllib3.HTTPResponse
     ) -> typing.Union[bytes, io.BufferedReader]:
@@ -890,16 +890,16 @@
 
     @staticmethod
     def __deserialize_multipart_form_data(
             response: urllib3.HTTPResponse) -> typing.Dict[str, typing.Any]:
         msg = email.message_from_bytes(response.data)
         return {
             part.get_param("name", header="Content-Disposition"):
-            part.get_payload(decode=True).decode(part.get_content_charset())
-            if part.get_content_charset() else part.get_payload()
+                part.get_payload(decode=True).decode(part.get_content_charset())
+                if part.get_content_charset() else part.get_payload()
             for part in msg.get_payload()
         }
 
     def deserialize(self, response: urllib3.HTTPResponse,
                     configuration: Configuration) -> ApiResponse:
         content_type = response.getheader('content-type')
         deserialized_body = unset
```

### Comparing `inductiva-0.0.9/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.2.0/inductiva/client/apis/tags/admin_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
-from inductiva.client.paths.task_task_id_output.get import DownloadTaskOutput
-from inductiva.client.paths.task_task_id_status.get import GetTaskStatus
-from inductiva.client.paths.task_task_id_kill.post import KillTask
-from inductiva.client.paths.task_submit.post import SubmitTask
-from inductiva.client.paths.task_task_id_input.post import UploadTaskInput
+from inductiva.client.paths.admin_users.post import AddUser
+from inductiva.client.paths.admin_tasks.get import GetTasks
+from inductiva.client.paths.admin_users_username_tasks.get import GetTasksByUsername
+from inductiva.client.paths.admin_users_username.get import GetUser
 
 
-class TasksApi(
-        DownloadTaskOutput,
-        GetTaskStatus,
-        KillTask,
-        SubmitTask,
-        UploadTaskInput,
+class AdminApi(
+        AddUser,
+        GetTasks,
+        GetTasksByUsername,
+        GetUser,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `inductiva-0.0.9/inductiva/client/configuration.py` & `inductiva-0.2.0/inductiva/client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,18 @@
         """
         self.key_file = None
         """client key file
         """
         self.assert_hostname = None
         """Set this to True/False to enable/disable SSL hostname verification.
         """
+        self.tls_server_name = None
+        """SSL/TLS Server Name Indication (SNI)
+           Set this to the SNI value expected by the server.
+        """
 
         self.connection_pool_maxsize = multiprocessing.cpu_count() * 5
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
```

### Comparing `inductiva-0.0.9/inductiva/client/exceptions.py` & `inductiva-0.2.0/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.2.0/inductiva/client/model/resource_pool_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,77 +18,86 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class BodyUploadTaskInput(schemas.DictSchema):
+class ResourcePoolID(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
-            "file",
+            "id",
         }
 
         class properties:
-            file = schemas.BinarySchema
+            id = schemas.UUIDSchema
             __annotations__ = {
-                "file": file,
+                "id": id,
             }
 
-    file: MetaOapg.properties.file
+    id: MetaOapg.properties.id
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["file"]
-    ) -> MetaOapg.properties.file:
+            self,
+            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["file",],
-                                             str]):
+    def __getitem__(self,
+                    name: typing.Union[typing_extensions.Literal[
+                        "id",
+                    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-            self, name: typing_extensions.Literal["file"]
-    ) -> MetaOapg.properties.file:
+            self,
+            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["file",],
-                                         str]):
+                      name: typing.Union[typing_extensions.Literal[
+                          "id",
+                      ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        file: typing.Union[MetaOapg.properties.file, bytes, io.FileIO,
-                           io.BufferedReader,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        id: typing.Union[
+            MetaOapg.properties.id,
+            str,
+            uuid.UUID,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'BodyUploadTaskInput':
+    ) -> 'ResourcePoolID':
         return super().__new__(
             cls,
             *_args,
-            file=file,
+            id=id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.0.9/inductiva/client/model/http_validation_error.py` & `inductiva-0.2.0/inductiva/client/model/http_validation_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,17 @@
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal["detail",],
-                                       str]):
+                    name: typing.Union[typing_extensions.Literal[
+                        "detail",
+                    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["detail"]
     ) -> typing.Union[MetaOapg.properties.detail, schemas.Unset]:
@@ -86,21 +87,25 @@
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["detail",],
-                                         str]):
+                      name: typing.Union[typing_extensions.Literal[
+                          "detail",
+                      ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
         detail: typing.Union[MetaOapg.properties.detail, list, tuple,
                              schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
```

### Comparing `inductiva-0.0.9/inductiva/client/model/new_user.py` & `inductiva-0.2.0/inductiva/client/model/new_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,19 +73,19 @@
     ) -> MetaOapg.properties.is_admin:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
-    def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal["username",
-                                                                 "api_key",
-                                                                 "is_admin",],
-                                       str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
+        "username",
+        "api_key",
+        "is_admin",
+    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["username"]
     ) -> MetaOapg.properties.username:
@@ -105,26 +105,35 @@
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
-    def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["username",
-                                                                   "api_key",
-                                                                   "is_admin",],
-                                         str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
+        "username",
+        "api_key",
+        "is_admin",
+    ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        api_key: typing.Union[MetaOapg.properties.api_key, str,],
-        username: typing.Union[MetaOapg.properties.username, str,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        api_key: typing.Union[
+            MetaOapg.properties.api_key,
+            str,
+        ],
+        username: typing.Union[
+            MetaOapg.properties.username,
+            str,
+        ],
         is_admin: typing.Union[MetaOapg.properties.is_admin, bool,
                                schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
```

### Comparing `inductiva-0.0.9/inductiva/client/model/queue_status.py` & `inductiva-0.2.0/inductiva/client/model/queue_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,19 +75,19 @@
     ) -> MetaOapg.properties.tasks_ahead:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
-    def __getitem__(
-        self, name: typing.Union[typing_extensions.Literal["num_executers",
-                                                           "running_tasks",
-                                                           "tasks_ahead",],
-                                 str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
+        "num_executers",
+        "running_tasks",
+        "tasks_ahead",
+    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["num_executers"]
     ) -> MetaOapg.properties.num_executers:
@@ -107,30 +107,42 @@
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
-    def get_item_oapg(
-        self, name: typing.Union[typing_extensions.Literal["num_executers",
-                                                           "running_tasks",
-                                                           "tasks_ahead",],
-                                 str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
+        "num_executers",
+        "running_tasks",
+        "tasks_ahead",
+    ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        running_tasks: typing.Union[MetaOapg.properties.running_tasks,
-                                    decimal.Decimal, int,],
-        tasks_ahead: typing.Union[MetaOapg.properties.tasks_ahead,
-                                  decimal.Decimal, int,],
-        num_executers: typing.Union[MetaOapg.properties.num_executers,
-                                    decimal.Decimal, int,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        running_tasks: typing.Union[
+            MetaOapg.properties.running_tasks,
+            decimal.Decimal,
+            int,
+        ],
+        tasks_ahead: typing.Union[
+            MetaOapg.properties.tasks_ahead,
+            decimal.Decimal,
+            int,
+        ],
+        num_executers: typing.Union[
+            MetaOapg.properties.num_executers,
+            decimal.Decimal,
+            int,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'QueueStatus':
         return super().__new__(
```

### Comparing `inductiva-0.0.9/inductiva/client/model/task_request.py` & `inductiva-0.2.0/inductiva/client/model/inductiva_host_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,104 +18,98 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class TaskRequest(schemas.DictSchema):
+class InductivaHostInfo(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
-    Dataclass that represents a task request.
-
-Attributes:
-    method: Name of the requested method, e.g. "math.matmul".
-    params: Dictionary containing the parameters request.
+    Info about the Inductiva server hosting the executer.
     """
 
     class MetaOapg:
         required = {
-            "method",
-            "params",
+            "host_type",
         }
 
         class properties:
-            method = schemas.StrSchema
-            params = schemas.DictSchema
+
+            class host_type(schemas.EnumBase, schemas.StrSchema):
+
+                class MetaOapg:
+                    enum_value_to_name = {
+                        "inductiva-hardware": "INDUCTIVAHARDWARE",
+                    }
+
+                @schemas.classproperty
+                def INDUCTIVAHARDWARE(cls):
+                    return cls("inductiva-hardware")
+
             __annotations__ = {
-                "method": method,
-                "params": params,
+                "host_type": host_type,
             }
 
-    method: MetaOapg.properties.method
-    params: MetaOapg.properties.params
-
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["method"]
-    ) -> MetaOapg.properties.method:
-        ...
+    host_type: MetaOapg.properties.host_type
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["params"]
-    ) -> MetaOapg.properties.params:
+        self, name: typing_extensions.Literal["host_type"]
+    ) -> MetaOapg.properties.host_type:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal["method",
-                                                                 "params",],
-                                       str]):
+                    name: typing.Union[typing_extensions.Literal[
+                        "host_type",
+                    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["method"]
-    ) -> MetaOapg.properties.method:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["params"]
-    ) -> MetaOapg.properties.params:
+        self, name: typing_extensions.Literal["host_type"]
+    ) -> MetaOapg.properties.host_type:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["method",
-                                                                   "params",],
-                                         str]):
+                      name: typing.Union[typing_extensions.Literal[
+                          "host_type",
+                      ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        method: typing.Union[MetaOapg.properties.method, str,],
-        params: typing.Union[MetaOapg.properties.params, dict,
-                             frozendict.frozendict,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        host_type: typing.Union[
+            MetaOapg.properties.host_type,
+            str,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'TaskRequest':
+    ) -> 'InductivaHostInfo':
         return super().__new__(
             cls,
             *_args,
-            method=method,
-            params=params,
+            host_type=host_type,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.0.9/inductiva/client/model/task_status.py` & `inductiva-0.2.0/inductiva/client/model/task_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,170 +18,188 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class TaskStatus(schemas.DictSchema):
+class TaskRequest(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-
-    Dataclass that represents the status of a task.
-
-Attributes:
-    id: Unique ID of the task.
-    status: String representing the status of the task.
     """
 
     class MetaOapg:
         required = {
-            "id",
-            "status",
+            "method",
+            "params",
         }
 
         class properties:
-            id = schemas.StrSchema
-            status = schemas.StrSchema
+            method = schemas.StrSchema
+            params = schemas.DictSchema
 
-            class queue(
+            class resource_pool(
                     schemas.ComposedSchema,):
 
                 class MetaOapg:
+                    format = 'uuid4'
+                    any_of_0 = schemas.StrSchema
                     any_of_1 = schemas.NoneSchema
 
                     @classmethod
                     @functools.lru_cache()
                     def any_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            QueueStatus,
+                            cls.any_of_0,
                             cls.any_of_1,
                         ]
 
                 def __new__(
                     cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, str, date,
-                                         datetime, uuid.UUID, int, float,
-                                         decimal.Decimal, bool, None, list,
-                                         tuple, bytes, io.FileIO,
-                                         io.BufferedReader,],
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
                     _configuration: typing.Optional[
                         schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                            frozendict.frozendict, str, date,
                                            datetime, uuid.UUID, int, float,
                                            decimal.Decimal, None, list, tuple,
                                            bytes],
-                ) -> 'queue':
+                ) -> 'resource_pool':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
             __annotations__ = {
-                "id": id,
-                "status": status,
-                "queue": queue,
+                "method": method,
+                "params": params,
+                "resource_pool": resource_pool,
             }
 
-    id: MetaOapg.properties.id
-    status: MetaOapg.properties.status
+    method: MetaOapg.properties.method
+    params: MetaOapg.properties.params
 
     @typing.overload
     def __getitem__(
-            self,
-            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
+        self, name: typing_extensions.Literal["method"]
+    ) -> MetaOapg.properties.method:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["status"]
-    ) -> MetaOapg.properties.status:
+        self, name: typing_extensions.Literal["params"]
+    ) -> MetaOapg.properties.params:
         ...
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["queue"]
-    ) -> MetaOapg.properties.queue:
+        self, name: typing_extensions.Literal["resource_pool"]
+    ) -> MetaOapg.properties.resource_pool:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
-    def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal["id", "status",
-                                                                 "queue",],
-                                       str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
+        "method",
+        "params",
+        "resource_pool",
+    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-            self,
-            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
+        self, name: typing_extensions.Literal["method"]
+    ) -> MetaOapg.properties.method:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["status"]
-    ) -> MetaOapg.properties.status:
+        self, name: typing_extensions.Literal["params"]
+    ) -> MetaOapg.properties.params:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["queue"]
-    ) -> typing.Union[MetaOapg.properties.queue, schemas.Unset]:
+        self, name: typing_extensions.Literal["resource_pool"]
+    ) -> typing.Union[MetaOapg.properties.resource_pool, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
-    def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["id",
-                                                                   "status",
-                                                                   "queue",],
-                                         str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
+        "method",
+        "params",
+        "resource_pool",
+    ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        id: typing.Union[MetaOapg.properties.id, str,],
-        status: typing.Union[MetaOapg.properties.status, str,],
-        queue: typing.Union[MetaOapg.properties.queue, dict,
-                            frozendict.frozendict, str, date, datetime,
-                            uuid.UUID, int, float, decimal.Decimal, bool, None,
-                            list, tuple, bytes, io.FileIO, io.BufferedReader,
-                            schemas.Unset] = schemas.unset,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        method: typing.Union[
+            MetaOapg.properties.method,
+            str,
+        ],
+        params: typing.Union[
+            MetaOapg.properties.params,
+            dict,
+            frozendict.frozendict,
+        ],
+        resource_pool: typing.Union[MetaOapg.properties.resource_pool, dict,
+                                    frozendict.frozendict, str, date, datetime,
+                                    uuid.UUID, int, float, decimal.Decimal,
+                                    bool, None, list, tuple, bytes, io.FileIO,
+                                    io.BufferedReader,
+                                    schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'TaskStatus':
+    ) -> 'TaskRequest':
         return super().__new__(
             cls,
             *_args,
-            id=id,
-            status=status,
-            queue=queue,
+            method=method,
+            params=params,
+            resource_pool=resource_pool,
             _configuration=_configuration,
             **kwargs,
         )
-
-
-from inductiva.client.model.queue_status import QueueStatus
```

### Comparing `inductiva-0.0.9/inductiva/client/model/validation_error.py` & `inductiva-0.2.0/inductiva/client/model/validation_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,19 +62,32 @@
                                 return [
                                     cls.any_of_0,
                                     cls.any_of_1,
                                 ]
 
                         def __new__(
                             cls,
-                            *_args: typing.Union[dict, frozendict.frozendict,
-                                                 str, date, datetime, uuid.UUID,
-                                                 int, float, decimal.Decimal,
-                                                 bool, None, list, tuple, bytes,
-                                                 io.FileIO, io.BufferedReader,],
+                            *_args: typing.Union[
+                                dict,
+                                frozendict.frozendict,
+                                str,
+                                date,
+                                datetime,
+                                uuid.UUID,
+                                int,
+                                float,
+                                decimal.Decimal,
+                                bool,
+                                None,
+                                list,
+                                tuple,
+                                bytes,
+                                io.FileIO,
+                                io.BufferedReader,
+                            ],
                             _configuration: typing.Optional[
                                 schemas.Configuration] = None,
                             **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                                    frozendict.frozendict, str,
                                                    date, datetime, uuid.UUID,
                                                    int, float, decimal.Decimal,
                                                    None, list, tuple, bytes],
@@ -84,29 +97,51 @@
                                 *_args,
                                 _configuration=_configuration,
                                 **kwargs,
                             )
 
                 def __new__(
                     cls,
-                    _arg: typing.Union[
-                        typing.Tuple[typing.Union[MetaOapg.items, dict,
-                                                  frozendict.frozendict, str,
-                                                  date, datetime, uuid.UUID,
-                                                  int, float, decimal.Decimal,
-                                                  bool, None, list, tuple,
-                                                  bytes, io.FileIO,
-                                                  io.BufferedReader,]],
-                        typing.List[typing.Union[MetaOapg.items, dict,
-                                                 frozendict.frozendict, str,
-                                                 date, datetime, uuid.UUID, int,
-                                                 float, decimal.Decimal, bool,
-                                                 None, list, tuple, bytes,
-                                                 io.FileIO,
-                                                 io.BufferedReader,]]],
+                    _arg: typing.Union[typing.Tuple[typing.Union[
+                        MetaOapg.items,
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ]], typing.List[typing.Union[
+                        MetaOapg.items,
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ]]],
                     _configuration: typing.Optional[
                         schemas.Configuration] = None,
                 ) -> 'loc':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
@@ -145,18 +180,19 @@
     ) -> MetaOapg.properties.type:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
-    def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal["loc", "msg",
-                                                                 "type",],
-                                       str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
+        "loc",
+        "msg",
+        "type",
+    ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
             self,
             name: typing_extensions.Literal["loc"]) -> MetaOapg.properties.loc:
@@ -176,26 +212,40 @@
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
-    def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal["loc", "msg",
-                                                                   "type",],
-                                         str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
+        "loc",
+        "msg",
+        "type",
+    ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict,],
-        msg: typing.Union[MetaOapg.properties.msg, str,],
-        loc: typing.Union[MetaOapg.properties.loc, list, tuple,],
-        type: typing.Union[MetaOapg.properties.type, str,],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        msg: typing.Union[
+            MetaOapg.properties.msg,
+            str,
+        ],
+        loc: typing.Union[
+            MetaOapg.properties.loc,
+            list,
+            tuple,
+        ],
+        type: typing.Union[
+            MetaOapg.properties.type,
+            str,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'ValidationError':
         return super().__new__(
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/admin_user/post.py` & `inductiva-0.2.0/inductiva/client/paths/admin_user/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 ]
 SchemaFor202ResponseBodyApplicationJson = schemas.AnyTypeSchema
 
 
 @dataclass
 class ApiResponseFor202(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor202ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor202ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_202 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor202,
     content={
         'application/json':
@@ -62,15 +64,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -86,63 +90,79 @@
 
 
 class BaseApi(api_client.Api):
 
     @typing.overload
     def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
     def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
@@ -205,63 +225,79 @@
 
 class AddUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
     def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
     def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._add_user_oapg(body=body,
@@ -274,63 +310,79 @@
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor202,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._add_user_oapg(body=body,
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/admin_user_username_tasks/get.py` & `inductiva-0.2.0/inductiva/client/paths/admin_user_username_tasks/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 
 from . import path
 
 # Path params
 UsernameSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams', {
-        'username': typing.Union[UsernameSchema, str,],
+        'username': typing.Union[
+            UsernameSchema,
+            str,
+        ],
     })
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams', {}, total=False)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
@@ -53,15 +56,17 @@
 ]
 SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor200ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json':
@@ -71,15 +76,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -100,15 +107,17 @@
     def _get_user_tasks_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _get_user_tasks_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -122,16 +131,18 @@
     def _get_user_tasks_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _get_user_tasks_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -201,15 +212,17 @@
     def get_user_tasks(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def get_user_tasks(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -223,16 +236,18 @@
     def get_user_tasks(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def get_user_tasks(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -254,15 +269,17 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -276,16 +293,18 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/task_submit/post.py` & `inductiva-0.2.0/inductiva/client/paths/admin_users/post.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,138 +20,158 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.task_request import TaskRequest
-from inductiva.client.model.task_status import TaskStatus
+from inductiva.client.model.user import User
 from inductiva.client.model.http_validation_error import HTTPValidationError
+from inductiva.client.model.user_create import UserCreate
 
 from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = TaskRequest
+SchemaForRequestBodyApplicationJson = UserCreate
 
-request_body_task_request = api_client.RequestBody(
+request_body_user_create = api_client.RequestBody(
     content={
         'application/json':
             api_client.MediaType(schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor202ResponseBodyApplicationJson = TaskStatus
+SchemaFor201ResponseBodyApplicationJson = User
 
 
 @dataclass
-class ApiResponseFor202(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor202ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor201ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_202 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor202,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json':
-            api_client.MediaType(schema=SchemaFor202ResponseBodyApplicationJson
+            api_client.MediaType(schema=SchemaFor201ResponseBodyApplicationJson
                                 ),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
             api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
                                 ),
     },
 )
 _status_code_to_response = {
-    '202': _response_for_202,
+    '201': _response_for_201,
     '422': _response_for_422,
 }
 _all_accept_content_types = ('application/json',)
 
 
 class BaseApi(api_client.Api):
 
     @typing.overload
-    def _submit_task_oapg(
+    def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
-    def _submit_task_oapg(
+    def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
-    def _submit_task_oapg(
+    def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
-    def _submit_task_oapg(
+    def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
-    def _submit_task_oapg(
+    def _add_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Submit Task
+        Add User
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
 
         _headers = HTTPHeaderDict()
@@ -162,16 +182,15 @@
 
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead'
             )
         _fields = None
         _body = None
-        serialized_data = request_body_task_request.serialize(
-            body, content_type)
+        serialized_data = request_body_user_create.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -201,143 +220,175 @@
             raise exceptions.ApiException(status=response.status,
                                           reason=response.reason,
                                           api_response=api_response)
 
         return api_response
 
 
-class SubmitTask(BaseApi):
+class AddUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def submit_task(
+    def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
-    def submit_task(
+    def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
-    def submit_task(
+    def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
-    def submit_task(
+    def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
-    def submit_task(
+    def add_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._submit_task_oapg(body=body,
-                                      content_type=content_type,
-                                      accept_content_types=accept_content_types,
-                                      stream=stream,
-                                      timeout=timeout,
-                                      skip_deserialization=skip_deserialization)
+        return self._add_user_oapg(body=body,
+                                   content_type=content_type,
+                                   accept_content_types=accept_content_types,
+                                   stream=stream,
+                                   timeout=timeout,
+                                   skip_deserialization=skip_deserialization)
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor202,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization:
         ...
 
     @typing.overload
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor202,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor201,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._submit_task_oapg(body=body,
-                                      content_type=content_type,
-                                      accept_content_types=accept_content_types,
-                                      stream=stream,
-                                      timeout=timeout,
-                                      skip_deserialization=skip_deserialization)
+        return self._add_user_oapg(body=body,
+                                   content_type=content_type,
+                                   accept_content_types=accept_content_types,
+                                   stream=stream,
+                                   timeout=timeout,
+                                   skip_deserialization=skip_deserialization)
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/task_task_id_input/post.py` & `inductiva-0.2.0/inductiva/client/paths/task_task_id_input/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 
 from . import path
 
 # Path params
 TaskIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams', {
-        'task_id': typing.Union[TaskIdSchema, str,],
+        'task_id': typing.Union[
+            TaskIdSchema,
+            str,
+        ],
     })
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams', {}, total=False)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
@@ -62,15 +65,17 @@
 ]
 SchemaFor200ResponseBodyApplicationJson = TaskStatus
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor200ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json':
@@ -80,15 +85,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -112,29 +119,33 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _upload_task_input_oapg(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _upload_task_input_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
@@ -154,16 +165,18 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _upload_task_input_oapg(
         self,
         content_type: str = 'multipart/form-data',
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
@@ -250,29 +263,33 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def upload_task_input(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def upload_task_input(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
@@ -292,16 +309,18 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def upload_task_input(
         self,
         content_type: str = 'multipart/form-data',
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
@@ -331,29 +350,33 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
@@ -373,16 +396,18 @@
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def post(
         self,
         content_type: str = 'multipart/form-data',
         body: typing.Union[SchemaForRequestBodyMultipartFormData,
                            schemas.Unset] = schemas.unset,
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/task_task_id_kill/post.py` & `inductiva-0.2.0/inductiva/client/paths/task_task_id_kill/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 from . import path
 
 # Path params
 TaskIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams', {
-        'task_id': typing.Union[TaskIdSchema, str,],
+        'task_id': typing.Union[
+            TaskIdSchema,
+            str,
+        ],
     })
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams', {}, total=False)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
@@ -54,15 +57,17 @@
 ]
 SchemaFor200ResponseBodyApplicationJson = TaskStatus
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor200ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json':
@@ -72,15 +77,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -101,15 +108,17 @@
     def _kill_task_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _kill_task_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -123,16 +132,18 @@
     def _kill_task_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _kill_task_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -202,15 +213,17 @@
     def kill_task(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def kill_task(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -224,16 +237,18 @@
     def kill_task(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def kill_task(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -254,15 +269,17 @@
     def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -276,16 +293,18 @@
     def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/task_task_id_output/get.py` & `inductiva-0.2.0/inductiva/client/paths/task_task_id_output/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 
 from . import path
 
 # Path params
 TaskIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams', {
-        'task_id': typing.Union[TaskIdSchema, str,],
+        'task_id': typing.Union[
+            TaskIdSchema,
+            str,
+        ],
     })
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams', {}, total=False)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
@@ -53,15 +56,17 @@
 ]
 SchemaFor200ResponseBodyApplicationOctetStream = schemas.BinarySchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor200ResponseBodyApplicationOctetStream,]
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationOctetStream,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/octet-stream':
@@ -71,15 +76,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -103,15 +110,17 @@
     def _download_task_output_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _download_task_output_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -125,16 +134,18 @@
     def _download_task_output_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _download_task_output_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -204,15 +215,17 @@
     def download_task_output(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def download_task_output(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -226,16 +239,18 @@
     def download_task_output(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def download_task_output(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -257,15 +272,17 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -279,16 +296,18 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
```

### Comparing `inductiva-0.0.9/inductiva/client/paths/task_task_id_status/get.py` & `inductiva-0.2.0/inductiva/client/paths/task_task_id_status/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 from . import path
 
 # Path params
 TaskIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams', {
-        'task_id': typing.Union[TaskIdSchema, str,],
+        'task_id': typing.Union[
+            TaskIdSchema,
+            str,
+        ],
     })
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams', {}, total=False)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
@@ -54,15 +57,17 @@
 ]
 SchemaFor200ResponseBodyApplicationJson = TaskStatus
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor200ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json':
@@ -72,15 +77,17 @@
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[SchemaFor422ResponseBodyApplicationJson,]
+    body: typing.Union[
+        SchemaFor422ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
         'application/json':
@@ -101,15 +108,17 @@
     def _get_task_status_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def _get_task_status_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -123,16 +132,18 @@
     def _get_task_status_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def _get_task_status_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -202,15 +213,17 @@
     def get_task_status(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def get_task_status(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -224,16 +237,18 @@
     def get_task_status(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def get_task_status(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
@@ -255,15 +270,17 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+    ]:
         ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
@@ -277,16 +294,18 @@
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200,
-                      api_client.ApiResponseWithoutDeserialization,]:
+    ) -> typing.Union[
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
         ...
 
     def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
```

### Comparing `inductiva-0.0.9/inductiva/client/rest.py` & `inductiva-0.2.0/inductiva/client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         if configuration.assert_hostname is not None:
             addition_pool_args[
                 'assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.tls_server_name:
+            addition_pool_args[
+                'server_hostname'] = configuration.tls_server_name
+
         if configuration.socket_options is not None:
             addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
```

### Comparing `inductiva-0.0.9/inductiva/client/schemas.py` & `inductiva-0.2.0/inductiva/client/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -2025,16 +2025,17 @@
         f"Invalid type. Required value type is str and passed type was {type(arg)} at {path_to_item}"
     )
     if isinstance(arg, str):
         return str(arg)
     elif isinstance(arg, (dict, frozendict.frozendict)):
         return frozendict.frozendict({
             key:
-            cast_to_allowed_types(val, from_server, validated_path_to_schemas,
-                                  path_to_item + (key,))
+                cast_to_allowed_types(val, from_server,
+                                      validated_path_to_schemas,
+                                      path_to_item + (key,))
             for key, val in arg.items()
         })
     elif isinstance(arg, (bool, BoolClass)):
         """
         this check must come before isinstance(arg, (int, float))
         because isinstance(True, int) is True
         """
```

### Comparing `inductiva-0.0.9/inductiva/core/math.py` & `inductiva-0.2.0/inductiva/core/math.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/fluid_types.py` & `inductiva-0.2.0/inductiva/fluids/fluid_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/post_processing/splishsplash.py` & `inductiva-0.2.0/inductiva/fluids/post_processing/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/dam_break/dam_break.py` & `inductiva-0.2.0/inductiva/fluids/scenarios/dam_break/dam_break.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Describes the physical scenarios and runs its simulation via API."""
 from typing import List, Literal, Optional
 from enum import Enum
 from dataclasses import dataclass
+from uuid import UUID
 
+from inductiva import tasks
 from inductiva.simulation import Simulator
 from inductiva.fluids.simulators import DualSPHysics
 from inductiva.fluids.scenarios.fluid_block import FluidBlock
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.fluid_types import WATER
-from inductiva.types import Path
 
 from inductiva.fluids.scenarios._post_processing import SPHSimulationOutput
 
 
 @dataclass
 class ParticleRadius(Enum):
     """Sets particle radius according to resolution."""
@@ -48,31 +49,35 @@
                          dimensions=dimensions,
                          position=position)
 
     # pylint: disable=arguments-renamed
     def simulate(
         self,
         simulator: Simulator = DualSPHysics(),
-        output_dir: Optional[Path] = None,
+        resource_pool_id: Optional[UUID] = None,
         device: Literal["cpu", "gpu"] = "gpu",
         resolution: Literal["high", "medium", "low"] = "medium",
         simulation_time: float = 1,
-    ):
+        run_async: bool = False,
+    ) -> tasks.Task:
         """Simulates the scenario.
 
         Args:
             simulator: Simulator to use.
-            output_dir: Directory to store the simulation output.
             device: Device in which to run the simulation.
             resolution: Resolution of the simulation.
             simulation_time: Simulation time, in seconds.
+            run_async: Whether to run the simulation asynchronously.
         """
 
         particle_radius = ParticleRadius[resolution.upper()].value
 
-        sim_output_path = super().simulate(simulator=simulator,
-                                           output_dir=output_dir,
-                                           device=device,
-                                           particle_radius=particle_radius,
-                                           simulation_time=simulation_time)
+        task = super().simulate(simulator=simulator,
+                                resource_pool_id=resource_pool_id,
+                                device=device,
+                                particle_radius=particle_radius,
+                                simulation_time=simulation_time,
+                                run_async=run_async)
+
+        task.set_output_class(SPHSimulationOutput)
 
-        return SPHSimulationOutput(sim_output_path.sim_output_dir)
+        return task
```

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block.py` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Describes the physical scenarios and runs its simulation via API."""
 
 from functools import singledispatchmethod
 import os
 from typing import List, Literal, Optional
 import shutil
+from uuid import UUID
 
-from inductiva.types import Path
+from inductiva import tasks
 from inductiva.scenarios import Scenario
 from inductiva.simulation import Simulator
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.simulators import SPlisHSPlasH
 from inductiva.fluids.simulators import DualSPHysics
 from inductiva.utils.templates import replace_params_in_template
 from inductiva.fluids.scenarios._post_processing import SPHSimulationOutput
@@ -21,143 +22,157 @@
 UNIT_BOX_MESH_FILENAME = "unit_box.obj"
 
 DUALSPHYSICS_TEMPLATE_FILENAME = "fluid_block_template.dualsphysics.xml.jinja"
 DUALSPHYSICS_CONFIG_FILENAME = "dam_break.xml"
 
 
 class FluidBlock(Scenario):
-    """Physical scenario of a general fluid block simulation."""
+    """Fluid block scenario.
+    
+    This is a simulation scenario for a fluid block moving in a cubic tank under
+    the action of gravity. The tank is a cube of dimensions 1 x 1 x 1 m. The
+    fluid block is also cubic, but has configurable dimensions and initial
+    position and velocity. The fluid properties such as density and kinematic
+    viscosity are also configurable.
+
+    Schematic representation of the simulation scenario:
+    _________________________________
+    |                               |  tank
+    |         ___________           |
+    |         |         |           |
+    |         |  fluid  |  ->       |
+    |         |  block  |  initial  |
+    |         |_________|  velocity |
+    |                               |
+    |                               |
+    |_______________________________|
+
+    The scenario can be simulated with SPlisSPlasH and DualSPHysics.
+    """
+
+    valid_simulators = [SPlisHSPlasH, DualSPHysics]
 
     def __init__(self,
                  density: float,
                  kinematic_viscosity: float,
                  dimensions: List[float],
                  position: Optional[List[float]] = None,
-                 inital_velocity: Optional[List[float]] = None):
-        """Initializes a `FluidBlock` object.
+                 initial_velocity: Optional[List[float]] = None):
+        """Initializes the fluid block scenario.
 
         Args:
-            density: Density of the fluid in kg/m^3.
-            kinematic_viscosity: Kinematic viscosity of the fluid,
-                in m^2/s.
-            dimensions: A list containing fluid column dimensions,
-                in meters.
-            position: Position of the fluid column in the tank,
-                in meters.
-            initial_velocity: Initial velocity of the fluid block
-                in the [x, y, z] axes, in m/s.
+            density: The density of the fluid in kg/m^3.
+            kinematic_viscosity: The kinematic viscosity of the fluid, in m^2/s.
+            dimensions: The fluid block dimensions (in x, y, z), in meters.
+            position: The position of the fluid block in the tank (in x, y, z),
+              in meters.
+            initial_velocity: The initial velocity of the fluid block (in x, y,
+              z), in m/s.
         """
 
         self.fluid = FluidType(density=density,
                                kinematic_viscosity=kinematic_viscosity)
 
         if len(dimensions) != 3:
             raise ValueError("`fluid_dimensions` must have 3 values.")
         self.dimensions = dimensions
 
         if position is None:
             self.position = [0, 0, 0]
         else:
             self.position = position
 
-        if inital_velocity is None:
+        if initial_velocity is None:
             self.initial_velocity = [0, 0, 0]
         else:
-            self.initial_velocity = inital_velocity
+            self.initial_velocity = initial_velocity
 
     def simulate(
         self,
         simulator: Simulator = DualSPHysics(),
-        output_dir: Optional[Path] = None,
+        resource_pool_id: Optional[UUID] = None,
+        run_async: bool = False,
         device: Literal["cpu", "gpu"] = "gpu",
         particle_radius: float = 0.02,
         simulation_time: float = 1,
         adaptive_time_step: bool = True,
         particle_sorting: bool = True,
         time_step: float = 0.001,
         output_time_step: float = 1 / 60,
-    ):
+    ) -> tasks.Task:
         """Simulates the scenario.
 
         Args:
-            simulator: Simulator to use.
-            output_dir: Directory to store the simulation output.
-            device: Device in which to run the simulation.
+            simulator: The simulator to use for the simulation. Supported
+              simulators are: SPlisHSPlasH, DualSPHysics.
+            device: Device in which to run the simulation. Available options are
+              "cpu" and "gpu".
             particle_radius: Radius of the fluid particles, in meters.
-            simulation_time: Simulation time, in seconds.
-            adaptive_time_step: Whether to use adaptive time step.
+              Determines the resolution of the simulation. Lower values result
+              in higher resolution and longer simulation times.
+            simulation_time: The simulation time, in seconds.
+            adaptive_time_step: Whether to use adaptive time stepping.
             particle_sorting: Whether to use particle sorting.
             time_step: Time step, in seconds.
             output_time_step: Time step between outputs, in seconds.
+            run_async: Whether to run the simulation asynchronously.
         """
 
         # TODO: Avoid storing these as class attributes.
         self.particle_radius = particle_radius
         self.simulation_time = simulation_time
         self.adaptive_time_step = adaptive_time_step
         self.particle_sorting = particle_sorting
         self.time_step = time_step
         self.output_time_step = output_time_step
 
-        output_path = super().simulate(
-            simulator,
-            output_dir=output_dir,
-            device=device,
-        )
+        task = super().simulate(simulator=simulator,
+                                resource_pool_id=resource_pool_id,
+                                run_async=run_async,
+                                device=device)
 
         # TODO: Add any kind of post-processing here, e.g. convert files?
         # convert_vtk_data_dir_to_netcdf(
         #     data_dir=os.path.join(output_path, "vtk"),
         #     output_time_step=SPLISHSPLASH_OUTPUT_TIM_STEP,
         #     netcdf_data_dir=os.path.join(output_path, "netcdf"))
+        task.set_output_class(SPHSimulationOutput)
 
-        return SPHSimulationOutput(output_path)
+        return task
 
     @singledispatchmethod
-    @classmethod
-    def get_config_filename(cls, simulator: Simulator):  # pylint: disable=unused-argument
-        raise ValueError(
-            f"Simulator not supported for `{cls.__name__}` scenario.")
+    def get_config_filename(self, simulator: Simulator):
+        pass
 
     @singledispatchmethod
-    def gen_aux_files(self, simulator: Simulator, input_dir: str):
-        raise ValueError(
-            f"Simulator not supported for `{self.__class__.__name__}` scenario."
-        )
-
-    @singledispatchmethod
-    def gen_config(self, simulator: Simulator, input_dir: str):
-        raise ValueError(
-            f"Simulator not supported for `{self.__class__.__name__}` scenario."
-        )
+    def create_input_files(self, simulator: Simulator):
+        pass
 
 
 @FluidBlock.get_config_filename.register
 def _(cls, simulator: SPlisHSPlasH):  # pylint: disable=unused-argument
     """Returns the configuration filename for SPlisHSPlasH."""
     return SPLISHSPLASH_CONFIG_FILENAME
 
 
-@FluidBlock.gen_aux_files.register
+@FluidBlock.create_input_files.register
 def _(self, simulator: SPlisHSPlasH, input_dir):  # pylint: disable=unused-argument
-    """Generates auxiliary files for SPlisHSPlasH."""
+    """Creates SPlisHSPlasH simulation input files."""
+
+    # Copy the unit box mesh file to the input directory.
     unit_box_file_path = os.path.join(os.path.dirname(__file__),
                                       UNIT_BOX_MESH_FILENAME)
     shutil.copy(unit_box_file_path, input_dir)
 
-
-@FluidBlock.gen_config.register
-def _(self, simulator: SPlisHSPlasH, input_dir: str):  # pylint: disable=unused-argument
-    """Generates the configuration file for SPlisHSPlasH."""
-
+    # Generate the simulation configuration file.
     fluid_margin = 2 * self.particle_radius
 
     replace_params_in_template(
-        templates_dir=os.path.dirname(__file__),
-        template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
+        template_path=os.path.join(os.path.dirname(__file__),
+                                   SPLISHSPLASH_TEMPLATE_FILENAME),
         params={
             "simulation_time": self.simulation_time,
             "time_step": self.time_step,
             "particle_radius": self.particle_radius,
             "data_export_rate": 1 / self.output_time_step,
             "tank_filename": UNIT_BOX_MESH_FILENAME,
             "tank_dimensions": TANK_DIMENSIONS,
@@ -179,26 +194,21 @@
 
 @FluidBlock.get_config_filename.register
 def _(cls, simulator: DualSPHysics):  # pylint: disable=unused-argument
     """Returns the configuration filename for DualSPHysics."""
     return DUALSPHYSICS_CONFIG_FILENAME
 
 
-@FluidBlock.gen_aux_files.register
+@FluidBlock.create_input_files.register
 def _(self, simulator: DualSPHysics, input_dir):  # pylint: disable=unused-argument
-    pass
-
-
-@FluidBlock.gen_config.register
-def _(self, simulator: DualSPHysics, input_dir: str):  # pylint: disable=unused-argument
-    """Generates the configuration file for DualSPHysics."""
+    """Creates DualSPHysics simulation input files."""
 
     replace_params_in_template(
-        templates_dir=os.path.dirname(__file__),
-        template_filename=DUALSPHYSICS_TEMPLATE_FILENAME,
+        template_path=os.path.join(os.path.dirname(__file__),
+                                   DUALSPHYSICS_TEMPLATE_FILENAME),
         params={
             "simulation_time": self.simulation_time,
             "time_step": self.time_step,
             "particle_distance": 2 * self.particle_radius,
             "output_time_step": self.output_time_step,
             "tank_dimensions": TANK_DIMENSIONS,
             "fluid_dimensions": self.dimensions,
```

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "particleAttributes": "velocity;density",
         "enableZSort": {{ particle_sorting | tojson }}
     },
     "RigidBodies": [
         {
             "geometryFile": "{{ tank_filename }}",
             "translation": [0, 0, 0],
-            "scale": {{ tank_dimensions }},
+            "scale": {{ tank_dimensions | list }},
             "isDynamic": false
         }
     ],
     "Materials": [
         {
             "id": "Fluid",
             "density0": {{ fluid.density }},
@@ -33,13 +33,13 @@
             "viscosityMethod": 6
         }
     ],
     "FluidModels": [
         {
             "id": "Fluid",
             "particleFile": "{{ fluid_filename }}",
-            "translation": {{ fluid_position }},
-            "scale": {{ fluid_dimensions }},
-            "initialVelocity": {{ fluid_velocity }}
+            "translation": {{ fluid_position | list }},
+            "scale": {{ fluid_dimensions | list }},
+            "initialVelocity": {{ fluid_velocity | list }}
         }
     ]
 }
```

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_block/unit_box.obj` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_block/unit_box.obj`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Classes describing fluid tank scenarios."""
-
+"""Fluid tank scenario."""
 from dataclasses import dataclass, field
 from enum import Enum
 from functools import singledispatchmethod
 import os
 from typing import List, Literal, Optional
+from uuid import UUID
 
-from inductiva.types import Path
+from inductiva import tasks
 from inductiva.scenarios import Scenario
 from inductiva.simulation import Simulator
 from inductiva.fluids.shapes import BaseShape
 from inductiva.fluids.shapes import Rectangle
 from inductiva.fluids.shapes import Circle
 from inductiva.fluids.shapes import Cube
 from inductiva.fluids.shapes import Cylinder
 from inductiva.fluids.fluid_types import FluidType
 from inductiva.fluids.fluid_types import WATER
 from inductiva.fluids.simulators import SPlisHSPlasH
-from inductiva.fluids.post_processing.splishsplash import convert_vtk_data_dir_to_netcdf
 from inductiva.utils.templates import replace_params_in_template
+from inductiva.fluids.scenarios.fluid_tank.output import FluidTankOutput
 
 from . import mesh_file_utils
 
 SPLISHSPLASH_TEMPLATE_FILENAME = "fluid_tank_template.splishsplash.json.jinja"
 SPLISHSPLASH_CONFIG_FILENAME = "fluid_tank.json"
 TANK_MESH_FILENAME = "tank.obj"
 FLUID_MESH_FILENAME = "fluid.obj"
@@ -114,82 +114,117 @@
             radius=radius,
             height=height,
             position=[*top_base_position, -height],
         )
 
 
 class FluidTank(Scenario):
-    """Fluid tank."""
+    """Fluid tank scenario.
+    
+    This is a simulation scenario for a fluid tank. The tank has a 3D shape that
+    may be cubic or cylindrical. Fluid is injected in the tank via an inlet
+    located at the top of the tank, and flows out of the tank via an outlet
+    located at the bottom of the tank. The motion of the fluid is controled
+    by gravity. The fluid properties such as density and kinematic viscosity
+    are configurable. The initial fluid level in the tank is also configurable,
+    as well as the inlet and outlet positions and dimensions.
+
+    The main axis of the tank is the z axis. The inlet and outlet are located at
+    the top and bottom of the tank, respectively, along the z axis. Fluid is
+    injected from the inlet in the negative z direction with a given velocity.
+
+    Schematic representation of the simulation scenario: e.g. x/y points right,
+    z points up.
+    
+       inlet        
+    _____________________
+    |    |              |
+    |    v              |
+    |                   |
+    |                   |
+    |___________________|  fluid level
+    |                   |
+    |                   |
+    |                   |
+    |                   |
+    |___________________|
+                    |
+                    v  outlet    
+    
+    The scenario can be simulated with SPlisHSPlasH.
+    """
+
+    valid_simulators = [SPlisHSPlasH]
 
     def __init__(
         self,
         shape: BaseShape = Cylinder(radius=0.5, height=1),
         fluid: FluidType = WATER,
-        fluid_level: float = 0,
+        fluid_level: float = 0.5,
         inlet: Optional[BaseTankInlet] = CircularTankInlet(radius=0.1),
         outlet: Optional[BaseTankOutlet] = CylindricalTankOutlet(radius=0.1,
                                                                  height=0.1),
     ):
         """Initializes a fluid tank.
 
         Args:
-            shape: Shape of the tank.
-            fluid: Fluid type.
-            fluid_level: Fluid level initially in the tank.
-            inlet: Inlet of the tank.
-            outlet: Outlet of the tank.
+            shape: The shape of the tank.
+            fluid: The fluid type.
+            fluid_level: The fluid level initially in the tank.
+            inlet: The inlet of the tank.
+            outlet: The outlet of the tank.
         """
         self.shape = shape
         self.fluid = fluid
         self.fluid_level = fluid_level
         self.inlet = inlet
         self.outlet = outlet
 
     def simulate(
         self,
         simulator: Simulator = SPlisHSPlasH(),
-        output_dir: Optional[Path] = None,
+        resource_pool_id: Optional[UUID] = None,
+        run_async: bool = False,
         device: Literal["cpu", "gpu"] = "cpu",
         simulation_time: float = 5,
         resolution: Literal["low", "medium", "high"] = "low",
         output_time_step: float = 0.1,
         particle_sorting: bool = False,
-    ):
+    ) -> tasks.Task:
         """Simulates the scenario.
 
         Args:
-            simulator: Simulator to use.
-            output_dir: Directory to store the simulation output.
-            device: Device in which to run the simulation.
-            simulation_time: Simulation time, in seconds.
-            output_time_step: Time step between output files, in seconds.
+            simulator: Simulator to use. Supported simulators are: SPlisHSPlasH.
+            resource_pool_id: Resource pool to use for the simulation.
+            simulation_time: Total simulation time, in seconds.
+            output_time_step: Time step for the output, in seconds.
             resolution: Resolution of the simulation. Controls the particle
-                radius and time step.
+              radius and time step. Accepted values are: "low", "medium",
+              "high".
             particle_sorting: Whether to use particle sorting.
+            run_async: Whether to run the simulation asynchronously.
         """
 
         self.simulation_time = simulation_time
         self.particle_radius = ParticleRadius[resolution.upper()].value
         self.time_step = TimeStep[resolution.upper()].value
         self.output_time_step = output_time_step
         self.particle_sorting = particle_sorting
 
-        output_path = super().simulate(
+        task = super().simulate(
             simulator,
-            output_dir=output_dir,
+            resource_pool_id=resource_pool_id,
+            run_async=run_async,
             device=device,
+            sim_config_filename=self.get_config_filename(simulator),
         )
 
-        # TODO: Add any kind of post-processing here, e.g. convert files?
-        convert_vtk_data_dir_to_netcdf(
-            data_dir=os.path.join(output_path, "vtk"),
-            output_time_step=self.output_time_step,
-            netcdf_data_dir=os.path.join(output_path, "netcdf"))
+        task.set_output_class(FluidTankOutput)
 
-        return output_path
+        return task
 
     def get_bounding_box(self):
         """Gets the bounding box of the tank.
 
         Returns:
             Tuple of two lists representing the minimum and maximum coordinates
             of the bounding box of the tank, respectively.
@@ -200,70 +235,60 @@
         # Extend the bounding box to include the outlet.
         if self.outlet is not None:
             outlet_bounding_box_min, _ = self.outlet.shape.get_bounding_box()
             bounding_box_min[2] = outlet_bounding_box_min[2]
 
         return bounding_box_min, bounding_box_max
 
-    @singledispatchmethod
-    @classmethod
-    def get_config_filename(cls, simulator: Simulator):  # pylint: disable=unused-argument
-        raise ValueError(
-            f"Simulator not supported for `{cls.__name__}` scenario.")
+    def create_mesh_files(self, output_dir: str):
+        """Creates mesh files for the tank and fluid in the given directory."""
+        mesh_file_utils.create_tank_mesh_file(
+            shape=self.shape,
+            outlet=self.outlet,
+            path=os.path.join(output_dir, TANK_MESH_FILENAME),
+        )
 
-    @singledispatchmethod
-    def gen_aux_files(self, simulator: Simulator, input_dir: str):
-        raise ValueError(
-            f"Simulator not supported for `{self.__class__.__name__}` scenario."
+        mesh_file_utils.create_tank_fluid_mesh_file(
+            shape=self.shape,
+            fluid_level=self.fluid_level,
+            margin=2 * self.particle_radius,
+            path=os.path.join(output_dir, FLUID_MESH_FILENAME),
         )
 
     @singledispatchmethod
-    def gen_config(self, simulator: Simulator, input_dir: str):
-        raise ValueError(
-            f"Simulator not supported for `{self.__class__.__name__}` scenario."
-        )
+    def get_config_filename(self, simulator: Simulator):
+        pass
+
+    @singledispatchmethod
+    def create_input_files(self, simulator: Simulator):
+        pass
 
 
 @FluidTank.get_config_filename.register
 def _(cls, simulator: SPlisHSPlasH) -> str:  # pylint: disable=unused-argument
     """Returns the config filename for SPlisHSPlasH."""
     return SPLISHSPLASH_CONFIG_FILENAME
 
 
-@FluidTank.gen_aux_files.register
+@FluidTank.create_input_files.register
 def _(self, simulator: SPlisHSPlasH, input_dir):  # pylint: disable=unused-argument
-    """Generates auxiliary files for SPlisHSPlasH."""
-    mesh_file_utils.create_tank_mesh_file(
-        shape=self.shape,
-        outlet=self.outlet,
-        path=os.path.join(input_dir, TANK_MESH_FILENAME),
-    )
-
-    mesh_file_utils.create_tank_fluid_mesh_file(
-        shape=self.shape,
-        fluid_level=self.fluid_level,
-        margin=2 * self.particle_radius,
-        path=os.path.join(input_dir, FLUID_MESH_FILENAME),
-    )
-
-
-@FluidTank.gen_config.register
-def _(self, simulator: SPlisHSPlasH, input_dir: str):  # pylint: disable=unused-argument
-    """Generates the configuration file for SPlisHSPlasH."""
+    """Creates SPlisHSPlasH simulation input files."""
+
+    self.create_mesh_files(input_dir)
 
     bounding_box_min, bounding_box_max = self.get_bounding_box()
     inlet_position = [
         self.inlet.position[0],
         self.inlet.position[1],
         bounding_box_max[2],
     ]
 
     replace_params_in_template(
-        templates_dir=os.path.dirname(__file__),
-        template_filename=SPLISHSPLASH_TEMPLATE_FILENAME,
+        template_path=os.path.join(os.path.dirname(__file__),
+                                   SPLISHSPLASH_TEMPLATE_FILENAME),
         params={
             "simulation_time": self.simulation_time,
             "time_step": self.time_step,
             "particle_radius": self.particle_radius,
             "data_export_rate": 1 / self.output_time_step,
             "z_sort": self.particle_sorting,
             "tank_filename": TANK_MESH_FILENAME,
```

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py` & `inductiva-0.2.0/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/shapes.py` & `inductiva-0.2.0/inductiva/fluids/shapes.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/fluids/simulators/dualsphysics.py` & `inductiva-0.2.0/inductiva/fluids/simulators/openfoam.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-"""DualSPHysics module of the API."""
-import pathlib
-from typing import Literal, Optional
+"""OpenFOAM module of the API for fluid dynamics."""
+from typing import Optional, List
+from uuid import UUID
 
-from inductiva import types
+from inductiva import types, tasks
 from inductiva.simulation import Simulator
 
 
-class DualSPHysics(Simulator):
+class OpenFOAM(Simulator):
     """Class to invoke a generic DualSPHysics simulation on the API."""
 
+    def __init__(self, api_method: str = "fvm.openfoam.run_simulation"):
+        super().__init__()
+        self.api_method = api_method
+
     @property
     def api_method_name(self) -> str:
-        return "sph.dualsphysics.run_simulation"
+        return self.api_method
 
     def run(
         self,
         input_dir: types.Path,
-        sim_config_filename: str,
-        output_dir: Optional[types.Path] = None,
-        device: Literal["gpu", "cpu"] = "cpu",
-        track_logs: bool = False,
-    ) -> pathlib.Path:
+        commands: List[dict],
+        resource_pool_id: Optional[UUID] = None,
+        n_cores: int = 1,
+        run_async: bool = False,
+    ) -> tasks.Task:
         """Run the simulation.
 
         Args:
-            device: Device in which to run the simulation.
-            sim_config_filename: Name of the simulation configuration file.
+            commands: List of commands to run using the OpenFOAM simulator.
+            n_cores: Number of MPI cores to use for the simulation.
             other arguments: See the documentation of the base class.
         """
         return super().run(input_dir,
-                           output_dir=output_dir,
-                           track_logs=track_logs,
-                           device=device,
-                           input_filename=sim_config_filename)
+                           resource_pool_id=resource_pool_id,
+                           n_cores=n_cores,
+                           commands=commands,
+                           run_async=run_async)
```

### Comparing `inductiva-0.0.9/inductiva/fluids/simulators/openfoam.py` & `inductiva-0.2.0/inductiva/fluids/simulators/dualsphysics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-"""OpenFOAM module of the API for fluid dynamics."""
-import pathlib
-from typing import Optional
+"""DualSPHysics module of the API."""
 
-from inductiva import types
+from typing import Literal, Optional
+from uuid import UUID
+
+from inductiva import types, tasks
 from inductiva.simulation import Simulator
 
 
-class OpenFOAM(Simulator):
+class DualSPHysics(Simulator):
     """Class to invoke a generic DualSPHysics simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
-        return "fvm.openfoam.run_simulation"
+        return "sph.dualsphysics.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
-        output_dir: Optional[types.Path] = None,
-        openfoam_solver: str = "interFoam",
-        n_cores=1,
-        track_logs: bool = False,
-    ) -> pathlib.Path:
+        sim_config_filename: str,
+        device: Literal["gpu", "cpu"] = "cpu",
+        resource_pool_id: Optional[UUID] = None,
+        run_async: bool = False,
+    ) -> tasks.Task:
         """Run the simulation.
 
         Args:
-            n_cores: Number of MPI cores to use for the simulation.
-            openfoam_solver: specific solver to simulate with OpenFOAM.
-                OpenFOAM contains lots of solvers inside of it, which are used
-                to call the run simulation through terminal, e.g.,
-                [isoFoam, sonicFoam, ...]. The default solver is isoFoam.
+            device: Device in which to run the simulation.
+            sim_config_filename: Name of the simulation configuration file.
             other arguments: See the documentation of the base class.
         """
-        return super().run(
-            input_dir,
-            output_dir=output_dir,
-            track_logs=track_logs,
-            openfoam_solver=openfoam_solver,
-            n_cores=n_cores,
-        )
+        return super().run(input_dir,
+                           resource_pool_id=resource_pool_id,
+                           device=device,
+                           input_filename=sim_config_filename,
+                           run_async=run_async)
```

### Comparing `inductiva-0.0.9/inductiva/fluids/simulators/splishsplash.py` & `inductiva-0.2.0/inductiva/tasks/run_simulation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-"""DualSPHysics module of the API."""
+"""Functions for running simulations via Inductiva Web API."""
 import pathlib
-from typing import Literal, Optional
+from typing import Any, Optional
+from uuid import UUID
 
-from inductiva import types
-from inductiva.simulation import Simulator
+from inductiva import tasks
+from inductiva.api import methods
 
 
-class SPlisHSPlasH(Simulator):
-    """Class to invoke a generic SPlisHSPlasH simulation on the API."""
+def run_simulation(
+    api_method_name: str,
+    input_dir: pathlib.Path,
+    resource_pool_id: Optional[UUID] = None,
+    run_async: bool = False,
+    **kwargs: Any,
+) -> tasks.Task:
+    """Run a simulation via Inductiva Web API."""
+
+    params = {
+        "sim_dir": input_dir,
+        **kwargs,
+    }
+    type_annotations = {
+        "sim_dir": pathlib.Path,
+    }
+
+    task_id = methods.invoke_async_api(api_method_name,
+                                       params,
+                                       type_annotations,
+                                       resource_pool_id=resource_pool_id)
+    task = tasks.Task(task_id)
+    if not isinstance(task_id, str):
+        raise RuntimeError(
+            f"Expected result to be a string with task_id, got {type(task_id)}")
+
+    # Blocking call for sync execution
+    if not run_async:
+        with task:
+            task.wait()
 
-    @property
-    def api_method_name(self) -> str:
-        return "sph.splishsplash.run_simulation"
-
-    def run(
-        self,
-        input_dir: types.Path,
-        sim_config_filename: str,
-        output_dir: Optional[types.Path] = None,
-        device: Literal["gpu", "cpu"] = "cpu",
-        track_logs: bool = False,
-    ) -> pathlib.Path:
-        """Run the simulation.
-
-        Args:
-            sim_config_filename: Name of the simulation configuration file.
-            device: Device in which to run the simulation.
-            other arguments: See the documentation of the base class.
-        """
-        return super().run(
-            input_dir,
-            output_dir=output_dir,
-            track_logs=track_logs,
-            device=device,
-            input_filename=sim_config_filename,
-        )
+    return task
```

### Comparing `inductiva-0.0.9/inductiva/fluids/simulators/swash.py` & `inductiva-0.2.0/inductiva/fluids/simulators/swash.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """SWASH module of the API."""
-import pathlib
 from typing import Optional
+from uuid import UUID
 from inductiva.simulation import Simulator
-from inductiva import types
+from inductiva import types, tasks
 
 
 class SWASH(Simulator):
     """Class to invoke a generic SWASH simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
         return "sw.swash.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
         sim_config_filename: str,
-        output_dir: Optional[types.Path] = None,
-        n_cores=1,
-        track_logs: bool = False,
-    ) -> pathlib.Path:
+        resource_pool_id: Optional[UUID] = None,
+        n_cores: int = 1,
+        run_async: bool = False,
+    ) -> tasks.Task:
         """Run the simulation.
 
         Args:
             n_cores: Number of MPI cores to use for the simulation.
             sim_config_filename: Name of the simulation configuration file.
             other arguments: See the documentation of the base class.
         """
         return super().run(input_dir,
-                           track_logs=track_logs,
+                           resource_pool_id=resource_pool_id,
                            input_filename=sim_config_filename,
                            n_cores=n_cores,
-                           output_dir=output_dir)
+                           run_async=run_async)
```

### Comparing `inductiva-0.0.9/inductiva/fluids/simulators/xbeach.py` & `inductiva-0.2.0/inductiva/fluids/simulators/xbeach.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """DualSPHysics module of the API."""
-import pathlib
 from typing import Optional
+from uuid import UUID
 
-from inductiva import types
+from inductiva import types, tasks
 from inductiva.simulation import Simulator
 
 
 class XBeach(Simulator):
     """Class to invoke a generic XBeach simulation on the API."""
 
     @property
     def api_method_name(self) -> str:
         return "sw.xbeach.run_simulation"
 
     def run(
         self,
         input_dir: types.Path,
         sim_config_filename: Optional[str] = "params.txt",
-        output_dir: Optional[types.Path] = None,
+        resource_pool_id: Optional[UUID] = None,
         n_cores: int = 1,
-        track_logs: bool = False,
-    ) -> pathlib.Path:
+        run_async: bool = False,
+    ) -> tasks.Task:
         """Run the simulation.
 
         Args:
+            sim_config_filename: Name of the simulation configuration file.
             n_cores: Number of MPI cores to use for the simulation.
             other arguments: See the documentation of the base class.
         """
         return super().run(
             input_dir,
             input_filename=sim_config_filename,
             n_cores=n_cores,
-            track_logs=track_logs,
-            output_dir=output_dir,
+            resource_pool_id=resource_pool_id,
+            run_async=run_async,
         )
```

### Comparing `inductiva-0.0.9/inductiva/scenarios.py` & `inductiva-0.2.0/inductiva/scenarios.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 """Base class for scenarios."""
 
-from abc import ABC
+from abc import ABC, abstractmethod
 import tempfile
 from typing import Optional
-
+from uuid import UUID
 from inductiva.types import Path
 from inductiva.simulation import Simulator
-from inductiva.utils.files import resolve_path, get_timestamped_path
-from inductiva.utils.misc import split_camel_case
+import json
 
 
 class Scenario(ABC):
     """Base class for scenarios."""
+    valid_simulators = []
+
+    @abstractmethod
+    def create_input_files(self, simulator: Simulator, input_dir: Path):
+        """To be implemented in subclasses."""
+        pass
+
+    def read_commands_from_file(self, commands_path: str):
+        "Read list of commands from commands.json file"
+        with open(commands_path, "r", encoding="utf-8") as f:
+            commands = json.load(f)
+        return commands
+
+    def validate_simulator(self, simulator: Simulator):
+        """Checks if the scenario can be simulated with the given simulator."""
+        if type(simulator) not in self.valid_simulators:
+            raise ValueError(
+                f"Simulator not supported for `{self.__class__.__name__}` "
+                "scenario.")
 
     def simulate(
         self,
         simulator: Simulator,
-        output_dir: Optional[Path] = None,
+        resource_pool_id: Optional[UUID] = None,
+        run_async: bool = False,
         **kwargs,
     ):
-        """Simulates the scenario."""
-        if output_dir is None:
-            scenario_name_splitted = split_camel_case(self.__class__.__name__)
-            output_dir_prefix = "-".join(scenario_name_splitted).lower()
-            output_dir = get_timestamped_path(f"{output_dir_prefix}-output")
-
-        output_dir = resolve_path(output_dir)
+        """Simulates the scenario synchronously."""
+        self.validate_simulator(simulator)
 
         with tempfile.TemporaryDirectory() as input_dir:
+            self.create_input_files(simulator, input_dir)
 
-            self.gen_aux_files(simulator, input_dir)
-            self.gen_config(simulator, input_dir)
-
-            args = ()
-            config_filename = self.get_config_filename(simulator)
-            if config_filename:
-                args += (config_filename,)
-
-            output_path = simulator.run(
+            return simulator.run(
                 input_dir,
-                *args,
-                output_dir=output_dir,
+                resource_pool_id=resource_pool_id,
+                run_async=run_async,
                 **kwargs,
             )
-
-        return output_path
```

### Comparing `inductiva-0.0.9/inductiva/simulation/simulator.py` & `inductiva-0.2.0/inductiva/design.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""Base class for low-level simulators."""
-from abc import ABC, abstractmethod
-import pathlib
-from typing import Optional
+"""Functions to explore design space of simulations."""
+import os
+from typing import Any, List, Optional
+from absl import logging
 
-from inductiva import api
 from inductiva import types
+from inductiva.simulation import Simulator
+from inductiva.utils import templates
 from inductiva.utils import files
 
 
-class Simulator(ABC):
-    """Base simulator class."""
+def explore_design_space(simulator: Simulator,
+                         input_dir: types.Path,
+                         template_filename: str,
+                         tag: str,
+                         values: List[Any],
+                         output_dir: Optional[types.Path] = None,
+                         **extra_sim_kwargs):
+    """Explore over design parameters with a template file.
+
+    Args:
+        simulator: Simulator to use.
+        input_dir: Directory where the input files (including the template
+            file) are located.
+        template_filename: Name of the template file.
+        tag: Name of the parameter to explore.
+        values: Values of the parameter to explore.
+        output_dir: Directory where the output files will be stored.
+        extra_sim_kwargs: Extra keyword arguments to pass to the simulator.
+    """
+    input_dir = files.resolve_path(input_dir)
+    file_format = os.path.splitext(template_filename)[1]
+
+    if output_dir is None:
+        output_dir = input_dir.with_name(f"{input_dir.name}-output")
+    else:
+        output_dir = files.resolve_path(output_dir)
+
+    logging.info("Exploring design space for attribute \"%s\".", tag)
+
+    for value in values:
+        logging.info("Running simulation for %s=%s.", tag, value)
+
+        input_filename = f"input_file_{value}{file_format}"
+        template_path = os.path.join(input_dir, template_filename)
+        input_file = os.path.join(input_dir, input_filename)
+
+        templates.replace_params_in_template(
+            template_path,
+            {tag: value},
+            input_file,
+        )
 
-    @property
-    @abstractmethod
-    def api_method_name(self) -> str:
-        pass
-
-    def run(
-        self,
-        input_dir: types.Path,
-        *_args,
-        output_dir: Optional[types.Path] = None,
-        track_logs: bool = False,
-        **kwargs,
-    ) -> pathlib.Path:
-        """Run the simulation.
-
-        Args:
-            input_dir: Path to the directory containing the input files.
-            _args: Unused in this method, but defined to allow for more
-                non-default arguments in method override in subclasses.
-            output_dir: Path to the directory where the output files will be
-                stored. If not provided, a timestamped directory will be
-                created with the same name as the input directory appended
-                with "-output".
-            track_logs: If True, the logs of the remote execution will be
-                streamed to the console.
-            **kwargs: Additional keyword arguments to be passed to the
-                simulation API method.
-        """
-        input_dir = files.resolve_path(input_dir)
-        if not input_dir.is_dir():
-            raise ValueError(
-                f"The provided path (\"{input_dir}\") is not a directory.")
-
-        if output_dir is None:
-            output_dir = input_dir.with_name(f"{input_dir.name}-output")
-            output_dir = files.get_timestamped_path(output_dir)
-        else:
-            output_dir = files.resolve_path(output_dir)
-
-        return api.run_simulation(
-            self.api_method_name,
-            input_dir,
-            output_dir,
-            params=kwargs,
-            log_remote_execution=track_logs,
+        simulator.run(
+            input_dir=input_dir,
+            sim_config_filename=input_filename,
+            output_dir=output_dir.joinpath(f"design_{tag}={value}"),
+            **extra_sim_kwargs,
         )
```

### Comparing `inductiva-0.0.9/inductiva/utils/data.py` & `inductiva-0.2.0/inductiva/utils/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import pathlib
 import zipfile
 import tempfile
 import shutil
 import numpy as np
 import scipy
+from tqdm import tqdm
+import urllib3
 
 from absl import logging
 
 from .meta import is_tuple
 from inductiva.types import Path
 
 INPUT_FILENAME = "input.json"
@@ -241,7 +243,68 @@
     """Compress a directory into a zip file."""
     zip_path = shutil.make_archive(
         os.path.join(tempfile.gettempdir(), zip_name), "zip", dir_path)
 
     logging.debug("Compressed inputs to %s", zip_path)
 
     return zip_path
+
+
+def download_file(
+    response: urllib3.response.HTTPResponse,
+    output_path: pathlib.Path,
+    chunk_size=1024,
+) -> None:
+    """Download a file from a urllib3 response object.
+
+    Use a urllib3 response object to download a file, showing a progress bar.
+
+    Args:
+        response: urllib3 response object.
+        output_path: Path where to store the downloaded file.
+        chunk_size: Size of the chunks in which to download the file.
+    """
+    # if the response header does not contain a content-length,
+    # the progress bar will not be displayed correctly, but download
+    # will still work
+    download_size = response.headers.get("content-length", 0)
+
+    with tqdm(
+            total=int(download_size),
+            unit="iB",
+            unit_scale=True,
+            unit_divisor=1024,  # Use 1 KiB = 1024 bytes instead of 1000 bytes
+    ) as progress_bar:
+        with open(output_path, "wb") as f:
+            while chunk := response.read(chunk_size):
+                f.write(chunk)
+                progress_bar.update(len(chunk))
+
+    response.release_conn()
+
+
+def uncompress_task_outputs(zip_path: pathlib.Path, output_dir: pathlib.Path):
+    """Uncompress a ZIP archive containing the outputs of a task.
+
+    If the archive contains the directory called artifacts, it means that the
+    download includes the full ouputs of the task with the full directory
+    structure of the outputs (output.json, artifacts/*). Only the contents
+    inside artifacts are extracted to the output directory. If the archive
+    does not contain the artifacts directory, it means that the download
+    only includes a few files, which are directly in the root of the archive,
+    without the `artifacts` directory.
+    """
+    with zipfile.ZipFile(zip_path, "r") as zip_f:
+        full_output = True
+        try:
+            zip_f.getinfo("artifacts/")
+        except KeyError:
+            full_output = False
+
+        if full_output:
+            extract_subdir_files(
+                zip_f,
+                "artifacts",
+                output_dir,
+            )
+        else:
+            zip_f.extractall(output_dir)
```

### Comparing `inductiva-0.0.9/inductiva/utils/files.py` & `inductiva-0.2.0/inductiva/utils/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """Utilities for working with the file system."""
 import os
 import time
 import pathlib
-import inductiva
 
+import inductiva
 from inductiva import types
 
 
+def find_path_to_package(package_dir: str):
+    """Find path to package directory in inductiva library in local computer.
+
+    Args:
+        package_dir: Name of package directory.
+    """
+    return os.path.abspath(
+        os.path.join(os.path.dirname(__file__), "..", package_dir))
+
+
 def get_timestamped_path(path: types.Path, sep: str = "-") -> pathlib.Path:
     """Return a path that does not exist by appending a timestamp.
 
     Args:
         path: Path to a file or directory.
 
     Returns:
```

### Comparing `inductiva-0.0.9/inductiva/utils/files_test.py` & `inductiva-0.2.0/inductiva/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/utils/flags.py` & `inductiva-0.2.0/inductiva/utils/flags.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/utils/meta.py` & `inductiva-0.2.0/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/inductiva/utils/misc_test.py` & `inductiva-0.2.0/inductiva/utils/misc_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.9/setup.cfg` & `inductiva-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 [metadata]
 name = inductiva
-version = 0.0.9
+version = 0.2.0
 description = Python client for the Inductiva API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Inductiva Research Labs
 author_email = contact@inductiva.ai
 url = https://github.com/inductiva/inductiva
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	urllib3 >= 1.15
-	certifi
+	certifi >= 14.5.14
+	frozendict ~= 2.3.4
+	setuptools >= 21.0.0
+	typing-extensions ~= 4.3.0
+	urllib3 ~= 1.26.7
 	python-dateutil
-	frozendict
-	typing_extensions
+	
 	absl-py
 	tqdm
 	jinja2
 	numpy
 	scipy
 	matplotlib
 	xarray
 	gmsh
 	meshio
 	vtk
+	imageio
 	pyvista
 	imageio-ffmpeg
 	ipython
-	websockets
+	nglview
+	MDAnalysis
 
 [options.package_data]
 * = *.obj, *.jinja
+inductiva = templates/**
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [egg_info]
```

