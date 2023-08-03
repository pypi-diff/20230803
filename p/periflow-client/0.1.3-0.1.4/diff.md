# Comparing `tmp/periflow_client-0.1.3.tar.gz` & `tmp/periflow_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.1.3.tar", max compression
+gzip compressed data, was "periflow_client-0.1.4.tar", max compression
```

## Comparing `periflow_client-0.1.3.tar` & `periflow_client-0.1.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     7965 2023-07-26 11:08:22.666762 periflow_client-0.1.3/README.md
--rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.3/periflow/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.3/periflow/auth.py
--rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.3/periflow/cli/__init__.py
--rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.3/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.3/periflow/cli/credential.py
--rw-r--r--   0        0        0    18875 2023-07-26 11:08:22.668089 periflow_client-0.1.3/periflow/cli/deployment.py
--rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.3/periflow/cli/group.py
--rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.3/periflow/cli/key.py
--rw-r--r--   0        0        0     6051 2023-07-26 09:29:06.022825 periflow_client-0.1.3/periflow/cli/main.py
--rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.3/periflow/cli/project.py
--rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.3/periflow/cli/vm.py
--rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.3/periflow/client/__init__.py
--rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.3/periflow/client/base.py
--rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.3/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.3/periflow/client/credential.py
--rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.3/periflow/client/deployment.py
--rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.3/periflow/client/file.py
--rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.3/periflow/client/group.py
--rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.3/periflow/client/project.py
--rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.3/periflow/client/user.py
--rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.3/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.3/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.3/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.3/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.3/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.3/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.3/periflow/context.py
--rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.3/periflow/converter/__init__.py
--rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.3/periflow/converter/base.py
--rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.3/periflow/converter/interface.py
--rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.3/periflow/converter/maps.py
--rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.3/periflow/converter/models/blenderbot.py
--rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.3/periflow/converter/models/bloom.py
--rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.3/periflow/converter/models/codegen.py
--rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.3/periflow/converter/models/falcon.py
--rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.3/periflow/converter/models/gpt2.py
--rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.3/periflow/converter/models/gpt_neox.py
--rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.3/periflow/converter/models/gptj.py
--rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.3/periflow/converter/models/llama.py
--rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.3/periflow/converter/models/mpt.py
--rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.3/periflow/converter/models/opt.py
--rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.3/periflow/converter/models/t5.py
--rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.3/periflow/converter/utils.py
--rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.3/periflow/enums.py
--rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.3/periflow/errors.py
--rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.3/periflow/formatter.py
--rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.3/periflow/logging.py
--rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.3/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.3/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.3/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.3/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.3/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.3/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.3/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.3/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.3/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.3/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.3/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.3/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5757 2023-07-26 11:08:22.668388 periflow_client-0.1.3/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    25710 2023-07-26 11:08:22.668715 periflow_client-0.1.3/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.3/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.3/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.3/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0    31619 2023-07-26 09:29:06.024041 periflow_client-0.1.3/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.3/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    17721 2023-07-26 11:08:22.669040 periflow_client-0.1.3/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.3/periflow/utils/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.3/periflow/utils/format.py
--rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.3/periflow/utils/fs.py
--rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.3/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.3/periflow/utils/prompt.py
--rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.3/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.3/periflow/utils/testing.py
--rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.3/periflow/utils/url.py
--rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.3/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.3/periflow/utils/version.py
--rw-r--r--   0        0        0     3417 2023-07-26 11:08:22.669323 periflow_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9700 1970-01-01 00:00:00.000000 periflow_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-08-03 04:10:39.047104 periflow_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7938 2023-08-03 04:10:39.047445 periflow_client-0.1.4/README.md
+-rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.4/periflow/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.4/periflow/auth.py
+-rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.4/periflow/cli/__init__.py
+-rw-r--r--   0        0        0    19433 2023-08-03 04:10:39.048824 periflow_client-0.1.4/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.4/periflow/cli/credential.py
+-rw-r--r--   0        0        0    18875 2023-07-26 11:08:22.668089 periflow_client-0.1.4/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.4/periflow/cli/group.py
+-rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.4/periflow/cli/key.py
+-rw-r--r--   0        0        0     6095 2023-08-03 04:10:39.049149 periflow_client-0.1.4/periflow/cli/main.py
+-rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.4/periflow/cli/project.py
+-rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.4/periflow/cli/vm.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.4/periflow/client/__init__.py
+-rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.4/periflow/client/base.py
+-rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.4/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.4/periflow/client/credential.py
+-rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.4/periflow/client/deployment.py
+-rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.4/periflow/client/file.py
+-rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.4/periflow/client/group.py
+-rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.4/periflow/client/project.py
+-rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.4/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.4/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.4/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.4/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.4/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.4/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3108 2023-08-03 04:10:39.049617 periflow_client-0.1.4/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.4/periflow/context.py
+-rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.4/periflow/converter/__init__.py
+-rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.4/periflow/converter/base.py
+-rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.4/periflow/converter/interface.py
+-rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.4/periflow/converter/maps.py
+-rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.4/periflow/converter/models/blenderbot.py
+-rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.4/periflow/converter/models/bloom.py
+-rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.4/periflow/converter/models/codegen.py
+-rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.4/periflow/converter/models/falcon.py
+-rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.4/periflow/converter/models/gpt2.py
+-rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.4/periflow/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.4/periflow/converter/models/gptj.py
+-rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.4/periflow/converter/models/llama.py
+-rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.4/periflow/converter/models/mpt.py
+-rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.4/periflow/converter/models/opt.py
+-rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.4/periflow/converter/models/t5.py
+-rw-r--r--   0        0        0     4653 2023-08-03 04:10:39.050057 periflow_client-0.1.4/periflow/converter/utils.py
+-rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.4/periflow/enums.py
+-rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.4/periflow/errors.py
+-rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.4/periflow/formatter.py
+-rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.4/periflow/logging.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.4/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.4/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.4/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.4/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.4/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.4/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.4/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.4/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.4/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.4/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.4/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.4/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5757 2023-07-26 11:08:22.668388 periflow_client-0.1.4/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    25710 2023-07-26 11:08:22.668715 periflow_client-0.1.4/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.4/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.4/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.4/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0    31434 2023-08-03 04:10:39.050373 periflow_client-0.1.4/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.4/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    18055 2023-08-03 04:10:39.050794 periflow_client-0.1.4/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.4/periflow/utils/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.4/periflow/utils/format.py
+-rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.4/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.4/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.4/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.4/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.4/periflow/utils/testing.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.4/periflow/utils/url.py
+-rw-r--r--   0        0        0     3938 2023-08-03 04:10:39.051071 periflow_client-0.1.4/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.4/periflow/utils/version.py
+-rw-r--r--   0        0        0     3417 2023-08-03 04:10:34.206346 periflow_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 periflow_client-0.1.4/PKG-INFO
```

### Comparing `periflow_client-0.1.3/README.md` & `periflow_client-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!---
 Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
 -->
 
 <p align="center">
