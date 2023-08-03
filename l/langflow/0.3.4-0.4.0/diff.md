# Comparing `tmp/langflow-0.3.4.tar.gz` & `tmp/langflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.3.4.tar", max compression
+gzip compressed data, was "langflow-0.4.0.tar", max compression
```

## Comparing `langflow-0.3.4.tar` & `langflow-0.4.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0     1065 2023-08-03 00:57:59.215266 langflow-0.3.4/LICENSE
--rw-r--r--   0        0        0    15941 2023-08-03 00:57:59.215266 langflow-0.3.4/README.md
--rw-r--r--   0        0        0     3072 2023-08-03 00:57:59.699296 langflow-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      514 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0    10217 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       61 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      485 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0     2380 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      526 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     4486 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     4979 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0     7325 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     2534 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/components.py
--rw-r--r--   0        0        0     4740 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     2691 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/flow_styles.py
--rw-r--r--   0        0        0     3868 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     2625 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     4439 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      152 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     1815 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4554 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/cache/flow.py
--rw-r--r--   0        0        0     4481 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     5062 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/cache/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/chat/__init__.py
--rw-r--r--   0        0        0       45 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/chat/config.py
--rw-r--r--   0        0        0     8554 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/chat/manager.py
--rw-r--r--   0        0        0     1272 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/chat/utils.py
--rw-r--r--   0        0        0    13474 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1733 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/__init__.py
--rw-r--r--   0        0        0     1665 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/models/__init__.py
--rw-r--r--   0        0        0      363 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/models/base.py
--rw-r--r--   0        0        0     1120 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/models/component.py
--rw-r--r--   0        0        0     1705 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/models/flow.py
--rw-r--r--   0        0        0      831 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/database/models/flow_style.py
--rw-r--r--   0        0        0  4229439 2023-08-03 00:59:26.076636 langflow-0.3.4/src/backend/langflow/frontend/assets/index-5ae96ba1.js
--rw-r--r--   0        0        0   206636 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/assets/index-e6b0df28.css
--rw-r--r--   0        0        0    23161 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0    26806 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0     4310 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      724 2023-08-03 00:59:26.072635 langflow-0.3.4/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      764 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     2349 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     7854 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2165 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      642 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0     9589 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0     8507 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2423 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10224 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4682 2023-08-03 00:57:59.699296 langflow-0.3.4/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     3068 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4843 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0      194 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/__init__.py
--rw-r--r--   0        0        0     1594 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/base.py
--rw-r--r--   0        0        0     8937 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/code_parser.py
--rw-r--r--   0        0        0     2099 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/component.py
--rw-r--r--   0        0        0     1700 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/constants.py
--rw-r--r--   0        0        0     6354 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/custom_component.py
--rw-r--r--   0        0        0     8115 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/directory_reader.py
--rw-r--r--   0        0        0      529 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom/schema.py
--rw-r--r--   0        0        0     2306 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1479 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     6123 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      385 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    18655 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     3407 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/initialize/utils.py
--rw-r--r--   0        0        0     7779 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0     2048 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2135 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/output_parsers/__init__.py
--rw-r--r--   0        0        0     2355 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/output_parsers/base.py
--rw-r--r--   0        0        0       87 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2483 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2086 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     2764 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1450 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2598 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5418 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      913 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1269 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0    12782 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2696 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1500 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      428 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0     2505 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     2013 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     8650 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      579 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/server.py
--rw-r--r--   0        0        0     4805 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     2571 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      423 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     7033 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     9840 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7796 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1694 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0      998 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/custom_components.py
--rw-r--r--   0        0        0     8636 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     1680 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      297 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5569 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5370 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6559 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0      364 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/output_parsers.py
--rw-r--r--   0        0        0     3540 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2023-08-03 00:57:59.703296 langflow-0.3.4/src/backend/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2355 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     4016 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     9428 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     1181 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      915 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0       23 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/types.py
--rw-r--r--   0        0        0    13928 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     7665 2023-08-03 00:57:59.707296 langflow-0.3.4/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    19015 1970-01-01 00:00:00.000000 langflow-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-02 19:09:35.287042 langflow-0.4.0/LICENSE
+-rw-r--r--   0        0        0    15941 2023-08-02 19:09:35.287042 langflow-0.4.0/README.md
+-rw-r--r--   0        0        0     3038 2023-08-02 19:09:35.735039 langflow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      514 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0    10217 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       61 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      485 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0     2380 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      526 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     4486 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     4979 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0     7325 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     2534 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/components.py
+-rw-r--r--   0        0        0     4740 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     2691 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/flow_styles.py
+-rw-r--r--   0        0        0     3868 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     2625 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     4439 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      152 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4554 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/cache/flow.py
+-rw-r--r--   0        0        0     4481 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     5062 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/cache/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/chat/__init__.py
+-rw-r--r--   0        0        0       45 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/chat/config.py
+-rw-r--r--   0        0        0     8554 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/chat/manager.py
+-rw-r--r--   0        0        0     1272 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/chat/utils.py
+-rw-r--r--   0        0        0    13474 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1733 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/__init__.py
+-rw-r--r--   0        0        0     1665 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/models/base.py
+-rw-r--r--   0        0        0     1120 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/models/component.py
+-rw-r--r--   0        0        0     1705 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/models/flow.py
+-rw-r--r--   0        0        0      831 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/database/models/flow_style.py
+-rw-r--r--   0        0        0  4229439 2023-08-02 19:10:34.027084 langflow-0.4.0/src/backend/langflow/frontend/assets/index-5ae96ba1.js
+-rw-r--r--   0        0        0   206636 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/assets/index-e6b0df28.css
+-rw-r--r--   0        0        0    23161 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0    26806 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0     4310 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      724 2023-08-02 19:10:34.023084 langflow-0.4.0/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      764 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     2349 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     7854 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     2165 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      642 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0     9589 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0     8507 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     2423 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10224 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4682 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2867 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4843 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0      194 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/__init__.py
+-rw-r--r--   0        0        0     1594 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/base.py
+-rw-r--r--   0        0        0     8937 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/code_parser.py
+-rw-r--r--   0        0        0     2099 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/component.py
+-rw-r--r--   0        0        0     1700 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/constants.py
+-rw-r--r--   0        0        0     6354 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/custom_component.py
+-rw-r--r--   0        0        0     8115 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/directory_reader.py
+-rw-r--r--   0        0        0      529 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom/schema.py
+-rw-r--r--   0        0        0     2306 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1479 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     6123 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0    18655 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     3407 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/initialize/utils.py
+-rw-r--r--   0        0        0     7704 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0     2048 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     2135 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2355 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/output_parsers/base.py
+-rw-r--r--   0        0        0       87 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2483 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/retrievers/__init__.py
+-rw-r--r--   0        0        0     2086 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/retrievers/base.py
+-rw-r--r--   0        0        0     2764 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1450 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.739039 langflow-0.4.0/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2598 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5418 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      913 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1269 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0    12782 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2696 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1500 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      428 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0     2505 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     2013 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     8650 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      579 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     4805 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     2571 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      423 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     7033 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     9840 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7796 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1694 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0      998 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/custom_components.py
+-rw-r--r--   0        0        0     8636 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     1680 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      297 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5569 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0     5370 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     6559 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0      364 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/output_parsers.py
+-rw-r--r--   0        0        0     3540 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0      523 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/retrievers.py
+-rw-r--r--   0        0        0     2355 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     4016 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0      823 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0     9428 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     1181 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      915 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0       23 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/types.py
+-rw-r--r--   0        0        0    13928 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     7665 2023-08-02 19:09:35.743039 langflow-0.4.0/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    18960 1970-01-01 00:00:00.000000 langflow-0.4.0/PKG-INFO
```

### Comparing `langflow-0.3.4/LICENSE` & `langflow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/README.md` & `langflow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/pyproject.toml` & `langflow-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.3.4"
+version = "0.4.0"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
@@ -72,15 +72,14 @@
 supabase = "^1.0.3"
 pymongo = "^4.4.0"
 certifi = "^2023.5.7"
 google-cloud-aiplatform = "^1.26.1"
 psycopg = "^3.1.9"
 psycopg-binary = "^3.1.9"
 fastavro = "^1.8.0"
