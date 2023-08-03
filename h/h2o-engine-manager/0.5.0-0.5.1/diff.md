# Comparing `tmp/h2o_engine_manager-0.5.0.tar.gz` & `tmp/h2o_engine_manager-0.5.1.tar.gz`

## Comparing `h2o_engine_manager-0.5.0.tar` & `h2o_engine_manager-0.5.1.tar`

### file list

```diff
@@ -1,273 +1,275 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/Makefile
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/requirements.txt
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/docs/templates/config.mako
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/docs/templates/text.mako
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/local/ambassador_host.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/local/example.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/.openapi-generator-ignore
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/__init__.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/connection_config.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/exception.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_cli_config.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/login.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/duration_convertor.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/client_info.py
--rw-r--r--   0        0        0    21489 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
--rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/expression.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/client.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/dai_version.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/mapper.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/__init__.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/client.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/engine.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/mapper.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/page.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/state.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/token_api_client.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/__init__.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/__init__.py
--rw-r--r--   0        0        0    18472 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py
--rw-r--r--   0        0        0    12778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/page.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/state.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/client.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/mapper.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
--rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
--rw-r--r--   0        0        0    65707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
--rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
--rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
--rw-r--r--   0        0        0    21803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
--rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py
--rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
--rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
--rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/__init__.py
--rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api_client.py
--rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/configuration.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/exceptions.py
--rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model_utils.py
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/rest.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/__init__.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/__init__.py
--rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    20794 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
--rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
--rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
--rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
--rw-r--r--   0        0        0    20349 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
--rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/setup.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_admission_webhook.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/create_dai_request.py
--rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_create.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_delete.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_get.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list_versions.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_upgrade_available.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/engine/test_list_engines.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_create_h2o_engine.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_delete_h2o_engine.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_get_h2o_engine.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_engines.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_versions.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_connect.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_current_idle_running_duration.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_resume.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_lifecycle.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_login_discovery.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migrate_creator.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migration.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_update.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_upgrade_version.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_logs.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-connect.yaml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-setup.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/system.default.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_3.yaml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_4.yaml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5_mock.yaml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6.yaml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6_1.yaml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/system.default.yaml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/0_0_0_0_latest.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_38_0_4.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_40_0_4.yaml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/sw_pods_creation/no_labels.yaml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_dai_engine.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_duration_convertor.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_engine_id_generator.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_engine_state.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_filter.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_h2o_cli_config.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/dai_version/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/dai_version/test_mapper.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_data/h2o-cli-config.toml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/README.md
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/Makefile
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/requirements.txt
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/docs/templates/config.mako
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/docs/templates/text.mako
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/local/ambassador_host.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/local/example.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/.openapi-generator-ignore
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/__init__.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/connection_config.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/exception.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_cli_config.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/login.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/convert/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/convert/duration_convertor.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/convert/quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/client_info.py
+-rw-r--r--   0        0        0    21489 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
+-rw-r--r--   0        0        0    20402 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/expression.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/client.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/dai_version.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/mapper.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/__init__.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/client.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/engine.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/mapper.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/page.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/state.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/token_api_client.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine_id/__init__.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine_id/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/__init__.py
+-rw-r--r--   0        0        0    18906 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/client.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/client_info.py
+-rw-r--r--   0        0        0    12778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/page.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/state.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/__init__.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/client.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/mapper.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
+-rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    65707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
+-rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
+-rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
+-rw-r--r--   0        0        0    21803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
+-rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/__init__.py
+-rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
+-rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/__init__.py
+-rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/api_client.py
+-rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/configuration.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/exceptions.py
+-rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model_utils.py
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/rest.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/api/__init__.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/__init__.py
+-rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    20794 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
+-rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
+-rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
+-rw-r--r--   0        0        0    20349 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
+-rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/setup.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_admission_webhook.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/create_dai_request.py
+-rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_create.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_delete.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_get.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_list.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_list_versions.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai/test_upgrade_available.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/engine/test_list_engines.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_create_h2o_engine.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_delete_h2o_engine.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_get_h2o_engine.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_list_h2o_engines.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_list_h2o_versions.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_connect.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_current_idle_running_duration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_dai_pod_template_spec.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_dai_resume.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_lifecycle.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_login_discovery.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_migrate_creator.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_migration.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_update.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_upgrade_version.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_logs.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-connect.yaml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-setup.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/system.default.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_3.yaml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_4.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_5.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_5_mock.yaml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_6.yaml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_6_1.yaml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/h2o-setup.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/system.default.yaml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_versions/0_0_0_0_latest.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_versions/3_38_0_4.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_versions/3_40_0_4.yaml
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/sw_pods_creation/no_labels.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_dai_engine.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_duration_convertor.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_engine_id_generator.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_engine_state.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_filter.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_h2o_cli_config.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/dai_version/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/dai_version/test_mapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/ssl/__init__.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/ssl/test_client_ssl_config.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/tests/unit/test_data/h2o-cli-config.toml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/README.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.1/PKG-INFO
```