-  <img src="https://drive.google.com/uc?id=1daafphR0ABKylj_0b1wtZ6n0ZRSVq5-s" width="80%" alt="system">
+  <img src="https://docs.periflow.ai/img/logo.svg" width="80%" alt="system">
 </p>
 
 <h2><p align="center">Supercharge Generative AI Serving 🚀</p></h2>
 
 <p align="center">
   <a href="https://github.com/friendliai/periflow-client/actions/workflows/ci.yaml">
     <img alt="CI Status" src="https://github.com/friendliai/periflow-client/actions/workflows/ci.yaml/badge.svg">
```

### Comparing `periflow_client-0.1.3/periflow/__init__.py` & `periflow_client-0.1.4/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/auth.py` & `periflow_client-0.1.4/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/checkpoint.py` & `periflow_client-0.1.4/periflow/cli/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 """PeriFlow Checkpoint CLI."""
 
 from __future__ import annotations
 
 import os
 from datetime import datetime
-from typing import Optional
+from typing import List, Optional
 from uuid import UUID
 
 import typer
 
 from periflow.enums import CheckpointCategory, CheckpointDataType, StorageType
 from periflow.errors import (
     CheckpointConversionError,
     InvalidAttributesError,
     InvalidConfigError,
     InvalidPathError,
     NotFoundError,
     NotSupportedError,
-    TokenizerNotFoundError,
 )
 from periflow.formatter import (
     JSONFormatter,
     PanelFormatter,
     TableFormatter,
     TreeFormatter,
 )