-langchain-experimental = "^0.0.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ipykernel = "^6.21.2"
 mypy = "^1.1.1"
 ruff = "^0.0.254"
 httpx = "*"
```

### Comparing `langflow-0.3.4/src/backend/langflow/__init__.py` & `langflow-0.4.0/src/backend/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/__main__.py` & `langflow-0.4.0/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/utils.py` & `langflow-0.4.0/src/backend/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/__init__.py` & `langflow-0.4.0/src/backend/langflow/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/base.py` & `langflow-0.4.0/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/callback.py` & `langflow-0.4.0/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/chat.py` & `langflow-0.4.0/src/backend/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/components.py` & `langflow-0.4.0/src/backend/langflow/api/v1/components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.4.0/src/backend/langflow/api/v1/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/flow_styles.py` & `langflow-0.4.0/src/backend/langflow/api/v1/flow_styles.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/flows.py` & `langflow-0.4.0/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/schemas.py` & `langflow-0.4.0/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/api/v1/validate.py` & `langflow-0.4.0/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/cache/base.py` & `langflow-0.4.0/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/cache/flow.py` & `langflow-0.4.0/src/backend/langflow/cache/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/cache/manager.py` & `langflow-0.4.0/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/cache/utils.py` & `langflow-0.4.0/src/backend/langflow/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/chat/manager.py` & `langflow-0.4.0/src/backend/langflow/chat/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/chat/utils.py` & `langflow-0.4.0/src/backend/langflow/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/config.yaml` & `langflow-0.4.0/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/custom/customs.py` & `langflow-0.4.0/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/database/base.py` & `langflow-0.4.0/src/backend/langflow/database/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/database/models/component.py` & `langflow-0.4.0/src/backend/langflow/database/models/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/database/models/flow.py` & `langflow-0.4.0/src/backend/langflow/database/models/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/database/models/flow_style.py` & `langflow-0.4.0/src/backend/langflow/database/models/flow_style.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/assets/index-5ae96ba1.js` & `langflow-0.4.0/src/backend/langflow/frontend/assets/index-5ae96ba1.js`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/assets/index-e6b0df28.css` & `langflow-0.4.0/src/backend/langflow/frontend/assets/index-e6b0df28.css`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow-0.4.0/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/assets/robot-95e1b00d.png` & `langflow-0.4.0/src/backend/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.4.0/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/favicon.ico` & `langflow-0.4.0/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/frontend/index.html` & `langflow-0.4.0/src/backend/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/__init__.py` & `langflow-0.4.0/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/edge/base.py` & `langflow-0.4.0/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/graph/base.py` & `langflow-0.4.0/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/graph/constants.py` & `langflow-0.4.0/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/utils.py` & `langflow-0.4.0/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/vertex/base.py` & `langflow-0.4.0/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/graph/vertex/types.py` & `langflow-0.4.0/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/agents/base.py` & `langflow-0.4.0/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/agents/custom.py` & `langflow-0.4.0/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.4.0/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/base.py` & `langflow-0.4.0/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/chains/base.py` & `langflow-0.4.0/src/backend/langflow/interface/chains/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from langflow.interface.base import LangChainTypeCreator
 from langflow.interface.importing.utils import import_class
 from langflow.settings import settings
 from langflow.template.frontend_node.chains import ChainFrontendNode
 from langflow.utils.logger import logger
 from langflow.utils.util import build_template_from_class, build_template_from_method
 from langchain import chains
