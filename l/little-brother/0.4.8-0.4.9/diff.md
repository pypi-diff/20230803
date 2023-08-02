# Comparing `tmp/little-brother-0.4.8.tar.gz` & `tmp/little-brother-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "little-brother-0.4.8.tar", last modified: Fri Aug 27 19:04:53 2021, max compression
+gzip compressed data, was "little-brother-0.4.9.tar", last modified: Fri Sep 17 21:16:28 2021, max compression
```

## Comparing `little-brother-0.4.8.tar` & `little-brother-0.4.9.tar`

### file list

```diff
@@ -1,250 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.481934 little-brother-0.4.8/
--rw-r--r--   0 root         (0) root         (0)     1752 2021-08-27 19:04:51.000000 little-brother-0.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      470 2021-08-27 19:04:53.481934 little-brother-0.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25733 2021-08-27 19:04:51.000000 little-brother-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.461933 little-brother-0.4.8/little_brother/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14644 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/admin_data_handler.py
--rw-r--r--   0 root         (0) root         (0)     3808 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/admin_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.461933 little-brother-0.4.8/little_brother/alembic/
--rw-r--r--   0 root         (0) root         (0)     3060 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.461933 little-brother-0.4.8/little_brother/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      953 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/0a5c7b6ad27a_fb_issue_124.py
--rw-r--r--   0 root         (0) root         (0)      708 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/2f458b3a313e_add_max_activity_duration.py
--rw-r--r--   0 root         (0) root         (0)     2495 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/647cf46033a9_initial_db_model_at_488c798.py
--rw-r--r--   0 root         (0) root         (0)      849 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/96ff8f93ef32_add_downtime_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1498 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/9713cef84918_userstatus_issue_130.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      725 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/e0c0d7048235_prohibited_process_name_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4420 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic/versions/version_0_3_added_tables_for_configuration_gui.py
--rw-r--r--   0 root         (0) root         (0)     1764 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.461933 little-brother-0.4.8/little_brother/api/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15217 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/api/api_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     5072 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/api/master_connector.py
--rw-r--r--   0 root         (0) root         (0)    20223 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/app.py
--rw-r--r--   0 root         (0) root         (0)    28714 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/app_control.py
--rw-r--r--   0 root         (0) root         (0)     3468 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/app_control_config_model.py
--rw-r--r--   0 root         (0) root         (0)    13155 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/client_device_handler.py
--rw-r--r--   0 root         (0) root         (0)     3269 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/client_info.py
--rw-r--r--   0 root         (0) root         (0)     9485 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/client_process_handler.py
--rw-r--r--   0 root         (0) root         (0)     1571 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/client_stats.py
--rw-r--r--   0 root         (0) root         (0)     4206 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/constants.py
--rw-r--r--   0 root         (0) root         (0)     2088 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/context_rule_handler.py
--rw-r--r--   0 root         (0) root         (0)     5914 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/db_migrations.py
--rw-r--r--   0 root         (0) root         (0)      115 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/dependency_injection.py
--rw-r--r--   0 root         (0) root         (0)     5509 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/entity_forms.py
--rw-r--r--   0 root         (0) root         (0)     6117 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/event_handler.py
--rw-r--r--   0 root         (0) root         (0)     9239 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/german_vacation_context_rule_handler.py
--rw-r--r--   0 root         (0) root         (0)     1277 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/git.py
--rw-r--r--   0 root         (0) root         (0)      146 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/git_metadata.py
--rw-r--r--   0 root         (0) root         (0)     6556 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/language.py
--rw-r--r--   0 root         (0) root         (0)     5738 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/login_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/persistence/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1155 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/base_entity.py
--rw-r--r--   0 root         (0) root         (0)     1794 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/base_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)    12235 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistence.py
--rw-r--r--   0 root         (0) root         (0)     1228 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistence_base.py
--rw-r--r--   0 root         (0) root         (0)     1457 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_admin_event.py
--rw-r--r--   0 root         (0) root         (0)     2084 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_admin_event_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     2134 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_daily_user_status.py
--rw-r--r--   0 root         (0) root         (0)     2570 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_daily_user_status_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     5276 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_dependency_injection_mix_in.py
--rw-r--r--   0 root         (0) root         (0)     3029 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_device.py
--rw-r--r--   0 root         (0) root         (0)     4261 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_device_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     2033 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_process_info.py
--rw-r--r--   0 root         (0) root         (0)     3924 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_process_info_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1985 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_rule_override.py
--rw-r--r--   0 root         (0) root         (0)     3717 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_rule_override_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     4582 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_rule_set.py
--rw-r--r--   0 root         (0) root         (0)     3550 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_rule_set_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1640 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_time_extension.py
--rw-r--r--   0 root         (0) root         (0)     5211 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_time_extension_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     7162 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_user.py
--rw-r--r--   0 root         (0) root         (0)     2885 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_user_2_device.py
--rw-r--r--   0 root         (0) root         (0)     4094 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_user_2_device_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     4955 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/persistent_user_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     2398 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/persistence/session_context.py
--rw-r--r--   0 root         (0) root         (0)     7550 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/process_handler.py
--rw-r--r--   0 root         (0) root         (0)    21532 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/process_handler_manager.py
--rw-r--r--   0 root         (0) root         (0)     2873 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/process_info.py
--rw-r--r--   0 root         (0) root         (0)    15434 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/process_statistics.py
--rw-r--r--   0 root         (0) root         (0)     9062 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/prometheus.py
--rw-r--r--   0 root         (0) root         (0)    21988 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/rule_handler.py
--rw-r--r--   0 root         (0) root         (0)     3257 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/rule_override.py
--rw-r--r--   0 root         (0) root         (0)     8323 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/rule_result_info.py
--rw-r--r--   0 root         (0) root         (0)     1408 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/settings.py
--rw-r--r--   0 root         (0) root         (0)     4154 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/simple_context_rule_handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/static/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/static/contrib/fontawesome/
--rw-r--r--   0 root         (0) root         (0)     1548 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/static/contrib/fontawesome/css/
--rw-r--r--   0 root         (0) root         (0)    58935 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/css/all.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/static/contrib/fontawesome/js/
--rw-r--r--   0 root         (0) root         (0)  1182553 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/js/all.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.465934 little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/
--rw-r--r--   0 root         (0) root         (0)   740737 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 root         (0) root         (0)   148309 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 root         (0) root         (0)   935897 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-solid-900.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/static/contrib/initializr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.469934 little-brother-0.4.8/little_brother/static/contrib/initializr/css/
--rw-r--r--   0 root         (0) root         (0)    22474 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap-theme.css
--rw-r--r--   0 root         (0) root         (0)    19835 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap-theme.min.css
--rw-r--r--   0 root         (0) root         (0)   137067 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap.css
--rw-r--r--   0 root         (0) root         (0)   113498 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)      204 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/static/contrib/initializr/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.469934 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/
--rw-r--r--   0 root         (0) root         (0)    67155 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/bootstrap.js
--rw-r--r--   0 root         (0) root         (0)    35602 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)    95931 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/jquery-1.11.2.min.js
--rw-r--r--   0 root         (0) root         (0)    20106 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js
--rw-r--r--   0 root         (0) root         (0)      484 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/npm.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.469934 little-brother-0.4.8/little_brother/static/contrib/js-cookie/
--rw-r--r--   0 root         (0) root         (0)     3885 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/contrib/js-cookie/js-cookie.js
--rw-r--r--   0 root         (0) root         (0)     7380 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/default.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.473934 little-brother-0.4.8/little_brother/static/icons/
--rw-r--r--   0 root         (0) root         (0)     4286 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/baby-panda-32x32.ico
--rw-r--r--   0 root         (0) root         (0)    37193 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/baby-panda-sad-128x128.png
--rw-r--r--   0 root         (0) root         (0)    26465 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/baby-panda-sad-256x256.png
--rw-r--r--   0 root         (0) root         (0)    19721 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/baby-panda.png
--rw-r--r--   0 root         (0) root         (0)     6295 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/docker-logo-128x128.png
--rw-r--r--   0 root         (0) root         (0)    18438 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/icon-baby-panda-128x128.png
--rw-r--r--   0 root         (0) root         (0)     7914 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/icons/icon-baby-panda-32x32.png
--rw-r--r--   0 root         (0) root         (0)      930 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/static/login.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.473934 little-brother-0.4.8/little_brother/templates/
--rw-r--r--   0 root         (0) root         (0)     4920 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/about.template.html
--rw-r--r--   0 root         (0) root         (0)    14698 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/admin.template.html
--rw-r--r--   0 root         (0) root         (0)     3299 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/bootstrap_accordion.macros.html
--rw-r--r--   0 root         (0) root         (0)     6909 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/devices.template.html
--rw-r--r--   0 root         (0) root         (0)     3835 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/helper.macros.html
--rw-r--r--   0 root         (0) root         (0)     3102 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/internal_error.template.html
--rw-r--r--   0 root         (0) root         (0)     2975 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/login.template.html
--rw-r--r--   0 root         (0) root         (0)     3667 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/navbar.include.html
--rw-r--r--   0 root         (0) root         (0)    11100 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/status.template.html
--rw-r--r--   0 root         (0) root         (0)     4320 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/topology.template.html
--rw-r--r--   0 root         (0) root         (0)    19365 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/templates/users.template.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.473934 little-brother-0.4.8/little_brother/test/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/dummy_process_handler.py
--rw-r--r--   0 root         (0) root         (0)     2254 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/dummy_process_iterator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/test/persistence/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2686 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/base_test_case_persistent_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     5759 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistence.py
--rw-r--r--   0 root         (0) root         (0)     2740 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_admin_event_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1512 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_daily_user_status_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1474 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_device_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     4106 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_process_info_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     4729 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_rule_override_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1479 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_rule_set_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     4435 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_time_extension_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1496 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_user_2_device_entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     1466 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_persistent_user_entity_manager.py
--rwxr-xr-x   0 root         (0) root         (0)     4098 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/persistence/test_suite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/test/resources/
--rw-r--r--   0 root         (0) root         (0)     1929 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/resources/app.config
--rw-r--r--   0 root         (0) root         (0)     3885 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/resources/ruleset_handler.test.config
--rw-r--r--   0 root         (0) root         (0)     4107 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_app.py
--rw-r--r--   0 root         (0) root         (0)     6140 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_app_control.py
--rw-r--r--   0 root         (0) root         (0)     5382 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_client_device_handler.py
--rw-r--r--   0 root         (0) root         (0)    16016 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_client_process_handler.py
--rw-r--r--   0 root         (0) root         (0)     5914 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_data.py
--rw-r--r--   0 root         (0) root         (0)     4149 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_german_vacation_context_rule_handler.py
--rw-r--r--   0 root         (0) root         (0)     5113 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_language.py
--rw-r--r--   0 root         (0) root         (0)    17650 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_process_handler.py
--rw-r--r--   0 root         (0) root         (0)     8217 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_process_handler_manager.py
--rw-r--r--   0 root         (0) root         (0)     1703 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_process_info.py
--rw-r--r--   0 root         (0) root         (0)    12602 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_process_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1908 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_prometheus.py
--rw-r--r--   0 root         (0) root         (0)    35682 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_rule_handler.py
--rw-r--r--   0 root         (0) root         (0)     4814 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_simple_weekday_context_rule_handler.py
--rwxr-xr-x   0 root         (0) root         (0)     5739 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_suite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/test_user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/test/web/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10111 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/base_test_status_server.py
--rw-r--r--   0 root         (0) root         (0)     1363 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server.py
--rw-r--r--   0 root         (0) root         (0)     2016 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_about.py
--rw-r--r--   0 root         (0) root         (0)    16406 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_admin.py
--rw-r--r--   0 root         (0) root         (0)     8718 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_devices.py
--rw-r--r--   0 root         (0) root         (0)     2953 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_index.py
--rw-r--r--   0 root         (0) root         (0)     2323 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_topology.py
--rw-r--r--   0 root         (0) root         (0)    14868 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_status_server_users.py
--rwxr-xr-x   0 root         (0) root         (0)     3392 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/test/web/test_suite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/bn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/bn/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     8733 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/bn/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/da/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5639 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/da/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11257 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/de/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5970 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/es/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/fi/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     6121 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/fi/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    10394 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/fr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.453934 little-brother-0.4.8/little_brother/translations/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/hr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5850 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/hr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/hu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/hu/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      436 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/hu/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/it/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11691 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/it/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/ja/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     6271 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/ja/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/lt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/lt/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      506 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/lt/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/nl/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5652 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/nl/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/ru/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     7937 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/ru/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/sr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/sr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      517 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/sr/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/th/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/th/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     8285 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/th/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.457934 little-brother-0.4.8/little_brother/translations/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.477934 little-brother-0.4.8/little_brother/translations/tr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     6061 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 root         (0) root         (0)     1586 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/user_locale_handler.py
--rw-r--r--   0 root         (0) root         (0)     7769 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/user_manager.py
--rw-r--r--   0 root         (0) root         (0)     1457 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/user_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.481934 little-brother-0.4.8/little_brother/web/
--rw-r--r--   0 root         (0) root         (0)        0 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/about_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     5463 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/admin_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     5553 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/base_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     5764 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/devices_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     2097 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/login_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     3420 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/status_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     2939 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/topology_view_handler.py
--rw-r--r--   0 root         (0) root         (0)    12108 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/users_view_handler.py
--rw-r--r--   0 root         (0) root         (0)     9267 2021-08-27 19:04:52.000000 little-brother-0.4.8/little_brother/web/web_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 19:04:53.461933 little-brother-0.4.8/little_brother.egg-info/
--rw-r--r--   0 root         (0) root         (0)      470 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9235 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-08-27 19:04:53.000000 little-brother-0.4.8/little_brother.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      315 2021-08-27 19:04:52.000000 little-brother-0.4.8/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      991 2021-08-27 19:04:52.000000 little-brother-0.4.8/run_little_brother.py
--rwxr-xr-x   0 root         (0) root         (0)     1008 2021-08-27 19:04:52.000000 little-brother-0.4.8/run_little_brother_test_suite.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-27 19:04:53.481934 little-brother-0.4.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3783 2021-08-27 19:04:52.000000 little-brother-0.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.689494 little-brother-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)     1752 2021-09-17 21:16:26.000000 little-brother-0.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      470 2021-09-17 21:16:28.689494 little-brother-0.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26183 2021-09-17 21:16:26.000000 little-brother-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.669494 little-brother-0.4.9/little_brother/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15746 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/admin_data_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/admin_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.669494 little-brother-0.4.9/little_brother/alembic/
+-rw-r--r--   0 root         (0) root         (0)     3060 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.669494 little-brother-0.4.9/little_brother/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      953 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/0a5c7b6ad27a_fb_issue_124.py
+-rw-r--r--   0 root         (0) root         (0)      708 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/2f458b3a313e_add_max_activity_duration.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/647cf46033a9_initial_db_model_at_488c798.py
+-rw-r--r--   0 root         (0) root         (0)      849 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/96ff8f93ef32_add_downtime_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/9713cef84918_userstatus_issue_130.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      725 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/e0c0d7048235_prohibited_process_name_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic/versions/version_0_3_added_tables_for_configuration_gui.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/api/api_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/api/master_connector.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/api/version_checker.py
+-rw-r--r--   0 root         (0) root         (0)    20833 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/app.py
+-rw-r--r--   0 root         (0) root         (0)    28051 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/app_control.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2021-09-17 21:16:26.000000 little-brother-0.4.9/little_brother/app_control_config_model.py
+-rw-r--r--   0 root         (0) root         (0)    13155 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/client_device_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/client_info.py
+-rw-r--r--   0 root         (0) root         (0)     9883 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/client_process_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/client_stats.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/context_rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5914 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/db_migrations.py
+-rw-r--r--   0 root         (0) root         (0)      115 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/dependency_injection.py
+-rw-r--r--   0 root         (0) root         (0)     5509 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/entity_forms.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9239 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/german_vacation_context_rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/git.py
+-rw-r--r--   0 root         (0) root         (0)      146 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/git_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/language.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/login_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/persistence/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/base_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/base_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)    12235 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistence.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistence_base.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_admin_event.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_admin_event_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_daily_user_status.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_daily_user_status_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_dependency_injection_mix_in.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_device.py
+-rw-r--r--   0 root         (0) root         (0)     4261 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_device_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_process_info.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_process_info_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_rule_override.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_rule_override_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_rule_set.py
+-rw-r--r--   0 root         (0) root         (0)     3550 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_rule_set_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_time_extension.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_time_extension_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_user.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_user_2_device.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_user_2_device_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/persistent_user_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/persistence/session_context.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/process_handler.py
+-rw-r--r--   0 root         (0) root         (0)    21597 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/process_handler_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/process_info.py
+-rw-r--r--   0 root         (0) root         (0)    15434 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/process_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/prometheus.py
+-rw-r--r--   0 root         (0) root         (0)    21988 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/rule_override.py
+-rw-r--r--   0 root         (0) root         (0)     8323 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/rule_result_info.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/settings.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/simple_context_rule_handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/static/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/static/contrib/fontawesome/
+-rw-r--r--   0 root         (0) root         (0)     1548 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/static/contrib/fontawesome/css/
+-rw-r--r--   0 root         (0) root         (0)    58935 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/css/all.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.673494 little-brother-0.4.9/little_brother/static/contrib/fontawesome/js/
+-rw-r--r--   0 root         (0) root         (0)  1182553 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/js/all.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.677494 little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/
+-rw-r--r--   0 root         (0) root         (0)   740737 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 root         (0) root         (0)   148309 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 root         (0) root         (0)   935897 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-solid-900.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/static/contrib/initializr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.677494 little-brother-0.4.9/little_brother/static/contrib/initializr/css/
+-rw-r--r--   0 root         (0) root         (0)    22474 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap-theme.css
+-rw-r--r--   0 root         (0) root         (0)    19835 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap-theme.min.css
+-rw-r--r--   0 root         (0) root         (0)   137067 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap.css
+-rw-r--r--   0 root         (0) root         (0)   113498 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)      204 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/static/contrib/initializr/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.677494 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/
+-rw-r--r--   0 root         (0) root         (0)    67155 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/bootstrap.js
+-rw-r--r--   0 root         (0) root         (0)    35602 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)    95931 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/jquery-1.11.2.min.js
+-rw-r--r--   0 root         (0) root         (0)    20106 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js
+-rw-r--r--   0 root         (0) root         (0)      484 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/npm.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.677494 little-brother-0.4.9/little_brother/static/contrib/js-cookie/
+-rw-r--r--   0 root         (0) root         (0)     3885 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/contrib/js-cookie/js-cookie.js
+-rw-r--r--   0 root         (0) root         (0)     7380 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/default.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.677494 little-brother-0.4.9/little_brother/static/icons/
+-rw-r--r--   0 root         (0) root         (0)     4286 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/baby-panda-32x32.ico
+-rw-r--r--   0 root         (0) root         (0)    37193 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/baby-panda-sad-128x128.png
+-rw-r--r--   0 root         (0) root         (0)    26465 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/baby-panda-sad-256x256.png
+-rw-r--r--   0 root         (0) root         (0)    19721 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/baby-panda.png
+-rw-r--r--   0 root         (0) root         (0)     6295 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/docker-logo-128x128.png
+-rw-r--r--   0 root         (0) root         (0)    18438 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/icon-baby-panda-128x128.png
+-rw-r--r--   0 root         (0) root         (0)     7914 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/icons/icon-baby-panda-32x32.png
+-rw-r--r--   0 root         (0) root         (0)      930 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/static/login.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.681494 little-brother-0.4.9/little_brother/templates/
+-rw-r--r--   0 root         (0) root         (0)     4898 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/about.template.html
+-rw-r--r--   0 root         (0) root         (0)    14625 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/admin.template.html
+-rw-r--r--   0 root         (0) root         (0)     3309 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/bootstrap_accordion.macros.html
+-rw-r--r--   0 root         (0) root         (0)     6990 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/devices.template.html
+-rw-r--r--   0 root         (0) root         (0)     3839 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/helper.macros.html
+-rw-r--r--   0 root         (0) root         (0)     3106 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/internal_error.template.html
+-rw-r--r--   0 root         (0) root         (0)     2761 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/login.template.html
+-rw-r--r--   0 root         (0) root         (0)     3607 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/navbar.include.html
+-rw-r--r--   0 root         (0) root         (0)    11116 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/status.template.html
+-rw-r--r--   0 root         (0) root         (0)     4510 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/topology.template.html
+-rw-r--r--   0 root         (0) root         (0)    19447 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/users.template.html
+-rw-r--r--   0 root         (0) root         (0)     1325 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/templates/version_check.include.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.681494 little-brother-0.4.9/little_brother/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/dummy_process_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/dummy_process_iterator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/test/persistence/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/base_test_case_persistent_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistence.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_admin_event_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_daily_user_status_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_device_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4106 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_process_info_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4729 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_rule_override_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_rule_set_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_time_extension_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_user_2_device_entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_persistent_user_entity_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)     4098 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/persistence/test_suite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/test/resources/
+-rw-r--r--   0 root         (0) root         (0)     1929 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/resources/app.config
+-rw-r--r--   0 root         (0) root         (0)     3885 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/resources/ruleset_handler.test.config
+-rw-r--r--   0 root         (0) root         (0)     4107 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_app.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_app_control.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_client_device_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_client_info.py
+-rw-r--r--   0 root         (0) root         (0)    21084 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_client_process_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5914 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_german_vacation_context_rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_language.py
+-rw-r--r--   0 root         (0) root         (0)    17650 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_process_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8217 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_process_handler_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_process_info.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_process_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_prometheus.py
+-rw-r--r--   0 root         (0) root         (0)    35686 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_rule_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_simple_weekday_context_rule_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     5927 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_suite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/test_user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/test/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10755 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/base_test_status_server.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_about.py
+-rw-r--r--   0 root         (0) root         (0)    16406 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_admin.py
+-rw-r--r--   0 root         (0) root         (0)     7954 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_index.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_topology.py
+-rw-r--r--   0 root         (0) root         (0)    14857 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_status_server_users.py
+-rwxr-xr-x   0 root         (0) root         (0)     3392 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/test/web/test_suite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/bn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/bn/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     8733 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/bn/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/da/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5639 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/da/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11954 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/de/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5970 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/es/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/fi/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     6121 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/fi/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    10394 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/fr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5850 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/hr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/hu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      436 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/hu/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/it/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11691 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/it/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     6271 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/ja/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/lt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      506 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/lt/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5652 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/nl/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     7937 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/ru/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/sr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/sr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      517 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/sr/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/th/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/th/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     8285 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/th/LC_MESSAGES/messages.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.665494 little-brother-0.4.9/little_brother/translations/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.685494 little-brother-0.4.9/little_brother/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     6061 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 root         (0) root         (0)     1586 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/user_locale_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7769 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/user_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/user_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.689494 little-brother-0.4.9/little_brother/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/about_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/admin_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7247 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/base_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5779 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/devices_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/login_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/status_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/topology_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12919 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/users_view_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2021-09-17 21:16:27.000000 little-brother-0.4.9/little_brother/web/web_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-17 21:16:28.669494 little-brother-0.4.9/little_brother.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      470 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9365 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      346 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-09-17 21:16:28.000000 little-brother-0.4.9/little_brother.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      411 2021-09-17 21:16:27.000000 little-brother-0.4.9/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      991 2021-09-17 21:16:27.000000 little-brother-0.4.9/run_little_brother.py
+-rwxr-xr-x   0 root         (0) root         (0)     1008 2021-09-17 21:16:27.000000 little-brother-0.4.9/run_little_brother_test_suite.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-09-17 21:16:28.689494 little-brother-0.4.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3919 2021-09-17 21:16:27.000000 little-brother-0.4.9/setup.py
```

### Comparing `little-brother-0.4.8/MANIFEST.in` & `little-brother-0.4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/README.md` & `little-brother-0.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 
 # Parental Control Application `LittleBrother`
 
 ## Overview
 
 `LittleBrother` is a simple parental control application monitoring specific processes (read "games") on Linux hosts
 to monitor and limit the play time of (young) children. It is designed as a client server application running
-on several hosts and combining playing time spent across these hosts but it also works on a standalone host.
+on several hosts and combining playing time spent across these hosts, but it also works on a standalone host.
 