@@ -360,15 +359,22 @@
     panel_formatter.render([ckpt_dict])
     json_formatter.render(ckpt_dict["attributes"])
     tree_formatter.render(ckpt_dict["forms"][0]["files"])
 
 
 @app.command()
 def delete(
-    checkpoint_id: UUID = typer.Argument(..., help="ID of checkpoint to delete."),
+    checkpoint_ids: List[UUID] = typer.Argument(
+        ...,
+        help=(
+            "IDs of checkpoint to delete. "
+            "When multiple IDs are provided in a space-separated string format, all "
+            "corresponding checkpoints will be deleted."
+        ),
+    ),
     force: bool = typer.Option(
         False,
         "--force",
         "-f",
         help="Forcefully delete checkpoint without confirmation prompt.",
     ),
 ):
@@ -379,22 +385,31 @@
     checkpoint from the PeriFlow system. That is, it does not physically delete the
     checkpoint objects from the source cloud storage (your cloud storage).
 
     Checkpoints that are uploaded or generated from training jobs are physically deleted.
     :::
 
     """
+    targets_str = ""
+    for checkpoint_id in checkpoint_ids:
+        targets_str += str(checkpoint_id)
+        targets_str += "\n"
+
     if not force:
-        do_delete = typer.confirm("Are you sure to delete checkpoint?")
+        do_delete = typer.confirm(
+            f"Following checkpoints will be deleted:\n\n{targets_str}\n"
+            "Are your sure to delete these?"
+        )
         if not do_delete:
             raise typer.Abort()
 
-    CheckpointAPI.delete(id=checkpoint_id)
+    for checkpoint_id in checkpoint_ids:
+        CheckpointAPI.delete(id=checkpoint_id)
 
-    typer.secho("Checkpoint is deleted successfully!", fg=typer.colors.BLUE)
+    typer.secho("Checkpoints are deleted successfully!", fg=typer.colors.BLUE)
 
 
 @app.command()
 def download(
     checkpoint_id: UUID = typer.Argument(..., help="ID of checkpoint to download."),
     save_directory: Optional[str] = typer.Option(
         None,
@@ -688,15 +703,15 @@
             model_output_path=model_output_path,
             data_type=data_type,
             tokenizer_output_dir=tokenizer_output_dir,
             attr_output_path=attr_output_path,
             cache_dir=cache_dir,
             dry_run=dry_run,
         )
-    except (NotFoundError, CheckpointConversionError, TokenizerNotFoundError) as exc:
+    except (NotFoundError, CheckpointConversionError) as exc:
         secho_error_and_exit(str(exc))
 
     msg = (
         f"Checkpoint({model_name_or_path}) can be converted."
         if dry_run
         else f"Checkpoint({model_name_or_path}) is converted successfully."
     )
```

### Comparing `periflow_client-0.1.3/periflow/cli/credential.py` & `periflow_client-0.1.4/periflow/cli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/deployment.py` & `periflow_client-0.1.4/periflow/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/group.py` & `periflow_client-0.1.4/periflow/cli/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/key.py` & `periflow_client-0.1.4/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/main.py` & `periflow_client-0.1.4/periflow/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,24 @@
     project_context_path,
     set_current_group_id,
 )
 from periflow.formatter import PanelFormatter
 from periflow.utils.format import secho_error_and_exit
 from periflow.utils.request import DEFAULT_REQ_TIMEOUT
 from periflow.utils.url import get_training_uri
-from periflow.utils.validate import validate_cli_version
+from periflow.utils.validate import validate_package_version
 from periflow.utils.version import get_installed_version
 
 app = typer.Typer(
     help="Supercharge Generative AI Serving 🚀",
     no_args_is_help=True,
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
-    callback=validate_cli_version,
+    callback=validate_package_version,
+    pretty_exceptions_enable=False,
 )
 
 app.add_typer(credential.app, name="credential", help="Manage credentials")
 app.add_typer(checkpoint.app, name="checkpoint", help="Manage checkpoints")
 app.add_typer(vm.app, name="vm", help="Manage VMs")
 app.add_typer(deployment.app, name="deployment", help="Manage deployments")
 app.add_typer(project.app, name="project", help="Manage projects")
```

### Comparing `periflow_client-0.1.3/periflow/cli/project.py` & `periflow_client-0.1.4/periflow/cli/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cli/vm.py` & `periflow_client-0.1.4/periflow/cli/vm.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/base.py` & `periflow_client-0.1.4/periflow/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/checkpoint.py` & `periflow_client-0.1.4/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/credential.py` & `periflow_client-0.1.4/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/deployment.py` & `periflow_client-0.1.4/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/file.py` & `periflow_client-0.1.4/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/group.py` & `periflow_client-0.1.4/periflow/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/project.py` & `periflow_client-0.1.4/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/client/user.py` & `periflow_client-0.1.4/periflow/client/user.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/cloud/storage.py` & `periflow_client-0.1.4/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/configurator/base.py` & `periflow_client-0.1.4/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/configurator/credential.py` & `periflow_client-0.1.4/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/configurator/deployment.py` & `periflow_client-0.1.4/periflow/configurator/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,10 +86,10 @@
                 "orca_config": {
                     "type": "object",
                     "properties": {
                         "max_batch_size": {"type": "integer"},
                         "max_token_count": {"type": "integer"},
                     },
                 },
-                "required": ["orca_config"],
             },
+            "required": ["orca_config"],
         }
```

### Comparing `periflow_client-0.1.3/periflow/context.py` & `periflow_client-0.1.4/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/base.py` & `periflow_client-0.1.4/periflow/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/interface.py` & `periflow_client-0.1.4/periflow/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/maps.py` & `periflow_client-0.1.4/periflow/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/blenderbot.py` & `periflow_client-0.1.4/periflow/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/bloom.py` & `periflow_client-0.1.4/periflow/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/codegen.py` & `periflow_client-0.1.4/periflow/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/falcon.py` & `periflow_client-0.1.4/periflow/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/gpt2.py` & `periflow_client-0.1.4/periflow/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/gpt_neox.py` & `periflow_client-0.1.4/periflow/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/gptj.py` & `periflow_client-0.1.4/periflow/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/llama.py` & `periflow_client-0.1.4/periflow/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/mpt.py` & `periflow_client-0.1.4/periflow/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/opt.py` & `periflow_client-0.1.4/periflow/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/models/t5.py` & `periflow_client-0.1.4/periflow/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/converter/utils.py` & `periflow_client-0.1.4/periflow/converter/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,23 +117,30 @@
     cache_dir: Optional[str] = None,
     save_dir: str,
 ) -> None:
     """Try to save `tokenizer.json` of a pretrained model."""
     if not os.path.isdir(save_dir):
         raise NotFoundError(f"Directory '{save_dir}' is not found.")
 
-    tokenizer = AutoTokenizer.from_pretrained(
-        model_name_or_path,
-        cache_dir=cache_dir,
-        trust_remote_code=True,
-    )
+    try:
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_name_or_path,
+            cache_dir=cache_dir,
+            trust_remote_code=True,
+        )
+    except OSError as exc:
+        raise TokenizerNotFoundError(str(exc)) from exc
+
     if not tokenizer.is_fast:
-        raise TokenizerNotFoundError
+        raise TokenizerNotFoundError(
+            "This model does not support PeriFlow-compatible tokenizer"
+        )
 
     saved_file_paths = tokenizer.save_pretrained(save_directory=save_dir)
+
     tokenizer_json_path = None
     for path in saved_file_paths:
         if "tokenizer.json" == os.path.basename(path):
             tokenizer_json_path = path
         else:
             # Remove unnecessary files.
             try:
```

### Comparing `periflow_client-0.1.3/periflow/enums.py` & `periflow_client-0.1.4/periflow/enums.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/errors.py` & `periflow_client-0.1.4/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/formatter.py` & `periflow_client-0.1.4/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/logging.py` & `periflow_client-0.1.4/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/schema/api/v1/completion.py` & `periflow_client-0.1.4/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.1.4/periflow/schema/resource/v1/attributes.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.1.4/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/schema/resource/v1/credential.py` & `periflow_client-0.1.4/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.1.4/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/api/base.py` & `periflow_client-0.1.4/periflow/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/api/completion.py` & `periflow_client-0.1.4/periflow/sdk/api/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/init.py` & `periflow_client-0.1.4/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/resource/base.py` & `periflow_client-0.1.4/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.1.4/periflow/sdk/resource/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
 
 """PeriFlow Checkpoint SDK."""
 
-# pylint: disable=line-too-long, arguments-differ, too-many-arguments, too-many-locals, redefined-builtin
+# pylint: disable=line-too-long, arguments-differ, too-many-arguments, too-many-statements, too-many-locals, redefined-builtin
 
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import List, Optional, cast
 from uuid import UUID
@@ -20,14 +20,15 @@
 from periflow.enums import CheckpointCategory, CheckpointDataType, CredType, StorageType
 from periflow.errors import (
     CheckpointConversionError,
     InvalidConfigError,
     NotFoundError,
     NotSupportedCheckpointError,
     PeriFlowInternalError,
+    TokenizerNotFoundError,
 )
 from periflow.logging import logger
 from periflow.schema.resource.v1.checkpoint import V1Checkpoint
 from periflow.sdk.resource.base import ResourceAPI
 from periflow.utils.fs import (
     FileSizeType,
     attach_storage_path_prefix,
@@ -36,14 +37,15 @@
     get_file_info,
     strip_storage_path_prefix,
 )
 from periflow.utils.maps import cred_type_map, cred_type_map_inv
 from periflow.utils.validate import (
     validate_checkpoint_attributes,
     validate_cloud_storage_type,
+    validate_enums,
     validate_storage_region,
 )
 
 
 class Checkpoint(ResourceAPI[V1Checkpoint, UUID]):
     """Checkpoint resource API."""
 
@@ -89,16 +91,16 @@
                 api_key="YOUR_PERILFOW_API_KEY",
                 project_name="my-project",
             )
 
             # Create a checkpoint by linking an existing S3 bucket.
             checkpoint = pf.Checkpoint.create(
                 name="my-checkpoint",
-                credential_id=UUID("8ab9b5cf-8737-4d1b-873a-f4ef36a57cf1"),
-                cloud_stroage=StorageType.S3,
+                credential_id="YOUR_CREDENTIAL_ID",
+                cloud_stroage="s3",
                 region="us-east-1",
                 storage_name="my-bucket",
                 storage_path="path/to/ckpt",
                 attr_file_path="path/to/attr.yaml",
             )
             ```
 
@@ -225,14 +227,15 @@
             vocab_size: 32128
             eos_token: 1
             decoder_start_token: 0
             ```
             :::
 
         """