-from langchain_experimental.sql import SQLDatabaseChain
 
 # Assuming necessary imports for Field, Template, and FrontendNode classes
 
 
 class ChainCreator(LangChainTypeCreator):
     type_name: str = "chains"
 
@@ -32,17 +31,14 @@
         if self.type_dict is None:
             self.type_dict: dict[str, Any] = {
                 chain_name: import_class(f"langchain.chains.{chain_name}")
                 for chain_name in chains.__all__
             }
             from langflow.interface.chains.custom import CUSTOM_CHAINS
 
-            # Now add from langchain_experimental.sql import SQLDatabaseChain
-            self.type_dict["SQLDatabaseChain"] = SQLDatabaseChain
-
             self.type_dict.update(CUSTOM_CHAINS)
             # Filter according to settings.chains
             self.type_dict = {
                 name: chain
                 for name, chain in self.type_dict.items()
                 if name in settings.chains or settings.dev
             }
```

### Comparing `langflow-0.3.4/src/backend/langflow/interface/chains/custom.py` & `langflow-0.4.0/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/base.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/code_parser.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/code_parser.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/component.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/constants.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/custom_component.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/custom_component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/directory_reader.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/directory_reader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom/schema.py` & `langflow-0.4.0/src/backend/langflow/interface/custom/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/custom_lists.py` & `langflow-0.4.0/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.4.0/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.4.0/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/importing/utils.py` & `langflow-0.4.0/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.4.0/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/initialize/utils.py` & `langflow-0.4.0/src/backend/langflow/interface/initialize/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.4.0/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,27 +126,26 @@
 
 
 def initialize_pinecone(class_object: Type[Pinecone], params: dict):
     """Initialize pinecone and return the class object"""
 
     import pinecone  # type: ignore
 