### Comparing `h2o_engine_manager-0.5.0/requirements.txt` & `h2o_engine_manager-0.5.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/docs/templates/config.mako` & `h2o_engine_manager-0.5.1/docs/templates/config.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/docs/templates/text.mako` & `h2o_engine_manager-0.5.1/docs/templates/text.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/local/example.py` & `h2o_engine_manager-0.5.1/local/example.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/connection_config.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/connection_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/exception.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/exception.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_cli_config.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_cli_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/login.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 def login(
     environment: Optional[str] = None,
     token_provider: Callable[[], str] = None,
     platform_token: Optional[str] = None,
     default_workspace_id: str = "default",
     config_path: str = DEFAULT_CONFIG_PATH,
+    verify_ssl: bool = True,
+    ssl_ca_cert: Optional[str] = None,
 ) -> Clients:
     """Initializes AI Engine Manager clients for H2O AI Cloud.
 
     All arguments are optional. Configuration-less login is dependent on having the H2O CLI configured.
     See: https://docs.h2o.ai/h2o-ai-cloud/developerguide/cli#platform-token
     The Discovery Service is used to discover the Engine Manager service endpoint.
     See: https://pypi.org/project/h2o-cloud-discovery/
@@ -44,14 +46,16 @@
         platform_token (str, optional): H2O Platform Token.
             If neither 'token_provider' nor 'platform_token' is provided the platform token will be read
             from the H2O CLI configuration.
         default_workspace_id (str, optional): The default workspace ID which will client use to manipulate with
             resources. Defaults to `default`.
         config_path: (str, optional): Path to the H2O AI Cloud configuration file.
             Defaults to '~/.h2oai/h2o-cli-config.toml'.
+        verify_ssl: Set to False to disable SSL certificate verification.
+        ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
 
     Raises:
         FileNotFoundError: When the H2O CLI configuration file is needed but cannot be found.
         TomlDecodeError: When the H2O CLI configuration file is needed but cannot be processed.
         LookupError: When the service endpoint cannot be discovered.
         ConnectionError: When a communication with server failed.
     """
@@ -65,60 +69,75 @@
     else:
         cfg = discover_platform_connection(
             environment_url=environment,
             platform_token=platform_token,
             config_path=config_path,
         )
 
-    return __init_clients(cfg, default_workspace_id)
+    return __init_clients(
+        cfg=cfg, default_workspace_id=default_workspace_id, verify_ssl=verify_ssl, ssl_ca_cert=ssl_ca_cert,
+    )
 
 
 def login_custom(
     endpoint: str,
     refresh_token: str,
     issuer_url: str,
     client_id: str,
     client_secret: Optional[str] = None,
     default_workspace_id: str = "default",
+    verify_ssl: bool = True,
+    ssl_ca_cert: Optional[str] = None,
 ) -> Clients:
     """Initializes AI Engine Manager clients.
 
     Args:
         endpoint (str): The Engine Manager service endpoint URL (e.g. https://enginemanager.cloud.h2o.ai).
         refresh_token (str): The OIDC refresh token.
         issuer_url (str): The OIDC issuer URL.
         client_id (str): The OIDC Client ID that issued the 'refresh_token'.
         client_secret (str, optional): Optional OIDC Client Secret that issued the 'refresh_token'. Defaults to None.
         default_workspace_id (str, optional): The default workspace ID which will client use to manipulate with
             resources. Defaults to `default`.
+        verify_ssl: Set to False to disable SSL certificate verification.
+        ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
     """
     # Remove trailing slash from the URL for the generated clients
     endpoint = endpoint.rstrip("/")
     cfg = get_connection(
         aiem_url=endpoint,
         refresh_token=refresh_token,
         issuer_url=issuer_url,
         client_id=client_id,
         client_secret=client_secret,
     )
 
