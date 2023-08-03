# Comparing `tmp/aliyun-log-python-sdk-0.8.7.tar.gz` & `tmp/aliyun-log-python-sdk-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-log-python-sdk-0.8.7.tar", last modified: Fri Jul 28 08:58:17 2023, max compression
+gzip compressed data, was "dist/aliyun-log-python-sdk-0.8.8.tar", last modified: Thu Aug  3 11:34:44 2023, max compression
```

## Comparing `aliyun-log-python-sdk-0.8.7.tar` & `aliyun-log-python-sdk-0.8.8.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/
--rw-r--r--   0 haha       (502) staff       (20)      935 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/PKG-INFO
--rwxr-xr-x   0 haha       (502) staff       (20)     2677 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/README.md
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/
--rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/__init__.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/
--rwxr-xr-x   0 haha       (502) staff       (20)     1648 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/__init__.py
--rwxr-xr-x   0 haha       (502) staff       (20)      879 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/acl_config.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1629 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/acl_response.py
--rw-r--r--   0 haha       (502) staff       (20)     6712 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/auth.py
--rw-r--r--   0 haha       (502) staff       (20)     2784 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/common_response.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/
--rwxr-xr-x   0 haha       (502) staff       (20)      152 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/__init__.py
--rwxr-xr-x   0 haha       (502) staff       (20)     2319 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/checkpoint_tracker.py
--rwxr-xr-x   0 haha       (502) staff       (20)     4379 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/config.py
--rwxr-xr-x   0 haha       (502) staff       (20)     4577 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/consumer_client.py
--rw-r--r--   0 haha       (502) staff       (20)      531 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/exceptions.py
--rwxr-xr-x   0 haha       (502) staff       (20)      590 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/fetched_log_group.py
--rwxr-xr-x   0 haha       (502) staff       (20)     4159 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/heart_beat.py
--rwxr-xr-x   0 haha       (502) staff       (20)    11472 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/shard_worker.py
--rwxr-xr-x   0 haha       (502) staff       (20)     7454 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/tasks.py
--rwxr-xr-x   0 haha       (502) staff       (20)     8589 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/worker.py
--rwxr-xr-x   0 haha       (502) staff       (20)     3285 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_request.py
--rwxr-xr-x   0 haha       (502) staff       (20)     5252 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)      813 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)      808 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_time_response.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/
--rw-r--r--   0 haha       (502) staff       (20)      171 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/__init__.py
--rw-r--r--   0 haha       (502) staff       (20)     1690 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/doc_logitem_converter.py
--rw-r--r--   0 haha       (502) staff       (20)     2583 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/index_logstore_mappings.py
--rw-r--r--   0 haha       (502) staff       (20)    11037 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/mapping_index_converter.py
--rw-r--r--   0 haha       (502) staff       (20)     2347 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_log.py
--rw-r--r--   0 haha       (502) staff       (20)    16932 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_manager.py
--rw-r--r--   0 haha       (502) staff       (20)      281 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_response.py
--rw-r--r--   0 haha       (502) staff       (20)     8326 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_task.py
--rwxr-xr-x   0 haha       (502) staff       (20)      194 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/util.py
--rw-r--r--   0 haha       (502) staff       (20)     4373 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_config_response.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/
--rw-r--r--   0 haha       (502) staff       (20)      128 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/__init__.py
--rw-r--r--   0 haha       (502) staff       (20)     2301 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/config_parser.py
--rw-r--r--   0 haha       (502) staff       (20)     5370 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/etl_util.py
--rw-r--r--   0 haha       (502) staff       (20)      450 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/exceptions.py
--rw-r--r--   0 haha       (502) staff       (20)     2723 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/restrict_config_parser.py
--rw-r--r--   0 haha       (502) staff       (20)     1245 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/runner.py
--rw-r--r--   0 haha       (502) staff       (20)     1422 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/settings.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/
--rw-r--r--   0 haha       (502) staff       (20)      500 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/__init__.py
--rw-r--r--   0 haha       (502) staff       (20)     2523 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_base.py
--rw-r--r--   0 haha       (502) staff       (20)     2031 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_csv.py
--rw-r--r--   0 haha       (502) staff       (20)    14656 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_json.py
--rw-r--r--   0 haha       (502) staff       (20)     3649 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_kv.py
--rw-r--r--   0 haha       (502) staff       (20)     9141 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_lookup.py
--rw-r--r--   0 haha       (502) staff       (20)     4051 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_mv.py
--rw-r--r--   0 haha       (502) staff       (20)     5215 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_regex.py
--rw-r--r--   0 haha       (502) staff       (20)     3704 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_set_field.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/
--rw-r--r--   0 haha       (502) staff       (20)      156 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/__init__.py
--rw-r--r--   0 haha       (502) staff       (20)     4419 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_list.py
--rw-r--r--   0 haha       (502) staff       (20)     1923 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_transform.py
--rw-r--r--   0 haha       (502) staff       (20)      903 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_util.py
--rw-r--r--   0 haha       (502) staff       (20)      145 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_base.py
--rw-r--r--   0 haha       (502) staff       (20)     2126 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_list.py
--rw-r--r--   0 haha       (502) staff       (20)     3680 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_meta.py
--rw-r--r--   0 haha       (502) staff       (20)     2764 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/export_response.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/
--rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/__init__.py
--rw-r--r--   0 haha       (502) staff       (20)    13130 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/jupyter_magic.py
--rw-r--r--   0 haha       (502) staff       (20)     7247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/syslogclient.py
--rw-r--r--   0 haha       (502) staff       (20)     8125 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config.py
--rw-r--r--   0 haha       (502) staff       (20)     4315 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config_response.py
--rw-r--r--   0 haha       (502) staff       (20)     2931 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getcontextlogsresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     3400 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     7154 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)     6297 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1733 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/histogram.py
--rwxr-xr-x   0 haha       (502) staff       (20)    10335 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/index_config.py
--rwxr-xr-x   0 haha       (502) staff       (20)     2220 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/index_config_response.py
--rw-r--r--   0 haha       (502) staff       (20)     5180 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ingestion_response.py
--rw-r--r--   0 haha       (502) staff       (20)     6360 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/job.py
--rwxr-xr-x   0 haha       (502) staff       (20)      407 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1902 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1897 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1570 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     8952 2023-07-28 08:41:13.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_pb2.py
--rw-r--r--   0 haha       (502) staff       (20)     9641 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_raw_pb2.py
--rw-r--r--   0 haha       (502) staff       (20)   207442 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient.py
--rwxr-xr-x   0 haha       (502) staff       (20)    12625 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_core.py
--rw-r--r--   0 haha       (502) staff       (20)    39270 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_operator.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1998 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logexception.py
--rw-r--r--   0 haha       (502) staff       (20)    23176 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logger_hanlder.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logitem.py
--rwxr-xr-x   0 haha       (502) staff       (20)      700 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1375 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     5722 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logstore_config_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)    41883 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_detail.py
--rwxr-xr-x   0 haha       (502) staff       (20)     4086 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     2826 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/machine_group_detail.py
--rwxr-xr-x   0 haha       (502) staff       (20)     9341 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/machinegroup_response.py
--rw-r--r--   0 haha       (502) staff       (20)     2438 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/odps_sink.py
--rw-r--r--   0 haha       (502) staff       (20)     2517 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/oss_sink.py
--rw-r--r--   0 haha       (502) staff       (20)     2293 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/pluralize.py
--rwxr-xr-x   0 haha       (502) staff       (20)     3795 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/project_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     6141 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/pulllog_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     3388 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsrequest.py
--rwxr-xr-x   0 haha       (502) staff       (20)      545 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsresponse.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/queriedlog.py
--rw-r--r--   0 haha       (502) staff       (20)     9831 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/resource_params.py
--rw-r--r--   0 haha       (502) staff       (20)     7925 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/resource_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     1358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shard_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     4652 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_config.py
--rwxr-xr-x   0 haha       (502) staff       (20)     7532 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_response.py
--rw-r--r--   0 haha       (502) staff       (20)      358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/sink.py
--rw-r--r--   0 haha       (502) staff       (20)     1775 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/sql_instance_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     5833 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/substore_config_response.py
--rw-r--r--   0 haha       (502) staff       (20)    13437 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_params.py
--rw-r--r--   0 haha       (502) staff       (20)    13619 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_response.py
--rwxr-xr-x   0 haha       (502) staff       (20)     9206 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/util.py
--rw-r--r--   0 haha       (502) staff       (20)      341 2023-07-28 08:58:04.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/version.py
-drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/
--rw-r--r--   0 haha       (502) staff       (20)      935 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haha       (502) staff       (20)     3949 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haha       (502) staff       (20)        1 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haha       (502) staff       (20)       86 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/requires.txt
--rw-r--r--   0 haha       (502) staff       (20)        7 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 haha       (502) staff       (20)       38 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/setup.cfg
--rwxr-xr-x   0 haha       (502) staff       (20)     2847 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/setup.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/
+-rw-r--r--   0 haha       (502) staff       (20)      935 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/PKG-INFO
+-rwxr-xr-x   0 haha       (502) staff       (20)     2677 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/README.md
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun/
+-rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/__init__.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/
+-rwxr-xr-x   0 haha       (502) staff       (20)     1648 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/__init__.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      879 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/acl_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1629 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/acl_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     6712 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/auth.py
+-rw-r--r--   0 haha       (502) staff       (20)     2784 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/common_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/
+-rwxr-xr-x   0 haha       (502) staff       (20)      152 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/__init__.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2319 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/checkpoint_tracker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4379 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4577 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/consumer_client.py
+-rw-r--r--   0 haha       (502) staff       (20)      531 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/exceptions.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      590 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/fetched_log_group.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4159 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/heart_beat.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    11472 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/shard_worker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7454 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/tasks.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     8589 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/worker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3285 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer_group_request.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5252 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/consumer_group_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      813 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/cursor_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      808 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/cursor_time_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/
+-rw-r--r--   0 haha       (502) staff       (20)      171 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     1690 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/doc_logitem_converter.py
+-rw-r--r--   0 haha       (502) staff       (20)     2583 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/index_logstore_mappings.py
+-rw-r--r--   0 haha       (502) staff       (20)    11037 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/mapping_index_converter.py
+-rw-r--r--   0 haha       (502) staff       (20)     2347 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_log.py
+-rw-r--r--   0 haha       (502) staff       (20)    16932 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_manager.py
+-rw-r--r--   0 haha       (502) staff       (20)      281 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     8326 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_task.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      194 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/util.py
+-rw-r--r--   0 haha       (502) staff       (20)     4373 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_config_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/
+-rw-r--r--   0 haha       (502) staff       (20)      128 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     2301 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/config_parser.py
+-rw-r--r--   0 haha       (502) staff       (20)     5370 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/etl_util.py
+-rw-r--r--   0 haha       (502) staff       (20)      450 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/exceptions.py
+-rw-r--r--   0 haha       (502) staff       (20)     2723 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/restrict_config_parser.py
+-rw-r--r--   0 haha       (502) staff       (20)     1245 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/runner.py
+-rw-r--r--   0 haha       (502) staff       (20)     1422 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/settings.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/
+-rw-r--r--   0 haha       (502) staff       (20)      500 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     2523 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_base.py
+-rw-r--r--   0 haha       (502) staff       (20)     2031 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_csv.py
+-rw-r--r--   0 haha       (502) staff       (20)    14656 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_json.py
+-rw-r--r--   0 haha       (502) staff       (20)     3649 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_kv.py
+-rw-r--r--   0 haha       (502) staff       (20)     9141 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_lookup.py
+-rw-r--r--   0 haha       (502) staff       (20)     4051 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_mv.py
+-rw-r--r--   0 haha       (502) staff       (20)     5215 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_regex.py
+-rw-r--r--   0 haha       (502) staff       (20)     3704 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_set_field.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/
+-rw-r--r--   0 haha       (502) staff       (20)      156 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     4419 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_list.py
+-rw-r--r--   0 haha       (502) staff       (20)     1923 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_transform.py
+-rw-r--r--   0 haha       (502) staff       (20)      903 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_util.py
+-rw-r--r--   0 haha       (502) staff       (20)      145 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/transform_base.py
+-rw-r--r--   0 haha       (502) staff       (20)     2126 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/transform_list.py
+-rw-r--r--   0 haha       (502) staff       (20)     3680 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/transform_meta.py
+-rw-r--r--   0 haha       (502) staff       (20)     2764 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/export_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/ext/
+-rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/ext/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)    13130 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/ext/jupyter_magic.py
+-rw-r--r--   0 haha       (502) staff       (20)     7247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/ext/syslogclient.py
+-rw-r--r--   0 haha       (502) staff       (20)     8125 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/external_store_config.py
+-rw-r--r--   0 haha       (502) staff       (20)     4315 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/external_store_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     2931 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/getcontextlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3400 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/gethistogramsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/gethistogramsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7154 2023-08-03 11:34:25.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/getlogsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     6297 2023-08-03 11:34:25.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/getlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1733 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/histogram.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    10335 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/index_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2220 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/index_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     5180 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/ingestion_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     6360 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/job.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      407 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/listlogstoresrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1902 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/listlogstoresresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1897 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/listtopicsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1570 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/listtopicsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     8952 2023-07-28 08:41:13.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/log_logs_pb2.py
+-rw-r--r--   0 haha       (502) staff       (20)     9641 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/log_logs_raw_pb2.py
+-rw-r--r--   0 haha       (502) staff       (20)   213015 2023-08-03 11:34:32.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logclient.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    12625 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logclient_core.py
+-rw-r--r--   0 haha       (502) staff       (20)    39270 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logclient_operator.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1998 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logexception.py
+-rw-r--r--   0 haha       (502) staff       (20)    23176 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logger_hanlder.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logitem.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      700 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1375 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5722 2023-08-02 02:53:39.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logstore_config_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    41883 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logtail_config_detail.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4086 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/logtail_config_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2826 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/machine_group_detail.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     9341 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/machinegroup_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     2438 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/odps_sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     2517 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/oss_sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     2293 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/pluralize.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3990 2023-08-03 11:34:32.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/project_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     6141 2023-08-02 02:59:43.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/pulllog_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3388 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/putlogsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      545 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/putlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/queriedlog.py
+-rw-r--r--   0 haha       (502) staff       (20)     9831 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/resource_params.py
+-rw-r--r--   0 haha       (502) staff       (20)     7925 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/resource_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/shard_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4652 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/shipper_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7532 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/shipper_response.py
+-rw-r--r--   0 haha       (502) staff       (20)      358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     1775 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/sql_instance_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5833 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/substore_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     1107 2023-08-03 11:34:32.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/tag_response.py
+-rw-r--r--   0 haha       (502) staff       (20)    13437 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/topostore_params.py
+-rw-r--r--   0 haha       (502) staff       (20)    13619 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/topostore_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     9206 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/util.py
+-rw-r--r--   0 haha       (502) staff       (20)      341 2023-08-03 11:34:32.000000 aliyun-log-python-sdk-0.8.8/aliyun/log/version.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/
+-rw-r--r--   0 haha       (502) staff       (20)      935 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haha       (502) staff       (20)     3976 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haha       (502) staff       (20)        1 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haha       (502) staff       (20)       86 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 haha       (502) staff       (20)        7 2023-08-03 11:34:43.000000 aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haha       (502) staff       (20)       38 2023-08-03 11:34:44.000000 aliyun-log-python-sdk-0.8.8/setup.cfg
+-rwxr-xr-x   0 haha       (502) staff       (20)     2847 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.8/setup.py
```

### Comparing `aliyun-log-python-sdk-0.8.7/PKG-INFO` & `aliyun-log-python-sdk-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-log-python-sdk
-Version: 0.8.7
+Version: 0.8.8
 Summary: Aliyun log service Python client SDK
 Home-page: https://github.com/aliyun/aliyun-log-python-sdk
 Author: Aliyun
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: 
         Python SDK for Alicloud Log Service