-When the application determines that a user has exceeded her play time it will terminate the configured 
+When the application determines that a user has exceeded her play time, it will terminate the configured 
 process. Usually, the user will get several spoken notifications (using the 
 [LittleBrotherTaskbar](https://github.com/marcus67/little_brother_taskbar)) before she is actually kicked out so 
 that she can log out gracefully in time.
 
 ## What's New?
 
 The latest major feature changes are:
 
-| Version  | Feature/Fix                                                | Issue Link                                                         |
-|----------|------------------------------------------------------------|--------------------------------------------------------------------|
-| 0.4.8    | *New*: Full support for requesting optional time by users  | [Issue 130](https://github.com/marcus67/little_brother/issues/130) |
-| 0.4.4    | *New*: Use user specific patterns to prohibit applications | [Issue 129](https://github.com/marcus67/little_brother/issues/129) |
+| Version  | Feature/Fix                                                   | Issue Link                                                         |
+|----------|---------------------------------------------------------------|--------------------------------------------------------------------|
+| 0.4.9    | *New*: Automatic check for new versions of `LittleBrother`    | [Issue 150](https://github.com/marcus67/little_brother/issues/150) |
+|          | *Improvement*: Separate LDAP search DN for groups and users   | [Issue 144](https://github.com/marcus67/little_brother/issues/144) |
+|          | *Improvement*: Cache timeout for LDAP data                    | [Issue 138](https://github.com/marcus67/little_brother/issues/138) |
+| 0.4.8    | *New*: Full support for requesting optional time by users     | [Issue 130](https://github.com/marcus67/little_brother/issues/130) |
+| 0.4.4    | *New*: Use user specific patterns to prohibit applications    | [Issue 129](https://github.com/marcus67/little_brother/issues/129) |
 
 ## Contact
 
 Visit the project at [Facebook](https://www.facebook.com/littlebrotherdebian) or write comments 
 to little-brother(at)web.de.
 
 ## Screenshots
@@ -109,37 +112,37 @@
 
 *   The application has international language support. Currently English, Italian and German translations are provided.
 Users are invited to provide translations for other languages.
 
 *   Downtime of a server during playtime (e.g. due to hibernation) is automatically subtracted from the play time.
 
 *   In addition to the time spent on Linux hosts the application can also monitor activity time on other devices 
-such as smart phones or tables. It takes advantage of the fact that most modern operating systems put devices
+such as smartphones or tables. It takes advantage of the fact that most modern operating systems put devices
 in some kind of power saving mode while they are not being used. This way, the network response (by `pinging`) can
 be used to determine the activity on those devices. In contrast to the Linux hosts, the application
-will not be able the terminate the activity. The play time, however, will be added to the overall playtime and
+will not be able to terminate the activity. The play time, however, will be added to the overall playtime and
 hence will have an impact on the time allowed and also on the break time rules on the Linux hosts.
 
 *   As of version 0.3.12 `LittleBrother` is able to use [ProxyPing](https://github.com/marcus67/proxy_ping) to ping
 devices behind firewalls provided the tool can be deployed on a Debian server behind the firewall.
 
 *   As of version 0.3.13 `LittleBrother` slaves will terminate local user sessions if they cannot reach the master
 process for a certain time (defaults to 50 seconds). This ensures users cannot suppress being logged out by 
 *pulling the plug*.
 
 *   As of version 0.4.0 `LittleBrother` provides an administration feature to easily extend the current computer time 
-or grant computer when the usage would normally be prohibited. This is called a time extension. During a active 
+or grant computer when the usage would normally be prohibited. This is called a time extension. During an active 
 extension all other restrictions (maximum time per session, time of day, and maximum time per day) are deactivated.
 Time extension can even extend into the next day making long night session possible. However, any computer time
 actually spent during a time extension will contribute to the overall time played in the course of a day.   
 
 *   There is a Docker image available (currently for the slave only) which makes it really easy to run a slave on a 
 Linux host with a Docker daemon available.
 
-*   The application uses voice generation to inform the user over impending logouts. Also these spoken
+*   The application uses voice generation to inform the user over impending logouts. Also, these spoken
 messages are internationalized. Optionally, users can be notified using four different popup tools. Note that this
 functionality of the `LittleBrother` application has been replaced by the `LittleBrotherTaskbar.` 
 
 ## Architecture
 
 The [page](ARCHITECTURE.md) gives a detailed description of the architecture of the application.    
 
@@ -234,41 +237,41 @@
 ### Using the Web-Frontend
 
 You are all set now. It's time to set up users to be monitored and optionally devices. See the 
 [Web Frontend Manual](WEB_FRONTEND_MANUAL.md). 
 
 ### Troubleshooting
 
-So, you went through all of the above but LittleBrother does not seem to work? Maybe this 
+So, you went through all the above but LittleBrother does not seem to work? Maybe this 
 [troubleshooting page](TROUBLESHOOTING.md) can help you.
 
 ## Caveats
 
 The application `LittleBrother` is far from perfect. Some major caveats are listed here and/or in the 
 issue list on GitHub (see [here](../issues)).
 
 *   Every once in a while processes fail to terminate even though they have been killed by `LittleBrother`. 
 In these cases the user will still be regarded as logged in although he/she is not. Usually this can only be
 solved by trying to kill the processes again using the master user. Database eloquent users may try to 
 delete/correct the incorrect process time entries.
 
 *   The web server only responds to HTTP requests. This is probably always OK for communication between the
-slaves and the master in local area network. If the master host is to be accessible from the internet it should
+slaves and the master in local area network. If the master host is to be accessible from the internet, it should
 be put behind a reverse proxy handling the HTTPS termination (see below). 
 
 ## Internationalization
 
 The application uses the PIP package `Flask-Babel` to provide internationalization for the web frontend. Currently, 
 the following languages are supported or currently in preparation (in the order they were made available):
 
 | Flag                                                           | Language      | Locale | Status         | Translation provided by    |
 | ---------------------------------------------------------------| ------------- | ------ | -------------- | ---------------------------|
 | ![Flag USA](doc/united-states-of-america-flag-icon-32.png)     | English       | en     | Up-to-date     |  Marcus Rickert            |
 | ![Flag Germany](doc/germany-flag-icon-32.png)                  | German        | de     | Up-to-date     |  Marcus Rickert            |
-| ![Flag Italy](doc/italy-flag-icon-32.png)                      | Italian       | it     | Up-to-date     |  Albano Battistella        |
+| ![Flag Italy](doc/italy-flag-icon-32.png)                      | Italian       | it     | Revision 107   |  Albano Battistella        |
 | ![Flag Netherlands](doc/netherlands-flag-icon-32.png)          | Dutch         | nl     | Revision 63    |  Simone & Lex              |
 | ![Flag Finland](doc/finland-flag-icon-32.png)                  | Finnish       | fi     | Revision 63    |  Isakkii Kosonen           |
 | ![Flag France](doc/france-flag-icon-32.png)                    | French        | fr     | Revision 86    |  Albano Battistella        |
 | ![Flag Turkey](doc/turkey-flag-icon-32.png)                    | Turkish       | tr     | Revision 63    |  Selay Dogan               |
 | ![Flag Russia](doc/russia-flag-icon-32.png)                    | Russian       | ru     | Revision 63    |  J. Moldawski              |
 | ![Flag Japan](doc/japan-flag-icon-32.png)                      | Japanese      | ja     | Revision 63    |  Arik M.                   |
 | ![Flag Bangladesh](doc/bangladesh-flag-icon-32.png)            | Bangla        | bn     | Revision 63    |  Rownak Jyoti Zaman        |
```

#### html2text {}

```diff
@@ -1,29 +1,34 @@
 ![LittleBrother-Logo](little_brother/static/icons/icon-baby-panda-128x128.png)
 # Parental Control Application `LittleBrother` ## Overview `LittleBrother` is a
 simple parental control application monitoring specific processes (read
 "games") on Linux hosts to monitor and limit the play time of (young) children.
 It is designed as a client server application running on several hosts and
-combining playing time spent across these hosts but it also works on a
+combining playing time spent across these hosts, but it also works on a
 standalone host. When the application determines that a user has exceeded her
-play time it will terminate the configured process. Usually, the user will get
+play time, it will terminate the configured process. Usually, the user will get
 several spoken notifications (using the [LittleBrotherTaskbar](https://
 github.com/marcus67/little_brother_taskbar)) before she is actually kicked out
 so that she can log out gracefully in time. ## What's New? The latest major
 feature changes are: | Version | Feature/Fix | Issue Link | |----------|-------
------------------------------------------------------|-------------------------
--------------------------------------------| | 0.4.8 | *New*: Full support for
-requesting optional time by users | [Issue 130](https://github.com/marcus67/
-little_brother/issues/130) | | 0.4.4 | *New*: Use user specific patterns to
-prohibit applications | [Issue 129](https://github.com/marcus67/little_brother/
-issues/129) | ## Contact Visit the project at [Facebook](https://
-www.facebook.com/littlebrotherdebian) or write comments to little-brother
-(at)web.de. ## Screenshots The following screenshots show the web frontend of
-`LittleBrother`. Click on the thumbnails to enlarge. ![Screenshot_Status](doc/
-screenshot_status.thumb.png) ![Screenshot_Status](doc/
+--------------------------------------------------------|----------------------
+----------------------------------------------| | 0.4.9 | *New*: Automatic
+check for new versions of `LittleBrother` | [Issue 150](https://github.com/
+marcus67/little_brother/issues/150) | | | *Improvement*: Separate LDAP search
+DN for groups and users | [Issue 144](https://github.com/marcus67/
+little_brother/issues/144) | | | *Improvement*: Cache timeout for LDAP data |
+[Issue 138](https://github.com/marcus67/little_brother/issues/138) | | 0.4.8 |
+*New*: Full support for requesting optional time by users | [Issue 130](https:/
+/github.com/marcus67/little_brother/issues/130) | | 0.4.4 | *New*: Use user
+specific patterns to prohibit applications | [Issue 129](https://github.com/
+marcus67/little_brother/issues/129) | ## Contact Visit the project at
+[Facebook](https://www.facebook.com/littlebrotherdebian) or write comments to
+little-brother(at)web.de. ## Screenshots The following screenshots show the web
+frontend of `LittleBrother`. Click on the thumbnails to enlarge. ![Screenshot
+Status](doc/screenshot_status.thumb.png) ![Screenshot_Status](doc/
 screenshot_login.thumb.png) ![Screenshot_Status](doc/
 screenshot_admin.thumb.png) ![Screenshot_Status](doc/
 screenshot_users.thumb.png) ![Screenshot_Status](doc/
 screenshot_devices.thumb.png) ![Screenshot_Status](doc/
 screenshot_topology.thumb.png) ![Screenshot_Status](doc/
 screenshot_about.thumb.png) ## Change History See [here](CHANGES.md) ## GitHub
 Status [https://img.shields.io/github/forks/marcus67/
@@ -74,38 +79,38 @@
 [LittleBrotherTaskbar](https://github.com/marcus67/little_brother_taskbar)) to
 display the remaining playtime of a monitored user and speak the notifications.
 * The application has international language support. Currently English,
 Italian and German translations are provided. Users are invited to provide
 translations for other languages. * Downtime of a server during playtime (e.g.
 due to hibernation) is automatically subtracted from the play time. * In
 addition to the time spent on Linux hosts the application can also monitor
-activity time on other devices such as smart phones or tables. It takes
+activity time on other devices such as smartphones or tables. It takes
 advantage of the fact that most modern operating systems put devices in some
 kind of power saving mode while they are not being used. This way, the network
 response (by `pinging`) can be used to determine the activity on those devices.
-In contrast to the Linux hosts, the application will not be able the terminate
+In contrast to the Linux hosts, the application will not be able to terminate
 the activity. The play time, however, will be added to the overall playtime and
 hence will have an impact on the time allowed and also on the break time rules
 on the Linux hosts. * As of version 0.3.12 `LittleBrother` is able to use
 [ProxyPing](https://github.com/marcus67/proxy_ping) to ping devices behind
 firewalls provided the tool can be deployed on a Debian server behind the
 firewall. * As of version 0.3.13 `LittleBrother` slaves will terminate local
 user sessions if they cannot reach the master process for a certain time
 (defaults to 50 seconds). This ensures users cannot suppress being logged out
 by *pulling the plug*. * As of version 0.4.0 `LittleBrother` provides an
 administration feature to easily extend the current computer time or grant
 computer when the usage would normally be prohibited. This is called a time
-extension. During a active extension all other restrictions (maximum time per
+extension. During an active extension all other restrictions (maximum time per
 session, time of day, and maximum time per day) are deactivated. Time extension
 can even extend into the next day making long night session possible. However,
 any computer time actually spent during a time extension will contribute to the
 overall time played in the course of a day. * There is a Docker image available
 (currently for the slave only) which makes it really easy to run a slave on a
 Linux host with a Docker daemon available. * The application uses voice
-generation to inform the user over impending logouts. Also these spoken
+generation to inform the user over impending logouts. Also, these spoken
 messages are internationalized. Optionally, users can be notified using four
 different popup tools. Note that this functionality of the `LittleBrother`
 application has been replaced by the `LittleBrotherTaskbar.` ## Architecture
 The [page](ARCHITECTURE.md) gives a detailed description of the architecture of
 the application. ## Tested Distributions So far, `LittleBrother` has only been
 released as a Debian package. For other non-Debian based distributions there is
 some basic support using a generic installation script. See [this page](NON-
@@ -182,37 +187,37 @@
 use `sudo`): * Use your favorite editor to edit the file `/etc/little-brother/
 little-brother.conf`. * Find the setting `admin_password` in the section `
 [UnixUserHandler]`. * Change the password. * Save the file. * Restart the
 application by issuing: systemctl restart little-brother From now on the new
 password will have to be used to access the administration pages. ### Using the
 Web-Frontend You are all set now. It's time to set up users to be monitored and
 optionally devices. See the [Web Frontend Manual](WEB_FRONTEND_MANUAL.md). ###
-Troubleshooting So, you went through all of the above but LittleBrother does
-not seem to work? Maybe this [troubleshooting page](TROUBLESHOOTING.md) can
-help you. ## Caveats The application `LittleBrother` is far from perfect. Some
-major caveats are listed here and/or in the issue list on GitHub (see [here]
-(../issues)). * Every once in a while processes fail to terminate even though
-they have been killed by `LittleBrother`. In these cases the user will still be
+Troubleshooting So, you went through all the above but LittleBrother does not
+seem to work? Maybe this [troubleshooting page](TROUBLESHOOTING.md) can help
+you. ## Caveats The application `LittleBrother` is far from perfect. Some major
+caveats are listed here and/or in the issue list on GitHub (see [here](../
+issues)). * Every once in a while processes fail to terminate even though they
+have been killed by `LittleBrother`. In these cases the user will still be
 regarded as logged in although he/she is not. Usually this can only be solved
 by trying to kill the processes again using the master user. Database eloquent
 users may try to delete/correct the incorrect process time entries. * The web
 server only responds to HTTP requests. This is probably always OK for
 communication between the slaves and the master in local area network. If the
-master host is to be accessible from the internet it should be put behind a
+master host is to be accessible from the internet, it should be put behind a
 reverse proxy handling the HTTPS termination (see below). ##
 Internationalization The application uses the PIP package `Flask-Babel` to
 provide internationalization for the web frontend. Currently, the following
 languages are supported or currently in preparation (in the order they were
 made available): | Flag | Language | Locale | Status | Translation provided by
 | | ---------------------------------------------------------------| ----------
 --- | ------ | -------------- | ---------------------------| | ![Flag USA](doc/
 united-states-of-america-flag-icon-32.png) | English | en | Up-to-date | Marcus
 Rickert | | ![Flag Germany](doc/germany-flag-icon-32.png) | German | de | Up-
 to-date | Marcus Rickert | | ![Flag Italy](doc/italy-flag-icon-32.png) |
-Italian | it | Up-to-date | Albano Battistella | | ![Flag Netherlands](doc/
+Italian | it | Revision 107 | Albano Battistella | | ![Flag Netherlands](doc/
 netherlands-flag-icon-32.png) | Dutch | nl | Revision 63 | Simone & Lex | | !
 [Flag Finland](doc/finland-flag-icon-32.png) | Finnish | fi | Revision 63 |
 Isakkii Kosonen | | ![Flag France](doc/france-flag-icon-32.png) | French | fr |
 Revision 86 | Albano Battistella | | ![Flag Turkey](doc/turkey-flag-icon-
 32.png) | Turkish | tr | Revision 63 | Selay Dogan | | ![Flag Russia](doc/
 russia-flag-icon-32.png) | Russian | ru | Revision 63 | J. Moldawski | | ![Flag
 Japan](doc/japan-flag-icon-32.png) | Japanese | ja | Revision 63 | Arik M. | |
```

### Comparing `little-brother-0.4.8/little_brother/admin_data_handler.py` & `little-brother-0.4.9/little_brother/admin_data_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,110 +77,128 @@
         return self._user_locale_handler
 
     def get_admin_info(self, p_session_context, p_user_name, p_process_infos) -> ViewInfo:
 
         admin_infos = self.get_admin_infos(
             p_session_context=p_session_context,
             p_process_infos=p_process_infos,
-            p_user_names=[ p_user_name ])
+            p_user_names=[p_user_name])
 
         if len(admin_infos) == 0:
             return None
 
         return admin_infos[0]
 
+    def get_day_info_for_user(self, p_admin_info, p_username: str,
+                              p_reference_date: datetime.datetime, p_rule_set) -> view_info.ViewInfo:
+
+        if p_rule_set is not None:
+            key_rule_override = rule_override.get_key(p_username=p_username,
+                                                      p_reference_date=p_reference_date)
+            override = self._rule_overrides.get(key_rule_override)
+
+            if override is None:
+                override = rule_override.RuleOverride(p_reference_date=p_reference_date,
+                                                      p_username=p_username)
+
+            effective_rule_set = rule_result_info.apply_override(p_rule_set=p_rule_set,
+                                                                 p_rule_override=override)
+
+            day_info = view_info.ViewInfo(p_parent=p_admin_info,
+                                          p_html_key=tools.get_simple_date_as_string(
+                                              p_date=p_reference_date))
+
+            if p_reference_date == datetime.date.today():
+                day_info.long_format = _("'Today ('EEE')'", 'long')
+                day_info.short_format = _("'Today'", 'short')
+
+            elif p_reference_date == datetime.date.today() + datetime.timedelta(days=1):
+                day_info.long_format = _("'Tomorrow ('EEE')'", 'long')
+                day_info.short_format = _("'Tomorrow'", 'short')
+
+            else:
+                day_info.long_format = _("yyyy-MM-dd' ('EEE')'")
+                day_info.short_format = _("EEE")
+
+            day_info.reference_date = p_reference_date
+            day_info.rule_set = p_rule_set
+            day_info.override = override
+            day_info.effective_rule_set = effective_rule_set
+            day_info.max_lookahead_in_days = self._config.admin_lookahead_in_days
+
+            return day_info
+
+    def get_admin_info_for_user(self, p_session_context, p_user_infos, p_time_extensions, p_days, p_username):
+
+        user : User = self.user_entity_manager.user_map(p_session_context).get(p_username)
+
+        if user is None or not user.active:
+            return None
+
+        admin_info = view_info.ViewInfo(p_html_key=p_username)
+        admin_info.full_name = user.full_name
+        admin_info.username = p_username
+        admin_info.full_name = p_username
+
+        admin_info.time_extension = p_time_extensions.get(p_username)
+        admin_info.time_extension_periods = []
+
+        if admin_info.time_extension is not None:
+            # add special value 0 for "off"
+            admin_info.time_extension_periods.append(0)
+
+        for period in self._config.time_extension_periods_list:
+            if period > 0:
+                admin_info.time_extension_periods.append(period)
+
+            else:
+                if admin_info.time_extension is not None and \
+                        admin_info.time_extension.end_datetime + \
+                        datetime.timedelta(minutes=period) >= admin_info.time_extension.start_datetime:
+                    admin_info.time_extension_periods.append(period)
+
+
+        admin_info.day_infos = []
+
+        admin_info.user_info = p_user_infos.get(p_username)
+
+        if admin_info.user_info is not None:
+            for reference_date in sorted(p_days):
+                rule_set = self.rule_handler.get_active_ruleset(
+                    p_rule_sets=user.rulesets, p_reference_date=reference_date)
+
+                day_info = self.get_day_info_for_user(p_admin_info=admin_info, p_username=p_username,
+                                                      p_reference_date=reference_date, p_rule_set=rule_set)
+
+                admin_info.day_infos.append(day_info)
+
+        return admin_info
 
     def get_admin_infos(self, p_session_context, p_user_names, p_process_infos):
 
         admin_infos = []
 
         user_infos = self.get_user_status_infos(p_session_context=p_session_context, p_include_history=False,
                                                 p_process_infos=p_process_infos)
         time_extensions = self.time_extension_entity_manager.get_active_time_extensions(
             p_session_context=p_session_context, p_reference_datetime=tools.get_current_time())
 
         days = [datetime.date.today() + datetime.timedelta(days=i) for i in
                 range(0, self._config.admin_lookahead_in_days + 1)]
 
         for override in self._rule_overrides.values():
-            if not override.reference_date in days and override.reference_date >= datetime.date.today():
+            if override.reference_date not in days and override.reference_date >= datetime.date.today():
                 days.append(override.reference_date)
 
         for username in p_user_names:
-            admin_info = view_info.ViewInfo(p_html_key=username)
-            admin_info.username = username
-            admin_info.full_name = username
-
-            admin_info.time_extension = time_extensions.get(username)
-            admin_info.time_extension_periods = []
-
-            if admin_info.time_extension is not None:
-                # add special value 0 for "off"
-                admin_info.time_extension_periods.append(0)
-
-            for period in self._config.time_extension_periods_list:
-                if period > 0:
-                    admin_info.time_extension_periods.append(period)
-
-                else:
-                    if admin_info.time_extension is not None and \
-                            admin_info.time_extension.end_datetime + \
-                            datetime.timedelta(minutes=period) >= admin_info.time_extension.start_datetime:
-                        admin_info.time_extension_periods.append(period)
-
-            user = self.user_entity_manager.user_map(p_session_context).get(username)
-
-            if user is not None:
-                admin_info.full_name = user.full_name
-
-            admin_info.user_info = user_infos.get(username)
-
-            if admin_info.user_info is not None:
-                admin_info.day_infos = []
-
-                for reference_date in sorted(days):
-                    rule_set = self.rule_handler.get_active_ruleset(
-                        p_rule_sets=user.rulesets, p_reference_date=reference_date)
-
-                    if rule_set is not None:
-                        key_rule_override = rule_override.get_key(p_username=username,
-                                                                  p_reference_date=reference_date)
-                        override = self._rule_overrides.get(key_rule_override)
-
-                        if override is None:
-                            override = rule_override.RuleOverride(p_reference_date=reference_date,
-                                                                  p_username=username)
-
-                        effective_ruleset = rule_result_info.apply_override(p_rule_set=rule_set,
-                                                                            p_rule_override=override)
-
-                        day_info = view_info.ViewInfo(p_parent=admin_info,
-                                                      p_html_key=tools.get_simple_date_as_string(
-                                                          p_date=reference_date))
-
-                        if reference_date == datetime.date.today():
-                            day_info.long_format = _("'Today ('EEE')'", 'long')
-                            day_info.short_format = _("'Today'", 'short')
-
-                        elif reference_date == datetime.date.today() + datetime.timedelta(days=1):
-                            day_info.long_format = _("'Tomorrow ('EEE')'", 'long')
-                            day_info.short_format = _("'Tomorrow'", 'short')
-
-                        else:
-                            day_info.long_format = _("yyyy-MM-dd' ('EEE')'")
-                            day_info.short_format = _("EEE")
-
-                        admin_info.day_infos.append(day_info)
-
-                        day_info.reference_date = reference_date
-                        day_info.rule_set = rule_set
-                        day_info.override = override
-                        day_info.effective_rule_set = effective_ruleset
-                        day_info.max_lookahead_in_days = self._config.admin_lookahead_in_days
+            admin_info = self.get_admin_info_for_user(p_session_context=p_session_context, p_user_infos=user_infos,
+                                                      p_days=days, p_time_extensions=time_extensions,
+                                                      p_username=username)
 
+            if admin_info is not None:
                 admin_infos.append(admin_info)
 
         return sorted(admin_infos, key=lambda info: info.full_name)
 
     def update_rule_override(self, p_rule_override):
 
         fmt = "Updating '{override}'"
@@ -188,14 +206,59 @@
 
         self._rule_overrides[p_rule_override.get_key()] = p_rule_override
 
         with SessionContext(p_persistence=self.persistence) as session_context:
             self.rule_override_entity_manager.update_rule_override(
                 p_session_context=session_context, p_rule_override=p_rule_override)
 
+    def get_user_info_for_user(self, p_session_context, p_user, p_reference_time,
+                               p_users_stat_infos, p_active_time_extensions):
+
+        user_info = None
+
+        rule_set = self.rule_handler.get_active_ruleset(
+            p_rule_sets=p_user.rulesets, p_reference_date=p_reference_time.date())
+        stat_infos = p_users_stat_infos.get(p_user.username)
+        active_time_extension = p_active_time_extensions.get(p_user.username)
+        user_locale = self.user_locale_handler.get_user_locale(
+            p_session_context=p_session_context, p_username=p_user.username)
+
+        if stat_infos is not None:
+            stat_info = stat_infos.get(rule_set.context)
+
+            if stat_info is not None:
+                self._logger.debug(str(stat_info))
+
+                key_rule_override = rule_override.get_key(p_username=p_user.username,
+                                                          p_reference_date=p_reference_time.date())
+                override = self._rule_overrides.get(key_rule_override)
+
+                rule_result_info = self.rule_handler.process_rule_sets_for_user(
+                    p_rule_sets=p_user.rulesets,
+                    p_stat_info=stat_info,
+                    p_active_time_extension=active_time_extension,
+                    p_reference_time=p_reference_time,
+                    p_rule_override=override,
+                    p_locale=user_locale)
+
+                activity_permitted = rule_result_info.activity_allowed()
+
+                user_info = {
+                    'username': p_user.username,
+                    'full_name': p_user.full_name,
+                    'active_rule_set': rule_set,
+                    'active_stat_info': stat_info,
+                    'active_rule_result_info': rule_result_info,
+                    'max_lookback_in_days': self._config.process_lookback_in_days,
+                    'activity_permitted': activity_permitted,
+                    'history_labels': self.history_labels
+                }
+
+        return user_info
+
     def get_user_status_infos(self, p_session_context, p_process_infos, p_include_history=True):
 
         user_infos = {}
 
         reference_time = datetime.datetime.now()
 
         active_time_extensions = self.time_extension_entity_manager.get_active_time_extensions(
@@ -208,51 +271,21 @@
             p_max_lookback_in_days=self._config.process_lookback_in_days if p_include_history else 1,
             p_min_activity_duration=self._config.min_activity_duration)
 
         for username in self.user_entity_manager.user_map(p_session_context).keys():
             user: User = self.user_entity_manager.user_map(p_session_context).get(username)
 
             if user is not None:
-                rule_set = self.rule_handler.get_active_ruleset(
-                    p_rule_sets=user.rulesets, p_reference_date=reference_time.date())
-                stat_infos = users_stat_infos.get(username)
-                active_time_extension = active_time_extensions.get(username)
-                user_locale = self.user_locale_handler.get_user_locale(
-                    p_session_context=p_session_context, p_username=username)
-
-                if stat_infos is not None:
-                    stat_info = stat_infos.get(rule_set.context)
-
-                    if stat_info is not None:
-                        self._logger.debug(str(stat_info))
-
-                        key_rule_override = rule_override.get_key(p_username=username,
-                                                                  p_reference_date=reference_time.date())
-                        override = self._rule_overrides.get(key_rule_override)
-
-                        rule_result_info = self.rule_handler.process_rule_sets_for_user(
-                            p_rule_sets=user.rulesets,
-                            p_stat_info=stat_info,
-                            p_active_time_extension=active_time_extension,
-                            p_reference_time=reference_time,
-                            p_rule_override=override,
-                            p_locale=user_locale)
-
-                        activity_permitted = rule_result_info.activity_allowed()
+                user_info = self.get_user_info_for_user(p_session_context=p_session_context, p_user=user,
+                                                        p_users_stat_infos=users_stat_infos,
+                                                        p_active_time_extensions=active_time_extensions,
+                                                        p_reference_time=reference_time)
 
-                        user_infos[username] = {
-                            'username': username,
-                            'full_name': user.full_name,
-                            'active_rule_set': rule_set,
-                            'active_stat_info': stat_info,
-                            'active_rule_result_info': rule_result_info,
-                            'max_lookback_in_days': self._config.process_lookback_in_days,
-                            'activity_permitted': activity_permitted,
-                            'history_labels': self.history_labels
-                        }
+                if user_info is not None:
+                    user_infos[username] = user_info
 
         return user_infos
 
     def load_rule_overrides(self):
 
         with SessionContext(p_persistence=self.persistence) as session_context:
             overrides = self.rule_override_entity_manager.load_rule_overrides(
@@ -294,29 +327,29 @@
                                                                     p_username=p_username)
             user: User = self.user_entity_manager.user_map(p_session_context=session_context).get(p_username)
 
             if user is not None:
                 rule_set = self.rule_handler.get_active_ruleset(p_rule_sets=user.rulesets,
                                                                 p_reference_date=p_reference_time.date())
 
-            stat_infos = users_stat_infos.get(p_username)
-            active_time_extension = active_time_extensions.get(p_username)
+                stat_infos = users_stat_infos.get(p_username)
+                active_time_extension = active_time_extensions.get(p_username)
 
-            if stat_infos is not None:
-                stat_info = stat_infos.get(rule_set.context)
+                if stat_infos is not None:
+                    stat_info = stat_infos.get(rule_set.context)
 
-                if stat_info is not None:
-                    self._logger.debug(str(stat_info))
+                    if stat_info is not None:
+                        self._logger.debug(str(stat_info))
 
-                    key_rule_override = rule_override.get_key(p_username=p_username,
-                                                              p_reference_date=p_reference_time.date())
-                    override = self._rule_overrides.get(key_rule_override)
-
-                    rule_result_info = self.rule_handler.process_rule_sets_for_user(
-                        p_rule_sets=user.rulesets,
-                        p_stat_info=stat_info,
-                        p_reference_time=p_reference_time,
-                        p_active_time_extension=active_time_extension,
-                        p_rule_override=override,
-                        p_locale=user_locale)
+                        key_rule_override = rule_override.get_key(p_username=p_username,
+                                                                  p_reference_date=p_reference_time.date())
+                        override = self._rule_overrides.get(key_rule_override)
+
+                        rule_result_info = self.rule_handler.process_rule_sets_for_user(
+                            p_rule_sets=user.rulesets,
+                            p_stat_info=stat_info,
+                            p_reference_time=p_reference_time,
+                            p_active_time_extension=active_time_extension,
+                            p_rule_override=override,
+                            p_locale=user_locale)
 
         return rule_result_info
```

### Comparing `little-brother-0.4.8/little_brother/admin_event.py` & `little-brother-0.4.9/little_brother/admin_event.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/env.py` & `little-brother-0.4.9/little_brother/alembic/env.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/0a5c7b6ad27a_fb_issue_124.py` & `little-brother-0.4.9/little_brother/alembic/versions/0a5c7b6ad27a_fb_issue_124.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/2f458b3a313e_add_max_activity_duration.py` & `little-brother-0.4.9/little_brother/alembic/versions/2f458b3a313e_add_max_activity_duration.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/647cf46033a9_initial_db_model_at_488c798.py` & `little-brother-0.4.9/little_brother/alembic/versions/647cf46033a9_initial_db_model_at_488c798.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/96ff8f93ef32_add_downtime_attributes.py` & `little-brother-0.4.9/little_brother/alembic/versions/96ff8f93ef32_add_downtime_attributes.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/9713cef84918_userstatus_issue_130.py` & `little-brother-0.4.9/little_brother/alembic/versions/9713cef84918_userstatus_issue_130.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/e0c0d7048235_prohibited_process_name_pattern.py` & `little-brother-0.4.9/little_brother/alembic/versions/e0c0d7048235_prohibited_process_name_pattern.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic/versions/version_0_3_added_tables_for_configuration_gui.py` & `little-brother-0.4.9/little_brother/alembic/versions/version_0_3_added_tables_for_configuration_gui.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/alembic.ini` & `little-brother-0.4.9/little_brother/alembic.ini`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/api/api_view_handler.py` & `little-brother-0.4.9/little_brother/api/api_view_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/api/master_connector.py` & `little-brother-0.4.9/little_brother/api/master_connector.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/app.py` & `little-brother-0.4.9/little_brother/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from little_brother import dependency_injection
 from little_brother import login_mapping
 from little_brother import rule_handler
 from little_brother.admin_data_handler import AdminDataHandler
 from little_brother.alembic.versions import version_0_3_added_tables_for_configuration_gui as alembic_version_gui
 from little_brother.api.master_connector import MasterConnector, MasterConnectorConfigModel, \
     SECTION_NAME as MASTER_CONNECTOR_SECTION_NAME
+from little_brother.api.version_checker import VersionChecker
+from little_brother.api.version_checker import VersionCheckerConfigModel, \
+    SECTION_NAME as VERSION_CHECKER_SECTION_NAME, SOURCEFORGE_CHANNEL_INFOS
 from little_brother.app_control import AppControl, AppControlConfigModel, SECTION_NAME as APP_CONTROL_SECTION_NAME
 from little_brother.german_vacation_context_rule_handler import GermanVacationContextRuleHandler
 from little_brother.persistence import persistence
 from little_brother.persistence.persistent_rule_set_entity_manager import RuleSetEntityManager
 from little_brother.persistence.persistent_time_extension_entity_manager import TimeExtensionEntityManager
 from little_brother.persistence.persistent_user import User
 from little_brother.prometheus import PrometheusClient, PrometheusClientConfigModel, \
@@ -157,14 +160,17 @@
 
         self._login_mapping_section_handler = login_mapping.LoginMappingSectionHandler()
         p_configuration.register_section_handler(p_section_handler=self._login_mapping_section_handler)
 
         pinger_section = pinger.PingerConfigModel()
         p_configuration.add_section(pinger_section)
 
+        version_checker_section = VersionCheckerConfigModel()
+        p_configuration.add_section(version_checker_section)
+
         return super(App, self).prepare_configuration(p_configuration=p_configuration)
 
     def is_master(self):
 
         return self._config[MASTER_CONNECTOR_SECTION_NAME].host_url is None
 
     def check_migrations(self):
@@ -368,14 +374,20 @@
             msg = "Master instance requires port number for web server"
             raise configuration.ConfigurationException(msg)
 
         else:
             msg = "Slave instance will not start web server due to missing port number"
             self._logger.warn(msg)
 
+        self._version_checker = VersionChecker(p_config=self._config[VERSION_CHECKER_SECTION_NAME],
+                                               p_channel_infos=SOURCEFORGE_CHANNEL_INFOS)
+
+        dependency_injection.container[VersionChecker] = self._version_checker
+
+
         task = base_app.RecurringTask(p_name="app_control.check", p_handler_method=self._app_control.check,
                                       p_interval=self._app_control.check_interval)
         self.add_recurring_task(p_recurring_task=task)
 
     def run_special_commands(self, p_arguments):
 
         if p_arguments.stamp_databases:
```

### Comparing `little-brother-0.4.8/little_brother/app_control.py` & `little-brother-0.4.9/little_brother/app_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,14 @@
 from little_brother.rule_handler import RuleHandler
 from little_brother.user_locale_handler import UserLocaleHandler
 from little_brother.user_manager import UserManager
 from python_base_app import log_handling
 from python_base_app import tools
 from python_base_app.base_user_handler import BaseUserHandler
 
-DEFAULT_SCAN_ACTIVE = True
-DEFAULT_ADMIN_LOOKAHEAD_IN_DAYS = 7  # days
-DEFAULT_PROCESS_LOOKUP_IN_DAYS = 7  # days
-DEFAULT_HISTORY_LENGTH_IN_DAYS = 180  # days
-DEFAULT_MIN_ACTIVITY_DURATION = 60  # seconds
-DEFAULT_CHECK_INTERVAL = 5  # seconds
-DEFAULT_INDEX_REFRESH_INTERVAL = 60  # seconds
-DEFAULT_TOPOLOGY_REFRESH_INTERVAL = 60  # seconds
-DEFAULT_MAXIMUM_CLIENT_PING_INTERVAL = 60  # seconds
-DEFAULT_WARNING_TIME_WITHOUT_SEND_EVENTS = 3 * DEFAULT_CHECK_INTERVAL  # seconds
-DEFAULT_MAXIMUM_TIME_WITHOUT_SEND_EVENTS = 10 * DEFAULT_CHECK_INTERVAL  # minutes
-DEFAULT_KILL_PROCESS_DELAY = 10  # seconds
-DEFAULT_TIME_EXTENSION_PERIODS = "-30,-15,-5,5,10,15,30,45,60"
-
 ALEMBIC_VERSION_INIT_GUI_CONFIGURATION = ""
 
 SECTION_NAME = "AppControl"
 
 LAST_VERSION_WITHOUT_CLIENT_STAT_SUPPORT = "0.3.8"
 MINIMUM_VERSION_WITH_CLIENT_STAT_SUPPORT = "0.3.9"
```

### Comparing `little-brother-0.4.8/little_brother/app_control_config_model.py` & `little-brother-0.4.9/little_brother/app_control_config_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from little_brother import login_mapping
+from little_brother import settings
 from python_base_app import configuration
 
 DEFAULT_SCAN_ACTIVE = True
 DEFAULT_ADMIN_LOOKAHEAD_IN_DAYS = 7  # days
 DEFAULT_PROCESS_LOOKUP_IN_DAYS = 7  # days
 DEFAULT_HISTORY_LENGTH_IN_DAYS = 180  # days
 DEFAULT_MIN_ACTIVITY_DURATION = 60  # seconds
@@ -28,14 +29,15 @@
 DEFAULT_TOPOLOGY_REFRESH_INTERVAL = 60  # seconds
 DEFAULT_LOCALE = "en_US"
 DEFAULT_MAXIMUM_CLIENT_PING_INTERVAL = 60  # seconds
 DEFAULT_WARNING_TIME_WITHOUT_SEND_EVENTS = 3 * DEFAULT_CHECK_INTERVAL  # seconds
 DEFAULT_MAXIMUM_TIME_WITHOUT_SEND_EVENTS = 10 * DEFAULT_CHECK_INTERVAL  # minutes
 DEFAULT_KILL_PROCESS_DELAY = 10  # seconds
 DEFAULT_TIME_EXTENSION_PERIODS = "-30,-15,-5,5,10,15,30,45,60"
+DEFAULT_UPDATE_CHANNEL = settings.MASTER_BRANCH_NAME
 
 SECTION_NAME = "AppControl"
 
 
 class AppControlConfigModel(configuration.ConfigModel):
 
     def __init__(self):
@@ -53,14 +55,15 @@
         self.index_refresh_interval = DEFAULT_INDEX_REFRESH_INTERVAL
         self.topology_refresh_interval = DEFAULT_TOPOLOGY_REFRESH_INTERVAL
         self.maximum_client_ping_interval = DEFAULT_MAXIMUM_CLIENT_PING_INTERVAL
         self.maximum_time_without_send_events = DEFAULT_MAXIMUM_TIME_WITHOUT_SEND_EVENTS
         self.warning_time_without_send_events = DEFAULT_WARNING_TIME_WITHOUT_SEND_EVENTS
         self.kill_process_delay = DEFAULT_KILL_PROCESS_DELAY
         self.time_extension_periods = DEFAULT_TIME_EXTENSION_PERIODS
+        self.update_channel = DEFAULT_UPDATE_CHANNEL
 
         self._time_extension_periods_list = None
 
     @property
     def time_extension_periods_list(self):
 
         if self._time_extension_periods_list is None:
```

### Comparing `little-brother-0.4.8/little_brother/client_device_handler.py` & `little-brother-0.4.9/little_brother/client_device_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/client_info.py` & `little-brother-0.4.9/little_brother/client_info.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/client_process_handler.py` & `little-brother-0.4.9/little_brother/client_process_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (C) 2019  Marcus Rickert
+# Copyright (C) 2019-2021  Marcus Rickert
 #
 # See https://github.com/marcus67/little_brother
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 # This program is distributed in the hope that it will be useful,
@@ -79,16 +79,25 @@
             self._logger.warning(fmt)
             pinfo = admin_event.create_process_info_from_event(p_event=p_event)
             return [self.create_admin_event_process_end_from_pinfo(p_pinfo=pinfo)]
 
         uid = p_login_mapping.get_uid_by_login(p_server_group=p_server_group, p_login=p_event.username)
 
         if uid is None:
-            fmt = "handle_event_kill_process: cannot find uid for username '{username}'"
+            fmt = "handle_event_kill_process: cannot find uid for username '{username}' -> ignoring event"
             self._logger.warning(fmt.format(username=p_event.username))
+            return []
+
+        current_uid = proc.uids().effective
+
+        if uid != current_uid:
+            fmt = "handle_event_kill_process: current uid {current_uid} of process " \
+                  "does not match the one of event {event_uid} -> ignoring event"
+            self._logger.warning(fmt.format(current_uid=current_uid, event_uid=uid))
+            return []
 
         params = {
             'pid': p_event.pid,
             'username': p_event.username,
             'uid': uid,
             'signal': 'SIGHUP',
             'host': p_event.hostname
```

### Comparing `little-brother-0.4.8/little_brother/client_stats.py` & `little-brother-0.4.9/little_brother/client_stats.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/constants.py` & `little-brother-0.4.9/little_brother/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -133,7 +133,12 @@
 
 USERS_BLUEPRINT_NAME = "users"
 USERS_HTML_TEMPLATE = "users.template.html"
 USERS_REL_URL = "users"
 USERS_VIEW_NAME = "main_view"
 
 CSS_CLASS_EMPHASIZE_RULE_OVERRIDE = "rule-override"
+
+SOURCEFORGE_VERSION_RSS_URL = "https://sourceforge.net/projects/little-brother/rss?path=/"
+SOURCEFORGE_VERSION_XPATH = "./channel/item/title"
+SOURCEFORGE_VERSION_REGEX = "^/([a-z]+)/little-brother_([.0-9]+)_([0-9]+)\.deb$"
+
```

### Comparing `little-brother-0.4.8/little_brother/context_rule_handler.py` & `little-brother-0.4.9/little_brother/context_rule_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/db_migrations.py` & `little-brother-0.4.9/little_brother/db_migrations.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/entity_forms.py` & `little-brother-0.4.9/little_brother/entity_forms.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/event_handler.py` & `little-brother-0.4.9/little_brother/event_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/german_vacation_context_rule_handler.py` & `little-brother-0.4.9/little_brother/german_vacation_context_rule_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/git.py` & `little-brother-0.4.9/little_brother/git.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/language.py` & `little-brother-0.4.9/little_brother/language.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/login_mapping.py` & `little-brother-0.4.9/little_brother/login_mapping.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/base_entity.py` & `little-brother-0.4.9/little_brother/persistence/base_entity.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/base_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/base_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistence.py` & `little-brother-0.4.9/little_brother/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistence_base.py` & `little-brother-0.4.9/little_brother/persistence/persistence_base.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_admin_event.py` & `little-brother-0.4.9/little_brother/persistence/persistent_admin_event.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_admin_event_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_admin_event_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_daily_user_status.py` & `little-brother-0.4.9/little_brother/persistence/persistent_daily_user_status.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_daily_user_status_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_daily_user_status_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_dependency_injection_mix_in.py` & `little-brother-0.4.9/little_brother/persistence/persistent_dependency_injection_mix_in.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_device.py` & `little-brother-0.4.9/little_brother/persistence/persistent_device.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_device_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_device_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_process_info.py` & `little-brother-0.4.9/little_brother/persistence/persistent_process_info.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_process_info_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_process_info_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_rule_override.py` & `little-brother-0.4.9/little_brother/persistence/persistent_rule_override.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_rule_override_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_rule_override_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_rule_set.py` & `little-brother-0.4.9/little_brother/persistence/persistent_rule_set.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_rule_set_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_rule_set_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_time_extension.py` & `little-brother-0.4.9/little_brother/persistence/persistent_time_extension.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_time_extension_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_time_extension_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_user.py` & `little-brother-0.4.9/little_brother/persistence/persistent_user.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_user_2_device.py` & `little-brother-0.4.9/little_brother/persistence/persistent_user_2_device.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_user_2_device_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_user_2_device_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/persistent_user_entity_manager.py` & `little-brother-0.4.9/little_brother/persistence/persistent_user_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/persistence/session_context.py` & `little-brother-0.4.9/little_brother/persistence/session_context.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/process_handler.py` & `little-brother-0.4.9/little_brother/process_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/process_handler_manager.py` & `little-brother-0.4.9/little_brother/process_handler_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,15 @@
                         p_session_context=session_context, p_process_info=pinfo)
 
         if self._is_master:
             rule_result_info = self.admin_data_handler.get_current_rule_result_info(
                 p_reference_time=datetime.datetime.now(), p_process_infos=self.get_process_infos(),
                 p_username=p_event.username)
 
-            if rule_result_info.activity_allowed():
-
+            if rule_result_info is not None and rule_result_info.activity_allowed():
                 with SessionContext(p_persistence=self.persistence) as session_context:
 
                     if rule_result_info.limited_session_time():
                         self.user_manager.issue_notification(
                             p_session_context=session_context,
                             p_username=p_event.username,
                             p_message=self._language.get_text_limited_session_start(p_locale=rule_result_info.locale,
@@ -260,15 +259,15 @@
             return
 
         if self._is_master:
             rule_result_info = self.admin_data_handler.get_current_rule_result_info(
                 p_reference_time=datetime.datetime.now(), p_process_infos=self.get_process_infos(),
                 p_username=p_event.username)
 
-            if rule_result_info.activity_allowed():
+            if rule_result_info is not None and rule_result_info.activity_allowed():
                 with SessionContext(p_persistence=self.persistence) as session_context:
 
                     variables = rule_result_info.args
                     variables['process_name'] = p_event.processname
 
                     self.user_manager.issue_notification(
                         p_session_context=session_context,
```

### Comparing `little-brother-0.4.8/little_brother/process_info.py` & `little-brother-0.4.9/little_brother/process_info.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/process_statistics.py` & `little-brother-0.4.9/little_brother/process_statistics.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/prometheus.py` & `little-brother-0.4.9/little_brother/prometheus.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/rule_handler.py` & `little-brother-0.4.9/little_brother/rule_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/rule_override.py` & `little-brother-0.4.9/little_brother/rule_override.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/rule_result_info.py` & `little-brother-0.4.9/little_brother/rule_result_info.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/settings.py` & `little-brother-0.4.9/little_brother/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,20 +14,34 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 settings = {
     "name": "little-brother",
     "url": "https://github.com/marcus67/little_brother",
-    "version": "0.4.8",
+    "version": "0.4.9",
     "description": "Simple parental control application monitoring specific processes on Linux hosts "
                    "to monitor and limit the play time of (young) children.",
     "author": "Marcus Rickert",
     "author_email": "little-brother@web.de",
 }
 
 extended_settings = {
     "display_url": "github.com/marcus67/little_brother",
-    "debian_package_revision": "107",
+    "debian_package_revision": "108",
     "debian_package_architecture": "all",
     "babel_rel_directory": "translations",
+    "analyze_extra_coverage_exclusions": "run_python_base_app_test_suite_no_venv.py",
 }
+
+RELEASE_BRANCH_NAME = "release"
+MASTER_BRANCH_NAME = "master"
+
+SOURCEFORGE_CHANNELS = [
+    MASTER_BRANCH_NAME,
+    RELEASE_BRANCH_NAME
+]
+
+DOCKER_CHANNELS = [
+    MASTER_BRANCH_NAME,
+    RELEASE_BRANCH_NAME
+]
```

### Comparing `little-brother-0.4.8/little_brother/simple_context_rule_handlers.py` & `little-brother-0.4.9/little_brother/simple_context_rule_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         else:
             fmt = "invalid context details '{details}' for context {name}"
             raise configuration.ConfigurationException(fmt.format(details=p_details, name=self.context_name))
 
         time_tuple = p_reference_date.timetuple()
 
-        return weekday_string[time_tuple.tm_wday] in VALID_ACTIVE_DAY_CHARACTERS
+        return weekday_string.upper()[time_tuple.tm_wday] in VALID_ACTIVE_DAY_CHARACTERS
 
     def get_choices(self):
 
         return WEEKPLAN_PREDEFINED_DETAILS.keys()
 
     def validate_context_details(self, p_context_detail):
 
@@ -89,15 +89,15 @@
 
         invalid = False
 
         if len(p_context_detail) != 7:
             invalid = True
 
         else:
-            for c in p_context_detail:
+            for c in p_context_detail.upper():
                 if c not in VALID_ACTIVE_DAY_CHARACTERS + VALID_INACTIVE_DAY_CHARACTERS:
                     invalid = True
 
         if invalid:
             localized_choices = "'" + "', '".join(
                 [self.locale_helper.gettext(p_text=choice) for choice in WEEKPLAN_PREDEFINED_DETAILS.keys()]) + "'"
```

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/LICENSE.txt` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/css/all.min.css` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/js/all.min.js` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-brands-400.svg` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-regular-400.svg` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/fontawesome/webfonts/fa-solid-900.svg` & `little-brother-0.4.9/little_brother/static/contrib/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap-theme.css` & `little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap-theme.min.css` & `little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap.css` & `little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/css/bootstrap.min.css` & `little-brother-0.4.9/little_brother/static/contrib/initializr/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/bootstrap.js` & `little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/bootstrap.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/bootstrap.min.js` & `little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/jquery-1.11.2.min.js` & `little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/jquery-1.11.2.min.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js` & `little-brother-0.4.9/little_brother/static/contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/contrib/js-cookie/js-cookie.js` & `little-brother-0.4.9/little_brother/static/contrib/js-cookie/js-cookie.js`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/default.css` & `little-brother-0.4.9/little_brother/static/default.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/baby-panda-32x32.ico` & `little-brother-0.4.9/little_brother/static/icons/baby-panda-32x32.ico`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/baby-panda-sad-128x128.png` & `little-brother-0.4.9/little_brother/static/icons/baby-panda-sad-128x128.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/baby-panda-sad-256x256.png` & `little-brother-0.4.9/little_brother/static/icons/baby-panda-sad-256x256.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/baby-panda.png` & `little-brother-0.4.9/little_brother/static/icons/baby-panda.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/docker-logo-128x128.png` & `little-brother-0.4.9/little_brother/static/icons/docker-logo-128x128.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/icon-baby-panda-128x128.png` & `little-brother-0.4.9/little_brother/static/icons/icon-baby-panda-128x128.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/icons/icon-baby-panda-32x32.png` & `little-brother-0.4.9/little_brother/static/icons/icon-baby-panda-32x32.png`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/static/login.css` & `little-brother-0.4.9/little_brother/static/login.css`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/templates/about.template.html` & `little-brother-0.4.9/little_brother/templates/topology.template.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!--
-#    Copyright (C) 2019  Marcus Rickert
+{#<!--
+#    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -12,23 +12,25 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 <HTML>
 {% import 'helper.macros.html' as helper %}
+
   {{ helper.locale_font(rel_font_size) }}
 
-  <META http-equiv="Content-Type" content="text/html;charset=UTF-9">
+  <META http-equiv="Content-Type" content="text/html;charset=UTF-8">
   <HEAD>
       <META http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
+      <META http-equiv="refresh" content="{{app_control_config.topology_refresh_interval}}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/bootstrap-theme.min.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/main.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/bootstrap.min.css') }}">
       <LINK REL="stylesheet" TYPE="text/css" HREF="{{ url_for('little_brother.static', filename='default.css') }}">
@@ -36,76 +38,47 @@
             HREF="{{ url_for('little_brother.static', filename='contrib/fontawesome/css/all.min.css') }}">
 
       <LINK REL="shortcut icon" TYPE="image/x-icon"
             HREF="{{ url_for('little_brother.static', filename='icons/baby-panda-32x32.ico') }}">
 
       <meta name="viewport" content="width=device-width, initial-scale=1">
 
-      <TITLE>LittleBrother-{{ _('About')}}</TITLE>
+      <TITLE>LittleBrother-{{_('Topology')}}</TITLE>
 
   </HEAD>
 
   <BODY>
-  {{ helper.fontawesome_script() }}
-  {% include 'navbar.include.html' %}
-  <CENTER>
-	  <img alt="Brand" src="{{ url_for('little_brother.static', filename='icons/icon-baby-panda-128x128.png') }}">
-	  <BR>
-	  <H2>Little&nbsp;Brother</H2>
-	  <BR>
-  </CENTER>
-
-    <DIV CLASS="container STANDARD_TABLE condensed-container">
-
-    	<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
-    		<DIV CLASS="col-xs-3 localetext">{{_('Setting')}}</DIV>
-    		<DIV CLASS="col-xs-9 localetext">{{_('Value')}}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_('Repository')}}</DIV>
-			<DIV CLASS="col-xs-9"><A HREF="{{ settings.url }}">{{ extended_settings.display_url }}</A></DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_('Version')}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ settings.version }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-			<DIV CLASS="col-xs-3 localetext"><SPAN CLASS="nonlocaletext">Debian</SPAN> {{_('Package Revision')}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ extended_settings.debian_package_revision }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_('Git Commit ID')}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ git_metadata.commit_id }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_('Git Branch Name')}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ git_metadata.branch }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_("Git Author's Name")}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ git_metadata.author_name }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_("Git Author's Email Address")}}</DIV>
-    		<DIV CLASS="col-xs-9">{{ git_metadata.author_email }}</DIV>
-    	</DIV>
-    	<DIV CLASS="row  ROWLEVEL_3">
-    		<DIV CLASS="col-xs-3 localetext">{{_("Supported Languages")}}</DIV>
-    		<DIV CLASS="col-xs-9">
-				<UL>
-					{% for language in languages %}
-						<LI>{{ language[1] }} ({{ language[0] }})</LI>
-					{% endfor %}
-				</UL>
-			</DIV>
-    	</DIV>
+	{{ helper.fontawesome_script() }}
+	<DIV class="container-fluid">
+
+        {% include 'navbar.include.html' %}
+        {% include 'version_check.include.html' %}
 
-    </DIV> <!-- CLASS="container" -->
+        <DIV CLASS="container STANDARD_TABLE">
+            <DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{_('Node Type')}}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{_('Node Name')}}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{_('App Version')}}</DIV>
+                <DIV CLASS="col-xs-2 hidden-xs localetext">{{_('Revision')}}</DIV>
+                <DIV CLASS="col-xs-2 hidden-xs localetext">{{_('Python Version')}}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{_('Time Since Last Ping')}}</DIV>
+            </DIV>
+            {% for info in topology_infos %}
+            <DIV CLASS="row  ROWLEVEL_3">
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{ _(info.node_type) }}{% if info.client_stats.running_in_docker %} (Docker){% endif%}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext">{{ info.host_name }}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext {{ info.version_class }}">{{ info.version_string }}</DIV>
+                <DIV CLASS="col-xs-2 hidden-xs localetext">{{ info.client_stats.revision }}</DIV>
+                <DIV CLASS="col-xs-2 hidden-xs localetext">{{ info.client_stats.python_version }}</DIV>
+                <DIV CLASS="col-xs-3 col-sm-2 localetext {{ info.last_message_class}}">{{ info.seconds_without_ping | seconds_as_humanized_duration }}</DIV>
+            </DIV>
+            {% endfor %}
+        </DIV>
+    </DIV>
 
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
 
   </BODY>
-  
 </HTML>
```

#### html2text {}

 * *error from `html2text {}` (a):*

 * *Recoding from 'UTF-9' to 'UTF-8' is not available.*

 * *Check that 'UTF-9' is a valid encoding.*

```diff
@@ -0,0 +1,28 @@
+{##}
+{% import 'helper.macros.html' as helper %} {{ helper.locale_font
+(rel_font_size) }}
+
+
+
+
+
+
+
+
+{{ helper.fontawesome_script() }}
+{% include 'navbar.include.html' %} {% include 'version_check.include.html' %}
+{{_('Node Type')}}
+{{_('Node Name')}}
+{{_('App Version')}}
+{{_('Revision')}}
+{{_('Python Version')}}
+{{_('Time Since Last Ping')}}
+{% for info in topology_infos %}
+{{ _(info.node_type) }}{% if info.client_stats.running_in_docker %} (Docker){%
+endif%}
+{{ info.host_name }}
+{{ info.version_string }}
+{{ info.client_stats.revision }}
+{{ info.client_stats.python_version }}
+{{ info.seconds_without_ping | seconds_as_humanized_duration }}
+{% endfor %}
```

### Comparing `little-brother-0.4.8/little_brother/templates/admin.template.html` & `little-brother-0.4.9/little_brother/templates/admin.template.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!--
+{#<!--
 #    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 <HTML>
 {% import 'bootstrap_accordion.macros.html' as accordion %}
 {% import 'helper.macros.html' as helper %}
 
   {{ helper.locale_font(rel_font_size) }}
 
@@ -44,237 +44,236 @@
 
       <TITLE>LittleBrother-{{_('Administration')}}</TITLE>
 
   </HEAD>
 
   <BODY>
 	{{ helper.fontawesome_script() }}
-	{% include 'navbar.include.html' %}
+	<DIV class="container-fluid">
 
-	<FORM ACTION="{{ url_for('admin.main_view') }}" METHOD="POST" CLASS="form-horizontal">
-		<!-- The following button ensures that pressing enter will trigger a normal save and not a more specialized
-		     button. -->
-		<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
-		<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
-	    <DIV CLASS="container STANDARD_TABLE">
-	    	<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
-	    		<DIV CLASS="col-xs-2 localetext">{{_('User')}}</DIV>
-				<DIV CLASS="col-xs-10 hidden-xs"></DIV>
-	    	</DIV>
-	    	{% for admin_info in admin_infos %}
-	    	   	{% call accordion.begin() %}{{admin_info.html_key}}{% endcall %}	    			        
-	    	
-			    	<DIV CLASS="row ROWLEVEL_2">
-						<DIV CLASS="col-xs-2  col-sm-2  col-md-2  col-lg-2">
-							<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-							<!-- {{ _('Show configurations of upcoming days') }} -->
-							{% call accordion.toggle_begin(tooltip="Show configurations of upcoming days")
-							%}{{admin_info.html_key}}{% endcall %}
-							{{ admin_info.full_name }}
-							{{ helper.check_or_cross(admin_info.user_info.activity_permitted) }}
-							{{ accordion.toggle_end() }}
-						</DIV>
-						<DIV CLASS="col-xs-3  col-sm-3  col-md-3  col-lg-3 localetext">
-							{% if admin_info.user_info.active_stat_info is defined %}
-							{{_("Today's Activity")}}:
-							<SPAN CLASS="nonlocaletext">
-								{{ admin_info.user_info.active_stat_info.todays_activity_duration|seconds_to_string }} /
-								{% if admin_info.day_infos[0].effective_rule_set.free_play %}
-									{{ _("unlimited") }}
-								{% else %}
-									{{ admin_info.day_infos[0].effective_rule_set.max_time_per_day|seconds_to_string }}
-								{% endif %}
-							</SPAN>
-							{% endif %}
-						</DIV>
-						<DIV CLASS="col-xs-7  col-sm-7  col-md-7  col-lg-7 localetext">
-							<UL>
-								{% for rule_template in
-								admin_info.user_info.active_rule_result_info.applying_rule_text_templates %}
-								<LI>{{ _(rule_template[0])|format(rule_template[1])|safe }}</LI>
-								{% endfor %}
-							</UL>
-						</DIV>
+		{% include 'navbar.include.html' %}
+		{% include 'version_check.include.html' %}
+
+		<FORM ACTION="{{ url_for('admin.main_view') }}" METHOD="POST" CLASS="form-horizontal">
+			{#<!-- The following button ensures that pressing enter will trigger a normal save and not a more specialized
+				 button. -->#}
+			<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
+			<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
+			<DIV CLASS="container STANDARD_TABLE">
+				<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
+					<DIV CLASS="col-xs-2 localetext">{{_('User')}}</DIV>
+					<DIV CLASS="col-xs-10 hidden-xs"></DIV>
+				</DIV>
+				{% for admin_info in admin_infos %}
+					{% call accordion.begin() %}{{admin_info.html_key}}{% endcall %}
 
-					</DIV>
-			    {% call accordion.details() %}{{admin_info.html_key}}{% endcall %}
-			        {% if admin_info.time_extension_periods|length > 0 %}
-						<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
+						<DIV CLASS="row ROWLEVEL_2">
 							<DIV CLASS="col-xs-2  col-sm-2  col-md-2  col-lg-2">
+								{#<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->#}
+								<!-- {{ _('Show configurations of upcoming days') }} -->
+								{% call accordion.toggle_begin(tooltip="Show configurations of upcoming days")
+								%}{{admin_info.html_key}}{% endcall %}
+								{{ admin_info.full_name }}
+								{{ helper.check_or_cross(admin_info.user_info.activity_permitted) }}
+								{{ accordion.toggle_end() }}
 							</DIV>
 							<DIV CLASS="col-xs-3  col-sm-3  col-md-3  col-lg-3 localetext">
-								{{ _("Manage Time Extension") }}
+								{% if admin_info.user_info.active_stat_info is defined %}
+								{{_("Today's Activity")}}:
+								<SPAN CLASS="nonlocaletext">
+									{{ admin_info.user_info.active_stat_info.todays_activity_duration|seconds_to_string }} /
+									{% if admin_info.day_infos[0].effective_rule_set.free_play %}
+										{{ _("unlimited") }}
+									{% else %}
+										{{ admin_info.day_infos[0].effective_rule_set.max_time_per_day|seconds_to_string }}
+									{% endif %}
+								</SPAN>
+								{% endif %}
 							</DIV>
 							<DIV CLASS="col-xs-7  col-sm-7  col-md-7  col-lg-7 localetext">
-								{% for period in admin_info.time_extension_periods %}
-								    {% if period == 0 %}
-										{% set period_string = - period %}
-										<BUTTON id="time_extension_{{ admin_info.username }}_0"
-												class="btn btn-time-extension-off" type="submit" name="submit"
-												value="time_extension_{{ admin_info.username }}_0"
-												title="{{_('Deactivate time extension')}}">
-											<I class="fas fa-power-off"></I>
-										</BUTTON>
-								    {% elif period < 0 %}
-										{% set period_string = - period %}
-										<BUTTON id="time_extension_{{ admin_info.username }}_{{period}}"
-												class="btn btn-time-extension-minus" type="submit" name="submit"
-												value="time_extension_{{ admin_info.username }}_{{period}}"
-												title="{{_('Decrease time extension by {minutes} minutes')|format({'minutes':period_string})}}">
-											<I class="far fa-minus-square"></I> {{ period_string }}
-										</BUTTON>
-								    {% else %}
-										<BUTTON id="time_extension_{{ admin_info.username }}_{{period}}"
-												class="btn btn-time-extension-plus" type="submit" name="submit"
-												value="time_extension_{{ admin_info.username }}_{{period}}"
-												title="{{_('Increase time extension by {minutes} minutes')|format({'minutes':period})}}">
-											<I class="far fa-plus-square"></I> {{ period }}
-										</BUTTON>
-								    {% endif %}
-								{% endfor %}
+								<UL>
+									{% for rule_template in
+									admin_info.user_info.active_rule_result_info.applying_rule_text_templates %}
+									<LI>{{ _(rule_template[0])|format(rule_template[1])|safe }}</LI>
+									{% endfor %}
+								</UL>
 							</DIV>
 
 						</DIV>
-			        {% endif %}
-			    	<DIV CLASS="row ALTERNATE_ROWLEVEL_1 TITLE_ROW">
-			    		<DIV CLASS="hidden-xs hidden-sm col-md-1"></DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-2  col-md-2 localetext">{{_('Day')}}</DIV>
-			    		<DIV CLASS="hidden-xs hidden-sm col-md-2 localetext">{{_('Context')}}</DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Min Time of Day')}}</DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Max Time of Day')}}</DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Time per Day')}}</DIV>
-						<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
-						<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-						<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-1  col-md-1 localetext">{{_('Minimum Break')}}</DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-1  col-md-1 localetext">{{_('Max Duration')}}</DIV>
-			    		<DIV CLASS="col-xs-3  col-sm-2  col-md-2 localetext">{{_('Free Play')}}</DIV>
-			    	</DIV>
-			    	{% for day_info in admin_info.day_infos %}
-			    	   	{% call accordion.begin() %}{{day_info.html_key}}{% endcall %}
-				    		<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
-				    			<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1 "></DIV>
-				    			<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg localetext">
-									<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-									<!-- {{ _('Show overrides for day') }}-->
-				    				{% call accordion.toggle_begin(tooltip="Show overrides for day") %}{{day_info.html_key}}{% endcall %}
-        								<!-- { { _(day_info.short_label[0])|format(day_info.short_label[1]) }} -->
-        								{{ day_info.reference_date|format_babel_date(_(day_info.short_format))|safe }}
-				        			{{ accordion.toggle_end() }}
-					    		</DIV>
-				    			<DIV CLASS="hidden-xs col-sm-2 col-md-2 localetext">
-				    				{% call accordion.toggle_begin(tooltip="Show overrides for day") %}{{day_info.html_key}}{% endcall %}
-        								<!-- { { _(day_info.label[0])|format(day_info.label[1]) }} -->
-        								{{ day_info.reference_date|format_babel_date(_(day_info.long_format))|safe }}
-				        			{{ accordion.toggle_end() }}
-								</DIV>
-								<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-2  CONTEXT localetext">{{
-									_(day_info.rule_set.label) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.min_time_of_day_class }} ">
-									{{ day_info.effective_rule_set.min_time_of_day|time_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_time_of_day_class }} ">
-									{{ day_info.effective_rule_set.max_time_of_day|time_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_time_per_day_class }} ">
-									{{ day_info.effective_rule_set.max_time_per_day|seconds_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
-								<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg "></DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  {{ day_info.effective_rule_set.min_break_class }} ">
-									{{ day_info.effective_rule_set.min_break|seconds_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_activity_duration_class }} ">
-									{{ _(day_info.effective_rule_set.max_activity_duration|seconds_to_string) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  {{ day_info.effective_rule_set.free_play_class }} localetext">
-									{{ day_info.effective_rule_set.free_play|boolean_to_string|_base }}
-								</DIV>
-							</DIV>
-					    {% call accordion.details() %}{{day_info.html_key}}{% endcall %}
-				    		<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
-				    			<DIV CLASS="hidden-xs hidden-sm col-md-3  col-lg-3  "></DIV>
-								<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-2  CONTEXT localetext">{{
-									_(day_info.rule_set.label) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  hidden-md hidden-lg CONTEXT localetext">{{
-									_(day_info.rule_set.label) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									day_info.rule_set.min_time_of_day|time_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									day_info.rule_set.max_time_of_day|time_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									day_info.rule_set.max_time_per_day|seconds_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
-								<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
-									day_info.rule_set.min_break|seconds_to_string }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
-									_(day_info.rule_set.max_activity_duration|seconds_to_string) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  localetext ">{{
-									day_info.rule_set.free_play|boolean_to_string|_base }}
+					{% call accordion.details() %}{{admin_info.html_key}}{% endcall %}
+						{% if admin_info.time_extension_periods|length > 0 %}
+							<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
+								<DIV CLASS="col-xs-2  col-sm-2  col-md-2  col-lg-2">
+								</DIV>
+								<DIV CLASS="col-xs-3  col-sm-3  col-md-3  col-lg-3 localetext">
+									{{ _("Manage Time Extension") }}
+								</DIV>
+								<DIV CLASS="col-xs-7  col-sm-7  col-md-7  col-lg-7 localetext">
+									{% for period in admin_info.time_extension_periods %}
+										{% if period == 0 %}
+											{% set period_string = - period %}
+											<BUTTON id="time_extension_{{ admin_info.username }}_0"
+													class="btn btn-time-extension-off" type="submit" name="submit"
+													value="time_extension_{{ admin_info.username }}_0"
+													title="{{_('Deactivate time extension')}}">
+												<I class="fas fa-power-off"></I>
+											</BUTTON>
+										{% elif period < 0 %}
+											{% set period_string = - period %}
+											<BUTTON id="time_extension_{{ admin_info.username }}_{{period}}"
+													class="btn btn-time-extension-minus" type="submit" name="submit"
+													value="time_extension_{{ admin_info.username }}_{{period}}"
+													title="{{_('Decrease time extension by {minutes} minutes')|format({'minutes':period_string})}}">
+												<I class="far fa-minus-square"></I> {{ period_string }}
+											</BUTTON>
+										{% else %}
+											<BUTTON id="time_extension_{{ admin_info.username }}_{{period}}"
+													class="btn btn-time-extension-plus" type="submit" name="submit"
+													value="time_extension_{{ admin_info.username }}_{{period}}"
+													title="{{_('Increase time extension by {minutes} minutes')|format({'minutes':period})}}">
+												<I class="far fa-plus-square"></I> {{ period }}
+											</BUTTON>
+										{% endif %}
+									{% endfor %}
 								</DIV>
+
 							</DIV>
-				    		<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
-								<DIV CLASS="hidden-xs hidden-sm col-md-3  col-lg-3  "></DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  CONTEXT localetext">
-									{{_('override')}}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									helper.render_field(forms[day_info.html_key].min_time_of_day) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									helper.render_field(forms[day_info.html_key].max_time_of_day) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
-									helper.render_field(forms[day_info.html_key].max_time_per_day) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
-								<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-								<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
-									helper.render_field(forms[day_info.html_key].min_break) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
-									helper.render_field(forms[day_info.html_key].max_activity_duration) }}
-								</DIV>
-								<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  "><DIV CLASS="check-box-wrapper">{{
-									helper.render_field(forms[day_info.html_key].free_play) }}</DIV>
-								</DIV>
-								<DIV class="col-xs-1  col-sm-1  col-md-1  col-lg-1 text-right localetext">
-									<BUTTON id="save" class="btn" type="submit" name="submit" title="{{_('Save')}}">
-										<I class="fas fa-save"></I>
-									</BUTTON>
+						{% endif %}
+						<DIV CLASS="row ALTERNATE_ROWLEVEL_1 TITLE_ROW">
+							<DIV CLASS="hidden-xs hidden-sm col-md-1"></DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-2 localetext">{{_('Day')}}</DIV>
+							<DIV CLASS="hidden-xs hidden-sm col-md-2 localetext">{{_('Context')}}</DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Min Time of Day')}}</DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Max Time of Day')}}</DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-1 localetext">{{_('Time per Day')}}</DIV>
+							<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
+							<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+							<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
+							<DIV CLASS="col-xs-3  col-sm-1  col-md-1 localetext">{{_('Minimum Break')}}</DIV>
+							<DIV CLASS="col-xs-3  col-sm-1  col-md-1 localetext">{{_('Max Duration')}}</DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-2 localetext">{{_('Free Play')}}</DIV>
+						</DIV>
+						{% for day_info in admin_info.day_infos %}
+							{% call accordion.begin() %}{{day_info.html_key}}{% endcall %}
+								<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
+									<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1 "></DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg localetext">
+										{#<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->#}
+										<!-- {{ _('Show overrides for day') }}-->
+										{% call accordion.toggle_begin(tooltip="Show overrides for day") %}{{day_info.html_key}}{% endcall %}
+											{{ day_info.reference_date|format_babel_date(_(day_info.short_format))|safe }}
+										{{ accordion.toggle_end() }}
+									</DIV>
+									<DIV CLASS="hidden-xs col-sm-2 col-md-2 localetext">
+										{% call accordion.toggle_begin(tooltip="Show overrides for day") %}{{day_info.html_key}}{% endcall %}
+											{{ day_info.reference_date|format_babel_date(_(day_info.long_format))|safe }}
+										{{ accordion.toggle_end() }}
+									</DIV>
+									<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-2  CONTEXT localetext">{{
+										_(day_info.rule_set.label) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.min_time_of_day_class }} ">
+										{{ day_info.effective_rule_set.min_time_of_day|time_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_time_of_day_class }} ">
+										{{ day_info.effective_rule_set.max_time_of_day|time_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_time_per_day_class }} ">
+										{{ day_info.effective_rule_set.max_time_per_day|seconds_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
+									<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg "></DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  {{ day_info.effective_rule_set.min_break_class }} ">
+										{{ day_info.effective_rule_set.min_break|seconds_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  {{ day_info.effective_rule_set.max_activity_duration_class }} ">
+										{{ _(day_info.effective_rule_set.max_activity_duration|seconds_to_string) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  {{ day_info.effective_rule_set.free_play_class }} localetext">
+										{{ day_info.effective_rule_set.free_play|boolean_to_string|_base }}
+									</DIV>
+								</DIV>
+							{% call accordion.details() %}{{day_info.html_key}}{% endcall %}
+								<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
+									<DIV CLASS="hidden-xs hidden-sm col-md-3  col-lg-3  "></DIV>
+									<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-2  CONTEXT localetext">{{
+										_(day_info.rule_set.label) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  hidden-md hidden-lg CONTEXT localetext">{{
+										_(day_info.rule_set.label) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										day_info.rule_set.min_time_of_day|time_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										day_info.rule_set.max_time_of_day|time_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										day_info.rule_set.max_time_per_day|seconds_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
+									<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
+										day_info.rule_set.min_break|seconds_to_string }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
+										_(day_info.rule_set.max_activity_duration|seconds_to_string) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  localetext ">{{
+										day_info.rule_set.free_play|boolean_to_string|_base }}
+									</DIV>
+								</DIV>
+								<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
+									<DIV CLASS="hidden-xs hidden-sm col-md-3  col-lg-3  "></DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  CONTEXT localetext">
+										{{_('override')}}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										helper.render_field(forms[day_info.html_key].min_time_of_day) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										helper.render_field(forms[day_info.html_key].max_time_of_day) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  ">{{
+										helper.render_field(forms[day_info.html_key].max_time_per_day) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg SEPERATOR_ROW"></DIV>
+									<DIV CLASS="col-xs-9  hidden-sm hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+									<DIV CLASS="col-xs-3  hidden-sm hidden-md hidden-lg"></DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
+										helper.render_field(forms[day_info.html_key].min_break) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  ">{{
+										helper.render_field(forms[day_info.html_key].max_activity_duration) }}
+									</DIV>
+									<DIV CLASS="col-xs-3  col-sm-1  col-md-1  col-lg-1  "><DIV CLASS="check-box-wrapper">{{
+										helper.render_field(forms[day_info.html_key].free_play) }}</DIV>
+									</DIV>
+									<DIV class="col-xs-1  col-sm-1  col-md-1  col-lg-1 text-right localetext">
+										<BUTTON id="save" class="btn" type="submit" name="submit" title="{{_('Save')}}">
+											<I class="fas fa-save"></I>
+										</BUTTON>
+									</DIV>
 								</DIV>
-							</DIV>
-						{{ accordion.end() }}    	
-			    	{% endfor %}
-				{{ accordion.end() }}
-	    	{% endfor %}
-	    </DIV>
-    </FORM>    		
-    
-    
+							{{ accordion.end() }}
+						{% endfor %}
+					{{ accordion.end() }}
+				{% endfor %}
+			</DIV>
+		</FORM>
+	</DIV>
+
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
 
 	{% for admin_info in admin_infos %}
     	{% call accordion.script() %}{{admin_info.html_key}}{% endcall %}
     	{% for day_info in admin_info.day_infos %}
     		{% call accordion.script() %}{{day_info.html_key}}{% endcall %}    		    			        
     	{% endfor %}
 	{% endfor %}
-
   </BODY>
-  
 </HTML>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
+{##}
 {% import 'bootstrap_accordion.macros.html' as accordion %} {% import
 'helper.macros.html' as helper %} {{ helper.locale_font(rel_font_size) }}
 
 
 
 
 
 
 
-{{ helper.fontawesome_script() }} {% include 'navbar.include.html' %}
-
+{{ helper.fontawesome_script() }}
+{% include 'navbar.include.html' %} {% include 'version_check.include.html' %}
+{##}
 {{_('User')}}
 {% for admin_info in admin_infos %} {% call accordion.begin() %}{
 {admin_info.html_key}}{% endcall %}
-  {% call accordion.toggle_begin(tooltip="Show configurations of upcoming
+{##}  {% call accordion.toggle_begin(tooltip="Show configurations of upcoming
 days") %}{{admin_info.html_key}}{% endcall %} {{ admin_info.full_name }} {
 { helper.check_or_cross(admin_info.user_info.activity_permitted) }} {
 { accordion.toggle_end() }}
 {% if admin_info.user_info.active_stat_info is defined %} {{_("Today's
 Activity")}}:  {
 {
 admin_info.user_info.active_stat_info.todays_activity_duration|seconds_to_string
@@ -44,19 +46,19 @@
 {{_('Time per Day')}}
  
 {{_('Minimum Break')}}
 {{_('Max Duration')}}
 {{_('Free Play')}}
 {% for day_info in admin_info.day_infos %} {% call accordion.begin() %}{
 {day_info.html_key}}{% endcall %}
-  {% call accordion.toggle_begin(tooltip="Show overrides for day") %}{
-{day_info.html_key}}{% endcall %}  {{ day_info.reference_date|format_babel_date
+{##}  {% call accordion.toggle_begin(tooltip="Show overrides for day") %}{
+{day_info.html_key}}{% endcall %} {{ day_info.reference_date|format_babel_date
 (_(day_info.short_format))|safe }} {{ accordion.toggle_end() }}
 {% call accordion.toggle_begin(tooltip="Show overrides for day") %}{
-{day_info.html_key}}{% endcall %}  {{ day_info.reference_date|format_babel_date
+{day_info.html_key}}{% endcall %} {{ day_info.reference_date|format_babel_date
 (_(day_info.long_format))|safe }} {{ accordion.toggle_end() }}
 {{ _(day_info.rule_set.label) }}
 {{ day_info.effective_rule_set.min_time_of_day|time_to_string }}
 {{ day_info.effective_rule_set.max_time_of_day|time_to_string }}
 {{ day_info.effective_rule_set.max_time_per_day|seconds_to_string }}
 {{ day_info.effective_rule_set.min_break|seconds_to_string }}
 {{ _(day_info.effective_rule_set.max_activity_duration|seconds_to_string) }}
```

### Comparing `little-brother-0.4.8/little_brother/templates/bootstrap_accordion.macros.html` & `little-brother-0.4.9/little_brother/templates/bootstrap_accordion.macros.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!--
+{#<!--
 #    Copyright (C) 2019  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 {% macro begin() -%}
 <DIV ID="accordion{{caller()}}" ROLE="tablist">
   	<DIV CLASS="card">
     	<DIV CLASS="card-header" ROLE="tab" ID="summary{{caller()}}">
 {%- endmacro %}
 
@@ -41,27 +41,29 @@
 <A data-toggle="collapse" href="#details{{caller()}}" aria-expanded="false" aria-controls="details{{caller()}}" TITLE="{{ _(tooltip) }}">
 {%- endmacro %}
 
 {% macro toggle_end() -%}
 </A>
 {%- endmacro %}
 
+{#
 // The following comments have deliberately been moved out of the macro to reduce the size of the generated file.
 
 // The following code snippet is based on https://www.geekpub.de/2015/01/bootstrap-3-accordion-status-merken-mit-cookies/
 // ad (1): The following handler creates a cookie if the accordion is not collapsed.
 
 // ad (2): The following handler removes the cookie when the accordion is collapsed.
 // In the following handler we have to make sure we only call the Cookies.remove method for the
 // element by which the trigger was raised. In Bootstrap (or JavaScript?) there seems to be a mechanism which makes the event
 // travel up the DOM tree so that the trigger handler is also called for enclosing accordions. This would lead to the cookies
 // of whole path of accordions up the root be removed and hence to be collapsed.
 // The correction is based on https://stackoverflow.com/questions/32070392/jquery-show-bs-collapse-event-for-nested-bootstrap-collapsible-buttons-fires-on
 
 // ad (3): The following is executed when the page is loaded. It opens the accordion when a matching cookie is found.
+#}
 
 {% macro script() -%}
 <SCRIPT type="text/javascript">
 	// (1)
 	$("#accordion{{caller()}}").on('shown.bs.collapse', function () {
         var active = $("#accordion{{caller()}} .in").attr('id');
         Cookies.set('activeAccordionGroup_{{caller()}}', active);
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
- {% macro begin() -%}
+{##} {% macro begin() -%}
 {%- endmacro %} {% macro details() -%}
 {%- endmacro %} {% macro end() -%}
 {%- endmacro %} {% macro toggle_begin(tooltip='') -%} {%-_endmacro_%}_{%_macro
-toggle_end()_-%} {%- endmacro %} // The following comments have deliberately
+toggle_end()_-%} {%- endmacro %} {# // The following comments have deliberately
 been moved out of the macro to reduce the size of the generated file. // The
 following code snippet is based on https://www.geekpub.de/2015/01/bootstrap-3-
 accordion-status-merken-mit-cookies/ // ad (1): The following handler creates a
 cookie if the accordion is not collapsed. // ad (2): The following handler
 removes the cookie when the accordion is collapsed. // In the following handler
 we have to make sure we only call the Cookies.remove method for the // element
 by which the trigger was raised. In Bootstrap (or JavaScript?) there seems to
 be a mechanism which makes the event // travel up the DOM tree so that the
 trigger handler is also called for enclosing accordions. This would lead to the
 cookies // of whole path of accordions up the root be removed and hence to be
 collapsed. // The correction is based on https://stackoverflow.com/questions/
 32070392/jquery-show-bs-collapse-event-for-nested-bootstrap-collapsible-
 buttons-fires-on // ad (3): The following is executed when the page is loaded.
-It opens the accordion when a matching cookie is found. {% macro script() -%}
+It opens the accordion when a matching cookie is found. #} {% macro script() -
+%}
  {%- endmacro %}
```

### Comparing `little-brother-0.4.8/little_brother/templates/devices.template.html` & `little-brother-0.4.9/little_brother/templates/devices.template.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!--
-#    Copyright (C) 2019  Marcus Rickert
+{#<!--
+#    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -12,15 +12,16 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
+
 <HTML>
 {% import 'bootstrap_accordion.macros.html' as accordion %}
 {% import 'helper.macros.html' as helper %}
 
 {{ helper.locale_font(rel_font_size) }}
 
 <HEAD>
@@ -39,97 +40,100 @@
     <TITLE>LittleBrother-{{_('Device Configuration')}}</TITLE>
     
   </HEAD>
 
 
   <BODY>
     {{ helper.fontawesome_script() }}
-	{% include 'navbar.include.html' %}
 
-	<FORM ACTION="{{ url_for('devices.main_view') }}" METHOD="POST" CLASS="form-horizontal">
-		<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
-		<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
-	    <DIV CLASS="container STANDARD_TABLE">
-	    	<DIV CLASS="row ALTERNATE2_ROWLEVEL_1 TITLE_ROW">
-	    		<DIV CLASS="col-xs-2 localetext">{{_('Device')}}</DIV>
-				<DIV CLASS="col-xs-9 hidden-xs"></DIV>
-				<DIV CLASS="col-xs-1 hidden-xs text-right">
-						<BUTTON id="add_device" type="submit" name="submit" class="btn" title="{{_('Add device')}}"
-								value="{{ new_device_submit_value }}"><I class="fas fa-plus"></I></BUTTON>
-				</DIV>
-	    	</DIV>
-	    	{% for device in devices %}
-	    	   	{% call accordion.begin() %}{{device.html_key}}{% endcall %}
-	    	
-			    	<DIV CLASS="row ALTERNATE2_ROWLEVEL_2">
-			    		<DIV CLASS="col-xs-3  col-sm-3  col-md-2  col-lg-2">
-							<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-							<!-- {{ _('Edit device details') }} -->
-		    				{% call accordion.toggle_begin(tooltip="Edit device details") %}{{device.html_key}}{% endcall %}
-							{{ device.device_name }}
-			        		{{ accordion.toggle_end() }}
-		        		</DIV>
-						<DIV CLASS="col-xs-6  col-sm-6  col-md-8  col-lg-8 localetext">
-							{{ device.summary|format_text_array|safe }}
+	<DIV class="container-fluid">
+		{% include 'navbar.include.html' %}
+		{% include 'version_check.include.html' %}
+
+		<FORM ACTION="{{ url_for('devices.main_view') }}" METHOD="POST" CLASS="form-horizontal">
+			<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
+			<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
+			<DIV CLASS="container STANDARD_TABLE">
+				<DIV CLASS="row ALTERNATE2_ROWLEVEL_1 TITLE_ROW">
+					<DIV CLASS="col-xs-2 localetext">{{_('Device')}}</DIV>
+					<DIV CLASS="col-xs-9 hidden-xs"></DIV>
+					<DIV CLASS="col-xs-1 hidden-xs text-right">
+							<BUTTON id="add_device" type="submit" name="submit" class="btn" title="{{_('Add device')}}"
+									value="{{ new_device_submit_value }}"><I class="fas fa-plus"></I></BUTTON>
+					</DIV>
+				</DIV>
+				{% for device in devices %}
+					{% call accordion.begin() %}{{device.html_key}}{% endcall %}
+
+						<DIV CLASS="row ALTERNATE2_ROWLEVEL_2">
+							<DIV CLASS="col-xs-3  col-sm-3  col-md-2  col-lg-2">
+								<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
+								<!-- {{ _('Edit device details') }} -->
+								{% call accordion.toggle_begin(tooltip="Edit device details") %}{{device.html_key}}{% endcall %}
+								{{ device.device_name }}
+								{{ accordion.toggle_end() }}
+							</DIV>
+							<DIV CLASS="col-xs-6  col-sm-6  col-md-8  col-lg-8 localetext">
+								{{ device.summary|format_text_array|safe }}
+							</DIV>
+							<DIV class="col-xs-3  col-sm-3  col-md-2  col-lg-2 text-right localetext">
+								<BUTTON id="{{ device.delete_html_key }}" class="btn" title="{{_('Remove device from monitoring')}}"><I class="fas fa-trash"></I></BUTTON>
+								<BUTTON id="save" type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
+							</DIV>
 						</DIV>
-		        		<DIV class="col-xs-3  col-sm-3  col-md-2  col-lg-2 text-right localetext">
-							<BUTTON id="{{ device.delete_html_key }}" class="btn" title="{{_('Remove device from monitoring')}}"><I class="fas fa-trash"></I></BUTTON>
-							<BUTTON id="save" type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
-		        		</DIV>
-			    	</DIV>			    			        
-			    {% call accordion.details() %}{{device.html_key}}{% endcall %}
-			<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW">
-				<DIV CLASS="col-xs-1 "></DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-3 localetext">{{_('Name')}}</DIV>
-				<DIV CLASS="col-xs-7  col-md-3  col-lg-5 localetext">{{_('Host Name')}}</DIV>
-				<!-- line break for xs -->
-				<DIV CLASS="clearfix  visible-xs-block visible-sm-block"></DIV>
-				<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW"></DIV>
-				<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-				<!-- line break for xs -->
-				<DIV CLASS="col-xs-1  hidden-md hidden-lg  "></DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{_('Min Activity Duration [s]')}}</DIV>
-				<DIV CLASS="col-xs-3  col-md-2  col-lg-1 localetext">{{_('Sample Size')}}</DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{_('Max Active Response Delay [ms]')}}</DIV>
-			</DIV>
-			<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW">
-				<DIV CLASS="col-xs-1 "></DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-3 localetext">{{
-					helper.render_field(forms[device.device_name].device_name) }}
-				</DIV>
-				<DIV CLASS="col-xs-7  col-md-3  col-lg-5 localetext">{{
-					helper.render_field(forms[device.device_name].hostname) }}
-				</DIV>
-				<!-- line break for xs -->
-				<DIV CLASS="clearfix  visible-xs-block visible-sm-block"></DIV>
-				<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW"></DIV>
-				<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-				<!-- line break for xs -->
-				<DIV CLASS="col-xs-1 hidden-md hidden-lg  "></DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{
-					helper.render_field(forms[device.device_name].min_activity_duration) }}
-				</DIV>
-				<DIV CLASS="col-xs-3  col-md-2  col-lg-1 localetext">{{
-					helper.render_field(forms[device.device_name].sample_size) }}
-				</DIV>
-				<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{
-					helper.render_field(forms[device.device_name].max_active_ping_delay) }}
+					{% call accordion.details() %}{{device.html_key}}{% endcall %}
+				<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW">
+					<DIV CLASS="col-xs-1 "></DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-3 localetext">{{_('Name')}}</DIV>
+					<DIV CLASS="col-xs-7  col-md-3  col-lg-5 localetext">{{_('Host Name')}}</DIV>
+					<!-- line break for xs -->
+					<DIV CLASS="clearfix  visible-xs-block visible-sm-block"></DIV>
+					<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW"></DIV>
+					<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+					<!-- line break for xs -->
+					<DIV CLASS="col-xs-1  hidden-md hidden-lg  "></DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{_('Min Activity Duration [s]')}}</DIV>
+					<DIV CLASS="col-xs-3  col-md-2  col-lg-1 localetext">{{_('Sample Size')}}</DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{_('Max Active Response Delay [ms]')}}</DIV>
+				</DIV>
+				<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW">
+					<DIV CLASS="col-xs-1 "></DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-3 localetext">{{
+						helper.render_field(forms[device.device_name].device_name) }}
+					</DIV>
+					<DIV CLASS="col-xs-7  col-md-3  col-lg-5 localetext">{{
+						helper.render_field(forms[device.device_name].hostname) }}
+					</DIV>
+					<!-- line break for xs -->
+					<DIV CLASS="clearfix  visible-xs-block visible-sm-block"></DIV>
+					<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW"></DIV>
+					<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+					<!-- line break for xs -->
+					<DIV CLASS="col-xs-1 hidden-md hidden-lg  "></DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{
+						helper.render_field(forms[device.device_name].min_activity_duration) }}
+					</DIV>
+					<DIV CLASS="col-xs-3  col-md-2  col-lg-1 localetext">{{
+						helper.render_field(forms[device.device_name].sample_size) }}
+					</DIV>
+					<DIV CLASS="col-xs-4  col-md-2  col-lg-1 localetext">{{
+						helper.render_field(forms[device.device_name].max_active_ping_delay) }}
+					</DIV>
 				</DIV>
+					{{ accordion.end() }}
+				{% endfor %}
 			</DIV>
-				{{ accordion.end() }}
-	    	{% endfor %}
-	    </DIV>
-
-		<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
-		<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
-		<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
-		<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
-
-		{% for device in devices %}
-			{{ helper.modal_confirm(device.delete_html_key, _("Do you really want to permanently remove the device from monitoring?"), _("Remove from Monitoring"), _("Cancel")) }}
-			{% call accordion.script() %}{{device.html_key}}{% endcall %}
-		{% endfor %}
-    </FORM>
+
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
+
+			{% for device in devices %}
+				{{ helper.modal_confirm(device.delete_html_key, _("Do you really want to permanently remove the device from monitoring?"), _("Remove from Monitoring"), _("Cancel")) }}
+				{% call accordion.script() %}{{device.html_key}}{% endcall %}
+			{% endfor %}
+		</FORM>
+	</DIV>
 
   </BODY>
-  
 </HTML>
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
+{##}
 {% import 'bootstrap_accordion.macros.html' as accordion %} {% import
 'helper.macros.html' as helper %} {{ helper.locale_font(rel_font_size) }}
 
 
 
 
 
 
 
-{{ helper.fontawesome_script() }} {% include 'navbar.include.html' %}
+{{ helper.fontawesome_script() }}
+{% include 'navbar.include.html' %} {% include 'version_check.include.html' %}
 
 {{_('Device')}}
 {% for device in devices %} {% call accordion.begin() %}{{device.html_key}}{%
 endcall %}
   {% call accordion.toggle_begin(tooltip="Edit device details") %}{
 {device.html_key}}{% endcall %} {{ device.device_name }} {
 { accordion.toggle_end() }}
 {{ device.summary|format_text_array|safe }}
 
- {% call accordion.details() %}{{device.html_key}}{% endcall %}
+{% call accordion.details() %}{{device.html_key}}{% endcall %}
 {{_('Name')}}
 {{_('Host Name')}}
 {{_('Min Activity Duration [s]')}}
 {{_('Sample Size')}}
 {{_('Max Active Response Delay [ms]')}}
 {{ helper.render_field(forms[device.device_name].device_name) }}
 {{ helper.render_field(forms[device.device_name].hostname) }}
```

### Comparing `little-brother-0.4.8/little_brother/templates/helper.macros.html` & `little-brother-0.4.9/little_brother/templates/helper.macros.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!--
+{#<!--
 #    Copyright (C) 2019  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 {% macro render_field(field, read_only=False, rows=None) %}
 {% if field.errors %}
 <div class="has-error">
     {% if field.extra_css_classes is defined %}
     {{ field(class_="form-control " + field.extra_css_classes, readonly=read_only, rows=rows) }}
     {% else %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
- {% macro render_field(field, read_only=False, rows=None) %} {% if field.errors
-%}
+{##} {% macro render_field(field, read_only=False, rows=None) %} {% if
+field.errors %}
 {% if field.extra_css_classes is defined %} {{ field(class_="form-control " +
 field.extra_css_classes, readonly=read_only, rows=rows) }} {% else %} {{ field
 (class_="form-control", readonly=read_only, rows=rows) }} {% endif %}  {% if
 field.errors|length == 1 %} {{ field.errors[0]|_base }} {% else %}
     * {% for error in field.errors %}
     * {{ error|_base }}
     * {% endfor %}
```

### Comparing `little-brother-0.4.8/little_brother/templates/internal_error.template.html` & `little-brother-0.4.9/little_brother/templates/internal_error.template.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!--
+{#<!--
 #    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
@@ -12,21 +12,21 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 <HTML>
 {% import 'helper.macros.html' as helper %}
   {{ helper.locale_font(rel_font_size) }}
 
-  <META http-equiv="Content-Type" content="text/html;charset=UTF-9">
+  <META http-equiv="Content-Type" content="text/html;charset=UTF-8">
   <HEAD>
       <META http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/bootstrap-theme.min.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/main.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
```

#### html2text {}

 * *error from `html2text {}` (a):*

 * *Recoding from 'UTF-9' to 'UTF-8' is not available.*

 * *Check that 'UTF-9' is a valid encoding.*

```diff
@@ -0,0 +1,16 @@
+{##}
+{% import 'helper.macros.html' as helper %} {{ helper.locale_font
+(rel_font_size) }}
+
+
+
+
+
+
+
+{{ helper.fontawesome_script() }}
+                                   [Brand]
+                          ***** Little Brother *****
+
+                     **** An internal error occurred! ****
+                             {{ error_message }}
```

### Comparing `little-brother-0.4.8/little_brother/templates/login.template.html` & `little-brother-0.4.9/little_brother/templates/login.template.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- https://codepen.io/ace-subido/pen/Cuiep -->
+{#<!-- https://codepen.io/ace-subido/pen/Cuiep -->#}
 {% import 'helper.macros.html' as helpers %}
 
 <HTML>
   {{ helpers.locale_font(rel_font_size) }}
 
   <META http-equiv="Content-Type" content="text/html;charset=UTF-8">
   <HEAD>
@@ -25,33 +25,26 @@
       <META name="viewport" content="width=device-width, initial-scale=1">
 
       <TITLE>LittleBrother-{{_('Login')}}</TITLE>
 
   </HEAD>
 
   <BODY>
-    <!-- { % include 'navbar.include.html' % } -->
-
     <div class="wrapper">
     	<form class="form-signin" ACTION="" METHOD="post">
  		    <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
             <h2 class="form-signin-heading localetext"><IMG
                     SRC="{{url_for('little_brother.static', filename='icons/icon-baby-panda-128x128.png')}}">
                 <div>Little Brother</div>
             </h2>
 
             {{ helpers.render_flashed_messages() }}
 
   			<input type="text" class="form-control localetext" name="username" placeholder="{{_('Username')}}" required="" autofocus="" />
   			<input type="password" class="form-control localetext" name="password" placeholder="{{_('Password')}}" required=""/>
-  			<!--      
-  			<label class="checkbox">
-    			<input type="checkbox" value="remember-me" id="rememberMe" name="rememberMe"> Remember me
-  			</label>
-  			-->
       		<button class="btn btn-lg btn-primary btn-block localetext" type="submit">{{_('Login')}}</button>
 	    </form>
   	</div>
 
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
     <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
- {% import 'helper.macros.html' as helpers %}
+{##} {% import 'helper.macros.html' as helpers %}
 {{ helpers.locale_font(rel_font_size) }}
 
 
 
 
 
 
 
 
 [{{url_for('little_brother.static', filename='icons/icon-baby-panda-
 128x128.png')}}]
 Little Brother
 {{ helpers.render_flashed_messages() }} [username            ]
-[********************]  {{_('Login')}}
+[********************] {{_('Login')}}
```

### Comparing `little-brother-0.4.8/little_brother/templates/navbar.include.html` & `little-brother-0.4.9/little_brother/templates/navbar.include.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!--
-#    Copyright (C) 2019  Marcus Rickert
+{#<!--
+#    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -12,18 +12,17 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
     <nav class="navbar navbar-default">
-	  <div class="container-fluid">
 	    <div class="navbar-header">
 			<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar-collapse-1" aria-expanded="false" aria-controls="navbar">
               <span class="sr-only">Toggle navigation</span>
               <span class="icon-bar"></span>
               <span class="icon-bar"></span>
               <span class="icon-bar"></span>
             </button>
@@ -51,9 +50,8 @@
 	      <form class="navbar-form navbar-right" ACTION="{{ url_for('auth.logout') }}" METHOD="POST">
 			  <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
 			  <button type="submit" class="btn btn-default localetext" title="{{_('Logout')}}"><I
 					  class="fas fa-sign-out-alt"></I></button>
 		  </form>
 	      {% endif %}
 		</div><!-- /.navbar-collapse -->
-	  </div><!-- /.container-fluid -->
 	</nav>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-
+{##}
  Toggle navigation
 [Brand] Little Brother
     * % if navigation.current_view == "status.main_view" %}class="active"{%
       endif %}>{{_('Status')}}_(current)
 % if navigation.current_view == "admin.main_view" %}class="active"{% endif %}>{
 {_('Admin')}}_(current)
 % if navigation.current_view == "users.main_view" %}class="active"{% endif %}>{
```

### Comparing `little-brother-0.4.8/little_brother/templates/status.template.html` & `little-brother-0.4.9/little_brother/templates/status.template.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!--
+{#<!--
 #    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 <HTML>
 {% import 'bootstrap_accordion.macros.html' as accordion %}
 {% import 'helper.macros.html' as helper %}
 
   {{ helper.locale_font(rel_font_size) }}
 
@@ -42,167 +42,168 @@
             HREF="{{ url_for('little_brother.static', filename='icons/baby-panda-32x32.ico') }}">
 
       <TITLE>LittleBrother-{{ _('Status')}}</TITLE>
   </HEAD>
 
   <BODY>
     {{ helper.fontawesome_script() }}
-	{% include 'navbar.include.html' %}
-    <DIV CLASS="container STANDARD_TABLE container">
-    	<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
-			<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('User')}}</DIV>
-			<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('Context')}}</DIV>
-
-			<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-1  localetext">
-				{{_("Today's Activity")}}
-				{% if has_downtime_today %}
-				<DIV CLASS="downtime"> {{_("Downtime")}}</DIV>
-				{% endif %}
-			</DIV>
-			<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Today')}}</DIV>
+	<DIV class="container-fluid">
+		{% include 'navbar.include.html' %}
+		<DIV CLASS="container STANDARD_TABLE container">
+			<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
+				<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('User')}}</DIV>
+				<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('Context')}}</DIV>
+
+				<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-1  localetext">
+					{{_("Today's Activity")}}
+					{% if has_downtime_today %}
+					<DIV CLASS="downtime"> {{_("Downtime")}}</DIV>
+					{% endif %}
+				</DIV>
+				<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Today')}}</DIV>
 
-			<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Previous Activity Start Time')}}</DIV>
-			<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Previous Activity End Time')}}</DIV>
-			<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Current Activity Start Time')}}</DIV>
-
-			<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-1  localetext">{{_('Current Activity Duration')}}</DIV>
-			<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Current')}}</DIV>
-
-			<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  center  localetext">{{_('Activity permitted')}}</DIV>
-    		<DIV CLASS="col-xs-1  col-sm-1  col-md-1  hidden-lg center  localetext">{{_('OK?')}}</DIV>
-    		<!--<DIV CLASS="col-xs-1 hidden-sm hidden-md hidden-lg"></DIV> -->
-    		<DIV CLASS="hidden-xs col-sm-5  col-md-3 col-lg-4 localetext">{{_('Reasons')}}</DIV>
-    	</DIV>
-		{% for user_info in user_infos %}
-			{% set username = user_info.username %}
-	    	{% call accordion.begin() %}status_{{username}}_summary{% endcall %}	    			        
-		    	<DIV CLASS="row ROWLEVEL_2">
-		    		<DIV CLASS="col-xs-3  col-sm-2            col-lg-1 ">
-						<!-- {{ _('Show durations of most recent days') }} -->
-						{% call accordion.toggle_begin(tooltip="Show durations of most recent days")
-						%}status_{{username}}_summary{% endcall %}
-						{{ user_info.active_stat_info.full_name }}
-						{{ accordion.toggle_end() }}
-					</DIV>
-		    		<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">
-						{{ _(user_info.active_rule_set.label) }}
-					</DIV>
-		    		<DIV CLASS="col-xs-2  col-sm-1  col-md-2  col-lg-1 ">
-						{{ user_info.active_stat_info.todays_activity_duration|seconds_to_string }} /
-						{% if user_info.active_rule_set.free_play %}
-						{{ _("unlimited") }}
-						{% else %}
-						{{ user_info.active_rule_set.max_time_per_day|seconds_to_string }}
-						{% endif %}
-						{% if user_info.active_stat_info.todays_downtime %}
-						<DIV CLASS="downtime"> {{user_info.active_stat_info.todays_downtime|seconds_to_string}}</DIV>
-						{% endif %}
-					</DIV>
+				<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Previous Activity Start Time')}}</DIV>
+				<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Previous Activity End Time')}}</DIV>
+				<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  localetext">{{_('Current Activity Start Time')}}</DIV>
+
+				<DIV CLASS="hidden-xs hidden-sm col-md-2  col-lg-1  localetext">{{_('Current Activity Duration')}}</DIV>
+				<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Current')}}</DIV>
+
+				<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1  center  localetext">{{_('Activity permitted')}}</DIV>
+				<DIV CLASS="col-xs-1  col-sm-1  col-md-1  hidden-lg center  localetext">{{_('OK?')}}</DIV>
+				<DIV CLASS="hidden-xs col-sm-5  col-md-3 col-lg-4 localetext">{{_('Reasons')}}</DIV>
+			</DIV>
+			{% for user_info in user_infos %}
+				{% set username = user_info.username %}
+				{% call accordion.begin() %}status_{{username}}_summary{% endcall %}
+					<DIV CLASS="row ROWLEVEL_2">
+						<DIV CLASS="col-xs-3  col-sm-2            col-lg-1 ">
+							<!-- {{ _('Show durations of most recent days') }} -->
+							{% call accordion.toggle_begin(tooltip="Show durations of most recent days")
+							%}status_{{username}}_summary{% endcall %}
+							{{ user_info.active_stat_info.full_name }}
+							{{ accordion.toggle_end() }}
+						</DIV>
+						<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">
+							{{ _(user_info.active_rule_set.label) }}
+						</DIV>
+						<DIV CLASS="col-xs-2  col-sm-1  col-md-2  col-lg-1 ">
+							{{ user_info.active_stat_info.todays_activity_duration|seconds_to_string }} /
+							{% if user_info.active_rule_set.free_play %}
+							{{ _("unlimited") }}
+							{% else %}
+							{{ user_info.active_rule_set.max_time_per_day|seconds_to_string }}
+							{% endif %}
+							{% if user_info.active_stat_info.todays_downtime %}
+							<DIV CLASS="downtime"> {{user_info.active_stat_info.todays_downtime|seconds_to_string}}</DIV>
+							{% endif %}
+						</DIV>
 
-		    		<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 ">
-						{{ user_info.active_stat_info.previous_activity_start_time|datetime_to_string }}
-					</DIV>
-		    		<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 ">
-						{{ user_info.active_stat_info.previous_activity_end_time|datetime_to_string }}
-					</DIV>
-		    		<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 {% if user_info.active_stat_info.current_activity_start_time %}blink{% endif %}">
-						{{ user_info.active_stat_info.current_activity_start_time|datetime_to_string }}
-					</DIV>
+						<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 ">
+							{{ user_info.active_stat_info.previous_activity_start_time|datetime_to_string }}
+						</DIV>
+						<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 ">
+							{{ user_info.active_stat_info.previous_activity_end_time|datetime_to_string }}
+						</DIV>
+						<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1 {% if user_info.active_stat_info.current_activity_start_time %}blink{% endif %}">
+							{{ user_info.active_stat_info.current_activity_start_time|datetime_to_string }}
+						</DIV>
 
-		    		<DIV CLASS="col-xs-2  col-sm-1  col-md-2  col-lg-1  {% if user_info.active_stat_info.current_activity_duration %}blink{% endif %}">
-						{{ user_info.active_stat_info.current_activity_duration|seconds_to_string }}
-						{% if user_info.active_stat_info.current_activity_downtime %}
-							<DIV CLASS="downtime"> {{user_info.active_stat_info.current_activity_downtime|seconds_to_string}}</DIV>
-						{% endif %}
-					</DIV>
+						<DIV CLASS="col-xs-2  col-sm-1  col-md-2  col-lg-1  {% if user_info.active_stat_info.current_activity_duration %}blink{% endif %}">
+							{{ user_info.active_stat_info.current_activity_duration|seconds_to_string }}
+							{% if user_info.active_stat_info.current_activity_downtime %}
+								<DIV CLASS="downtime"> {{user_info.active_stat_info.current_activity_downtime|seconds_to_string}}</DIV>
+							{% endif %}
+						</DIV>
 
-		    		<DIV CLASS="col-xs-1  col-sm-1  col-md-1  col-lg-1  center ">
-						{{ helper.check_or_cross(user_info.activity_permitted) }}
-					</DIV>
-		    		<DIV CLASS="col-xs-12 col-sm-5  col-md-3  col-lg-4 localetext">
-						<UL>
-			    		{% for rule_template in user_info.active_rule_result_info.applying_rule_text_templates %}
-			    			<LI>{{ _(rule_template[0])|format(rule_template[1]) }}</LI>
-			    		{% endfor %}
-						</UL>
-		    		</DIV>
-		    	</DIV>
-			{% call accordion.details() %}status_{{username}}_summary{% endcall %}
-				<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
-					<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1"></DIV>
-					<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('Day')}}</DIV>
-					<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">
-						{{_('Active Time')}}
-						{% if user_info.active_stat_info.has_downtime %}
-						<DIV CLASS="downtime"> {{_("Downtime")}}</DIV>
-						{% endif %}
+						<DIV CLASS="col-xs-1  col-sm-1  col-md-1  col-lg-1  center ">
+							{{ helper.check_or_cross(user_info.activity_permitted) }}
+						</DIV>
+						<DIV CLASS="col-xs-12 col-sm-5  col-md-3  col-lg-4 localetext">
+							<UL>
+							{% for rule_template in user_info.active_rule_result_info.applying_rule_text_templates %}
+								<LI>{{ _(rule_template[0])|format(rule_template[1]) }}</LI>
+							{% endfor %}
+							</UL>
+						</DIV>
 					</DIV>
-					<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Active')}}</DIV>
-					<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">{{_('Activity Start')}}</DIV>
-					<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Start')}}</DIV>
-					<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">{{_('Activity End')}}</DIV>
-					<DIV CLASS="hidden-xs col-sm-1  hidden-md hidden-lg localetext">{{_('End')}}</DIV>
-					<DIV CLASS="col-xs-5  col-sm-6  col-md-6  col-lg-7  localetext">{{_('Host(#procs)')}}</DIV>
-				</DIV>
-				{% for i in range (0, user_info.max_lookback_in_days) %}
-					{% call accordion.begin() %}status_{{username}}_{{i}}{% endcall %}
-						<DIV CLASS="row ROWLEVEL_3">
-							<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1"></DIV>
-							<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1 localetext">
-								<!-- {{ _('Show activity times') }} -->
-								{% call accordion.toggle_begin(tooltip='Show activity times') %}status_{{username}}_{{i}}{% endcall %}
-								{{ _(user_info.history_labels[i][0])|format(user_info.history_labels[i][1]) }}
-								{{ accordion.toggle_end() }}
-							</DIV>
-							<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">
-								{{ user_info.active_stat_info.day_statistics[i].duration|seconds_to_string }}
-								{% if user_info.active_stat_info.day_statistics[i].downtime %}
-								<DIV CLASS="downtime"> {{user_info.active_stat_info.day_statistics[i].downtime|seconds_to_string}}</DIV>
-								{% endif %}
-							</DIV>
-							<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">{{
-								user_info.active_stat_info.day_statistics[i].min_time|time_to_string }}
-							</DIV>
-							<DIV CLASS="hidden-xs col-sm-1  col-md-1  col-lg-1">{{
-								user_info.active_stat_info.day_statistics[i].max_time|time_to_string }}
-							</DIV>
-							<DIV CLASS="col-xs-5  col-sm-7  col-md-7  col-lg-7">{{
-								user_info.active_stat_info.day_statistics[i].host_infos }}
-							</DIV>
+				{% call accordion.details() %}status_{{username}}_summary{% endcall %}
+					<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
+						<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1"></DIV>
+						<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1  localetext">{{_('Day')}}</DIV>
+						<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">
+							{{_('Active Time')}}
+							{% if user_info.active_stat_info.has_downtime %}
+							<DIV CLASS="downtime"> {{_("Downtime")}}</DIV>
+							{% endif %}
 						</DIV>
-					{% call accordion.details() %}status_{{username}}_{{i}}{% endcall %}
-						{% for activity in user_info.active_stat_info.day_statistics[i].activities %}
-							<DIV CLASS="row ROWLEVEL_4 {% if not activity.end_time %}blink{% endif %}">
+						<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Active')}}</DIV>
+						<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">{{_('Activity Start')}}</DIV>
+						<DIV CLASS="col-xs-2  col-sm-1  hidden-md hidden-lg localetext">{{_('Start')}}</DIV>
+						<DIV CLASS="hidden-xs hidden-sm col-md-1  col-lg-1  localetext">{{_('Activity End')}}</DIV>
+						<DIV CLASS="hidden-xs col-sm-1  hidden-md hidden-lg localetext">{{_('End')}}</DIV>
+						<DIV CLASS="col-xs-5  col-sm-6  col-md-6  col-lg-7  localetext">{{_('Host(#procs)')}}</DIV>
+					</DIV>
+					{% for i in range (0, user_info.max_lookback_in_days) %}
+						{% call accordion.begin() %}status_{{username}}_{{i}}{% endcall %}
+							<DIV CLASS="row ROWLEVEL_3">
 								<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1"></DIV>
-								<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1"></DIV>
+								<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1 localetext">
+									<!-- {{ _('Show activity times') }} -->
+									{% call accordion.toggle_begin(tooltip='Show activity times') %}status_{{username}}_{{i}}{% endcall %}
+									{{ _(user_info.history_labels[i][0])|format(user_info.history_labels[i][1]) }}
+									{{ accordion.toggle_end() }}
+								</DIV>
 								<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">
-									{{ activity.duration|seconds_to_string }}
-									{% if activity.downtime %}
-									<DIV CLASS="downtime"> {{activity.downtime|seconds_to_string}}</DIV>
+									{{ user_info.active_stat_info.day_statistics[i].duration|seconds_to_string }}
+									{% if user_info.active_stat_info.day_statistics[i].downtime %}
+									<DIV CLASS="downtime"> {{user_info.active_stat_info.day_statistics[i].downtime|seconds_to_string}}</DIV>
 									{% endif %}
 								</DIV>
-								<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">{{ activity.start_time|time_to_string }}</DIV>
-								<DIV CLASS="hidden-xs col-sm-1  col-md-1  col-lg-1">{{ activity.end_time|time_to_string }}</DIV>
-								<DIV CLASS="col-xs-5  col-sm-7  col-md-7  col-lg-7">{{ activity.host_infos }}</DIV>
+								<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">{{
+									user_info.active_stat_info.day_statistics[i].min_time|time_to_string }}
+								</DIV>
+								<DIV CLASS="hidden-xs col-sm-1  col-md-1  col-lg-1">{{
+									user_info.active_stat_info.day_statistics[i].max_time|time_to_string }}
+								</DIV>
+								<DIV CLASS="col-xs-5  col-sm-7  col-md-7  col-lg-7">{{
+									user_info.active_stat_info.day_statistics[i].host_infos }}
+								</DIV>
 							</DIV>
-						{% endfor %} <!-- activity -->
-					{{ accordion.end() }}
-				{% endfor %} <!-- i -->
-			{{ accordion.end() }}
-    	{% endfor %} <!-- username -->
-    </DIV> <!-- CLASS="container" -->
-
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
+						{% call accordion.details() %}status_{{username}}_{{i}}{% endcall %}
+							{% for activity in user_info.active_stat_info.day_statistics[i].activities %}
+								<DIV CLASS="row ROWLEVEL_4 {% if not activity.end_time %}blink{% endif %}">
+									<DIV CLASS="hidden-xs hidden-sm hidden-md col-lg-1"></DIV>
+									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-1"></DIV>
+									<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">
+										{{ activity.duration|seconds_to_string }}
+										{% if activity.downtime %}
+										<DIV CLASS="downtime"> {{activity.downtime|seconds_to_string}}</DIV>
+										{% endif %}
+									</DIV>
+									<DIV CLASS="col-xs-2  col-sm-1  col-md-1  col-lg-1">{{ activity.start_time|time_to_string }}</DIV>
+									<DIV CLASS="hidden-xs col-sm-1  col-md-1  col-lg-1">{{ activity.end_time|time_to_string }}</DIV>
+									<DIV CLASS="col-xs-5  col-sm-7  col-md-7  col-lg-7">{{ activity.host_infos }}</DIV>
+								</DIV>
+							{% endfor %} {#<!-- activity -->#}
+						{{ accordion.end() }}
+					{% endfor %} {#<!-- i -->#}
+				{{ accordion.end() }}
+			{% endfor %} {#<!-- username -->#}
+		</DIV> {#<!-- CLASS="container" -->#}
+	</DIV>
+
+	<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
+	<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
+	<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
+	<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
 
 	{% for user_info in user_infos %}
 		{% set username = user_info.username %}
-    	{% call accordion.script() %}status_{{username}}_summary{% endcall %}
-    	{% for i in range (0, user_info.max_lookback_in_days) %}
+		{% call accordion.script() %}status_{{username}}_summary{% endcall %}
+		{% for i in range (0, user_info.max_lookback_in_days) %}
 			{% call accordion.script() %}status_{{username}}_{{i}}{% endcall %}
-    	{% endfor %}
+		{% endfor %}
 	{% endfor %}
 
   </BODY>
 </HTML>
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
+{##}
 {% import 'bootstrap_accordion.macros.html' as accordion %} {% import
 'helper.macros.html' as helper %} {{ helper.locale_font(rel_font_size) }}
 
 
 
 
 
 
 
 
-{{ helper.fontawesome_script() }} {% include 'navbar.include.html' %}
+{{ helper.fontawesome_script() }}
+{% include 'navbar.include.html' %}
 {{_('User')}}
 {{_('Context')}}
 {{_("Today's Activity")}} {% if has_downtime_today %}
 {{_("Downtime")}}
 {% endif %}
 {{_('Today')}}
 {{_('Previous Activity Start Time')}}
@@ -75,13 +77,14 @@
 activity in user_info.active_stat_info.day_statistics[i].activities %}
 {{ activity.duration|seconds_to_string }} {% if activity.downtime %}
 {{activity.downtime|seconds_to_string}}
 {% endif %}
 {{ activity.start_time|time_to_string }}
 {{ activity.end_time|time_to_string }}
 {{ activity.host_infos }}
-{% endfor %}  {{ accordion.end() }} {% endfor %}  {{ accordion.end() }} {%
-endfor %}
+{% endfor %} {##} {{ accordion.end() }} {% endfor %} {##} {{ accordion.end() }}
+{% endfor %} {##}
+{##}
  {% for user_info in user_infos %} {% set username = user_info.username %} {%
 call accordion.script() %}status_{{username}}_summary{% endcall %} {% for i in
 range (0, user_info.max_lookback_in_days) %} {% call accordion.script()
 %}status_{{username}}_{{i}}{% endcall %} {% endfor %} {% endfor %}
```

### Comparing `little-brother-0.4.8/little_brother/templates/users.template.html` & `little-brother-0.4.9/little_brother/templates/users.template.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!--
-#    Copyright (C) 2019  Marcus Rickert
+{#<!--
+#    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -12,15 +12,15 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
--->
+-->#}
 
 <HTML>
 {% import 'bootstrap_accordion.macros.html' as accordion %}
 {% import 'helper.macros.html' as helper %}
 
   {{ helper.locale_font(rel_font_size) }}
 
@@ -32,301 +32,305 @@
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/main.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/initializr/css/bootstrap.min.css') }}">
       <LINK REL="stylesheet" TYPE="text/css"
             HREF="{{ url_for('little_brother.static', filename='contrib/fontawesome/css/all.min.css') }}">
       <LINK REL="stylesheet" TYPE="text/css" HREF="{{ url_for('little_brother.static', filename='default.css') }}">
-      <!-- <LINK REL="stylesheet" TYPE="text/css" HREF="{{ url_for('little_brother.static', filename='contrib/font-awesome/font-awesome.min.css') }}"> -->
 
       <LINK REL="shortcut icon" TYPE="image/x-icon"
             HREF="{{ url_for('little_brother.static', filename='icons/baby-panda-32x32.ico') }}">
 
       <meta name="viewport" content="width=device-width, initial-scale=1">
 
       <TITLE>LittleBrother-{{_('User Configuration')}}</TITLE>
 
   </HEAD>
 
   <BODY>
 	{{ helper.fontawesome_script() }}
-	{% include 'navbar.include.html' %}
 
-	<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
-    <SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
-
-	<FORM ID="main_form" ACTION="{{ url_for('users.main_view') }}" METHOD="POST" CLASS="form-horizontal">
-		<!-- The following button ensures that pressing enter will trigger a normal save and not a more specialized
-		     button. -->
-		<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
-		<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
-	    <DIV CLASS="container STANDARD_TABLE">
-	    	<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
-				<DIV CLASS="col-lg-2 localetext">{{_('User')}}</DIV>
-				<DIV CLASS="col-lg-6"></DIV>
-				<DIV CLASS="col-lg-4 text-right">
-					<SPAN>
-					{% if forms[new_user_html_key] is defined %}
-	    				{{ _("Add to monitoring") }}:
-					    {{ forms[new_user_html_key].username(class_="form-control inline-field") }}
-			 			<BUTTON id="add_user" type="submit" name="submit" class="btn" title="{{_('Add User')}}"
-								value="{{ new_user_submit_value }}"><I class="fas fa-plus"></I></BUTTON>
-					{% endif %}
-					</SPAN>
+	<DIV class="container-fluid">
+		{% include 'navbar.include.html' %}
+		{% include 'version_check.include.html' %}
+
+		<FORM ID="main_form" ACTION="{{ url_for('users.main_view') }}" METHOD="POST" CLASS="form-horizontal">
+			{#<!-- The following button ensures that pressing enter will trigger a normal save and not a more specialized
+				 button. -->#}
+			<BUTTON type="submit" name="submit" style="visibility: hidden;"></BUTTON>
+			<input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
+			<DIV CLASS="container STANDARD_TABLE">
+				<DIV CLASS="row ROWLEVEL_1 TITLE_ROW">
+					<DIV CLASS="col-lg-2 localetext">{{_('User')}}</DIV>
+					<DIV CLASS="col-lg-6"></DIV>
+					<DIV CLASS="col-lg-4 text-right">
+						<SPAN>
+						{% if forms[new_user_html_key] is defined %}
+							{{ _("Add to monitoring") }}:
+							{{ forms[new_user_html_key].username(class_="form-control inline-field") }}
+							<BUTTON id="add_user" type="submit" name="submit" class="btn" title="{{_('Add User')}}"
+									value="{{ new_user_submit_value }}"><I class="fas fa-plus"></I></BUTTON>
+						{% endif %}
+						</SPAN>
+					</DIV>
 				</DIV>
-			</DIV>
-	    	{% for user in users %}
-				<!-- ************************************************************************************************-->
-				<!-- USER DETAILS                                                                                    -->
-				<!-- ************************************************************************************************-->
-
-	    	   	{% call accordion.begin() %}{{ user.html_key }}{% endcall %}
-			    	<DIV CLASS="row ROWLEVEL_2">
-			    		<DIV CLASS="col-xs-2  col-sm-2  col-md-2  col-lg-2">
-							<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-							<!-- {{ _('Edit user details') }} -->
-							{% call accordion.toggle_begin(tooltip="Edit user details") %}{{ user.html_key }}{% endcall
-							%}
-							{{ user.full_name }}
-							{{ accordion.toggle_end() }}
-						</DIV>
-			    		<DIV CLASS="col-xs-8  col-sm-7  col-md-8  col-lg-8 localetext">
-							{{ user.summary|format_text_array|safe }}
-						</DIV>
-		        		<DIV class="col-xs-2  col-sm-3  col-md-2  col-lg-2 text-right localetext">
-							<BUTTON id="{{ user.delete_html_key }}" class="btn" title="{{_('Remove user from monitoring')}}"><I class="fas fa-trash"></I></BUTTON>
-		        		</DIV>
-			    	</DIV>			    			        
-			    {% call accordion.details() %}{{user.html_key}}{% endcall %}
-			    	<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
-			    		<DIV CLASS="col-xs-1   col-sm-1  col-md-1           "></DIV>
-			    		<DIV CLASS="col-xs-2   col-sm-2  col-md-1           localetext">{{_('Monitored')}}</DIV>
-			    		<DIV CLASS="col-xs-3   col-sm-2  col-md-2           localetext">{{_('First Name')}}</DIV>
-			    		<DIV CLASS="col-xs-3   col-sm-2  col-md-2           localetext">{{_('Last Name')}}</DIV>
-						<DIV CLASS="col-xs-3   col-sm-2  col-md-2  col-lg-2 localetext">{{_('Locale')}}</DIV>
-			    		<DIV CLASS="hidden-xs  col-sm-3  col-md-4  col-lg-4 text-right localetext">
-							<BUTTON id="save" type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
-		        		</DIV>
-			    	</DIV>
-
-			    	<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
-			    		<DIV CLASS="col-xs-1   col-sm-1  col-md-1"></DIV>
-			    		<DIV CLASS="col-xs-2   col-sm-2  col-md-1                      ">{{ helper.render_field(forms[user.html_key].active) }}</DIV>
-			    		<DIV CLASS="col-xs-3   col-sm-2  col-md-2                      ">{{ forms[user.html_key].first_name(class_="form-control dense-font") }}</DIV>
-			    		<DIV CLASS="col-xs-3   col-sm-2  col-md-2                      ">{{ forms[user.html_key].last_name(class_="form-control dense-font") }}</DIV>
-			    		<DIV CLASS="col-xs-3   col-sm-2  col-md-2  col-lg-2  localetext">{{ forms[user.html_key].locale(class_="form-control dense-font") }}</DIV>
-			    		<DIV CLASS="hidden-xs  col-sm-3  col-md-4  col-lg-4  localetext"></DIV>
-			    	</DIV>
-
-					{% call accordion.begin() %}process_{{ user.html_key }}{% endcall %}
-			    	<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
-			    		<DIV CLASS="col-xs-1  col-sm-1  col-md-1           "></DIV>
-			    		<DIV CLASS="col-xs-11 col-sm-11 col-md-11 col-lg-11 localetext">
-							{% call accordion.toggle_begin(tooltip="Edit process patterns") %}process_{{ user.html_key }}{% endcall %}
-							{{_('Process Name Pattern')}}
-							{{ accordion.toggle_end() }}
+				{% for user in users %}
+					{#<!-- ************************************************************************************************-->
+					<!-- USER DETAILS                                                                                    -->
+					<!-- ************************************************************************************************-->#}
+
+					{% call accordion.begin() %}{{ user.html_key }}{% endcall %}
+						<DIV CLASS="row ROWLEVEL_2">
+							<DIV CLASS="col-xs-2  col-sm-2  col-md-2  col-lg-2">
+								{#<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->#}
+								<!-- {{ _('Edit user details') }} -->
+								{% call accordion.toggle_begin(tooltip="Edit user details") %}{{ user.html_key }}{% endcall
+								%}
+								{{ user.full_name }}
+								{{ accordion.toggle_end() }}
+							</DIV>
+							<DIV CLASS="col-xs-8  col-sm-7  col-md-8  col-lg-8 localetext">
+								{{ user.summary|format_text_array|safe }}
+							</DIV>
+							<DIV class="col-xs-2  col-sm-3  col-md-2  col-lg-2 text-right localetext">
+								<BUTTON id="{{ user.delete_html_key }}" class="btn" title="{{_('Remove user from monitoring')}}"><I class="fas fa-trash"></I></BUTTON>
+							</DIV>
 						</DIV>
-					</DIV>
-				    {% call accordion.details() %}process_{{user.html_key}}{% endcall %}
-			    	<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
-			    		<DIV CLASS="col-xs-1  col-sm-1  col-md-1  col-lg-1           "></DIV>
-						<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2 localetext">{{_('Login Process Name Pattern')}}</DIV>
-						<DIV CLASS="col-xs-8  col-sm-9  col-md-9  col-lg-9">
-							{{ helper.render_field(forms[user.html_key].process_name_pattern, rows=10) }}
+					{% call accordion.details() %}{{user.html_key}}{% endcall %}
+						<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
+							<DIV CLASS="col-xs-1   col-sm-1  col-md-1           "></DIV>
+							<DIV CLASS="col-xs-2   col-sm-2  col-md-1           localetext">{{_('Monitored')}}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2           localetext">{{_('First Name')}}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2           localetext">{{_('Last Name')}}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2  col-lg-2 localetext">{{_('Locale')}}</DIV>
+							<DIV CLASS="hidden-xs  col-sm-3  col-md-4  col-lg-4 text-right localetext">
+								<BUTTON id="save" type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
+							</DIV>
 						</DIV>
-					</DIV>
-			    	<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
-			    		<DIV CLASS="col-xs-1  col-sm-1  col-md-1  lol-lg-1           "></DIV>
-						<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2 localetext">{{_('Prohibited Process Name Pattern')}}</DIV>
-						<DIV CLASS="col-xs-8  col-sm-9  col-md-9  col-lg-9">
-							{{ helper.render_field(forms[user.html_key].prohibited_process_name_pattern, rows=10) }}
+
+						<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
+							<DIV CLASS="col-xs-1   col-sm-1  col-md-1"></DIV>
+							<DIV CLASS="col-xs-2   col-sm-2  col-md-1                      ">{{ helper.render_field(forms[user.html_key].active) }}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2                      ">{{ forms[user.html_key].first_name(class_="form-control dense-font") }}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2                      ">{{ forms[user.html_key].last_name(class_="form-control dense-font") }}</DIV>
+							<DIV CLASS="col-xs-3   col-sm-2  col-md-2  col-lg-2  localetext">{{ forms[user.html_key].locale(class_="form-control dense-font") }}</DIV>
+							<DIV CLASS="hidden-xs  col-sm-3  col-md-4  col-lg-4  localetext"></DIV>
 						</DIV>
-					</DIV>
- 					{{ accordion.end() }}
 
-					<!-- ********************************************************************************************-->
-					<!-- RULESETS                                                                                    -->
-					<!-- ********************************************************************************************-->
-
-	    	   	   	{% call accordion.begin() %}{{ user.rulesets_html_key }}{% endcall %}
-						<DIV CLASS="row ALTERNATE_ROWLEVEL_1">
-							<DIV CLASS="col-xs-1"></DIV>
-							<DIV CLASS="col-xs-9 localetext">
-								{% call accordion.toggle_begin(tooltip="Edit rulesets") %}{{ user.rulesets_html_key }}{%
-								endcall %}
-								{{_('Rulesets')}} ({{_('Count')}}: {{ user.sorted_rulesets|length }})
+						{% call accordion.begin() %}process_{{ user.html_key }}{% endcall %}
+						<DIV CLASS="row ROWLEVEL_3 TITLE_ROW dense-font">
+							<DIV CLASS="col-xs-1  col-sm-1  col-md-1           "></DIV>
+							<DIV CLASS="col-xs-11 col-sm-11 col-md-11 col-lg-11 localetext">
+								{% call accordion.toggle_begin(tooltip="Edit process patterns") %}process_{{ user.html_key }}{% endcall %}
+								{{_('Process Name Pattern')}}
 								{{ accordion.toggle_end() }}
 							</DIV>
-							<DIV class="col-xs-2 text-right">
-								<BUTTON id="{{ user.new_ruleset_html_key }}" type="submit" name="submit" class="btn"
-										title="{{_('Add ruleset')}}" value="{{ user.new_ruleset_html_key }}"><I class="fas fa-plus"></I></BUTTON>
+						</DIV>
+						{% call accordion.details() %}process_{{user.html_key}}{% endcall %}
+						<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
+							<DIV CLASS="col-xs-1  col-sm-1  col-md-1  col-lg-1           "></DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2 localetext">{{_('Login Process Name Pattern')}}</DIV>
+							<DIV CLASS="col-xs-8  col-sm-9  col-md-9  col-lg-9">
+								{{ helper.render_field(forms[user.html_key].process_name_pattern, rows=10) }}
 							</DIV>
 						</DIV>
-    			    {% call accordion.details() %}{{user.rulesets_html_key}}{% endcall %}
-						{% for ruleset in user.sorted_rulesets %}
-							{% call accordion.begin() %}{{ruleset.html_key}}{% endcall %}
-								<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
-									<DIV CLASS="col-xs-1"></DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1">
-										<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-										<!-- {{ _('Edit ruleset details') }} -->
-										{% call accordion.toggle_begin(tooltip="Edit ruleset details")
-										%}{{ruleset.html_key}}{% endcall %}
-										{{ _(ruleset.label) }}
-										{{ accordion.toggle_end() }}
-									</DIV>
-									<DIV CLASS="col-xs-5  col-sm-7  col-md-8  col-lg-8  localetext">
-										{{ ruleset.summary|format_text_array|safe }}
-									</DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  text-right">
-										{% if not ruleset.fixed_context %}
-										<BUTTON id="{{ ruleset.delete_html_key }}" class="btn"
-												title="{{_('Remove ruleset')}}"><I class="fas fa-trash"></I></BUTTON>
-										{% endif %}
-										{% if ruleset.can_move_up %}
-										<BUTTON id="{{ ruleset.move_up_html_key }}"
-												type="submit" name="submit" class="btn"
-												value="{{ ruleset.move_up_html_key }}"
-												title="{{ _('Move ruleset up')}}"><I class="fas fa-arrow-up"></I>
-										</BUTTON>
-										{% endif %}
-										{% if ruleset.can_move_down %}
-										<BUTTON id="{{ ruleset.move_down_html_key }}"
-												type="submit" name="submit" class="btn"
-												value="{{ ruleset.move_down_html_key }}"
-												title="{{ _('Move ruleset down')}}"><I class="fas fa-arrow-down"></I>
-										</BUTTON>
-										{% endif %}
-										<BUTTON type="submit" name="submit" class="btn" title="{{_('Save')}}"><I
-												class="fas fa-save"></I></BUTTON>
-									</DIV>
-								</DIV>
-							{% call accordion.details() %}{{ruleset.html_key}}{% endcall %}
-								<DIV CLASS="row ALTERNATE_ROWLEVEL_3 TITLE_ROW">
-									<DIV CLASS="col-xs-1 "></DIV>
-									<DIV CLASS="col-xs-3  col-md-1 localetext dense-font">{{_('Label')}}</DIV>
-									<DIV CLASS="col-xs-4  col-md-2 localetext dense-font">{{_('Context')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Context Details')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Optional Time')}}</DIV>
-									<!-- line break for sm -->
-									<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
-									<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-									<!-- line break for sm -->
-									<DIV CLASS="col-xs-1  hidden-md hidden-lg"></DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Min Time of Day')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Max Time of Day')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Time per Day')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Minimum Break')}}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Max Duration')}}</DIV>
-									<DIV CLASS="col-xs-1  col-md-1 localetext dense-font">{{_('Free Play')}}</DIV>
+						<DIV CLASS="row ROWLEVEL_3 TITLE_ROW">
+							<DIV CLASS="col-xs-1  col-sm-1  col-md-1  lol-lg-1           "></DIV>
+							<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2 localetext">{{_('Prohibited Process Name Pattern')}}</DIV>
+							<DIV CLASS="col-xs-8  col-sm-9  col-md-9  col-lg-9">
+								{{ helper.render_field(forms[user.html_key].prohibited_process_name_pattern, rows=10) }}
+							</DIV>
+						</DIV>
+						{{ accordion.end() }}
+
+						{#<!-- ********************************************************************************************-->
+						<!-- RULESETS                                                                                    -->
+						<!-- ********************************************************************************************-->#}
+
+						{% call accordion.begin() %}{{ user.rulesets_html_key }}{% endcall %}
+							<DIV CLASS="row ALTERNATE_ROWLEVEL_1">
+								<DIV CLASS="col-xs-1"></DIV>
+								<DIV CLASS="col-xs-9 localetext">
+									{% call accordion.toggle_begin(tooltip="Edit rulesets") %}{{ user.rulesets_html_key }}{%
+									endcall %}
+									{{_('Rulesets')}} ({{_('Count')}}: {{ user.sorted_rulesets|length }})
+									{{ accordion.toggle_end() }}
 								</DIV>
-								<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
-									<DIV CLASS="col-xs-1 "></DIV>
-									<DIV CLASS="col-xs-3  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].context_label) }}</DIV>
-									<DIV CLASS="col-xs-4  col-md-2  col-lg-2  ">
-										{{ helper.render_field(forms[ruleset.html_key].context, ruleset.fixed_context) }}
-									</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">
-										{{ helper.render_field(forms[ruleset.html_key].context_details,
-										ruleset.fixed_context) }}
-									</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].optional_time_per_day) }}</DIV>
-									<!-- line break for sm -->
-									<!-- See https://getbootstrap.com/docs/3.3/css/#grid-responsive-resets -->
-									<DIV CLASS="clearfix visible-xs-block"></DIV>
-									<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
-									<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
-									<!-- line break for sm -->
-									<DIV CLASS="col-xs-1  hidden-md hidden-lg"></DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].min_time_of_day) }}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_time_of_day) }}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_time_per_day) }}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].min_break) }}</DIV>
-									<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_activity_duration) }}</DIV>
-									<DIV CLASS="col-xs-1  col-md-1  col-lg-1  ">{{ forms[ruleset.html_key].free_play(class_="form-control inline-field") }}</DIV>
+								<DIV class="col-xs-2 text-right">
+									<BUTTON id="{{ user.new_ruleset_html_key }}" type="submit" name="submit" class="btn"
+											title="{{_('Add ruleset')}}" value="{{ user.new_ruleset_html_key }}"><I class="fas fa-plus"></I></BUTTON>
 								</DIV>