-    return __init_clients(cfg, default_workspace_id)
+    return __init_clients(
+        cfg=cfg, default_workspace_id=default_workspace_id, verify_ssl=verify_ssl, ssl_ca_cert=ssl_ca_cert,
+    )
 
 
-def __init_clients(cfg: ConnectionConfig, default_workspace_id: str):
+def __init_clients(
+    cfg: ConnectionConfig,
+    default_workspace_id: str,
+    verify_ssl: bool,
+    ssl_ca_cert: str,
+):
     # Verify that the server is reachable
     version_url = urljoin(cfg.aiem_url, "version")
     resp = requests.get(version_url)
     if not (200 <= resp.status_code <= 299):
         raise ConnectionError(
             f"Server is not reachable. Status code: {resp.status_code}, Response body: {resp.text}"
         )
 
     dai_engine_client = DAIEngineClient(
-        connection_config=cfg, default_workspace_id=default_workspace_id
+        connection_config=cfg, default_workspace_id=default_workspace_id, verify_ssl=verify_ssl,
+        ssl_ca_cert=ssl_ca_cert,
     )
     h2o_engine_client = H2OEngineClient(
-        connection_config=cfg, default_workspace_id=default_workspace_id
+        connection_config=cfg, default_workspace_id=default_workspace_id, verify_ssl=verify_ssl,
+        ssl_ca_cert=ssl_ca_cert,
     )
     return Clients(
         dai_engine_client=dai_engine_client, h2o_engine_client=h2o_engine_client
     )
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/duration_convertor.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/convert/duration_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/convert/quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/client_info.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict
 from typing import List
+from typing import Optional
 
 from h2o_engine_manager.clients.connection_config import ConnectionConfig
 from h2o_engine_manager.clients.convert import duration_convertor
 from h2o_engine_manager.clients.convert import quantity_convertor
 from h2o_engine_manager.clients.dai_engine.client_info import ClientInfo
 from h2o_engine_manager.clients.dai_engine.dai_engine import DAIEngine
 from h2o_engine_manager.clients.dai_engine.dai_engine import from_dai_engine_api_object
@@ -25,31 +26,46 @@
     V1DAIEngine as APIEngine,
 )
 
 
 class DAIEngineClient:
     """DAIEngineClient manages Driverless AI engines."""
 