```

### Comparing `aliyun-log-python-sdk-0.8.7/README.md` & `aliyun-log-python-sdk-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/__init__.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/__init__.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/acl_config.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/acl_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/acl_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/acl_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/auth.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/auth.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/common_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/common_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/checkpoint_tracker.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/checkpoint_tracker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/config.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/consumer_client.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/consumer_client.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/exceptions.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/exceptions.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/fetched_log_group.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/fetched_log_group.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/heart_beat.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/heart_beat.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/shard_worker.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/shard_worker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/tasks.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/worker.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer/worker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_request.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer_group_request.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/consumer_group_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/cursor_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_time_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/cursor_time_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/doc_logitem_converter.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/doc_logitem_converter.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/index_logstore_mappings.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/index_logstore_mappings.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/mapping_index_converter.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/mapping_index_converter.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_log.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_log.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_manager.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_manager.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_task.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/es_migration/migration_task.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/config_parser.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/config_parser.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/etl_util.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/etl_util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/restrict_config_parser.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/restrict_config_parser.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/runner.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/runner.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/settings.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/settings.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_base.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_base.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_csv.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_csv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_json.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_json.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_kv.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_kv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_lookup.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_lookup.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_mv.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_mv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_regex.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_regex.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_set_field.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/trans_comp/trans_set_field.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_list.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_list.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_transform.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_transform.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_util.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/condition_util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_list.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/transform_list.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_meta.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/etl_core/transform/transform_meta.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/export_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/export_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/ext/jupyter_magic.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/ext/jupyter_magic.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/ext/syslogclient.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/ext/syslogclient.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/external_store_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/external_store_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/getcontextlogsresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/getcontextlogsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsrequest.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/gethistogramsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/gethistogramsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsrequest.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/getlogsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/getlogsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/histogram.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/histogram.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/index_config.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/index_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/index_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/index_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/ingestion_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/ingestion_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/job.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/job.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/listlogstoresresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsrequest.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/listtopicsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/listtopicsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_pb2.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/log_logs_pb2.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_raw_pb2.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/log_logs_raw_pb2.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .project_response import *
 from .pulllog_response import PullLogResponse
 from .putlogsresponse import PutLogsResponse
 from .shard_response import *
 from .shipper_response import *
 from .resource_response import *
 from .resource_params import *