-							{{ accordion.end() }}
-						{% endfor %} <!-- rulesets -->
-					{{ accordion.end() }}
-
-					<!-- ********************************************************************************************-->
-					<!-- DEVICES                                                                                     -->
-					<!-- ********************************************************************************************-->
-
-	    	   	   	{% call accordion.begin() %}{{ user.devices_html_key }}{% endcall %}
-						<DIV CLASS="row ALTERNATE2_ROWLEVEL_1">
-							<DIV CLASS="col-xs-1"></DIV>
-							<DIV CLASS="col-xs-4 col-sm-4 localetext">
-								{% call accordion.toggle_begin(tooltip="Edit devices") %}{{ user.devices_html_key }}{% endcall %}
-								{{_('Devices')}} ({{user.device_list|_base}})
-								{{ accordion.toggle_end() }}
-							</DIV>
-							<DIV class="col-xs-7 col-sm-7 text-right">
-								{% if forms[user.new_device_html_key] is defined %}
-									{{ _("Add to monitoring") }}:
-									{{ forms[user.new_device_html_key].device_id(class_="form-control inline-field") }}
-									<BUTTON id="{{ user.new_device_html_key }}" type="submit" name="submit"
-											class="btn" title="{{_('Add device')}}"
-											value="{{ user.new_device_html_key }}"><I class="fas fa-plus"></I></BUTTON>
-								{% endif %}
 							</DIV>