-    def __init__(self, connection_config: ConnectionConfig, default_workspace_id: str):
+    def __init__(
+        self,
+        connection_config: ConnectionConfig,
+        default_workspace_id: str,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
+    ):
         """Initializes DAIEngineClient.
         Do not initialize manually, use `h2o_engine_manager.login()` instead.
 
         Args:
             connection_config (ConnectionConfig): AIEM connection configuration object.
             default_workspace_id (str): The default workspace ID which will client use to manipulate with DAI engines.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
         self.default_workspace_id = default_workspace_id
 
         configuration = Configuration(host=connection_config.aiem_url)
+        configuration.verify_ssl = verify_ssl
+        configuration.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiClient(
             configuration, connection_config.token_provider
         ) as api_client:
             api_instance = DAIEngineServiceApi(api_client)
 
-        self.dai_version_client = DAIVersionClient(connection_config=connection_config)
+        self.dai_version_client = DAIVersionClient(
+            connection_config=connection_config,
+            verify_ssl=verify_ssl,
+            ssl_ca_cert=ssl_ca_cert,
+        )
 
         self.client_info = ClientInfo(
             url=connection_config.aiem_url,
             token_provider=connection_config.token_provider,
             api_instance=api_instance,
         )
 
@@ -140,15 +156,16 @@
 
         if max_running_duration is not None:
             max_running_duration = duration_convertor.duration_to_seconds(
                 max_running_duration
             )
 
         if engine_id is None:
-            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="dai", engine_getter=self.get_engine)
+            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="dai",
+                                           engine_getter=self.get_engine)
 
         api_engine = APIEngine(
             version=version,
             cpu=cpu,
             gpu=gpu,
             memory_bytes=memory_bytes,
             storage_bytes=storage_bytes,
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/expression.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/expression.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,62 @@
+from typing import Optional
+
 from h2o_engine_manager.clients.connection_config import get_connection
-from h2o_engine_manager.clients.dai_engine_constraint.token_api_client import (
+from h2o_engine_manager.clients.h2o_engine_constraint.token_api_client import (
     TokenApiClient,
 )
-from h2o_engine_manager.gen.dai_engine_constraint_set_service.api.dai_engine_constraint_set_service_api import (
-    DAIEngineConstraintSetServiceApi,
+from h2o_engine_manager.gen.h2o_engine_constraint_set_service.api.h2_o_engine_constraint_set_service_api import (
+    H2OEngineConstraintSetServiceApi,
 )
-from h2o_engine_manager.gen.dai_engine_constraint_set_service.configuration import (
+from h2o_engine_manager.gen.h2o_engine_constraint_set_service.configuration import (
     Configuration,
 )
-from h2o_engine_manager.gen.dai_engine_constraint_set_service.model.v1_dai_engine_constraint_set import (
-    V1DAIEngineConstraintSet,
+from h2o_engine_manager.gen.h2o_engine_constraint_set_service.model.v1_h2_o_engine_constraint_set import (
+    V1H2OEngineConstraintSet,
 )
 
 
-class DAIEngineConstraintSetClient:
-    """DAIEngineConstraintSetClient manages DAIEngineConstraintSets."""
+class H2OEngineConstraintSetClient:
+    """H2OEngineConstraintSetClient manages H2OEngineConstraintSets."""
 
     def __init__(
         self,
         url: str,
         platform_token: str,
         platform_oidc_url: str,
         platform_oidc_client_id: str,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
     ):
-        """Initializes DAIEngineConstraintSetClient.
+        """Initializes H2OEngineConstraintSetClient.
 
         Args:
             url (str): URL of AI Engine Manager Gateway.
             platform_token (str): H2O.ai platform token.
             platform_oidc_url (str): Base URL of the platform_token OIDC issuer.
             platform_oidc_client_id (str): OIDC Client ID associated with the platform_token.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
 
         cfg = get_connection(
             aiem_url=url,
             refresh_token=platform_token,
             issuer_url=platform_oidc_url,
             client_id=platform_oidc_client_id,
         )
 
         engine_cfg = Configuration(host=url)
+        engine_cfg.verify_ssl = verify_ssl
+        engine_cfg.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiClient(
             engine_cfg, cfg.token_provider
         ) as engine_service_api_client:
-            self.service_api = DAIEngineConstraintSetServiceApi(
+            self.service_api = H2OEngineConstraintSetServiceApi(
                 engine_service_api_client
             )
 
-    def get_constraint_set(self, workspace_id: str) -> V1DAIEngineConstraintSet:
-        return self.service_api.d_ai_engine_constraint_set_service_get_dai_engine_constraint_set(
-            name=f"workspaces/{workspace_id}/daiEngineConstraintSet"
-        ).dai_engine_constraint_set
+    def get_constraint_set(self, workspace_id: str) -> V1H2OEngineConstraintSet:
+        return self.service_api.h2_o_engine_constraint_set_service_get_h2_o_engine_constraint_set(
+            name=f"workspaces/{workspace_id}/h2oEngineConstraintSet"
+        ).h2o_engine_constraint_set
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+from typing import Optional
 
 from h2o_engine_manager.clients.connection_config import ConnectionConfig
 from h2o_engine_manager.clients.dai_version.dai_version import DAIVersion
 from h2o_engine_manager.clients.dai_version.page import DAIVersionsPage
 from h2o_engine_manager.clients.dai_version.token_api_client import (
     TokenApiDAIVersionClient,
 )
@@ -15,24 +16,35 @@
     Configuration as DAIVersionConfiguration,
 )
 
 
 class DAIVersionClient:
     """DAIVersionClient manages Driverless AI versions."""
 
-    def __init__(self, connection_config: ConnectionConfig):
+    def __init__(
+        self,
+        connection_config:
+        ConnectionConfig,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
+    ):
         """Initializes DAIVersionClient.
 
         Args:
             connection_config (ConnectionConfig): AIEM connection configuration object.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
 
         configuration_dai_version = DAIVersionConfiguration(
             host=connection_config.aiem_url
         )