+        cloud_storage = validate_enums(cloud_storage, StorageType)
         validate_cloud_storage_type(cloud_storage)
         validate_storage_region(vendor=cloud_storage, region=region)
 
         attr = {}
         if attr_file_path is not None:
             try:
                 with open(attr_file_path, "r", encoding="utf-8") as attr_f:
@@ -354,17 +357,15 @@
 
             # Set up PeriFlow context.
             pf.init(
                 api_key="YOUR_PERILFOW_API_KEY",
                 project_name="my-project",
             )
 
-            checkpoint = pf.Checkpoint.get(
-                id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63)
-            )
+            checkpoint = pf.Checkpoint.get(id="YOUR_CHECKPOINT_ID")
             ```
 
         """
         client = CheckpointClient()
         raw_ckpt = client.get_checkpoint(id)
         ckpt = V1Checkpoint.model_validate(raw_ckpt)
         if ckpt.forms:
@@ -387,17 +388,15 @@
 
             # Set up PeriFlow context.
             pf.init(
                 api_key="YOUR_PERILFOW_API_KEY",
                 project_name="my-project",
             )
 
-            checkpoint = pf.Checkpoint.delete(
-                id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63)
-            )
+            checkpoint = pf.Checkpoint.delete(id="YOUR_CHECKPOINT_ID")
             ```
 
         """
         client = CheckpointClient()
         client.delete_checkpoint(id)
 
     @staticmethod
@@ -716,15 +715,15 @@
             # Set up PeriFlow context.
             pf.init(
                 api_key="YOUR_PERILFOW_API_KEY",
                 project_name="my-project",
             )
 
             pf.Checkpoint.download(
-                id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63),
+                id="YOUR_CHECKPOINT_ID",
                 save_dir="local/save/dir",
             )
             ```
 
         """
         if save_dir is not None and not os.path.isdir(save_dir):
             raise NotFoundError(f"Directory {save_dir} is not found.")