-						</DIV>
-					{% call accordion.details() %}{{user.devices_html_key}}{% endcall %}
-						{% for user2device in user.sorted_user2devices %}
-							{% call accordion.begin() %}{{user2device.html_key}}{% endcall %}
-								<DIV CLASS="row ALTERNATE2_ROWLEVEL_2">
-									<DIV CLASS="col-xs-1 "></DIV>
-									<DIV CLASS="col-xs-2">
-										<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->
-										<!-- {{ _('Edit ruleset details') }} -->
-										{% call accordion.toggle_begin(tooltip="Edit device assignment details") %}{{user2device.html_key}}{% endcall %}
-											{{ user2device.device.device_name }}
-										{{ accordion.toggle_end() }}
+						{% call accordion.details() %}{{user.rulesets_html_key}}{% endcall %}
+							{% for ruleset in user.sorted_rulesets %}
+								{% call accordion.begin() %}{{ruleset.html_key}}{% endcall %}
+									<DIV CLASS="row ALTERNATE_ROWLEVEL_2">
+										<DIV CLASS="col-xs-1"></DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1">
+											{#<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->#}
+											<!-- {{ _('Edit ruleset details') }} -->
+											{% call accordion.toggle_begin(tooltip="Edit ruleset details")
+											%}{{ruleset.html_key}}{% endcall %}
+											{{ _(ruleset.label) }}
+											{{ accordion.toggle_end() }}
+										</DIV>
+										<DIV CLASS="col-xs-5  col-sm-7  col-md-8  col-lg-8  localetext">
+											{{ ruleset.summary|format_text_array|safe }}
+										</DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  text-right">
+											{% if not ruleset.fixed_context %}
+											<BUTTON id="{{ ruleset.delete_html_key }}" class="btn"
+													title="{{_('Remove ruleset')}}"><I class="fas fa-trash"></I></BUTTON>
+											{% endif %}
+											{% if ruleset.can_move_up %}
+											<BUTTON id="{{ ruleset.move_up_html_key }}"
+													type="submit" name="submit" class="btn"
+													value="{{ ruleset.move_up_html_key }}"
+													title="{{ _('Move ruleset up')}}"><I class="fas fa-arrow-up"></I>
+											</BUTTON>
+											{% endif %}
+											{% if ruleset.can_move_down %}
+											<BUTTON id="{{ ruleset.move_down_html_key }}"
+													type="submit" name="submit" class="btn"
+													value="{{ ruleset.move_down_html_key }}"
+													title="{{ _('Move ruleset down')}}"><I class="fas fa-arrow-down"></I>
+											</BUTTON>
+											{% endif %}
+											<BUTTON type="submit" name="submit" class="btn" title="{{_('Save')}}"><I
+													class="fas fa-save"></I></BUTTON>
+										</DIV>
 									</DIV>
-									<DIV CLASS="col-xs-8 localetext">
-										{{ user2device.summary|format_text_array|safe }}
+								{% call accordion.details() %}{{ruleset.html_key}}{% endcall %}
+									<DIV CLASS="row ALTERNATE_ROWLEVEL_3 TITLE_ROW">
+										<DIV CLASS="col-xs-1 "></DIV>
+										<DIV CLASS="col-xs-3  col-md-1 localetext dense-font">{{_('Label')}}</DIV>
+										<DIV CLASS="col-xs-4  col-md-2 localetext dense-font">{{_('Context')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Context Details')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Optional Time')}}</DIV>
+										{#<!-- line break for sm -->#}
+										<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
+										<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+										{#<!-- line break for sm -->#}
+										<DIV CLASS="col-xs-1  hidden-md hidden-lg"></DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Min Time of Day')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Max Time of Day')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Time per Day')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Minimum Break')}}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1 localetext dense-font">{{_('Max Duration')}}</DIV>
+										<DIV CLASS="col-xs-1  col-md-1 localetext dense-font">{{_('Free Play')}}</DIV>
 									</DIV>