-    pinecone_api_key = params.pop("pinecone_api_key", None)
-    pinecone_env = params.pop("pinecone_env", None)
+    pinecone_api_key = params.get("pinecone_api_key")
+    pinecone_env = params.get("pinecone_env")
 
     if pinecone_api_key is None or pinecone_env is None:
         if os.getenv("PINECONE_API_KEY") is not None:
             pinecone_api_key = os.getenv("PINECONE_API_KEY")
         if os.getenv("PINECONE_ENV") is not None:
             pinecone_env = os.getenv("PINECONE_ENV")
 
     if pinecone_api_key is None or pinecone_env is None:
         raise ValueError(
-            "Pinecone API key and environment must be provided through the component params"
-            " or through environment variables"
+            "Pinecone API key and environment must be provided in the params"
         )
 
     # initialize pinecone
     pinecone.init(
         api_key=pinecone_api_key,  # find at app.pinecone.io
         environment=pinecone_env,  # next to api key in console
     )
```

### Comparing `langflow-0.3.4/src/backend/langflow/interface/listing.py` & `langflow-0.4.0/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/llms/base.py` & `langflow-0.4.0/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/memories/base.py` & `langflow-0.4.0/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/output_parsers/base.py` & `langflow-0.4.0/src/backend/langflow/interface/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/prompts/base.py` & `langflow-0.4.0/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.4.0/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/retrievers/base.py` & `langflow-0.4.0/src/backend/langflow/interface/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/run.py` & `langflow-0.4.0/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.4.0/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.4.0/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/tools/base.py` & `langflow-0.4.0/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/tools/constants.py` & `langflow-0.4.0/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/tools/custom.py` & `langflow-0.4.0/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/tools/util.py` & `langflow-0.4.0/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/types.py` & `langflow-0.4.0/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/utilities/base.py` & `langflow-0.4.0/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/utils.py` & `langflow-0.4.0/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.4.0/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.4.0/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/main.py` & `langflow-0.4.0/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/processing/base.py` & `langflow-0.4.0/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/processing/process.py` & `langflow-0.4.0/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/server.py` & `langflow-0.4.0/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/settings.py` & `langflow-0.4.0/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/field/base.py` & `langflow-0.4.0/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/custom_components.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/custom_components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/retrievers.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/retrievers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.4.0/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/template/template/base.py` & `langflow-0.4.0/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/utils/constants.py` & `langflow-0.4.0/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/utils/logger.py` & `langflow-0.4.0/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/utils/payload.py` & `langflow-0.4.0/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/utils/util.py` & `langflow-0.4.0/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/src/backend/langflow/utils/validate.py` & `langflow-0.4.0/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.4/PKG-INFO` & `langflow-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.3.4
+Version: 0.4.0
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -33,15 +33,14 @@
 Requires-Dist: google-api-python-client (>=2.79.0,<3.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: gunicorn (>=21.1.0,<22.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.16.0,<0.17.0)
 Requires-Dist: jina (==3.15.2)
 Requires-Dist: langchain (>=0.0.250,<0.0.251)
-Requires-Dist: langchain-experimental (>=0.0.8,<0.0.9)
 Requires-Dist: langchain-serve (>0.0.51) ; extra == "deploy"
 Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.3.4 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.4.0 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Carlos Coelho Maintainer-email:
 carlos@logspace.ai Requires-Python: >=3.9,<3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Provides-Extra: all Provides-Extra: deploy Provides-
@@ -14,37 +14,37 @@
 "local" Requires-Dist: docstring-parser (>=0.15,<0.16) Requires-Dist: faiss-cpu
 (>=1.7.4,<2.0.0) Requires-Dist: fake-useragent (>=1.1.3,<2.0.0) Requires-Dist:
 fastapi (>=0.100.0,<0.101.0) Requires-Dist: fastavro (>=1.8.0,<2.0.0) Requires-
 Dist: google-api-python-client (>=2.79.0,<3.0.0) Requires-Dist: google-cloud-
 aiplatform (>=1.26.1,<2.0.0) Requires-Dist: google-search-results
 (>=2.4.1,<3.0.0) Requires-Dist: gunicorn (>=21.1.0,<22.0.0) Requires-Dist:
 huggingface-hub[inference] (>=0.16.0,<0.17.0) Requires-Dist: jina (==3.15.2)
-Requires-Dist: langchain (>=0.0.250,<0.0.251) Requires-Dist: langchain-
-experimental (>=0.0.8,<0.0.9) Requires-Dist: langchain-serve (>0.0.51) ; extra
-== "deploy" Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
-Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: multiprocess
-(>=0.70.14,<0.71.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: openai
-(>=0.27.8,<0.28.0) Requires-Dist: orjson (>=3.9.1,<4.0.0) Requires-Dist: pandas
-(>=2.0.0,<3.0.0) Requires-Dist: pinecone-client (>=2.2.2,<3.0.0) Requires-Dist:
-psycopg (>=3.1.9,<4.0.0) Requires-Dist: psycopg-binary (>=3.1.9,<4.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0) Requires-Dist: pyarrow
-(>=12.0.0,<13.0.0) Requires-Dist: pymongo (>=4.4.0,<5.0.0) Requires-Dist: pypdf
-(>=3.11.0,<4.0.0) Requires-Dist: pysrt (>=1.1.2,<2.0.0) Requires-Dist: python-
-multipart (>=0.0.6,<0.0.7) Requires-Dist: qdrant-client (>=1.3.0,<2.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist: sentence-transformers
-(>=2.2.2,<3.0.0) ; extra == "local" Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
-Requires-Dist: supabase (>=1.0.3,<2.0.0) Requires-Dist: tiktoken
-(>=0.4.0,<0.5.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: types-
-cachetools (>=5.3.0.5,<6.0.0.0) Requires-Dist: unstructured (>=0.7.0,<0.8.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Requires-Dist: weaviate-client
-(>=3.21.0,<4.0.0) Requires-Dist: websockets (>=10.3,<11.0) Requires-Dist:
-wikipedia (>=1.4.0,<2.0.0) Project-URL: Repository, https://github.com/
-logspace-ai/langflow Description-Content-Type: text/markdown  # âï¸ Langflow
-~ An effortless way to experiment and prototype [LangChain](https://github.com/
-hwchase17/langchain) pipelines ~
+Requires-Dist: langchain (>=0.0.250,<0.0.251) Requires-Dist: langchain-serve
+(>0.0.51) ; extra == "deploy" Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0)
+; extra == "local" Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist:
+multiprocess (>=0.70.14,<0.71.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-
+Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: orjson (>=3.9.1,<4.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: pinecone-client
+(>=2.2.2,<3.0.0) Requires-Dist: psycopg (>=3.1.9,<4.0.0) Requires-Dist:
+psycopg-binary (>=3.1.9,<4.0.0) Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0) Requires-Dist: pymongo
+(>=4.4.0,<5.0.0) Requires-Dist: pypdf (>=3.11.0,<4.0.0) Requires-Dist: pysrt
+(>=1.1.2,<2.0.0) Requires-Dist: python-multipart (>=0.0.6,<0.0.7) Requires-
+Dist: qdrant-client (>=1.3.0,<2.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "local"
+Requires-Dist: sqlmodel (>=0.0.8,<0.0.9) Requires-Dist: supabase
+(>=1.0.3,<2.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0) Requires-Dist: typer
+(>=0.9.0,<0.10.0) Requires-Dist: types-cachetools (>=5.3.0.5,<6.0.0.0)
+Requires-Dist: unstructured (>=0.7.0,<0.8.0) Requires-Dist: uvicorn
+(>=0.22.0,<0.23.0) Requires-Dist: weaviate-client (>=3.21.0,<4.0.0) Requires-
+Dist: websockets (>=10.3,<11.0) Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
+Project-URL: Repository, https://github.com/logspace-ai/langflow Description-
+Content-Type: text/markdown  # âï¸ Langflow ~ An effortless way to
+experiment and prototype [LangChain](https://github.com/hwchase17/langchain)
+pipelines ~
 [GitHub Contributors] [GitHub Last Commit]  [GitHub Issues] [GitHub Pull
 Requests] [Github License]
 [Discord_Server] [HuggingFace_Spaces]
 [https://github.com/logspace-ai/langflow/blob/main/img/langflow-
 demo.gif?raw=true]
 # Table of Contents - [âï¸ Langflow](#ï¸-langflow) - [Table of Contents]
 (#table-of-contents) - [ð¦ Installation](#-installation) - [Locally]
```