@@ -765,15 +764,15 @@
             # Set up PeriFlow context.
             pf.init(
                 api_key="YOUR_PERILFOW_API_KEY",
                 project_name="my-project",
             )
 
             pf.Checkpoint.download(
-                id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63),
+                id="YOUR_CHECKPOINT_ID",
                 save_dir="local/save/dir",
             )
             ```
 
             :::info
             When a checkpoint is deleted, it becomes "soft-deleted", meaning it is
             recoverable within the 24-hour retention period. After the retention period,
@@ -814,15 +813,14 @@
             attr_output_path (Optional[str], optional): Path to create the attribute YAML file for the converted checkpoint. Defaults to None.
             cache_dir (Optional[str], optional): Path for downloading checkpoint. Defaults to None.
             dry_run (bool, optional): Check only if checkpoint is convertable. Defaults to False.
 
         Raises:
             NotFoundError: Raised when `model_name_or_path` is not found. Also raised when `tokenizer_output_dir` is not found.
             CheckpointConversionError: Raised when given model architecture from checkpoint is not supported to convert.
-            TokenizerNotFoundError: Raised when `tokenizer_output_dir` is not `None` and the model does not have the PeriFlow-compatible tokenizer implementation, which is equivalent to Hugging Face 'fast' tokenizer. Refer to [this link](https://huggingface.co/docs/transformers/main_classes/tokenizer#tokenizer) to get more info.
 
         """
         try:
             import torch  # type: ignore[import] # pylint: disable=import-outside-toplevel
         except ImportError as exc:
             raise CheckpointConversionError(
                 "To convert the checkpoint, you must install 'torch'."
@@ -838,14 +836,16 @@
                 save_tokenizer,
             )
         except ImportError as exc:
             raise CheckpointConversionError(
                 "To convert the checkpoint, your must install the package with 'pip install periflow-client[mllib]'"
             ) from exc
 
+        data_type = validate_enums(data_type, CheckpointDataType)
+
         try:
             config = transformers.AutoConfig.from_pretrained(
                 model_name_or_path, cache_dir=cache_dir, trust_remote_code=True
             )
         except OSError as exc:  # from transformers.AutoConfig.from_pretrained()
             config_dir = Path(model_name_or_path)
             model_output_dir = Path(model_output_path).parent
@@ -919,12 +919,15 @@
 
         if attr_output_path is not None:
             attr = converter.get_attributes()
             with open(attr_output_path, "w", encoding="utf-8") as file:
                 yaml.dump(attr, file, sort_keys=False)
 
         if tokenizer_output_dir is not None:
-            save_tokenizer(
-                model_name_or_path=model_name_or_path,
-                cache_dir=cache_dir,
-                save_dir=tokenizer_output_dir,
-            )
+            try:
+                save_tokenizer(
+                    model_name_or_path=model_name_or_path,
+                    cache_dir=cache_dir,
+                    save_dir=tokenizer_output_dir,
+                )
+            except TokenizerNotFoundError as exc:
+                logger.warn(str(exc))
```