-									<DIV CLASS="col-xs-1 text-right">
-										<BUTTON id="{{ user2device.delete_html_key }}" class="btn" title="{{_('Remove monitoring of this device for the user')}}"><I class="fas fa-trash"></I></BUTTON>
+									<DIV CLASS="row ALTERNATE_ROWLEVEL_3">
+										<DIV CLASS="col-xs-1 "></DIV>
+										<DIV CLASS="col-xs-3  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].context_label) }}</DIV>
+										<DIV CLASS="col-xs-4  col-md-2  col-lg-2  ">
+											{{ helper.render_field(forms[ruleset.html_key].context, ruleset.fixed_context) }}
+										</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">
+											{{ helper.render_field(forms[ruleset.html_key].context_details,
+											ruleset.fixed_context) }}
+										</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].optional_time_per_day) }}</DIV>
+										{#<!-- line break for sm -->
+										<!-- See https://getbootstrap.com/docs/3.3/css/#grid-responsive-resets -->#}
+										<DIV CLASS="clearfix visible-xs-block"></DIV>
+										<DIV CLASS="col-xs-1  hidden-md hidden-lg SEPERATOR_ROW">&nbsp;</DIV>
+										<DIV CLASS="col-xs-11 hidden-md hidden-lg SEPERATOR_ROW_LINE"></DIV>
+										{#<!-- line break for sm -->#}
+										<DIV CLASS="col-xs-1  hidden-md hidden-lg"></DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].min_time_of_day) }}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_time_of_day) }}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_time_per_day) }}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].min_break) }}</DIV>
+										<DIV CLASS="col-xs-2  col-md-1  col-lg-1  ">{{ helper.render_field(forms[ruleset.html_key].max_activity_duration) }}</DIV>
+										<DIV CLASS="col-xs-1  col-md-1  col-lg-1  ">{{ forms[ruleset.html_key].free_play(class_="form-control inline-field") }}</DIV>
 									</DIV>