+from .tag_response import GetResourceTagsResponse
 from .topostore_response import *
 from .topostore_params import *
 from .util import base64_encodestring as b64e
 from .util import base64_encodestring as e64, base64_decodestring as d64
 from .version import API_VERSION, USER_AGENT
 
 from .log_logs_raw_pb2 import LogGroupRaw as LogGroup
@@ -2269,31 +2270,34 @@
         headers['Content-Type'] = 'application/json'
         headers['x-log-bodyrawsize'] = str(len(body))
         resource = "/logstores/" + logstore_name + "/shipper/" + shipper_name + "/tasks"
 
         (resp, header) = self._send("PUT", project_name, body, resource, params, headers)
         return RetryShipperTasksResponse(header, resp)
 
-    def create_project(self, project_name, project_des):
+    def create_project(self, project_name, project_des, resource_group_id=''):
         """ Create a project
         Unsuccessful operation will cause an LogException.
 
         :type project_name: string
         :param project_name: the Project name 
 
         :type project_des: string
         :param project_des: the description of a project
 
+        type resource_group_id: string
+        :param resource_group_id: the resource group id, the project created will put in the resource group
+
         :return: CreateProjectResponse 
 
         :raise: LogException
         """
 
         params = {}
-        body = {"projectName": project_name, "description": project_des}
+        body = {"projectName": project_name, "description": project_des, "resourceGroupId": resource_group_id}
 
         body = six.b(json.dumps(body))
         headers = {'Content-Type': 'application/json', 'x-log-bodyrawsize': str(len(body))}
         resource = "/"
 
         (resp, header) = self._send("POST", project_name, body, resource, params, headers)
         return CreateProjectResponse(header, resp)