### Comparing `periflow_client-0.1.3/periflow/sdk/resource/credential.py` & `periflow_client-0.1.4/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/sdk/resource/deployment.py` & `periflow_client-0.1.4/periflow/sdk/resource/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 )
 from periflow.logging import logger
 from periflow.schema.resource.v1.deployment import V1Deployment
 from periflow.sdk.resource.base import ResourceAPI
 from periflow.utils.format import extract_datetime_part, extract_deployment_id_part
 from periflow.utils.fs import download_file, upload_file
 from periflow.utils.maps import cloud_vm_map, vm_num_gpu_map
+from periflow.utils.validate import validate_enums
 
 
 class Deployment(ResourceAPI[V1Deployment, str]):
     """Deployment resource API."""
 
     @staticmethod
     def create(
@@ -107,17 +108,17 @@
 
             # Create a deployment at GCP asia-northest3 region wtih one A100 GPU.
             config = {
                 "max_batch_size": 256,
                 "max_token_count": 8146,
             }
             deployment = pf.Deployment.create(
-                checkpoint_id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63),
+                checkpoint_id="YOUR_CHECKPOINT_ID",
                 name="my-deployment",
-                cloud=CloudType.GCP,
+                cloud="gcp",
                 region="asia-northeast3",
                 vm_type="a2-highgpu-1g",
                 config=config,
             )
             ```
 
             The format of `config` should be:
@@ -150,14 +151,20 @@
             When `min_replicas` and `max_replicas` are the same, deployment auto-scaling turns off.
             :::
 
         Returns:
             V1Deployment: The created deployment object.
 
         """
+        # pylint: disable=too-many-statements
+        cloud = validate_enums(cloud, CloudType)
+        vm_type = validate_enums(vm_type, VMType)
+        deployment_type = validate_enums(deployment_type, DeploymentType)
+        security_level = validate_enums(security_level, DeploymentSecurityLevel)
+
         org_id = get_current_group_id()
         if org_id is None:
             raise AuthenticationError(
                 "Not authenticated. Please authenticate with 'pf init()' or 'pf login'."
             )
         project_id = get_current_project_id()
         if project_id is None:
@@ -250,15 +257,15 @@
             "region": region,
             "total_gpus": num_gpus,
             "infrequest_perm_check": security_level
             == DeploymentSecurityLevel.PROTECTED,
             "infrequest_log": logging,
             **config,
         }
-        if description:
+        if description is not None:
             request_data["description"] = description
 
         client = DeploymentClient()
         deployment_raw = client.create_deployment(request_data)
         deployment = V1Deployment.model_validate(deployment_raw)
         return deployment
```