+								{{ accordion.end() }}
+							{% endfor %} {#<!-- rulesets -->#}
+						{{ accordion.end() }}
+
+						{#<!-- ********************************************************************************************-->
+						<!-- DEVICES                                                                                     -->
+						<!-- ********************************************************************************************-->#}
+
+						{% call accordion.begin() %}{{ user.devices_html_key }}{% endcall %}
+							<DIV CLASS="row ALTERNATE2_ROWLEVEL_1">
+								<DIV CLASS="col-xs-1"></DIV>
+								<DIV CLASS="col-xs-4 col-sm-4 localetext">
+									{% call accordion.toggle_begin(tooltip="Edit devices") %}{{ user.devices_html_key }}{% endcall %}
+									{{_('Devices')}} ({{user.device_list|_base}})
+									{{ accordion.toggle_end() }}
 								</DIV>
-							{% call accordion.details() %}{{user2device.html_key}}{% endcall %}
-								<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW dense-font">
-									<DIV CLASS="col-xs-1 "></DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  localetext">{{_('Monitored')}}</DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  localetext">{{_('Percent')}}</DIV>
-									<DIV CLASS="col-xs-5  col-sm-2  col-md-8  col-lg-8  text-right"></DIV>
+								<DIV class="col-xs-7 col-sm-7 text-right">
+									{% if forms[user.new_device_html_key] is defined %}
+										{{ _("Add to monitoring") }}:
+										{{ forms[user.new_device_html_key].device_id(class_="form-control inline-field") }}
+										<BUTTON id="{{ user.new_device_html_key }}" type="submit" name="submit"
+												class="btn" title="{{_('Add device')}}"
+												value="{{ user.new_device_html_key }}"><I class="fas fa-plus"></I></BUTTON>
+									{% endif %}
 								</DIV>
-								<DIV CLASS="row ALTERNATE2_ROWLEVEL_3">
-									<DIV CLASS="col-xs-1 "></DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-2 col-lg-2  ">{{ helper.render_field(forms[user2device.html_key].active) }}</DIV>
-									<DIV CLASS="col-xs-3  col-sm-2  col-md-1 col-lg-1  ">{{ helper.render_field(forms[user2device.html_key].percent) }}</DIV>
-									<DIV CLASS="col-xs-5  col-sm-7  col-md-8 col-lg-8 text-right ">
-										<BUTTON type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
+							</DIV>
+						{% call accordion.details() %}{{user.devices_html_key}}{% endcall %}
+							{% for user2device in user.sorted_user2devices %}
+								{% call accordion.begin() %}{{user2device.html_key}}{% endcall %}
+									<DIV CLASS="row ALTERNATE2_ROWLEVEL_2">
+										<DIV CLASS="col-xs-1 "></DIV>
+										<DIV CLASS="col-xs-2">
+											{#<!-- The following line will trigger the extraction of the tooltip for Babel. DO NOT REMOVE! -->#}
+											<!-- {{ _('Edit ruleset details') }} -->
+											{% call accordion.toggle_begin(tooltip="Edit device assignment details") %}{{user2device.html_key}}{% endcall %}
+												{{ user2device.device.device_name }}
+											{{ accordion.toggle_end() }}
+										</DIV>
+										<DIV CLASS="col-xs-8 localetext">
+											{{ user2device.summary|format_text_array|safe }}
+										</DIV>
+										<DIV CLASS="col-xs-1 text-right">
+											<BUTTON id="{{ user2device.delete_html_key }}" class="btn" title="{{_('Remove monitoring of this device for the user')}}"><I class="fas fa-trash"></I></BUTTON>
+										</DIV>
 									</DIV>
-								</DIV>
-							{{ accordion.end() }}
-						{% endfor %} <!-- user2devices -->
+								{% call accordion.details() %}{{user2device.html_key}}{% endcall %}
+									<DIV CLASS="row ALTERNATE2_ROWLEVEL_3 TITLE_ROW dense-font">
+										<DIV CLASS="col-xs-1 "></DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-2  col-lg-2  localetext">{{_('Monitored')}}</DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-1  col-lg-1  localetext">{{_('Percent')}}</DIV>
+										<DIV CLASS="col-xs-5  col-sm-2  col-md-8  col-lg-8  text-right"></DIV>
+									</DIV>
+									<DIV CLASS="row ALTERNATE2_ROWLEVEL_3">
+										<DIV CLASS="col-xs-1 "></DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-2 col-lg-2  ">{{ helper.render_field(forms[user2device.html_key].active) }}</DIV>
+										<DIV CLASS="col-xs-3  col-sm-2  col-md-1 col-lg-1  ">{{ helper.render_field(forms[user2device.html_key].percent) }}</DIV>
+										<DIV CLASS="col-xs-5  col-sm-7  col-md-8 col-lg-8 text-right ">
+											<BUTTON type="submit" name="submit" class="btn" title="{{_('Save')}}"><I class="fas fa-save"></I></BUTTON>
+										</DIV>
+									</DIV>
+								{{ accordion.end() }}
+							{% endfor %} {#<!-- user2devices -->#}
+						{{ accordion.end() }}
 					{{ accordion.end() }}
-		        {{ accordion.end() }}
-	    	{% endfor %} <!-- users -->
-	    </DIV> <!-- table -->
-	{% for user in users %}
-		{{ helper.modal_confirm(user.delete_html_key, _("Do you really want to permanently remove the user from monitoring?"), _("Remove from monitoring"), _("Cancel")) }}
-    	{% call accordion.script() %}{{user.html_key}}{% endcall %}
-		{% call accordion.script() %}process_{{ user.html_key }}{% endcall %}
-    	{% call accordion.script() %}{{user.rulesets_html_key}}{% endcall %}
-		{% for ruleset in user.rulesets %}
-			{{ helper.modal_confirm(ruleset.delete_html_key, _("Do you really want to permanently remove the ruleset?"), _("Remove ruleset"), _("Cancel")) }}
-	    	{% call accordion.script() %}{{ruleset.html_key}}{% endcall %}
-		{% endfor %}
-    	{% call accordion.script() %}{{user.devices_html_key}}{% endcall %}
-		{% for user2device in user.devices %}
-			{{ helper.modal_confirm(user2device.delete_html_key, _("Do you really want to permanently remove monitoring of the device for this user?"), _("Remove from monitoring"), _("Cancel")) }}
-	    	{% call accordion.script() %}{{user2device.html_key}}{% endcall %}
-		{% endfor %}
-	{% endfor %}
-    </FORM>
+				{% endfor %} {#<!-- users -->#}
+			</DIV> {#<!-- table -->#}
+
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/jquery-1.11.2.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/bootstrap.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/initializr/js/vendor/modernizr-2.8.3-respond-1.4.2.min.js') }}"></SCRIPT>
+			<SCRIPT type="text/javascript" SRC="{{ url_for('little_brother.static', filename='contrib/js-cookie/js-cookie.js') }}"></SCRIPT>
+
+			{% for user in users %}
+				{{ helper.modal_confirm(user.delete_html_key, _("Do you really want to permanently remove the user from monitoring?"), _("Remove from monitoring"), _("Cancel")) }}
+				{% call accordion.script() %}{{user.html_key}}{% endcall %}
+				{% call accordion.script() %}process_{{ user.html_key }}{% endcall %}
+				{% call accordion.script() %}{{user.rulesets_html_key}}{% endcall %}
+				{% for ruleset in user.rulesets %}
+					{{ helper.modal_confirm(ruleset.delete_html_key, _("Do you really want to permanently remove the ruleset?"), _("Remove ruleset"), _("Cancel")) }}
+					{% call accordion.script() %}{{ruleset.html_key}}{% endcall %}
+				{% endfor %}
+				{% call accordion.script() %}{{user.devices_html_key}}{% endcall %}
+				{% for user2device in user.devices %}
+					{{ helper.modal_confirm(user2device.delete_html_key, _("Do you really want to permanently remove monitoring of the device for this user?"), _("Remove from monitoring"), _("Cancel")) }}
+					{% call accordion.script() %}{{user2device.html_key}}{% endcall %}
+				{% endfor %}
+			{% endfor %}
+		</FORM>
+	  </DIV>
   </BODY>
 </HTML>
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
+{##}
 {% import 'bootstrap_accordion.macros.html' as accordion %} {% import
 'helper.macros.html' as helper %} {{ helper.locale_font(rel_font_size) }}
 
 
 
 
 
 
 
-{{ helper.fontawesome_script() }} {% include 'navbar.include.html' %}
-
+{{ helper.fontawesome_script() }}
+{% include 'navbar.include.html' %} {% include 'version_check.include.html' %}
+{##}
 {{_('User')}}
  {% if forms[new_user_html_key] is defined %} {{ _("Add to monitoring") }}: {
 { forms[new_user_html_key].username(class_="form-control inline-field") }}  {%
 endif %}
-{% for user in users %}    {% call accordion.begin() %}{{ user.html_key }}{%
-endcall %}
-  {% call accordion.toggle_begin(tooltip="Edit user details") %}{
+{% for user in users %} {#  #} {% call accordion.begin() %}{{ user.html_key }}
+{% endcall %}
+{##}  {% call accordion.toggle_begin(tooltip="Edit user details") %}{
 { user.html_key }}{% endcall %} {{ user.full_name }} {{ accordion.toggle_end()
 }}
 {{ user.summary|format_text_array|safe }}
- {% call accordion.details() %}{{user.html_key}}{% endcall %}
+{% call accordion.details() %}{{user.html_key}}{% endcall %}
 {{_('Monitored')}}
 {{_('First Name')}}
 {{_('Last Name')}}
 {{_('Locale')}}
 {{ helper.render_field(forms[user.html_key].active) }}
 {{ forms[user.html_key].first_name(class_="form-control dense-font") }}
 {{ forms[user.html_key].last_name(class_="form-control dense-font") }}
@@ -34,76 +36,80 @@
 { accordion.toggle_end() }}
 {% call accordion.details() %}process_{{user.html_key}}{% endcall %}
 {{_('Login Process Name Pattern')}}
 {{ helper.render_field(forms[user.html_key].process_name_pattern, rows=10) }}
 {{_('Prohibited Process Name Pattern')}}
 {{ helper.render_field(forms[user.html_key].prohibited_process_name_pattern,
 rows=10) }}
-{{ accordion.end() }}    {% call accordion.begin() %}{{ user.rulesets_html_key
-}}{% endcall %}
+{{ accordion.end() }} {#  #} {% call accordion.begin() %}{
+{ user.rulesets_html_key }}{% endcall %}
 {% call accordion.toggle_begin(tooltip="Edit rulesets") %}{
 { user.rulesets_html_key }}{% endcall %} {{_('Rulesets')}} ({{_('Count')}}: {
 { user.sorted_rulesets|length }}) {{ accordion.toggle_end() }}
 {% call accordion.details() %}{{user.rulesets_html_key}}{% endcall %} {% for
 ruleset in user.sorted_rulesets %} {% call accordion.begin() %}{
 {ruleset.html_key}}{% endcall %}
-  {% call accordion.toggle_begin(tooltip="Edit ruleset details") %}{
+{##}  {% call accordion.toggle_begin(tooltip="Edit ruleset details") %}{
 {ruleset.html_key}}{% endcall %} {{ _(ruleset.label) }} {{ accordion.toggle_end
 () }}
 {{ ruleset.summary|format_text_array|safe }}
 {% if not ruleset.fixed_context %}  {% endif %} {% if ruleset.can_move_up %}
 {% endif %} {% if ruleset.can_move_down %}   {% endif %}
 {% call accordion.details() %}{{ruleset.html_key}}{% endcall %}
 {{_('Label')}}
 {{_('Context')}}
 {{_('Context Details')}}
 {{_('Optional Time')}}
+{##}
  
+{##}
 {{_('Min Time of Day')}}
 {{_('Max Time of Day')}}
 {{_('Time per Day')}}
 {{_('Minimum Break')}}
 {{_('Max Duration')}}
 {{_('Free Play')}}
 {{ helper.render_field(forms[ruleset.html_key].context_label) }}
 {{ helper.render_field(forms[ruleset.html_key].context, ruleset.fixed_context)
 }}
 {{ helper.render_field(forms[ruleset.html_key].context_details,
 ruleset.fixed_context) }}
 {{ helper.render_field(forms[ruleset.html_key].optional_time_per_day) }}
-
+{# #}
  
+{##}
 {{ helper.render_field(forms[ruleset.html_key].min_time_of_day) }}
 {{ helper.render_field(forms[ruleset.html_key].max_time_of_day) }}
 {{ helper.render_field(forms[ruleset.html_key].max_time_per_day) }}
 {{ helper.render_field(forms[ruleset.html_key].min_break) }}
 {{ helper.render_field(forms[ruleset.html_key].max_activity_duration) }}
 {{ forms[ruleset.html_key].free_play(class_="form-control inline-field") }}
-{{ accordion.end() }} {% endfor %}  {{ accordion.end() }}    {% call
+{{ accordion.end() }} {% endfor %} {##} {{ accordion.end() }} {#  #} {% call
 accordion.begin() %}{{ user.devices_html_key }}{% endcall %}
 {% call accordion.toggle_begin(tooltip="Edit devices") %}{
 { user.devices_html_key }}{% endcall %} {{_('Devices')}} ({
 {user.device_list|_base}}) {{ accordion.toggle_end() }}
 {% if forms[user.new_device_html_key] is defined %} {{ _("Add to monitoring")
 }}: {{ forms[user.new_device_html_key].device_id(class_="form-control inline-
 field") }}  {% endif %}
 {% call accordion.details() %}{{user.devices_html_key}}{% endcall %} {% for
 user2device in user.sorted_user2devices %} {% call accordion.begin() %}{
 {user2device.html_key}}{% endcall %}
-  {% call accordion.toggle_begin(tooltip="Edit device assignment details") %}{
-{user2device.html_key}}{% endcall %} {{ user2device.device.device_name }} {
+{##}  {% call accordion.toggle_begin(tooltip="Edit device assignment details")
+%}{{user2device.html_key}}{% endcall %} {{ user2device.device.device_name }} {
 { accordion.toggle_end() }}
 {{ user2device.summary|format_text_array|safe }}
 {% call accordion.details() %}{{user2device.html_key}}{% endcall %}
 {{_('Monitored')}}
 {{_('Percent')}}
 {{ helper.render_field(forms[user2device.html_key].active) }}
 {{ helper.render_field(forms[user2device.html_key].percent) }}
-{{ accordion.end() }} {% endfor %}  {{ accordion.end() }} {{ accordion.end() }}
-{% endfor %}
+{{ accordion.end() }} {% endfor %} {##} {{ accordion.end() }} {{ accordion.end
+() }} {% endfor %} {##}
+{##}
  {% for user in users %} {{ helper.modal_confirm(user.delete_html_key, _("Do
 you really want to permanently remove the user from monitoring?"), _("Remove
 from monitoring"), _("Cancel")) }} {% call accordion.script() %}{
 {user.html_key}}{% endcall %} {% call accordion.script() %}process_{
 { user.html_key }}{% endcall %} {% call accordion.script() %}{
 {user.rulesets_html_key}}{% endcall %} {% for ruleset in user.rulesets %} {
 { helper.modal_confirm(ruleset.delete_html_key, _("Do you really want to
```

### Comparing `little-brother-0.4.8/little_brother/test/dummy_process_handler.py` & `little-brother-0.4.9/little_brother/test/dummy_process_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/dummy_process_iterator.py` & `little-brother-0.4.9/little_brother/test/dummy_process_iterator.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/base_test_case_persistent_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/base_test_case_persistent_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistence.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistence.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,14 +85,46 @@
 
     def test_create_database(self):
 
         self.create_dummy_persistence(self._logger)
 
         self.assertIsNotNone(dependency_injection.container[Persistence])
 
+    def test_get_admin_session(self):
+
+        self.create_dummy_persistence(self._logger)
+
+        persistence = dependency_injection.container[Persistence]
+
+        session = persistence.get_admin_session()
+
+        self.assertIsNotNone(session)
+
+        session2 = persistence.get_admin_session()
+
+        self.assertIsNotNone(session2)
+        self.assertEqual(session, session2)
+
+    def test_get_create_table_session(self):
+
+        self.create_dummy_persistence(self._logger)
+
+        persistence = dependency_injection.container[Persistence]
+
+        session = persistence.get_create_table_session()
+
+        self.assertIsNotNone(session)
+
+        session2 = persistence.get_create_table_session()
+
+        self.assertIsNotNone(session2)
+        self.assertEqual(session, session2)
+
+
+
     @staticmethod
     def create_pinfo(p_age_in_days, p_include_end_time=False):
 
         start_time = datetime.datetime.utcnow() + datetime.timedelta(days=-p_age_in_days)
 
         if p_include_end_time:
             end_time = start_time + datetime.timedelta(minutes=5)
```

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_admin_event_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_admin_event_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_daily_user_status_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_user_entity_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from little_brother import dependency_injection
 from little_brother.persistence.base_entity_manager import BaseEntityManager
-from little_brother.persistence.persistent_daily_user_status_entity_manager import DailyUserStatusEntityManager
+from little_brother.persistence.persistent_user_entity_manager import UserEntityManager
 from little_brother.test.persistence.base_test_case_persistent_entity_manager import BaseTestCasePersistentEntityManager
 
 
-class TestDailyUserStatusEntityManager(BaseTestCasePersistentEntityManager):
+class TestUserEntityManager(BaseTestCasePersistentEntityManager):
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
-        cls._entity_manager: BaseEntityManager = DailyUserStatusEntityManager()
+        cls._entity_manager: BaseEntityManager = UserEntityManager()
 
     def setUp(self):
         dependency_injection.reset()
```

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_device_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_device_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_process_info_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_process_info_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_rule_override_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_rule_override_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_rule_set_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_rule_set_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_time_extension_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_time_extension_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_persistent_user_2_device_entity_manager.py` & `little-brother-0.4.9/little_brother/test/persistence/test_persistent_user_2_device_entity_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/persistence/test_suite.py` & `little-brother-0.4.9/little_brother/test/persistence/test_suite.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/resources/app.config` & `little-brother-0.4.9/little_brother/test/resources/app.config`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/resources/ruleset_handler.test.config` & `little-brother-0.4.9/little_brother/test/resources/ruleset_handler.test.config`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_app.py` & `little-brother-0.4.9/little_brother/test/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         configuration = Configuration()
 
         config = app.prepare_configuration(configuration)
 
         self.assertIsNotNone(config)
 
-        self.assertEqual(13, len(configuration._sections))
+        self.assertEqual(14, len(configuration._sections))
 
     @classmethod
     def create_dummy_app(cls, p_logger):
 
         parser = get_argument_parser(p_app_name=APP_NAME)
         arguments = parser.parse_args(cls.get_default_sys_args())
```

### Comparing `little-brother-0.4.8/little_brother/test/test_app_control.py` & `little-brother-0.4.9/little_brother/test/test_app_control.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_client_device_handler.py` & `little-brother-0.4.9/little_brother/test/test_client_device_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_client_process_handler.py` & `little-brother-0.4.9/little_brother/test/test_client_process_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,30 +16,56 @@
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import copy
 import datetime
+import os
+import signal
+from multiprocessing import Process
+from time import sleep
 
 from little_brother import admin_event
 from little_brother import client_process_handler
 from little_brother import dependency_injection
 from little_brother import login_mapping
+from little_brother.admin_event import AdminEvent, EVENT_TYPE_KILL_PROCESS, EVENT_TYPE_PROCESS_END
+from little_brother.login_mapping import LoginUidMappingEntry, LoginMapping
 from little_brother.persistence.persistence import Persistence
 from little_brother.persistence.session_context import SessionContext
 from little_brother.test import dummy_process_iterator
 from little_brother.test import test_data
 from little_brother.test.persistence import test_persistence
+from python_base_app import tools
 from python_base_app.test import base_test
 
 
+def signal_handler(signum, _frame):
+    print("Ignoring signal", signum)
+
+
+def f(p_mask_sigterm:bool):
+    if p_mask_sigterm:
+        signal.signal(signal.SIGHUP, signal_handler)
+
+    while True:
+        sleep(1)
+
+
+def create_dummy_process(p_mask_sigterm:bool=False) -> Process:
+    p = Process(target=f, args=(p_mask_sigterm,))
+    p.start()
+    return p
+
+
 class TestClientProcessHandler(base_test.BaseTestCase):
 
     def setUp(self):
+
         dependency_injection.reset()
 
     def check_list_has_n_elements(self, p_list, p_n):
 
         self.assertIsNotNone(p_list)
         self.assertIsInstance(p_list, list)
         self.assertEqual(len(p_list), p_n)
@@ -304,7 +330,107 @@
             event = events[0]
 
             self.assertEqual(event.event_type, admin_event.EVENT_TYPE_PROCESS_END)
             self.assertEqual(event.event_time, now)
             self.assertEqual(event.processhandler, process_handler.id)
 
             self.check_default_data(p_event=event)
+
+    def test_handle_event_kill_non_existing_process(self):
+
+        config = client_process_handler.ClientProcessHandlerConfigModel()
+        config.scan_command_line_options = False
+
+        process_handler = self.get_dummy_process_handler(p_processes=test_data.PROCESSES_CMD_LINE_1,
+                                                         p_config=config)
+
+        event = AdminEvent(p_hostname="localhost", p_processname="sh", p_username="dummy",
+                           p_processhandler=process_handler.id, p_process_start_time=tools.get_current_time(),
+                           p_event_type=EVENT_TYPE_KILL_PROCESS, p_pid=-1)
+
+        admin_events = process_handler.handle_event_kill_process(p_event=event)
+
+        self.assertIsNotNone(admin_events)
+        self.assertEqual(1, len(admin_events))
+
+        admin_event = admin_events[0]
+
+        self.assertEqual(EVENT_TYPE_PROCESS_END, admin_event.event_type)
+        self.assertEqual(-1, admin_event.pid)
+
+    def test_handle_event_kill_existing_process_with_valid_user_on_sigterm(self):
+        config = client_process_handler.ClientProcessHandlerConfigModel()
+        config.sudo_command = ""
+        config.scan_command_line_options = False
+
+        process_handler = self.get_dummy_process_handler(p_processes=test_data.PROCESSES_CMD_LINE_1,
+                                                         p_config=config)
+
+        process = create_dummy_process()
+
+        event = AdminEvent(p_hostname="localhost", p_processname="sh", p_username="dummy",
+                           p_processhandler=process_handler.id, p_process_start_time=tools.get_current_time(),
+                           p_event_type=EVENT_TYPE_KILL_PROCESS, p_pid=process.pid)
+
+        mapping_entry = LoginUidMappingEntry("dummy", os.getuid())
+
+        login_mapping = LoginMapping()
+
+        login_mapping.add_entry(p_login_uid_mapping_entry=mapping_entry)
+
+        admin_events = process_handler.handle_event_kill_process(p_event=event, p_login_mapping=login_mapping)
+
+        self.assertIsNotNone(admin_events)
+        self.assertEqual(0, len(admin_events))
+
+    def test_handle_event_kill_existing_process_with_invalid_user(self):
+        config = client_process_handler.ClientProcessHandlerConfigModel()
+        config.sudo_command = ""
+        config.scan_command_line_options = False
+
+        process_handler = self.get_dummy_process_handler(p_processes=test_data.PROCESSES_CMD_LINE_1,
+                                                         p_config=config)
+
+        process = create_dummy_process()
+
+        event = AdminEvent(p_hostname="localhost", p_processname="sh", p_username="some-user",
+                           p_processhandler=process_handler.id, p_process_start_time=tools.get_current_time(),
+                           p_event_type=EVENT_TYPE_KILL_PROCESS, p_pid=process.pid)
+
+        mapping_entry = LoginUidMappingEntry("dummy", os.getuid())
+
+        login_mapping = LoginMapping()
+
+        login_mapping.add_entry(p_login_uid_mapping_entry=mapping_entry)
+
+        admin_events = process_handler.handle_event_kill_process(p_event=event, p_login_mapping=login_mapping)
+
+        self.assertIsNotNone(admin_events)
+        self.assertEqual(0, len(admin_events))
+
+        process.kill()
+        process.join()
+
+    def test_handle_event_kill_existing_process_with_valid_user_on_sigkill(self):
+        config = client_process_handler.ClientProcessHandlerConfigModel()
+        config.sudo_command = ""
+        config.scan_command_line_options = False
+
+        process_handler = self.get_dummy_process_handler(p_processes=test_data.PROCESSES_CMD_LINE_1,
+                                                         p_config=config)
+
+        process = create_dummy_process(p_mask_sigterm=True)
+
+        event = AdminEvent(p_hostname="localhost", p_processname="sh", p_username="dummy",
+                           p_processhandler=process_handler.id, p_process_start_time=tools.get_current_time(),
+                           p_event_type=EVENT_TYPE_KILL_PROCESS, p_pid=process.pid)
+
+        mapping_entry = LoginUidMappingEntry("dummy", os.getuid())
+
+        login_mapping = LoginMapping()
+
+        login_mapping.add_entry(p_login_uid_mapping_entry=mapping_entry)
+
+        admin_events = process_handler.handle_event_kill_process(p_event=event, p_login_mapping=login_mapping)
+
+        self.assertIsNotNone(admin_events)
+        self.assertEqual(0, len(admin_events))
```

### Comparing `little-brother-0.4.8/little_brother/test/test_data.py` & `little-brother-0.4.9/little_brother/test/test_data.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_german_vacation_context_rule_handler.py` & `little-brother-0.4.9/little_brother/test/test_german_vacation_context_rule_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_language.py` & `little-brother-0.4.9/little_brother/test/test_language.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_process_handler.py` & `little-brother-0.4.9/little_brother/test/test_process_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_process_handler_manager.py` & `little-brother-0.4.9/little_brother/test/test_process_handler_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_process_info.py` & `little-brother-0.4.9/little_brother/test/test_process_info.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_process_statistics.py` & `little-brother-0.4.9/little_brother/test/test_process_statistics.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_prometheus.py` & `little-brother-0.4.9/little_brother/test/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/test_rule_handler.py` & `little-brother-0.4.9/little_brother/test/test_rule_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-#    Copyright (C) 2019  Marcus Rickert
+#    Copyright (C) 2019-2021  Marcus Rickert
 #
 #    See https://github.com/marcus67/little_brother
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 3 of the License, or
 #    (at your option) any later version.
@@ -31,15 +31,15 @@
 from little_brother import rule_handler
 from little_brother import rule_override
 from little_brother import rule_result_info
 from little_brother import simple_context_rule_handlers
 from little_brother.persistence import persistent_user, persistent_user_entity_manager
 from little_brother.persistence.persistence import Persistence
 from little_brother.test.persistence import test_persistence
-from python_base_app import configuration
+from python_base_app import configuration, tools
 from python_base_app.test import base_test
 
 TEST_USER = "user1"
 
 NORMAL_DAY_1 = datetime.datetime.strptime("09.09.2020", "%d.%m.%Y").date()
 WEEKEND_DAY_1 = datetime.datetime.strptime("12.09.2020", "%d.%m.%Y").date()
 WEEKEND_DAY_2 = datetime.datetime.strptime("13.09.2020", "%d.%m.%Y").date()
@@ -471,15 +471,15 @@
         test_persistence.TestPersistence.create_dummy_persistence(self._logger)
         dummy_persistence: test_persistence.TestPersistence = \
             dependency_injection.container[Persistence]
         a_rule_handler = self.create_dummy_rule_handler(p_persistence=dummy_persistence,
                                                         p_create_complex_handlers=False)
 
         # Use reference time around noon so that we don't get trouble with time intervals spanning midnight
-        reference_time = datetime.datetime.today() + datetime.timedelta(hours=+12)
+        reference_time = tools.get_today() + datetime.timedelta(hours=+12)
         rule_set = TestRuleHandler.create_dummy_ruleset_config()
 
         activity_start = reference_time + datetime.timedelta(seconds=-2000)
         activity_end = reference_time + datetime.timedelta(seconds=-1700)
 
         stat_info = process_statistics.ProcessStatisticsInfo(p_username=USERNAME, p_reference_time=reference_time,
                                                              p_min_activity_duration=MIN_ACTIVITY_DURATION,
```

### Comparing `little-brother-0.4.8/little_brother/test/test_suite.py` & `little-brother-0.4.9/little_brother/test/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import unittest
 
-from little_brother.test import test_app
+from little_brother.test import test_app, test_client_info
 from little_brother.test import test_app_control
 from little_brother.test import test_client_device_handler
 from little_brother.test import test_client_process_handler
 from little_brother.test import test_german_vacation_context_rule_handler
 from little_brother.test import test_language
 from little_brother.test import test_process_handler
 from little_brother.test import test_process_handler_manager
@@ -108,14 +108,18 @@
         p_test_suite=p_test_suite,
         p_test_unit_class=test_user_status.TestUserStatus, p_config_filename=p_config_filename)
 
     base_test.add_tests_in_test_unit(
         p_test_suite=p_test_suite,
         p_test_unit_class=test_process_handler_manager.TestProcessHandlerManager, p_config_filename=p_config_filename)
 
+    base_test.add_tests_in_test_unit(
+        p_test_suite=p_test_suite,
+        p_test_unit_class=test_client_info.TestClientInfo, p_config_filename=p_config_filename)
+
 
 def main():
     log_handling.start_logging(p_use_filter=False)
     test_suite = unittest.TestSuite()
     add_test_cases(p_test_suite=test_suite, p_config_filename=base_test.get_config_filename())
 
     persistence_test_suite.add_test_cases(p_test_suite=test_suite, p_config_filename=base_test.get_config_filename())
```

### Comparing `little-brother-0.4.8/little_brother/test/test_user_status.py` & `little-brother-0.4.9/little_brother/test/test_user_status.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/base_test_status_server.py` & `little-brother-0.4.9/little_brother/test/web/base_test_status_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from little_brother import app
 from little_brother import client_process_handler
 from little_brother import constants
 from little_brother import dependency_injection
 from little_brother.admin_data_handler import AdminDataHandler
 from little_brother.api import master_connector
 from little_brother.api.master_connector import MasterConnector
+from little_brother.api.version_checker import VersionCheckerConfigModel, VersionChecker, SOURCEFORGE_CHANNEL_INFOS
 from little_brother.app_control import AppControl, AppControlConfigModel
 from little_brother.persistence.persistence import Persistence
 from little_brother.persistence.persistent_user_entity_manager import UserEntityManager
 from little_brother.persistence.session_context import SessionContext
 from little_brother.prometheus import PrometheusClient
 from little_brother.rule_handler import RuleHandler
 from little_brother.test import test_client_process_handler
@@ -127,14 +128,18 @@
         dependency_injection.container[AppControl] = self._app_control
 
         status_server_config = web_server.StatusServerConfigModel()
         status_server_config.app_secret = "123456"
 
         status_server_config.port = int(os.getenv("STATUS_SERVER_PORT", "5555"))
 
+        version_checker_config = VersionCheckerConfigModel()
+        version_checker = VersionChecker(p_config=version_checker_config, p_channel_infos=SOURCEFORGE_CHANNEL_INFOS)
+        dependency_injection.container[VersionChecker] = version_checker
+
         self._status_server = web_server.StatusServer(
             p_config=status_server_config,
             p_package_name=app.PACKAGE_NAME,
             p_app_control=self._app_control,
             p_master_connector=self._master_connector,
             p_is_master=True,
             p_user_handler=self._user_handler,
@@ -234,16 +239,21 @@
         self._driver.execute_script("arguments[0].value = '{value}'".format(value=p_value), p_elem)
 
     def add_new_user(self, p_user_entity_manager: UserEntityManager) -> int:
         with SessionContext(self._persistence) as session_context:
             user_id = p_user_entity_manager.add_new_user(
                 p_session_context=session_context, p_username=self.get_new_user_name(), p_locale="en")
 
-        user_manager : UserManager = dependency_injection.container[UserManager]
+        session = session_context.get_session()
+        user = p_user_entity_manager.get_by_id(p_session_context=session_context, p_id=user_id)
+        # activate monitoring of user so that it will show up on the admin page
+        user.active = True
+        session.commit()
 
+        user_manager : UserManager = dependency_injection.container[UserManager]
 
         user_manager.add_monitored_user(p_username=self.get_new_user_name())
         user_manager.retrieve_user_mappings()
 
         return user_id
 
     def get_new_user_name(self):
```

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_about.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_about.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_admin.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_admin.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_devices.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,25 +179,10 @@
             self.assertEqual(old_value, getattr(device, p_elem_name))
 
     @base_test.skip_if_env("NO_SELENIUM_TESTS")
     def test_page_devices_edit_invalid_hostname(self):
         self._test_page_devices_edit_invalid_data(
             p_elem_name="hostname", p_invalid_data=NEW_INVALID_HOST_NAME)
 
-    @base_test.skip_if_env("NO_SELENIUM_TESTS")
-    def test_page_devices_edit_invalid_min_activity_duration(self):
-        self._test_page_devices_edit_invalid_data(
-            p_elem_name="min_activity_duration", p_invalid_data=NEW_INVALID_MIN_ACTIVITY_DURATION)
-
-    @base_test.skip_if_env("NO_SELENIUM_TESTS")
-    def test_page_devices_edit_invalid_max_active_ping_delay(self):
-        self._test_page_devices_edit_invalid_data(
-            p_elem_name="max_active_ping_delay", p_invalid_data=NEW_INVALID_MAX_PING_DELAY)
-
-    @base_test.skip_if_env("NO_SELENIUM_TESTS")
-    def test_page_devices_edit_invalid_sample_size(self):
-        self._test_page_devices_edit_invalid_data(
-            p_elem_name="sample_size", p_invalid_data=NEW_INVALID_SAMPLE_SIZE)
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_index.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_index.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_topology.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_topology.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/test/web/test_status_server_users.py` & `little-brother-0.4.9/little_brother/test/web/test_status_server_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         with SessionContext(self._persistence) as session_context:
             user: User = user_entity_manager.get_by_username(
                 p_session_context=session_context, p_username=test_unix_user_handler.USER_2_UID)
             self.assertEqual(test_unix_user_handler.USER_2_UID, user.username)
             self.assertEqual(NEW_USER_FIRST_NAME, user.first_name)
             self.assertEqual(NEW_USER_LAST_NAME, user.last_name)
             self.assertEqual(NEW_USER_PROCESS_NAME_PATTERN, user.process_name_pattern)
-            self.assertEqual(NEW_USER_ACTIVE, user.active)
+            self.assertEqual(None, user.active)
             self.assertEqual(NEW_USER_LOCALE, user.locale)
 
     @base_test.skip_if_env("NO_SELENIUM_TESTS")
     def test_page_users_assign_rule_set(self):
         self.create_dummy_status_server()
         self.create_selenium_driver()
```

### Comparing `little-brother-0.4.8/little_brother/test/web/test_suite.py` & `little-brother-0.4.9/little_brother/test/web/test_suite.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/translations/bn/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/bn/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  LittleBrother\n"
 "Report-Msgid-Bugs-To: little-brother@web.de\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-20 10:00+0200\n"
 "Last-Translator: Rownak Jyoti Zaman <jyotizaman@yahoo.com>\n"
 "Language: bn\n"
 "Language-Team: bn <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/da/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/da/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  LittleBrother\n"
 "Report-Msgid-Bugs-To: little-brother@web.de\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-05-11 23:49+0200\n"
 "Last-Translator: Erik Husmark\n"
 "Language: da\n"
 "Language-Team: da <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/de/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/de/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  little-brother\n"
 "Report-Msgid-Bugs-To: marcus.rickert@web.de\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2019-02-27 23:25+0100\n"
 "Last-Translator: Marcus Rickert <marcus.rickert@web.de>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -262,14 +262,27 @@
 
 msgid "Move ruleset up"
 msgstr "Bewege Regelsatz nach oben"
 
 msgid "Name"
 msgstr "Name"
 
+msgid ""
+"New version of LittleBrother available for update channel <CODE>{channel}</"
+"CODE>: version <CODE>{suggested_version}</CODE> with revision "
+"<CODE>{suggested_revision}</CODE>. Currently installed: version "
+"<CODE>{current_version}</CODE> with revision <CODE>{current_revision}</"
+"CODE>. Download Debian package <a href=\"{download_url}\">here</a>."
+msgstr ""
+"Neue Version von LittleBrother für den Update-Kanal <CODE>{channel}</CODE> "
+"verfügbar: Version <CODE>{suggested_version}</CODE> in Revision "
+"<CODE>{suggested_revision}</CODE>. Zurzeit installiert: Version "
+"<CODE>{current_version}</CODE> in Revision <CODE>{current_revision}</CODE>. "
+"Debian-Paket <a href=\"{download_url}\">hier</a> herunterladen."
+
 msgid "No activity after {hh_mm} hours"
 msgstr "Keine Aktivität nach {hh_mm} Uhr"
 
 msgid "No activity before {hh_mm} hours"
 msgstr "Keine Aktivität vor {hh_mm} Uhr"
 
 msgid "No activity exceeding {hh_mm}"
```

### Comparing `little-brother-0.4.8/little_brother/translations/es/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/es/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-14 21:34+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/fi/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/fi/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-19 11:47+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fi\n"
 "Language-Team: fi <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/fr/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  LittleBrother\n"
 "Report-Msgid-Bugs-To: little-brother@web.de\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2021-02-21 10:30+0100\n"
 "Last-Translator: albano battistella <albano_battistella@hotmail.com>\n"
 "Language: fr\n"
 "Language-Team: Albano Battistella <albano_battistella@hotmail.com>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/hr/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-09-06 22:56+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hr\n"
 "Language-Team: hr <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2)\n"
 "MIME-Version: 1.0\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/it/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/it/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2021-06-19 20:00+0200\n"
 "Last-Translator: albano battistella <albano_battistella@hotmail.com>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/ja/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-20 09:49+0200\n"
 "Last-Translator: Arik Mahbub <arikmahbub@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/nl/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/nl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: LittleBrother 0.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-14 20:21+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/ru/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  LittleBrother\n"
 "Report-Msgid-Bugs-To: little-brother@web.de\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-20 09:53+0200\n"
 "Last-Translator: J. Moldawski\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2)\n"
 "MIME-Version: 1.0\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/sr/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/sr/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: PROJECT VERSION*

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 2c00 0000 d701 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2050 524f 4a45 4354 2056 4552 5349 4f4e   PROJECT VERSION
 00000050: 0a52 6570 6f72 742d 4d73 6769 642d 4275  .Report-Msgid-Bu
 00000060: 6773 2d54 6f3a 2045 4d41 494c 4041 4444  gs-To: EMAIL@ADD
 00000070: 5245 5353 0a50 4f54 2d43 7265 6174 696f  RESS.POT-Creatio
 00000080: 6e2d 4461 7465 3a20 3230 3231 2d30 382d  n-Date: 2021-08-
-00000090: 3135 2031 373a 3239 2b30 3230 300a 504f  15 17:29+0200.PO
+00000090: 3236 2032 333a 3539 2b30 3230 300a 504f  26 23:59+0200.PO
 000000a0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000b0: 3230 3230 2d30 342d 3231 2030 303a 3231  2020-04-21 00:21
 000000c0: 2b30 3230 300a 4c61 7374 2d54 7261 6e73  +0200.Last-Trans
 000000d0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000e0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
 000000f0: 0a4c 616e 6775 6167 653a 2073 720a 4c61  .Language: sr.La
 00000100: 6e67 7561 6765 2d54 6561 6d3a 2073 7220  nguage-Team: sr
```

### Comparing `little-brother-0.4.8/little_brother/translations/th/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/th/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-19 23:19+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: th\n"
 "Language-Team: th <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/translations/tr/LC_MESSAGES/messages.mo` & `little-brother-0.4.9/little_brother/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-08-15 17:29+0200\n"
+"POT-Creation-Date: 2021-08-26 23:59+0200\n"
 "PO-Revision-Date: 2020-04-19 23:19+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `little-brother-0.4.8/little_brother/user_locale_handler.py` & `little-brother-0.4.9/little_brother/user_locale_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/user_manager.py` & `little-brother-0.4.9/little_brother/user_manager.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/user_status.py` & `little-brother-0.4.9/little_brother/user_status.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/web/about_view_handler.py` & `little-brother-0.4.9/little_brother/web/login_view_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,54 +14,37 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import flask
 
 from little_brother import constants
-from little_brother import git
-from little_brother import settings
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import tools
 from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
+BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
+
 # Dummy function to trigger extraction by pybabel...
 _ = lambda x: x
 
-BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
-
-class AboutViewHandler(BaseViewHandler):
+class LoginViewHandler(BaseViewHandler):
 
     def __init__(self, p_package, p_languages):
-
-        super().__init__(p_blueprint_name=constants.ABOUT_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
+        super().__init__(p_blueprint_name=constants.LOGIN_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
                          p_package=p_package)
 
         self._languages = p_languages
 
-    @BLUEPRINT_ADAPTER.route_method("/about", endpoint="main_view")
-    def about_view(self):
-
+    def login_view(self):
         request = flask.request
-
         with tools.TimingContext(lambda duration: self.measure(p_hostname=request.remote_addr,
                                                                p_service=self.simplify_url(request.url_rule),
                                                                p_duration=duration)):
-            try:
-                page = flask.render_template(
-                    constants.ABOUT_HTML_TEMPLATE,
-                    rel_font_size=self.get_rel_font_size(),
-                    settings=settings.settings,
-                    extended_settings=settings.extended_settings,
-                    git_metadata=git.git_metadata,
-                    authentication=BaseWebServer.get_authentication_info(),
-                    languages=sorted([(a_locale, a_language) for a_locale, a_language in self._languages.items()]),
-                    navigation={
-                        'current_view': constants.ABOUT_BLUEPRINT_NAME + "." + constants.ABOUT_VIEW_NAME}
-                )
-
-            except Exception as e:
-                return self.handle_rendering_exception(p_page_name="about page", p_exception=e)
-
+            page = flask.render_template(
+                constants.LOGIN_HTML_TEMPLATE,
+                rel_font_size=self.get_rel_font_size(),
+                authentication=BaseWebServer.get_authentication_info(),
+            )
             return page
```

### Comparing `little-brother-0.4.8/little_brother/web/admin_view_handler.py` & `little-brother-0.4.9/little_brother/web/admin_view_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 import flask_login
 
 from little_brother import constants, entity_forms
 from little_brother import rule_override
 from little_brother.persistence.session_context import SessionContext
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import tools
-from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
 TIME_EXTENSION_SUBMIT_PATTERN = "time_extension_{username}_(off|-?[0-9]+)"
 
 BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
+
 # Dummy function to trigger extraction by pybabel...
-_ = lambda x: x
+def _(x):
+    return x
 
 
 class AdminViewHandler(BaseViewHandler):
 
     def __init__(self, p_package):
 
         super().__init__(p_blueprint_name=constants.ADMIN_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
@@ -67,22 +68,24 @@
                         self.save_admin_data(admin_infos, forms)
                         self.handle_button_press(admin_infos, request, session_context)
                         return flask.redirect(flask.url_for("admin.main_view"))
 
                     if not submitted:
                         self.load_from_model(admin_infos, forms)
 
-                    page = flask.render_template(
-                        constants.ADMIN_HTML_TEMPLATE,
-                        rel_font_size=self.get_rel_font_size(),
-                        admin_infos=admin_infos,
-                        authentication=BaseWebServer.get_authentication_info(),
-                        forms=forms,
-                        navigation={
-                            'current_view': constants.ADMIN_BLUEPRINT_NAME + "." + constants.ADMIN_VIEW_NAME})
+                    template_dict = {}
+                    self.add_general_template_data(p_dict=template_dict)
+                    template_dict["forms"] = forms
+                    template_dict["admin_infos"] = admin_infos
+                    template_dict["navigation"] = {
+                        'current_view': constants.ADMIN_BLUEPRINT_NAME + "." + constants.ADMIN_VIEW_NAME
+                    }
+                    self.add_version_info(p_dict=template_dict)
+
+                    page = flask.render_template(constants.ADMIN_HTML_TEMPLATE, **template_dict)
 
                 except Exception as e:
                     return self.handle_rendering_exception(p_page_name="admin page", p_exception=e)
 
                 return page
 
     def load_from_model(self, p_admin_infos, p_forms):
```

### Comparing `little-brother-0.4.8/little_brother/web/base_view_handler.py` & `little-brother-0.4.9/little_brother/web/base_view_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,31 +13,34 @@
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import flask
 
-from little_brother import dependency_injection, constants
+from little_brother import dependency_injection, constants, settings, git
 from little_brother.admin_data_handler import AdminDataHandler
+from little_brother.api.version_checker import VersionChecker, VersionInfo
 from little_brother.app_control import AppControl
 from little_brother.persistence.persistent_dependency_injection_mix_in import PersistenceDependencyInjectionMixIn
 from little_brother.process_handler_manager import ProcessHandlerManager
 from little_brother.rule_handler import RuleHandler
 from little_brother.user_manager import UserManager
 from python_base_app import log_handling
+from python_base_app.base_web_server import BaseWebServer
 from python_base_app.locale_helper import LocaleHelper
 from some_flask_helpers import blueprint_adapter
 
 LOCALE_REL_FONT_SIZES = {
     'bn': 125  # scale Bangla fonts to 125% for readability
 }
 
 FORM_ID_CSRF = 'csrf'
 
+
 class BaseViewHandler(PersistenceDependencyInjectionMixIn):
 
     def __init__(self, p_blueprint_name, p_blueprint_adapter, p_package):
 
         super().__init__()
 
         self._logger = log_handling.get_logger(self.__class__.__name__)
@@ -50,15 +53,15 @@
 
         self._app_control = None
         self._admin_data_handler = None
         self._rule_handler = None
         self._locale_helper = None
         self._process_handler_manager = None
         self._user_manager = None
-
+        self._version_checker = None
 
     @property
     def app_control(self) -> AppControl:
         if self._app_control is None:
             self._app_control = dependency_injection.container[AppControl]
 
         return self._app_control
@@ -95,14 +98,21 @@
     def user_manager(self) -> UserManager:
 
         if self._user_manager is None:
             self._user_manager = dependency_injection.container[UserManager]
 
         return self._user_manager
 
+    @property
+    def version_checker(self) -> VersionChecker:
+
+        if self._version_checker is None:
+            self._version_checker = dependency_injection.container[VersionChecker]
+
+        return self._version_checker
 
     @classmethod
     def validate(cls, p_forms):
 
         valid = True
         submitted = False
 
@@ -111,20 +121,19 @@
                 valid = False
 
             if form.is_submitted():
                 submitted = True
 
         return valid and submitted, submitted
 
-    def register(self, p_app, p_url_prefix:str=None):
+    def register(self, p_app, p_url_prefix: str = None):
 
         p_app.register_blueprint(self._blueprint, url_prefix=p_url_prefix)
         self._url_prefix = p_url_prefix
 
-
     def measure(self, p_hostname, p_service, p_duration):
 
         self.app_control.set_prometheus_http_requests_summary(
             p_hostname=p_hostname, p_service=p_service, p_duration=p_duration)
 
     def simplify_url(self, p_url):
         return str(p_url).replace(self._url_prefix, '')
@@ -140,14 +149,41 @@
     def get_rel_font_size(self):
 
         rel_font_size = LOCALE_REL_FONT_SIZES.get(self.locale_helper.locale)
         if not rel_font_size:
             rel_font_size = 100
         return rel_font_size
 
+    def add_general_template_data(self, p_dict):
+
+        p_dict["rel_font_size"] = self.get_rel_font_size()
+        p_dict["settings"] = settings.settings
+        p_dict["extended_settings"] = settings.extended_settings
+        p_dict["git_metadata"] = git.git_metadata
+        p_dict["authentication"] = BaseWebServer.get_authentication_info()
+
+    def add_version_info(self, p_dict):
+
+        current_revision = settings.extended_settings["debian_package_revision"]
+        channel = self.app_control._config.update_channel
+
+        suggested_version_info: VersionInfo = self.version_checker.is_revision_current(p_channel=channel,
+                                                                                       p_revision=current_revision)
+
+        if suggested_version_info is not None:
+            format_dict = {
+                "channel": channel,
+                "current_version": settings.settings["version"],
+                "current_revision": current_revision,
+                "suggested_version": suggested_version_info.version,
+                "suggested_revision": suggested_version_info.revision,
+                "download_url": self.version_checker.get_download_url(p_channel=channel)
+            }
+
+            p_dict["version_format_dict"] = format_dict
 
     def destroy(self):
         self._blueprint_adapter.unassign_view_handler_instances()
 
     def gettext(self, p_text):
         return self.locale_helper.gettext(p_text=p_text)
 
@@ -157,8 +193,7 @@
         self._logger.exception(msg.format(exception=str(p_exception), page_name=p_page_name))
 
         return flask.render_template(
             constants.INTERNAL_ERROR_HTML_TEMPLATE,
             rel_font_size=self.get_rel_font_size(),
             error_message=str(p_exception)
         )
-
```

### Comparing `little-brother-0.4.8/little_brother/web/devices_view_handler.py` & `little-brother-0.4.9/little_brother/web/devices_view_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 
 from little_brother import constants
 from little_brother import entity_forms
 from little_brother.persistence.session_context import SessionContext
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import custom_fields
 from python_base_app import tools
-from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
 HTML_KEY_NEW_DEVICE = "NewDevice"
 
 BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
+
 # Dummy function to trigger extraction by pybabel...
-_ = lambda x: x
+def _(x):
+    return x
 
 
 class DevicesViewHandler(BaseViewHandler):
 
     def __init__(self, p_package):
 
         super().__init__(p_blueprint_name=constants.DEVICES_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
@@ -112,24 +113,24 @@
 
                         return flask.redirect(flask.url_for("devices.main_view"))
 
                     if not submitted:
                         for device in devices:
                             forms[device.device_name].load_from_model(p_model=device)
 
-                    page = flask.render_template(
-                        constants.DEVICES_HTML_TEMPLATE,
-                        rel_font_size=self.get_rel_font_size(),
-                        devices=devices,
-                        authentication=BaseWebServer.get_authentication_info(),
-                        forms=forms,
-                        new_device_html_key=HTML_KEY_NEW_DEVICE,
-                        new_device_submit_value=HTML_KEY_NEW_DEVICE,
-                        navigation={
-                            'current_view': constants.DEVICES_BLUEPRINT_NAME + "." + constants.DEVICES_VIEW_NAME
-                        },
-                    )
+                    template_dict = {}
+                    self.add_general_template_data(p_dict=template_dict)
+                    template_dict["forms"] = forms
+                    template_dict["devices"] = devices
+                    template_dict["new_device_html_key"] = HTML_KEY_NEW_DEVICE
+                    template_dict["new_device_submit_value"] = HTML_KEY_NEW_DEVICE
+                    template_dict["navigation"] = {
+                        'current_view': constants.DEVICES_BLUEPRINT_NAME + "." + constants.DEVICES_VIEW_NAME
+                    }
+                    self.add_version_info(p_dict=template_dict)
+
+                    page = flask.render_template(constants.DEVICES_HTML_TEMPLATE, **template_dict)
 
                 except Exception as e:
                     return self.handle_rendering_exception(p_page_name="devices page", p_exception=e)
 
             return page
```

### Comparing `little-brother-0.4.8/little_brother/web/login_view_handler.py` & `little-brother-0.4.9/little_brother/web/about_view_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,50 @@
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import flask
 
 from little_brother import constants
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import tools
-from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
-BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
 # Dummy function to trigger extraction by pybabel...
-_ = lambda x: x
+def _(x):
+    return x
+
 
+BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
-class LoginViewHandler(BaseViewHandler):
+
+class AboutViewHandler(BaseViewHandler):
 
     def __init__(self, p_package, p_languages):
-        super().__init__(p_blueprint_name=constants.LOGIN_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
+
+        super().__init__(p_blueprint_name=constants.ABOUT_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
                          p_package=p_package)
 
         self._languages = p_languages
 
-    def login_view(self):
+    @BLUEPRINT_ADAPTER.route_method("/about", endpoint="main_view")
+    def about_view(self):
+
         request = flask.request
+
         with tools.TimingContext(lambda duration: self.measure(p_hostname=request.remote_addr,
                                                                p_service=self.simplify_url(request.url_rule),
                                                                p_duration=duration)):
-            page = flask.render_template(
-                constants.LOGIN_HTML_TEMPLATE,
-                rel_font_size=self.get_rel_font_size(),
-                authentication=BaseWebServer.get_authentication_info(),
-            )
+            try:
+                template_dict = {}
+                self.add_general_template_data(p_dict=template_dict)
+                template_dict["languages"] = sorted(
+                    [(a_locale, a_language) for a_locale, a_language in self._languages.items()])
+                template_dict["navigation"] = {
+                    'current_view': constants.ABOUT_BLUEPRINT_NAME + "." + constants.ABOUT_VIEW_NAME
+                }
+
+                page = flask.render_template(constants.ABOUT_HTML_TEMPLATE, **template_dict)
+
+            except Exception as e:
+                return self.handle_rendering_exception(p_page_name="about page", p_exception=e)
+
             return page
```

### Comparing `little-brother-0.4.8/little_brother/web/status_view_handler.py` & `little-brother-0.4.9/little_brother/web/status_view_handler.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother/web/topology_view_handler.py` & `little-brother-0.4.9/little_brother/web/topology_view_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 import flask
 import flask_login
 
 from little_brother import constants
 from little_brother.persistence.session_context import SessionContext
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import tools
-from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
+
 # Dummy function to trigger extraction by pybabel...
-_ = lambda x: x
+def _(x):
+    return x
+
 
 BLUEPRINT_NAME = "topology"
 
 BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
+
 class TopologyViewHandler(BaseViewHandler):
 
     def __init__(self, p_package):
 
         super().__init__(p_blueprint_name=BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
                          p_package=p_package)
 
@@ -46,21 +49,23 @@
         request = flask.request
         with tools.TimingContext(lambda duration: self.measure(p_hostname=request.remote_addr,
                                                                p_service=self.simplify_url(request.url_rule),
                                                                p_duration=duration)):
             with SessionContext(p_persistence=self.persistence) as session_context:
                 try:
                     topology_infos = self.app_control.get_topology_infos(p_session_context=session_context)
-                    page = flask.render_template(
-                        constants.TOPOLOGY_HTML_TEMPLATE,
-                        rel_font_size=self.get_rel_font_size(),
-                        topology_infos=topology_infos,
-                        app_control_config=self.app_control._config,
-                        authentication=BaseWebServer.get_authentication_info(),
-                        navigation={
-                            'current_view': constants.TOPOLOGY_BLUEPRINT_NAME + "." + constants.TOPOLOGY_VIEW_NAME},
-                    )
+
+                    template_dict = {}
+                    self.add_general_template_data(p_dict=template_dict)
+                    template_dict["topology_infos"] = topology_infos
+                    template_dict["app_control_config"] = self.app_control._config
+                    template_dict["navigation"] = {
+                        'current_view': constants.TOPOLOGY_BLUEPRINT_NAME + "." + constants.TOPOLOGY_VIEW_NAME
+                    }
+                    self.add_version_info(p_dict=template_dict)
+
+                    page = flask.render_template(constants.TOPOLOGY_HTML_TEMPLATE, **template_dict)
 
                 except Exception as e:
                     return self.handle_rendering_exception(p_page_name="topology page", p_exception=e)
 
                 return page
```

### Comparing `little-brother-0.4.8/little_brother/web/users_view_handler.py` & `little-brother-0.4.9/little_brother/web/users_view_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 
 from little_brother import constants
 from little_brother import entity_forms
 from little_brother.persistence.session_context import SessionContext
 from little_brother.web.base_view_handler import BaseViewHandler
 from python_base_app import custom_fields
 from python_base_app import tools
-from python_base_app.base_web_server import BaseWebServer
 from some_flask_helpers import blueprint_adapter
 
 ID_PREFIX = '{id}_'
 
 HTML_KEY_NEW_USER = "NewUser"
 
 BLUEPRINT_ADAPTER = blueprint_adapter.BlueprintAdapter()
 
+
 # Dummy function to trigger extraction by pybabel...
-_ = lambda x: x
+def _(x):
+    return x
 
 
 class UsersViewHandler(BaseViewHandler):
 
     def __init__(self, p_package, p_languages):
 
         super().__init__(p_blueprint_name=constants.USERS_BLUEPRINT_NAME, p_blueprint_adapter=BLUEPRINT_ADAPTER,
@@ -67,89 +68,101 @@
                         self.handle_button_press(p_forms=forms, p_request=request, p_session_context=session_context,
                                                  p_users=users)
                         return flask.redirect(flask.url_for("users.main_view"))
 
                     if not submitted:
                         self.load_from_model(p_forms=forms, p_users=users)
 
-                    page = flask.render_template(
-                        constants.USERS_HTML_TEMPLATE,
-                        rel_font_size=self.get_rel_font_size(),
-                        users=users,
-                        authentication=BaseWebServer.get_authentication_info(),
-                        forms=forms,
-                        new_user_html_key=HTML_KEY_NEW_USER,
-                        new_user_submit_value=HTML_KEY_NEW_USER,
-                        navigation={
-                            'current_view': constants.USERS_BLUEPRINT_NAME + "." + constants.USERS_VIEW_NAME
-                        },
-                    )
+                    dict = {}
+                    self.add_general_template_data(p_dict=dict)
+                    dict["forms"] = forms
+                    dict["users"] = users
+                    dict["new_user_html_key"] = HTML_KEY_NEW_USER
+                    dict["new_user_submit_value"] = HTML_KEY_NEW_USER
+                    dict["navigation"] = {
+                        'current_view': constants.USERS_BLUEPRINT_NAME + "." + constants.USERS_VIEW_NAME
+                    }
+                    self.add_version_info(p_dict=dict)
+
+                    page = flask.render_template(constants.USERS_HTML_TEMPLATE, **dict)
 
                 except Exception as e:
                     return self.handle_rendering_exception(p_page_name="users page", p_exception=e)
 
             return page
 
     def load_from_model(self, p_forms, p_users):
 
         for user in p_users:
             p_forms[user.html_key].load_from_model(p_model=user)
 
-            for ruleset in user.rulesets:
-                p_forms[ruleset.html_key].load_from_model(p_model=ruleset)
+            for rule_set in user.rulesets:
+                p_forms[rule_set.html_key].load_from_model(p_model=rule_set)
                 # provide a callback function so that the RuleSet can retrieve context summaries
-                ruleset._get_context_rule_handler = self.rule_handler.get_context_rule_handler
+                rule_set._get_context_rule_handler = self.rule_handler.get_context_rule_handler
 
             for user2device in user.devices:
                 p_forms[user2device.html_key].load_from_model(p_model=user2device)
 
+    def handle_button_press_for_rule_set(self, p_session_context, p_submit_id, p_rule_set):
+
+        if p_submit_id == p_rule_set.delete_html_key:
+            self.rule_set_entity_manager.delete_ruleset(
+                p_session_context=p_session_context, p_ruleset_id=p_rule_set.id)
+
+        elif p_submit_id == p_rule_set.move_down_html_key:
+            self.rule_set_entity_manager.move_down_ruleset(
+                p_session_context=p_session_context, p_ruleset_id=p_rule_set.id)
+
+        elif p_submit_id == p_rule_set.move_up_html_key:
+            self.rule_set_entity_manager.move_up_ruleset(
+                p_session_context=p_session_context, p_ruleset_id=p_rule_set.id)
+
+    def handle_button_press_for_user(self, p_forms, p_session_context, p_submit_id, p_user):
+
+        if p_submit_id == p_user.delete_html_key:
+            self.user_entity_manager.delete_user(
+                p_session_context=p_session_context, p_username=p_user.username)
+            self.persistence.clear_cache()
+            self.app_control.send_config_to_all_slaves()
+
+        elif p_submit_id == p_user.new_ruleset_html_key:
+            self.user_entity_manager.assign_ruleset(
+                p_session_context=p_session_context, p_username=p_user.username)
+
+        elif p_submit_id == p_user.new_device_html_key:
+            device_id = int(p_forms[p_user.new_device_html_key].device_id.data)
+            self.user_2_device_entity_manager.add_user2device(
+                p_session_context=p_session_context, p_device_id=device_id,
+                p_username=p_user.username)
+
+        else:
+            for rule_set in p_user.rulesets:
+                self.handle_button_press_for_rule_set(p_session_context=p_session_context,
+                                                      p_submit_id=p_submit_id, p_rule_set=rule_set)
+
+            for user2device in p_user.devices:
+                if p_submit_id == user2device.delete_html_key:
+                    self.user_2_device_entity_manager.delete_user2device(
+                        p_session_context=p_session_context, p_user2device_id=user2device.id)
+
     def handle_button_press(self, p_forms, p_request, p_session_context, p_users):
 
-        if p_request.form['submit'] == HTML_KEY_NEW_USER:
+        submit_id = p_request.form['submit']
+
+        if submit_id == HTML_KEY_NEW_USER:
             username = p_forms[HTML_KEY_NEW_USER].username.data
             self.app_control.add_new_user(p_session_context=p_session_context,
                                           p_username=username, p_locale=self._locale_helper.locale)
             # TODO: after adding new user Users window should be opened for new user
 
         else:
             for user in p_users:
-                if p_request.form['submit'] == user.delete_html_key:
-                    self.user_entity_manager.delete_user(
-                        p_session_context=p_session_context, p_username=user.username)
-                    self.persistence.clear_cache()
-                    self.app_control.send_config_to_all_slaves()
-
-                elif p_request.form['submit'] == user.new_ruleset_html_key:
-                    self.user_entity_manager.assign_ruleset(
-                        p_session_context=p_session_context, p_username=user.username)
-
-                elif p_request.form['submit'] == user.new_device_html_key:
-                    device_id = int(p_forms[user.new_device_html_key].device_id.data)
-                    self.user_2_device_entity_manager.add_user2device(
-                        p_session_context=p_session_context, p_device_id=device_id,
-                        p_username=user.username)
-
-                else:
-                    for ruleset in user.rulesets:
-                        if p_request.form['submit'] == ruleset.delete_html_key:
-                            self.rule_set_entity_manager.delete_ruleset(
-                                p_session_context=p_session_context, p_ruleset_id=ruleset.id)
-
-                        elif p_request.form['submit'] == ruleset.move_down_html_key:
-                            self.rule_set_entity_manager.move_down_ruleset(
-                                p_session_context=p_session_context, p_ruleset_id=ruleset.id)
-
-                        elif p_request.form['submit'] == ruleset.move_up_html_key:
-                            self.rule_set_entity_manager.move_up_ruleset(
-                                p_session_context=p_session_context, p_ruleset_id=ruleset.id)
-
-                    for user2device in user.devices:
-                        if p_request.form['submit'] == user2device.delete_html_key:
-                            self.user_2_device_entity_manager.delete_user2device(
-                                p_session_context=p_session_context, p_user2device_id=user2device.id)
+                self.handle_button_press_for_user(p_forms=p_forms, p_session_context=p_session_context,
+                                                  p_submit_id=submit_id, p_user=user)
 
     def get_users_forms(self, p_session_context, p_users):
 
         forms = {}
 
         unmonitored_users = self.app_control.get_unmonitored_users(p_session_context)
 
@@ -159,32 +172,32 @@
             forms[HTML_KEY_NEW_USER] = new_user_form
 
         for user in p_users:
             form = entity_forms.UserForm(prefix=ID_PREFIX.format(id=user.html_key), meta={'csrf': True})
             form.locale.choices = sorted([(locale, language) for locale, language in self._languages.items()])
             forms[user.html_key] = form
 
-            for ruleset in user.rulesets:
+            for rule_set in user.rulesets:
                 localized_values = [(value, self.gettext(value))
                                     for value in self.rule_handler.get_context_rule_handler_choices()]
 
-                if ruleset.fixed_context:
-                    choices = self.add_labels([ruleset.context])
+                if rule_set.fixed_context:
+                    choices = self.add_labels([rule_set.context])
 
                 else:
                     choices = self.add_labels(self.rule_handler.get_context_rule_handler_names())
 
                 context_details_filters = [
                     lambda x: custom_fields.unlocalize(p_localized_values=localized_values, p_value=x)]
 
                 form = entity_forms.create_rulesets_form(p_context_choices=choices,
                                                          p_localized_context_details=localized_values,
                                                          p_context_details_filters=context_details_filters,
-                                                         prefix=ID_PREFIX.format(id=ruleset.html_key))
-                forms[ruleset.html_key] = form
+                                                         prefix=ID_PREFIX.format(id=rule_set.html_key))
+                forms[rule_set.html_key] = form
 
                 form.context_details.validators = [
                     lambda a_form, a_field: self.rule_handler.validate_context_rule_handler_details(
                         p_context_name=a_form.context.data, p_context_details=a_field.data)]
 
             unmonitored_devices = self.app_control.get_unmonitored_devices(p_user=user,
                                                                            p_session_context=p_session_context)
@@ -199,51 +212,76 @@
             for user2device in user.devices:
                 form = entity_forms.User2DeviceForm(prefix=ID_PREFIX.format(id=user2device.html_key),
                                                     meta={'csrf': True})
                 forms[user2device.html_key] = form
 
         return forms
 
+    def save_for_user2device(self, p_form, p_session_context, p_user2device):
+
+        changed = False
+        a_persistent_user_2_device = self.user_2_device_entity_manager.get_by_id(
+            p_session_context=p_session_context, p_id=p_user2device.id)
+
+        if a_persistent_user_2_device is not None and p_form.differs_from_model(
+                p_model=a_persistent_user_2_device):
+            p_form.save_to_model(p_model=a_persistent_user_2_device)
+            changed = True
+
+        return changed
+
+    def save_for_rule_set(self, p_form, p_session_context, p_rule_set):
+
+        changed = False
+        a_persistent_rule_set = self.rule_set_entity_manager.get_by_id(
+            p_session_context=p_session_context, p_id=p_rule_set.id)
+
+        if a_persistent_rule_set is not None and p_form.differs_from_model(p_model=a_persistent_rule_set):
+            p_form.save_to_model(p_model=a_persistent_rule_set)
+            changed = True
+
+        return changed
+
     def save_users_data(self, p_users, p_forms):
 
         with SessionContext(p_persistence=self.persistence) as session_context:
             session = session_context.get_session()
             changed = False
 
             for user in p_users:
-                form = p_forms[user.html_key]
-                a_persistent_user = self.user_entity_manager.get_by_username(
-                    p_session_context=session_context, p_username=user.username)
-
-                if a_persistent_user is not None and form.differs_from_model(p_model=a_persistent_user):
-                    form.save_to_model(p_model=a_persistent_user)
+                if self.save_for_user(p_forms=p_forms, p_session_context=session_context, p_user=user):
                     changed = True
 
-                for ruleset in user.rulesets:
-                    form = p_forms[ruleset.html_key]
-                    a_persistent_ruleset = self.rule_set_entity_manager.get_by_id(
-                        p_session_context=session_context, p_id=ruleset.id)
-
-                    if a_persistent_ruleset is not None and form.differs_from_model(p_model=a_persistent_ruleset):
-                        form.save_to_model(p_model=a_persistent_ruleset)
-                        changed = True
-
-                for user2device in user.devices:
-                    form = p_forms[user2device.html_key]
-                    a_persistent_user_2_device = self.user_2_device_entity_manager.get_by_id(
-                        p_session_context=session_context, p_id=user2device.id)
-
-                    if a_persistent_user_2_device is not None and form.differs_from_model(
-                            p_model=a_persistent_user_2_device):
-                        form.save_to_model(p_model=a_persistent_user_2_device)
-                        changed = True
-
             if changed:
                 session.commit()
-
                 self._persistence.clear_cache()
                 self.app_control.send_config_to_all_slaves()
                 self.user_manager.reset_users(p_session_context=session_context)
 
+    def save_for_user(self, p_forms, p_session_context, p_user):
+
+        changed = False
+        form = p_forms[p_user.html_key]
+        a_persistent_user = self.user_entity_manager.get_by_username(
+            p_session_context=p_session_context, p_username=p_user.username)
+
+        if a_persistent_user is not None and form.differs_from_model(p_model=a_persistent_user):
+            form.save_to_model(p_model=a_persistent_user)
+            changed = True
+
+        for rule_set in p_user.rulesets:
+            form = p_forms[rule_set.html_key]
+
+            if self.save_for_rule_set(p_form=form, p_session_context=p_session_context, p_rule_set=rule_set):
+                changed = True
+
+        for user2device in p_user.devices:
+            form = p_forms[user2device.html_key]
+
+            if self.save_for_user2device(p_form=form, p_session_context=p_session_context, p_user2device=user2device):
+                changed = True
+
+        return changed
+
     def add_labels(self, p_value_list):
 
         return [(entry, self.gettext(entry)) for entry in p_value_list]
```

### Comparing `little-brother-0.4.8/little_brother/web/web_server.py` & `little-brother-0.4.9/little_brother/web/web_server.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/little_brother.egg-info/SOURCES.txt` & `little-brother-0.4.9/little_brother.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 little_brother/alembic/versions/9713cef84918_userstatus_issue_130.py
 little_brother/alembic/versions/__init__.py
 little_brother/alembic/versions/e0c0d7048235_prohibited_process_name_pattern.py
 little_brother/alembic/versions/version_0_3_added_tables_for_configuration_gui.py
 little_brother/api/__init__.py
 little_brother/api/api_view_handler.py
 little_brother/api/master_connector.py
+little_brother/api/version_checker.py
 little_brother/persistence/__init__.py
 little_brother/persistence/base_entity.py
 little_brother/persistence/base_entity_manager.py
 little_brother/persistence/persistence.py
 little_brother/persistence/persistence_base.py
 little_brother/persistence/persistent_admin_event.py
 little_brother/persistence/persistent_admin_event_entity_manager.py
@@ -114,20 +115,22 @@
 little_brother/templates/helper.macros.html
 little_brother/templates/internal_error.template.html
 little_brother/templates/login.template.html
 little_brother/templates/navbar.include.html
 little_brother/templates/status.template.html
 little_brother/templates/topology.template.html
 little_brother/templates/users.template.html
+little_brother/templates/version_check.include.html
 little_brother/test/__init__.py
 little_brother/test/dummy_process_handler.py
 little_brother/test/dummy_process_iterator.py
 little_brother/test/test_app.py
 little_brother/test/test_app_control.py
 little_brother/test/test_client_device_handler.py
+little_brother/test/test_client_info.py
 little_brother/test/test_client_process_handler.py
 little_brother/test/test_data.py
 little_brother/test/test_german_vacation_context_rule_handler.py
 little_brother/test/test_language.py
 little_brother/test/test_process_handler.py
 little_brother/test/test_process_handler_manager.py
 little_brother/test/test_process_info.py
```

### Comparing `little-brother-0.4.8/run_little_brother.py` & `little-brother-0.4.9/run_little_brother.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/run_little_brother_test_suite.py` & `little-brother-0.4.9/run_little_brother_test_suite.py`

 * *Files identical despite different names*

### Comparing `little-brother-0.4.8/setup.py` & `little-brother-0.4.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "long_description": "Tool to monitor login time of users on Debian hosts and terminate processes if usage times "
                         "are exceeded.",
 }
 
 extended_setup_params = {
 
     # Target version to be used to upgrade the database
-    "target_alembic_version": "647cf46033a9",
+    "target_alembic_version": "9713cef84918",
 
     "docker_registry_user": "marcusrickert",
     # Docker image contexts to be built. The second entry of the tuple denotes if the resulting image is to be uploaded
     "docker_contexts": [ ('little-brother-base', False),
                          #'docker/little-brother-master',
                          ('little-brother-slave', True),
                          ],
@@ -72,27 +72,29 @@
     "create_group": True,
     "user_group_mappings": [("little-brother", "audio")],
     "deploy_systemd_service": True,
     # "deploy_tmpfile_conf": True,
     "deploy_sudoers_file": True,
     "deploy_apparmor_file": True,
     "contributing_setups": ["python_base_app", "some_flask_helpers"],
-    "publish_debian_package": ["master", "release"],
-    "publish_docker_images": ["master", "release"],
-    "publish_latest_docker_image": "release",
+    "publish_debian_package": little_brother.settings.SOURCEFORGE_CHANNELS,
+    "publish_docker_images": little_brother.settings.DOCKER_CHANNELS,
+    "publish_latest_docker_image": little_brother.settings.RELEASE_BRANCH_NAME,
     "debian_extra_files": [
         ("etc/slave.config", "etc/little-brother/slave.config"),
         ("etc/master.config", "etc/little-brother/master.config"),
     ],
     "debian_templates": [
         ("/etc/little-brother/master.config", "/etc/little-brother/little-brother.config")
     ],
     "build_pypi_package": True,
-    "publish_pypi_package": {'release': ('https://upload.pypi.org/legacy/', 'PYPI_API_TOKEN'),
-                             'master': ('https://test.pypi.org/legacy/', 'TEST_PYPI_API_TOKEN')},
+    "publish_pypi_package": {
+        little_brother.settings.RELEASE_BRANCH_NAME: ('https://upload.pypi.org/legacy/', 'PYPI_API_TOKEN'),
+        little_brother.settings.MASTER_BRANCH_NAME: ('https://test.pypi.org/legacy/', 'TEST_PYPI_API_TOKEN')
+    },
     "generate_generic_install": True,
     "analyze": True,
     "analyze_extra_exclusions" : "vagrant/**",
     "script_timeout": 30,
 }
 
 setup_params.update(little_brother.settings.settings)
```