@@ -2330,14 +2334,39 @@
         headers = {}
         params = {}
         resource = "/"
 
         (resp, header) = self._send("DELETE", project_name, None, resource, params, headers)
         return DeleteProjectResponse(header, resp)
 
+    def change_resource_group(self, resource_id, resource_group_id, resource_type="PROJECT"):
+        """
+        Update the resource group of project
+
+        :type resource_id: string
+        :param resource_id: resource id
+
+        :type resource_group_id: string
+        :param resource_group_id: the resource group
+
+        :type resource_type: string
+        :param resource_type: the resource type (now only support PROJECT)
+
+        :return: ChangeResourceGroupResponse
+
+        :raise: LogException
+        """
+        params = {}
+        body = {'resourceId':resource_id, 'resourceGroupId':resource_group_id, 'resourceType':resource_type}
+        body_str = six.b(json.dumps(body))
+        headers = {'Content-Type': 'application/json', 'x-log-bodyrawsize': str(len(body_str))}
+        resource = "/resourcegroup"
+        (resp, header) = self._send("PUT", resource_id, body_str, resource, params, headers)
+        return LogResponse(header, resp)
+
     def tag_project(self, project_name, **tags):
         """ tag project
         Unsuccessful operation will cause an LogException.
 
         :type project_name: string
         :param project_name: the Project name 
 
@@ -2400,14 +2429,116 @@
             resp = GetProjectTagsResponse(header, resp)
             yield resp
 
             if resp.next_token == "":
                 break
             params["nextToken"] = resp.next_token
 
+    def tag_resources(self, resource_type, resource_id, **tags):
+        """ tag resources
+        Unsuccessful operation will cause an LogException.
+
+        :type resource_type: string
+        :param resource_type: the resource type, currently only support project, logstore, dashboard, machine_group, logtail_config
+
+        :type resource_id: string
+        :param resource_id: the resource id, if resource_type equals project resource_id equals project_name, else resource_id equals project_name + # + subResourceId
+
+        :return: LogResponse
+
+        :raise: LogException
+        """
+        project_name = None
+        if resource_type.lower() == "project":
+            project_name = resource_id
+        else:
+            position = resource_id.find("#")
+            if position != -1:
+                project_name = resource_id[:position]
+        resource = "/tag"
+        body = {
+            'resourceType': resource_type,
+            'resourceId': [resource_id],
+            'tags': [{'key': str(k), 'value': str(v)} for k, v in tags.items()],
+        }
+        body = json.dumps(body).encode()
+        resp, header = self._send("POST", project_name, body, resource, {}, {})
+        return LogResponse(header, resp)
+
+    def untag_resources(self, resource_type, resource_id, *tag_keys):
+        """ untag resources
+        Unsuccessful operation will cause an LogException.
+
+        :type resource_type: string
+        :param resource_type: the resource type, currently only support project, logstore, dashboard, machine_group, logtail_config
+
+        :type resource_id: string
+        :param resource_id: the resource id, if resource_type equals project resource_id equals project_name, else resource_id equals project_name + # + subResourceId
+
+        :return: LogResponse
+
+        :raise: LogException
+        """
+        project_name = None
+        if resource_type.lower() == "project":
+            project_name = resource_id
+        else:
+            position = resource_id.find("#")
+            if position != -1:
+                project_name = resource_id[:position]
+        resource = "/untag"
+        body = {
+            'resourceType': resource_type,
+            'resourceId': [resource_id],
+            'tags': tag_keys,
+        }
+        body = json.dumps(body).encode()
+        resp, header = self._send("POST", project_name, body, resource, {}, {})
+        return LogResponse(header, resp)
+
+    def list_tag_resources(self, resource_type, resource_id, **filer_tags):
+        """ list resource tags
+        Unsuccessful operation will cause an LogException.
+
+        :type resource_type: string
+        :param resource_type: the resource type, currently only support project, logstore, dashboard, machine_group, logtail_config
+
+        :type resource_id: string
+        :param resource_id: the resource id, if resource_type equals project resource_id equals project_name, else resource_id equals project_name + # + subResourceId
+
+        :return: LogResponse
+
+        :raise: LogException
+        """
+        resource = "/tags"
+        filer_tags = [{"key": str(k), "value": str(v)} for k, v in filer_tags.items()]
+        params = {
+            'resourceType': resource_type,
+            'tags': json.dumps(filer_tags),
+            'nextToken': "",
+        }
+        project_name = None
+        if resource_id is not None and resource_id != "":
+            params['resourceId'] = json.dumps([resource_id])
+            if resource_type.lower() == "project":
+                project_name = resource_id
+            else:
+                position = resource_id.find("#")
+                if position != -1:
+                    project_name = resource_id[:position]
+        while True:
+            resp, header = self._send("GET", project_name, None, resource, params, {})
+            resp = GetResourceTagsResponse(header, resp)
+            yield resp
+
+            if resp.next_token == "":
+                break
+            params["nextToken"] = resp.next_token
+
+
     def create_consumer_group(self, project, logstore, consumer_group, timeout, in_order=False):
         """ create consumer group
 
         :type project: string
         :param project: project name
 
         :type logstore: string