### Comparing `periflow_client-0.1.3/periflow/utils/format.py` & `periflow_client-0.1.4/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/fs.py` & `periflow_client-0.1.4/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/maps.py` & `periflow_client-0.1.4/periflow/utils/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/prompt.py` & `periflow_client-0.1.4/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/request.py` & `periflow_client-0.1.4/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/testing.py` & `periflow_client-0.1.4/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/url.py` & `periflow_client-0.1.4/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/periflow/utils/validate.py` & `periflow_client-0.1.4/periflow/utils/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
 
 """PeriFlow CLI Validation Utilities."""
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Dict, Optional
+from enum import Enum
+from typing import Any, Dict, Optional, Type
 
 import typer
 from pydantic import ValidationError
 
 from periflow.cloud.storage import cloud_region_map, storage_region_map
 from periflow.enums import CloudType, StorageType
 from periflow.errors import (
@@ -59,29 +60,29 @@
             "The datetime format should be {YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}"
         ) from exc
     return datetime_str
 
 
 def validate_cloud_storage_type(val: StorageType) -> None:
     """Validate the cloud storage type."""
-    if val is StorageType.FAI:
+    if val == StorageType.FAI:
         raise NotSupportedError(
             "Checkpoint creation with FAI storage is not supported now."
         )
 
 