+        configuration_dai_version.verify_ssl = verify_ssl
+        configuration_dai_version.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiDAIVersionClient(
             configuration_dai_version, connection_config.token_provider
         ) as api_dai_version_client:
             self.api_version_instance = DAIVersionServiceApi(api_dai_version_client)
 
     def list_versions(
         self,
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/mapper.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/page.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/dai_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+from typing import Optional
 
 from h2o_engine_manager.clients.connection_config import get_connection
 from h2o_engine_manager.clients.engine.engine import Engine
 from h2o_engine_manager.clients.engine.page import EnginesPage
 from h2o_engine_manager.clients.engine.token_api_client import TokenApiClient
 from h2o_engine_manager.gen.engine_service.api.engine_service_api import (
     EngineServiceApi,
@@ -15,32 +16,39 @@
 
     def __init__(
         self,
         url: str,
         platform_token: str,
         platform_oidc_url: str,
         platform_oidc_client_id: str,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
     ):
         """Initializes EngineClient.
 
         Args:
             url (str): URL of AI Engine Manager Gateway.
             platform_token (str): H2O.ai platform token.
             platform_oidc_url (str): Base URL of the platform_token OIDC issuer.
             platform_oidc_client_id (str): OIDC Client ID associated with the platform_token.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
 
         cfg = get_connection(
             aiem_url=url,
             refresh_token=platform_token,
             issuer_url=platform_oidc_url,
             client_id=platform_oidc_client_id,
         )
 
         engine_cfg = Configuration(host=url)
+        engine_cfg.verify_ssl = verify_ssl
+        engine_cfg.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiClient(
             engine_cfg, cfg.token_provider
         ) as engine_service_api_client:
             self.engine_service_api = EngineServiceApi(engine_service_api_client)
 
     def list_engines(
         self,
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/mapper.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/page.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/generator.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/engine_id/generator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict
 from typing import List
+from typing import Optional
 
 from h2o_engine_manager.clients.connection_config import ConnectionConfig
 from h2o_engine_manager.clients.convert import duration_convertor
 from h2o_engine_manager.clients.convert import quantity_convertor
 from h2o_engine_manager.clients.engine_id.generator import generate_engine_id
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_engine.client_info import ClientInfo
@@ -24,25 +25,36 @@
 )
 from h2o_engine_manager.gen.h2o_engine_service.model.v1_h2_o_engine import V1H2OEngine
 
 
 class H2OEngineClient:
     """H2OEngineClient manages H2O engines."""
 
-    def __init__(self, connection_config: ConnectionConfig, default_workspace_id: str):
+    def __init__(
+        self,
+        connection_config: ConnectionConfig,
+        default_workspace_id: str,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
+    ):
         """Initializes H2OEngineClient.
         Do not initialize manually, use `h2o_engine_manager.login()` instead.
 
         Args:
             connection_config (ConnectionConfig): AIEM connection configuration object.
             default_workspace_id (str): The default workspace ID which will client use to manipulate with H2O engines.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
         self.default_workspace_id = default_workspace_id
 
         configuration = Configuration(host=connection_config.aiem_url)
+        configuration.verify_ssl = verify_ssl
+        configuration.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiClient(
             configuration, connection_config.token_provider
         ) as api_client:
             api_instance = H2OEngineServiceApi(api_client)
 
         self.h2o_version_client = H2OVersionClient(connection_config=connection_config)
 
@@ -125,16 +137,16 @@
 
         if max_running_duration is not None:
             max_running_duration = duration_convertor.duration_to_seconds(
                 max_running_duration
             )
 
         if engine_id is None:
-            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="h2o", engine_getter=self.get_engine)
-
+            engine_id = generate_engine_id(display_name=display_name, workspace_id=workspace_id, engine_type="h2o",
+                                           engine_getter=self.get_engine)
 
         api_engine = V1H2OEngine(
             version=version,
             node_count=node_count,
             cpu=cpu,
             gpu=gpu,
             memory_bytes=memory_bytes,
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/page.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+from typing import Optional
 
 from h2o_engine_manager.clients.connection_config import ConnectionConfig
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_version.h2o_version import H2OVersion
 from h2o_engine_manager.clients.h2o_version.page import H2OVersionsPage
 from h2o_engine_manager.clients.h2o_version.token_api_client import (
     TokenApiH2OVersionClient,
@@ -15,24 +16,34 @@
     Configuration as H2OVersionConfiguration,
 )
 
 
 class H2OVersionClient:
     """H2OVersionClient manages H2O versions."""
 
-    def __init__(self, connection_config: ConnectionConfig):
+    def __init__(
+        self,
+        connection_config: ConnectionConfig,
+        verify_ssl: bool = True,
+        ssl_ca_cert: Optional[str] = None,
+    ):
         """Initializes H2OVersionClient.
 
         Args:
             connection_config (ConnectionConfig): AIEM connection configuration object.
+            verify_ssl: Set to False to disable SSL certificate verification.
+            ssl_ca_cert: Path to a CA cert bundle with certificates of trusted CAs.
         """
 
         configuration_h2o_version = H2OVersionConfiguration(
             host=connection_config.aiem_url
         )
+        configuration_h2o_version.verify_ssl = verify_ssl
+        configuration_h2o_version.ssl_ca_cert = ssl_ca_cert
+
         with TokenApiH2OVersionClient(
             configuration_h2o_version, connection_config.token_provider
         ) as api_h2o_version_client:
             self.api_version_instance = H2OVersionServiceApi(api_h2o_version_client)
 
     def list_versions(
         self,
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/mapper.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/page.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/clients/h2o_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py` & `h2o_engine_manager-0.5.1/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/conftest.py` & `h2o_engine_manager-0.5.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/setup.py` & `h2o_engine_manager-0.5.1/tests/integration/setup.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_admission_webhook.py` & `h2o_engine_manager-0.5.1/tests/integration/test_admission_webhook.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/create_dai_request.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/create_dai_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_create.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_create.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_delete.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_delete.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_get.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_get.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_list.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list_versions.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_list_versions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_upgrade_available.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai/test_upgrade_available.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py` & `h2o_engine_manager-0.5.1/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/engine/test_list_engines.py` & `h2o_engine_manager-0.5.1/tests/integration/api/engine/test_list_engines.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_create_h2o_engine.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_create_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_delete_h2o_engine.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_delete_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_get_h2o_engine.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_get_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_engines.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_list_h2o_engines.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_versions.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o/test_list_h2o_versions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py` & `h2o_engine_manager-0.5.1/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_connect.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_connect.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_current_idle_running_duration.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_current_idle_running_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_dai_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_resume.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_dai_resume.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_lifecycle.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_login_discovery.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_login_discovery.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migrate_creator.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_migrate_creator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migration.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_migration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_update.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_update.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_upgrade_version.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/dai/test_upgrade_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_logs.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_logs.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py` & `h2o_engine_manager-0.5.1/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-connect.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-connect.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-lifecycle.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-setup.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/dai-setup.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/system.default.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/dai_setups/system.default.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/h2o-setup.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/system.default.yaml` & `h2o_engine_manager-0.5.1/tests/integration/test_data/h2o_setups/system.default.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_dai_engine.py` & `h2o_engine_manager-0.5.1/tests/unit/test_dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_duration_convertor.py` & `h2o_engine_manager-0.5.1/tests/unit/test_duration_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_engine_id_generator.py` & `h2o_engine_manager-0.5.1/tests/unit/test_engine_id_generator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_engine_state.py` & `h2o_engine_manager-0.5.1/tests/unit/test_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_filter.py` & `h2o_engine_manager-0.5.1/tests/unit/test_filter.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/test_quantity_convertor.py` & `h2o_engine_manager-0.5.1/tests/unit/test_quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/tests/unit/dai_version/test_mapper.py` & `h2o_engine_manager-0.5.1/tests/unit/dai_version/test_mapper.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/README.md` & `h2o_engine_manager-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.5.0/pyproject.toml` & `h2o_engine_manager-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 pattern = "(?P<version>.*)"
 
 [tool.hatch.envs.test]
 dependencies = [
     "pytest==7.3.1",
     "pytest-timeout==2.1.0",
     "kubernetes==23.3.0",
-    "websocket-client==1.3.2"
+    "websocket-client==1.3.2",
+    "pytest-httpserver==1.0.6",
+    "trustme==1.1.0"
 ]
 
 [tool.hatch.envs.test.scripts]
 unit = "python -m pytest tests/unit"
 api = [
     "python tests/integration/setup.py",
     "python -m pytest tests/integration/api",
```

### Comparing `h2o_engine_manager-0.5.0/PKG-INFO` & `h2o_engine_manager-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-engine-manager
-Version: 0.5.0
+Version: 0.5.1
 Summary: H2O Engine Manager python client
 Project-URL: Documentation, https://github.com/h2oai/ai-engine-manager#readme
 Project-URL: Issues, https://github.com/h2oai/ai-engine-manager/issues
 Project-URL: Source, https://github.com/h2oai/ai-engine-manager/py/h2o-engine-manager
 Author-email: Jan Sykora <jan.sykora@h2o.ai>, Tomas Pastorek <tomas.pastorek@h2o.ai>, Ondrej Bilek <ondrej.bilek@h2o.ai>
 Requires-Python: >=3.7
 Requires-Dist: certifi>=2022.12.7
```