@@ -2685,27 +2816,30 @@
         :type to_region_endpoint: string
         :param to_region_endpoint: target region, use it to operate on the "to_project" while "to_client" not be specified
 
         :return:
         """
         return copy_logstore(self, from_project, from_logstore, to_logstore, to_project=to_project, to_client=to_client, to_region_endpoint=to_region_endpoint)
 
-    def list_project(self, offset=0, size=100, project_name_pattern=None):
+    def list_project(self, offset=0, size=100, project_name_pattern=None, resource_group_id=''):
         """ list the project
         Unsuccessful operation will cause an LogException.
 
         :type project_name_pattern: string
         :param project_name_pattern: the sub name project, used for the server to return project names contain this sub name
 
         :type offset: int
         :param offset: the offset of all the matched names
 
         :type size: int
         :param size: the max return names count, -1 means return all data
 
+        :type resource_group_id: string
+        :param resource_group_id: the resource group id, used for the server to return project in resource group
+
         :return: ListProjectResponse
 
         :raise: LogException
         """
 
         # need to use extended method to get more
         if int(size) == -1 or int(size) > MAX_LIST_PAGING_SIZE:
@@ -2714,14 +2848,15 @@
         headers = {}
         params = {}
         resource = "/"
         if project_name_pattern is not None:
             params['projectName'] = project_name_pattern
         params['offset'] = str(offset)
         params['size'] = str(size)
+        params['resourceGroupId'] = resource_group_id
         (resp, header) = self._send("GET", None, None, resource, params, headers)
         return ListProjectResponse(resp, header)
 
     def es_migration(
             self,
             cache_path,
             hosts,
```

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_core.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logclient_core.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_operator.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logclient_operator.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logexception.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logexception.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logger_hanlder.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logger_hanlder.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logitem.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logitem.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logrequest.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logstore_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logstore_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_detail.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logtail_config_detail.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/logtail_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/machine_group_detail.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/machine_group_detail.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/machinegroup_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/machinegroup_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/odps_sink.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/odps_sink.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/oss_sink.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/oss_sink.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/pluralize.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/pluralize.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/project_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/project_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self.status = resp['status']
         self.description = resp['description']
         self.projectName = resp['projectName']
         self.region = resp['region']
         self.owner = resp['owner']
         self.createTime = resp['createTime']
         self.lastModifyTime = resp['lastModifyTime']
+        self.resourceGroupId = resp['resourceGroupId']
 
     def get_owner(self):
         return self.owner
 
     def get_status(self):
         return self.status
 
@@ -64,25 +65,28 @@
 
     def get_create_time(self):
         return self.createTime
 
     def get_last_modify_time(self):
         return self.lastModifyTime
 
+    def get_resource_group_id(self):
+        return self.resourceGroupId
+
     def log_print(self):
         print('GetProjectResponse:')
         print('headers:', self.get_all_headers())
         print('owner:' + self.get_owner())
         print('project:' + self.get_projectname())
         print('description:' + self.get_description())
         print('region:' + self.get_region())
         print('status:' + self.get_status())
         print('create_time:' + self.get_create_time())
         print('last_modify_time:' + self.get_last_modify_time())
-
+        print('resource_group_id:' + self.get_resource_group_id())
 
 class ListProjectResponse(LogResponse):
     def __init__(self, resp, header):
         LogResponse.__init__(self, header, resp)
         self.count = int(resp['count'])
         self.total = int(resp['total'])
         self.projects = Util.convert_unicode_to_str(resp.get("projects", []))
```

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/pulllog_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/pulllog_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsrequest.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/putlogsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsresponse.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/putlogsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/queriedlog.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/queriedlog.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/resource_params.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/resource_params.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/resource_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/resource_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/shard_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/shard_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_config.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/shipper_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/shipper_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/sql_instance_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/sql_instance_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/substore_config_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/substore_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_params.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/topostore_params.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_response.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/topostore_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun/log/util.py` & `aliyun-log-python-sdk-0.8.8/aliyun/log/util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/PKG-INFO` & `aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-log-python-sdk
-Version: 0.8.7
+Version: 0.8.8
 Summary: Aliyun log service Python client SDK
 Home-page: https://github.com/aliyun/aliyun-log-python-sdk
 Author: Aliyun
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: 
         Python SDK for Alicloud Log Service
```

### Comparing `aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/SOURCES.txt` & `aliyun-log-python-sdk-0.8.8/aliyun_log_python_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 aliyun/log/resource_response.py
 aliyun/log/shard_response.py
 aliyun/log/shipper_config.py
 aliyun/log/shipper_response.py
 aliyun/log/sink.py
 aliyun/log/sql_instance_response.py
 aliyun/log/substore_config_response.py
+aliyun/log/tag_response.py
 aliyun/log/topostore_params.py
 aliyun/log/topostore_response.py
 aliyun/log/util.py
 aliyun/log/version.py
 aliyun/log/consumer/__init__.py
 aliyun/log/consumer/checkpoint_tracker.py
 aliyun/log/consumer/config.py
```

### Comparing `aliyun-log-python-sdk-0.8.7/setup.py` & `aliyun-log-python-sdk-0.8.8/setup.py`

 * *Files identical despite different names*