-def validate_cli_version() -> None:
+def validate_package_version() -> None:
     """Validate the installed CLI version."""
     installed_version = get_installed_version()
     if not is_latest_version(installed_version):
         latest_version = get_latest_version()
         secho_error_and_exit(
-            f"CLI version({installed_version}) is deprecated. "
+            f"Package version({installed_version}) is deprecated. "
             f"Please install the latest version({latest_version}) with "
-            f"'pip install {PERIFLOW_PACKAGE_NAME}=={latest_version} -U --no-cache-dir'."
+            f"'pip install {PERIFLOW_PACKAGE_NAME}=={latest_version} -U'."
         )
 
 
 def validate_checkpoint_attributes(attr: Dict[str, Any]) -> None:
     """Validate checkpoint attributes schema."""
     try:
         V1AttributesValidationModel.model_validate({"attr": attr})
@@ -97,7 +98,18 @@
                 msgs.append(f"{error['msg']}. Correct the field '{error['loc'][-1]}'")
 
         if len(msgs) == 1:
             msg = msgs[0]
         else:
             msg = "\n>>> " + "\n>>> ".join(msgs)
         raise InvalidAttributesError(msg) from exc
+
+
+def validate_enums(val: Any, enum_cls: Type[Enum]) -> Any:
+    """Validate if the value is the proper enum."""
+    try:
+        return enum_cls(val)
+    except ValueError as exc:
+        supported_values = set([e.value for e in enum_cls])
+        raise InvalidConfigError(
+            f"Invalid value. Please provide one of {supported_values}"
+        ) from exc
```

### Comparing `periflow_client-0.1.3/periflow/utils/version.py` & `periflow_client-0.1.4/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.3/pyproject.toml` & `periflow_client-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.1.3"
+version = "0.1.4"
 description = "Client of PeriFlow, the fastest generative AI serving available."
 license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
 packages = [
     { include = "periflow" },
 ]
 readme = "README.md"
```

### Comparing `periflow_client-0.1.3/PKG-INFO` & `periflow_client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: Client of PeriFlow, the fastest generative AI serving available.
 Home-page: https://docs.periflow.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8,<4.0
@@ -43,15 +43,15 @@
 Description-Content-Type: text/markdown
 
 <!---
 Copyright (c) 2022-present, FriendliAI Inc. All rights reserved.
 -->
 
 <p align="center">
-  <img src="https://drive.google.com/uc?id=1daafphR0ABKylj_0b1wtZ6n0ZRSVq5-s" width="80%" alt="system">
+  <img src="https://docs.periflow.ai/img/logo.svg" width="80%" alt="system">
 </p>
 
 <h2><p align="center">Supercharge Generative AI Serving 🚀</p></h2>
 
 <p align="center">
   <a href="https://github.com/friendliai/periflow-client/actions/workflows/ci.yaml">
     <img alt="CI Status" src="https://github.com/friendliai/periflow-client/actions/workflows/ci.yaml/badge.svg">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: periflow-client Version: 0.1.3 Summary: Client of
+Metadata-Version: 2.1 Name: periflow-client Version: 0.1.4 Summary: Client of
 PeriFlow, the fastest generative AI serving available. Home-page: https://
 docs.periflow.ai/ License: Apache-2.0 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams Author-email: eng@friendli.ai Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

