# Comparing `tmp/tons-0.0.49.tar.gz` & `tmp/tons-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tons-0.0.49.tar", last modified: Fri Jan 20 04:18:21 2023, max compression
+gzip compressed data, was "tons-1.0.0.tar", last modified: Thu Aug  3 15:34:46 2023, max compression
```

## Comparing `tons-0.0.49.tar` & `tons-1.0.0.tar`

### file list

```diff
@@ -1,128 +1,186 @@
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.837578 tons-0.0.49/
--rw-r--r--   0 akkireev   (501) staff       (20)    11357 2022-09-06 17:40:28.000000 tons-0.0.49/LICENSE
--rw-r--r--   0 akkireev   (501) staff       (20)    18600 2023-01-20 04:18:21.837812 tons-0.0.49/PKG-INFO
--rw-r--r--   0 akkireev   (501) staff       (20)    17400 2023-01-19 11:08:58.000000 tons-0.0.49/README.md
--rw-r--r--   0 akkireev   (501) staff       (20)       89 2022-06-10 12:18:43.000000 tons-0.0.49/pyproject.toml
--rw-r--r--   0 akkireev   (501) staff       (20)     1678 2023-01-20 04:18:21.839162 tons-0.0.49/setup.cfg
--rw-r--r--   0 akkireev   (501) staff       (20)      762 2022-10-07 09:19:02.000000 tons-0.0.49/setup.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.747650 tons-0.0.49/tons/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-0.0.49/tons/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.754100 tons-0.0.49/tons/config/
--rw-r--r--   0 akkireev   (501) staff       (20)     3745 2022-10-04 08:51:39.000000 tons-0.0.49/tons/config/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2479 2022-12-07 15:43:20.000000 tons-0.0.49/tons/config/_config.py
--rw-r--r--   0 akkireev   (501) staff       (20)      138 2022-09-29 13:45:25.000000 tons-0.0.49/tons/config/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.755952 tons-0.0.49/tons/config/_provider/
--rw-r--r--   0 akkireev   (501) staff       (20)      203 2022-09-29 13:45:25.000000 tons-0.0.49/tons/config/_provider/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      827 2022-10-04 08:59:24.000000 tons-0.0.49/tons/config/_provider/_dapp.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1187 2023-01-19 11:08:58.000000 tons-0.0.49/tons/config/_tons.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1337 2023-01-19 11:08:58.000000 tons-0.0.49/tons/settings.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.757706 tons-0.0.49/tons/tonclient/
--rw-r--r--   0 akkireev   (501) staff       (20)      200 2022-07-05 07:34:38.000000 tons-0.0.49/tons/tonclient/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.759636 tons-0.0.49/tons/tonclient/_client/
--rw-r--r--   0 akkireev   (501) staff       (20)      115 2022-07-05 07:34:38.000000 tons-0.0.49/tons/tonclient/_client/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2650 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonclient/_client/_base.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.762822 tons-0.0.49/tons/tonclient/_client/_dapp/
--rw-r--r--   0 akkireev   (501) staff       (20)       69 2022-07-05 07:34:38.000000 tons-0.0.49/tons/tonclient/_client/_dapp/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     6883 2022-11-09 09:44:40.000000 tons-0.0.49/tons/tonclient/_client/_dapp/_dapp.py
--rw-r--r--   0 akkireev   (501) staff       (20)      685 2022-11-09 09:38:08.000000 tons-0.0.49/tons/tonclient/_client/_dapp/_queries.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4556 2022-12-22 09:05:14.000000 tons-0.0.49/tons/tonclient/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.769235 tons-0.0.49/tons/tonclient/utils/
--rw-r--r--   0 akkireev   (501) staff       (20)      775 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      559 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.772907 tons-0.0.49/tons/tonclient/utils/_keystores/
--rw-r--r--   0 akkireev   (501) staff       (20)     4008 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/_keystores/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4010 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/_keystores/_backup.py
--rw-r--r--   0 akkireev   (501) staff       (20)     6559 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/_keystores/_keystore.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1040 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonclient/utils/_keystores/_record.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4187 2023-01-20 04:15:04.000000 tons-0.0.49/tons/tonclient/utils/_whitelist.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.773928 tons-0.0.49/tons/tonsdk/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-0.0.49/tons/tonsdk/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      351 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.776994 tons-0.0.49/tons/tonsdk/boc/
--rw-r--r--   0 akkireev   (501) staff       (20)      145 2022-07-04 20:10:06.000000 tons-0.0.49/tons/tonsdk/boc/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4916 2022-08-23 16:30:57.000000 tons-0.0.49/tons/tonsdk/boc/_bit_string.py
--rw-r--r--   0 akkireev   (501) staff       (20)    11140 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/boc/_cell.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.777910 tons-0.0.49/tons/tonsdk/contract/
--rw-r--r--   0 akkireev   (501) staff       (20)     4511 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/contract/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.784102 tons-0.0.49/tons/tonsdk/contract/wallet/
--rw-r--r--   0 akkireev   (501) staff       (20)     3227 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonsdk/contract/wallet/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4167 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1373 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v2.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2112 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v3.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4801 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v4.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.789447 tons-0.0.49/tons/tonsdk/crypto/
--rw-r--r--   0 akkireev   (501) staff       (20)      322 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonsdk/crypto/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      609 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonsdk/crypto/_keystore.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1850 2022-11-12 17:39:42.000000 tons-0.0.49/tons/tonsdk/crypto/_mnemonic.py
--rw-r--r--   0 akkireev   (501) staff       (20)       26 2022-06-10 12:18:43.000000 tons-0.0.49/tons/tonsdk/crypto/_settings.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1023 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/crypto/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.792734 tons-0.0.49/tons/tonsdk/crypto/bip39/
--rw-r--r--   0 akkireev   (501) staff       (20)       68 2022-06-10 12:18:43.000000 tons-0.0.49/tons/tonsdk/crypto/bip39/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)    21114 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/crypto/bip39/_english.py
--rw-r--r--   0 akkireev   (501) staff       (20)      138 2022-06-21 08:49:28.000000 tons-0.0.49/tons/tonsdk/crypto/exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.796588 tons-0.0.49/tons/tonsdk/provider/
--rw-r--r--   0 akkireev   (501) staff       (20)      225 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/provider/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4030 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/provider/_address.py
--rw-r--r--   0 akkireev   (501) staff       (20)      145 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/provider/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.797464 tons-0.0.49/tons/tonsdk/provider/_utils/
--rw-r--r--   0 akkireev   (501) staff       (20)     1245 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/provider/_utils/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.799906 tons-0.0.49/tons/tonsdk/provider/dapp/
--rw-r--r--   0 akkireev   (501) staff       (20)      143 2022-07-05 07:34:38.000000 tons-0.0.49/tons/tonsdk/provider/dapp/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3431 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/provider/dapp/_client.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.805227 tons-0.0.49/tons/tonsdk/utils/
--rw-r--r--   0 akkireev   (501) staff       (20)      667 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/utils/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4846 2023-01-19 11:08:58.000000 tons-0.0.49/tons/tonsdk/utils/_address.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2988 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/utils/_currency.py
--rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-06-21 08:49:28.000000 tons-0.0.49/tons/tonsdk/utils/_exceptions.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4242 2022-09-29 13:45:25.000000 tons-0.0.49/tons/tonsdk/utils/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.806901 tons-0.0.49/tons/ui/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-0.0.49/tons/ui/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4014 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.810140 tons-0.0.49/tons/ui/direct_cli/
--rw-r--r--   0 akkireev   (501) staff       (20)      315 2023-01-12 08:19:48.000000 tons-0.0.49/tons/ui/direct_cli/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.817612 tons-0.0.49/tons/ui/direct_cli/_commands/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-0.0.49/tons/ui/direct_cli/_commands/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1388 2023-01-20 04:15:04.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_base_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3658 2022-10-11 13:36:16.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_config_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2423 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_contract_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     6222 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_dev_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3719 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_keystore_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)    13891 2023-01-19 12:18:07.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_wallet_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3689 2022-11-09 10:13:33.000000 tons-0.0.49/tons/ui/direct_cli/_commands/_whitelist_cmd.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3597 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/direct_cli/_utils.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.818662 tons-0.0.49/tons/ui/gui/
--rw-r--r--   0 akkireev   (501) staff       (20)      196 2023-01-19 10:32:03.000000 tons-0.0.49/tons/ui/gui/__init__.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.822039 tons-0.0.49/tons/ui/interactive_cli/
--rw-r--r--   0 akkireev   (501) staff       (20)      891 2022-12-21 15:18:32.000000 tons-0.0.49/tons/ui/interactive_cli/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)       91 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_exceptions.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.828553 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/
--rw-r--r--   0 akkireev   (501) staff       (20)      455 2023-01-20 04:15:04.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)      851 2023-01-20 04:15:04.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_confirm_render.py
--rw-r--r--   0 akkireev   (501) staff       (20)      479 2022-09-22 19:59:46.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_prompt.py
--rw-r--r--   0 akkireev   (501) staff       (20)     4199 2023-01-20 04:15:04.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_render.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2746 2022-09-29 13:45:25.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_text_render.py
--rw-r--r--   0 akkireev   (501) staff       (20)      322 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_theme.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.834178 tons-0.0.49/tons/ui/interactive_cli/_sets/
--rw-r--r--   0 akkireev   (501) staff       (20)       75 2022-09-29 13:45:25.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3566 2023-01-20 04:17:40.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_base.py
--rw-r--r--   0 akkireev   (501) staff       (20)     1864 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_config.py
--rw-r--r--   0 akkireev   (501) staff       (20)      712 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_entrypoint.py
--rw-r--r--   0 akkireev   (501) staff       (20)    23121 2023-01-20 04:15:04.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_keystore.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3432 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_keystores.py
--rw-r--r--   0 akkireev   (501) staff       (20)     3724 2023-01-19 11:08:58.000000 tons-0.0.49/tons/ui/interactive_cli/_sets/_whitelist.py
--rw-r--r--   0 akkireev   (501) staff       (20)      433 2023-01-12 08:18:06.000000 tons-0.0.49/tons/ui/interactive_cli/_utils.py
--rw-r--r--   0 akkireev   (501) staff       (20)      293 2022-10-07 09:31:40.000000 tons-0.0.49/tons/ui/interactive_cli/_validators.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.836810 tons-0.0.49/tons/utils/
--rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-0.0.49/tons/utils/__init__.py
--rw-r--r--   0 akkireev   (501) staff       (20)       40 2022-06-10 12:18:43.000000 tons-0.0.49/tons/utils/exceptions.py
--rw-r--r--   0 akkireev   (501) staff       (20)     2676 2023-01-19 11:08:58.000000 tons-0.0.49/tons/utils/storage.py
--rw-r--r--   0 akkireev   (501) staff       (20)      496 2022-10-26 18:49:18.000000 tons-0.0.49/tons/utils/versioning.py
--rw-r--r--   0 akkireev   (501) staff       (20)       63 2023-01-20 04:15:20.000000 tons-0.0.49/tons/version.py
-drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-01-20 04:18:21.751046 tons-0.0.49/tons.egg-info/
--rw-r--r--   0 akkireev   (501) staff       (20)    18600 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/PKG-INFO
--rw-r--r--   0 akkireev   (501) staff       (20)     3373 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/SOURCES.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        1 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/dependency_links.txt
--rw-r--r--   0 akkireev   (501) staff       (20)      125 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/entry_points.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-12-21 09:05:02.000000 tons-0.0.49/tons.egg-info/not-zip-safe
--rw-r--r--   0 akkireev   (501) staff       (20)      237 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/requires.txt
--rw-r--r--   0 akkireev   (501) staff       (20)        5 2023-01-20 04:18:21.000000 tons-0.0.49/tons.egg-info/top_level.txt
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.247821 tons-1.0.0/
+-rw-r--r--   0 akkireev   (501) staff       (20)    35148 2023-08-03 15:01:41.000000 tons-1.0.0/LICENSE
+-rw-r--r--   0 akkireev   (501) staff       (20)     4538 2023-08-03 15:34:46.247974 tons-1.0.0/PKG-INFO
+-rw-r--r--   0 akkireev   (501) staff       (20)     3325 2023-08-03 15:01:41.000000 tons-1.0.0/README.md
+-rw-r--r--   0 akkireev   (501) staff       (20)       89 2022-06-10 12:18:43.000000 tons-1.0.0/pyproject.toml
+-rw-r--r--   0 akkireev   (501) staff       (20)     1967 2023-08-03 15:34:46.248367 tons-1.0.0/setup.cfg
+-rw-r--r--   0 akkireev   (501) staff       (20)      762 2023-01-20 04:34:49.000000 tons-1.0.0/setup.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.224390 tons-1.0.0/tests/
+-rw-r--r--   0 akkireev   (501) staff       (20)      731 2023-08-03 15:01:41.000000 tons-1.0.0/tests/test_settings.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.225166 tons-1.0.0/tons/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-1.0.0/tons/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.227498 tons-1.0.0/tons/config/
+-rw-r--r--   0 akkireev   (501) staff       (20)     4975 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3032 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_config.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      387 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_dns.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      138 2023-01-20 04:34:49.000000 tons-1.0.0/tons/config/_exceptions.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      220 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_jetton.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.227800 tons-1.0.0/tons/config/_provider/
+-rw-r--r--   0 akkireev   (501) staff       (20)      281 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_provider/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1687 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_provider/_dapp.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1286 2023-08-03 15:01:41.000000 tons-1.0.0/tons/config/_tons.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1235 2023-08-03 15:01:41.000000 tons-1.0.0/tons/settings.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.228109 tons-1.0.0/tons/tonclient/
+-rw-r--r--   0 akkireev   (501) staff       (20)      377 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.228432 tons-1.0.0/tons/tonclient/_client/
+-rw-r--r--   0 akkireev   (501) staff       (20)      287 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_client/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    12781 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_client/_base.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.229167 tons-1.0.0/tons/tonclient/_client/_dapp/
+-rw-r--r--   0 akkireev   (501) staff       (20)       69 2022-07-05 07:34:38.000000 tons-1.0.0/tons/tonclient/_client/_dapp/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4773 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_client/_dapp/_daemon.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    16383 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_client/_dapp/_dapp.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    12972 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_client/_dapp/_queries.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4697 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.229647 tons-1.0.0/tons/tonclient/utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)     1143 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1386 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.230364 tons-1.0.0/tons/tonclient/utils/_keystores/
+-rw-r--r--   0 akkireev   (501) staff       (20)    11725 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4668 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_backup.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2231 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_crypto.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.231022 tons-1.0.0/tons/tonclient/utils/_keystores/_keystore/
+-rw-r--r--   0 akkireev   (501) staff       (20)      234 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_keystore/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     9377 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_keystore/_base.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6492 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_keystore/_password.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     7063 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_keystore/_yubikey.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      985 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_keystores/_record.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.231668 tons-1.0.0/tons/tonclient/utils/_tonconnect/
+-rw-r--r--   0 akkireev   (501) staff       (20)     5172 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_tonconnect/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    11643 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_tonconnect/_handlers.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      825 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_tonconnect/_models.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      803 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_tonconnect/_utils.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     7534 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonclient/utils/_whitelist.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.231951 tons-1.0.0/tons/tonsdk/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-1.0.0/tons/tonsdk/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      351 2023-01-20 04:34:49.000000 tons-1.0.0/tons/tonsdk/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.232965 tons-1.0.0/tons/tonsdk/boc/
+-rw-r--r--   0 akkireev   (501) staff       (20)      335 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     7068 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/_bit_string.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2088 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/_builder.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    11944 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/_cell.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1309 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/_dict_builder.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4405 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/_slice.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.233404 tons-1.0.0/tons/tonsdk/boc/dict/
+-rw-r--r--   0 akkireev   (501) staff       (20)      157 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/dict/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      354 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/dict/find_common_prefix.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4198 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/boc/dict/serialize_dict.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.233545 tons-1.0.0/tons/tonsdk/contract/
+-rw-r--r--   0 akkireev   (501) staff       (20)     4913 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.233690 tons-1.0.0/tons/tonsdk/contract/token/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.234117 tons-1.0.0/tons/tonsdk/contract/token/ft/
+-rw-r--r--   0 akkireev   (501) staff       (20)      135 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/ft/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3269 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/ft/jetton_minter.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3167 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/ft/jetton_wallet.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.234870 tons-1.0.0/tons/tonsdk/contract/token/nft/
+-rw-r--r--   0 akkireev   (501) staff       (20)      168 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/nft/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5429 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/nft/nft_collection.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2647 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/nft/nft_item.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1983 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/nft/nft_sale.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      889 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/token/nft/nft_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.235627 tons-1.0.0/tons/tonsdk/contract/wallet/
+-rw-r--r--   0 akkireev   (501) staff       (20)     2953 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/wallet/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6534 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1401 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v2.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2101 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v3.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4790 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v4.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.236662 tons-1.0.0/tons/tonsdk/crypto/
+-rw-r--r--   0 akkireev   (501) staff       (20)      169 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/crypto/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1982 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/crypto/_mnemonic.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5427 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/crypto/_payload_encryption.py
+-rw-r--r--   0 akkireev   (501) staff       (20)       26 2022-06-10 12:18:43.000000 tons-1.0.0/tons/tonsdk/crypto/_settings.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1023 2023-01-20 04:34:49.000000 tons-1.0.0/tons/tonsdk/crypto/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.237048 tons-1.0.0/tons/tonsdk/crypto/bip39/
+-rw-r--r--   0 akkireev   (501) staff       (20)       68 2022-06-10 12:18:43.000000 tons-1.0.0/tons/tonsdk/crypto/bip39/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    21114 2023-01-20 04:34:49.000000 tons-1.0.0/tons/tonsdk/crypto/bip39/_english.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      138 2022-06-21 08:49:28.000000 tons-1.0.0/tons/tonsdk/crypto/exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.237791 tons-1.0.0/tons/tonsdk/provider/
+-rw-r--r--   0 akkireev   (501) staff       (20)      229 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/provider/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4111 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/provider/_address.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      145 2023-07-12 11:23:54.000000 tons-1.0.0/tons/tonsdk/provider/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.238012 tons-1.0.0/tons/tonsdk/provider/_utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)     1245 2023-01-20 04:34:49.000000 tons-1.0.0/tons/tonsdk/provider/_utils/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.238283 tons-1.0.0/tons/tonsdk/provider/dapp/
+-rw-r--r--   0 akkireev   (501) staff       (20)      143 2022-07-05 07:34:38.000000 tons-1.0.0/tons/tonsdk/provider/dapp/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5295 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/provider/dapp/_client.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.238960 tons-1.0.0/tons/tonsdk/utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)      730 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5370 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/_address.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4817 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/_currency.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      134 2022-06-21 08:49:28.000000 tons-1.0.0/tons/tonsdk/utils/_exceptions.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4019 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.239366 tons-1.0.0/tons/tonsdk/utils/tonconnect/
+-rw-r--r--   0 akkireev   (501) staff       (20)       61 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2300 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/_bridge.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1438 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/_session.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.239934 tons-1.0.0/tons/tonsdk/utils/tonconnect/requests_responses/
+-rw-r--r--   0 akkireev   (501) staff       (20)     1581 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/requests_responses/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1687 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/requests_responses/_app.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      480 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/requests_responses/_common.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3951 2023-08-03 15:01:41.000000 tons-1.0.0/tons/tonsdk/utils/tonconnect/requests_responses/_wallet.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.240323 tons-1.0.0/tons/ui/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-1.0.0/tons/ui/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     9984 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/_background.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    10293 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.240607 tons-1.0.0/tons/ui/direct_cli/
+-rw-r--r--   0 akkireev   (501) staff       (20)      496 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.242004 tons-1.0.0/tons/ui/direct_cli/_commands/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-1.0.0/tons/ui/direct_cli/_commands/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1943 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_base_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3740 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_config_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1218 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_contract_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     8281 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_dev_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5051 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_dns_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5368 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_keystore_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     3699 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_tonconnect.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    18372 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_wallet_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     8613 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_commands/_whitelist_cmd.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6934 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/direct_cli/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.242142 tons-1.0.0/tons/ui/gui/
+-rw-r--r--   0 akkireev   (501) staff       (20)      196 2023-05-11 08:26:10.000000 tons-1.0.0/tons/ui/gui/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.242458 tons-1.0.0/tons/ui/gui/_sets/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/gui/_sets/__init__.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.242973 tons-1.0.0/tons/ui/interactive_cli/
+-rw-r--r--   0 akkireev   (501) staff       (20)     1352 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      140 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_exceptions.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.244293 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/
+-rw-r--r--   0 akkireev   (501) staff       (20)      625 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1675 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_confirm_render.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4843 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_list_with_filter_render.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1605 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_menu_with_hotkeys.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      399 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_prompt.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     8009 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_render.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2765 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_text_render.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      334 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_theme.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     2367 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_utils.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.246644 tons-1.0.0/tons/ui/interactive_cli/_sets/
+-rw-r--r--   0 akkireev   (501) staff       (20)       75 2023-01-20 04:34:49.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4213 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_base.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4300 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_config.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     4725 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_config_advanced.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6119 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_dns.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1208 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_entrypoint.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    10597 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_jetton.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     7383 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_keystore.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     5678 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_keystores.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     9286 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_mixin.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6821 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_tonconnect.py
+-rw-r--r--   0 akkireev   (501) staff       (20)    22962 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_wallet.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6865 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_sets/_whitelist.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1175 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_utils.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      889 2023-08-03 15:01:41.000000 tons-1.0.0/tons/ui/interactive_cli/_validators.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.247498 tons-1.0.0/tons/utils/
+-rw-r--r--   0 akkireev   (501) staff       (20)        0 2022-06-10 12:18:43.000000 tons-1.0.0/tons/utils/__init__.py
+-rw-r--r--   0 akkireev   (501) staff       (20)       40 2022-06-10 12:18:43.000000 tons-1.0.0/tons/utils/exceptions.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     1562 2023-08-03 15:01:41.000000 tons-1.0.0/tons/utils/spinner.py
+-rw-r--r--   0 akkireev   (501) staff       (20)     6779 2023-08-03 15:01:41.000000 tons-1.0.0/tons/utils/storage.py
+-rw-r--r--   0 akkireev   (501) staff       (20)      496 2023-08-03 14:49:29.000000 tons-1.0.0/tons/utils/versioning.py
+-rw-r--r--   0 akkireev   (501) staff       (20)       22 2023-08-03 15:20:08.000000 tons-1.0.0/tons/version.py
+drwxr-xr-x   0 akkireev   (501) staff       (20)        0 2023-08-03 15:34:46.226256 tons-1.0.0/tons.egg-info/
+-rw-r--r--   0 akkireev   (501) staff       (20)     4538 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/PKG-INFO
+-rw-r--r--   0 akkireev   (501) staff       (20)     5438 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/SOURCES.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        1 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/dependency_links.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)      125 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/entry_points.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        1 2022-12-21 09:05:02.000000 tons-1.0.0/tons.egg-info/not-zip-safe
+-rw-r--r--   0 akkireev   (501) staff       (20)      415 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/requires.txt
+-rw-r--r--   0 akkireev   (501) staff       (20)        5 2023-08-03 15:34:46.000000 tons-1.0.0/tons.egg-info/top_level.txt
```

### Comparing `tons-0.0.49/setup.cfg` & `tons-1.0.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = tons
 version = attr: tons.version.__version__
 description = TON Stash - secure TON wallet
 long_description = file: README.md
 long_description_content_type = text/markdown
-keywords = TON, wallet, TON wallet, blockchain, security, safety
-license = Apache 2.0
+keywords = TON, wallet, TON wallet, blockchain, security, safety, cryptowallet, crypto
+license_files = 
+	LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	Environment :: Console
 	Environment :: Other Environment
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: Financial and Insurance Industry
 	Intended Audience :: End Users/Desktop
-	License :: OSI Approved :: Apache Software License
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -30,36 +31,48 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	aiohttp>=3.0.0
-	bitarray>=2.0.0
-	cffi>=1.13.0
-	click>=8.0.0
-	halo>=0.0.31
-	inquirer>=2.8.0
-	prettytable>=3.3.0
-	pycparser>=2.2
-	pydantic>=1.8.0
-	pynacl>=1.5.0
-	pyyaml>=6.0
-	requests>=2.19.0
-	tvm-valuetypes>=0.0.8
-	typing_extensions>=4.0.0
-	gql>=3.0.0
+	appdirs==1.4.4
+	aiohttp==3.8.4
+	bitarray==2.7.6
+	certifi>=2017.4.17
+	cffi==1.15.1
+	click==8.1.4
+	colorama==0.4.6
+	cryptography==38.0.3
+	fe25519==1.4.2
+	ge25519==1.4.3
+	graphql_query==1.1.1
+	inquirer==3.1.3
+	prettytable==3.8.0
+	pycparser==2.21
+	pydantic==1.10.11
+	pynacl==1.5.0
+	python-dateutil==2.8.2
+	pyyaml==6.0
+	requests==2.31.0
+	tvm-valuetypes==0.0.10
+	typing_extensions==4.7.1
+	gql==3.4.1
+	yubikey-manager==5.1.1
+	websockets==11.0.3
 
 [options.entry_points]
 console_scripts = 
 	tons = tons.ui.direct_cli:main
 	tons-interactive = tons.ui.interactive_cli:main
 	tons-gui = tons.ui.gui:main
 
+[options.package_data]
+* = _forms/img/*.png, _forms/ui/*.ui
+
 [options.packages.find]
 exclude = 
 	examples*
 	devtools*
 	docs*
 	tests*
 	.tons*
```

### Comparing `tons-0.0.49/setup.py` & `tons-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tons-0.0.49/tons/config/_config.py` & `tons-1.0.0/tons/config/_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 from enum import Enum
 from typing import Any, List, Tuple, Union, Generator
 
 from pydantic import BaseModel
 
+from ._dns import DnsConfig
+from ._jetton import JettonConfig
 from ._provider import ProviderConfig, DAppConfig
 from ._tons import TonsConfig
 
 
 class ConfigLocation(str, Enum):
-    local_location = 'local'
+    custom_location = 'custom'
     global_location = 'global'
 
 
 class Config(BaseModel):
     tons: TonsConfig = TonsConfig()
     provider: ProviderConfig = ProviderConfig()
+    dns: DnsConfig = DnsConfig()
+    jetton: JettonConfig = JettonConfig()
 
     class Config:
         use_enum_values = True
         validate_assignment = True
 
     @classmethod
     def field_names(cls) -> List[str]:
         fields = []
         fields += [f"tons.{field}" for field in list(
             TonsConfig.__fields__)]
         fields += [f"provider.dapp.{field}" for field in list(
             DAppConfig.__fields__)]
+        fields += [f"dns.{field}" for field in list(
+            DnsConfig.__fields__)]
+        fields += [f"jetton.{field}" for field in list(
+            JettonConfig.__fields__)]
 
         return fields
 
     def key_value(self, exclude_unset=False) -> Generator[Tuple[str, Any], None, None]:
         for key, val in self.tons.dict(exclude_unset=exclude_unset).items():
             yield f"tons.{key}", val
 
         for key, val in self.provider.dapp.dict(exclude_unset=exclude_unset).items():
             yield f"provider.dapp.{key}", val
 
+        for key, val in self.dns.dict(exclude_unset=exclude_unset).items():
+            yield f"dns.{key}", val
+
+        for key, val in self.jetton.dict(exclude_unset=exclude_unset).items():
+            yield f"jetton.{key}", val
+
     def get_nondefault_value(self, field: str) -> Union[None, Any]:
         attrs_tree = field.split(".")
         val = self.dict(exclude_unset=True)
 
         for attr in attrs_tree:
             if attr in val:
                 val = val[attr]
```

### Comparing `tons-0.0.49/tons/config/_provider/_dapp.py` & `tons-1.0.0/tons/tonclient/utils/_tonconnect/_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from enum import Enum
-from typing import Optional
+from typing import Optional, Union
 
 from pydantic import BaseModel
 
-from tons import settings
+from tons.config import TonNetworkEnum
+from tons.tonsdk.utils.tonconnect.requests_responses import TransactionPayload, TonconnectNetworkEnum
 
 
-class TonNetworkEnum(str, Enum):
-    mainnet = 'mainnet'
-    testnet = 'testnet'
+class SupportedTonconnectVersionEnum(str, Enum):
+    v2 = "2"
 
 
-class DAppConfig(BaseModel):
-    api_key: Optional[str] = None
-    network: TonNetworkEnum = TonNetworkEnum.mainnet
+class UniversalLink(BaseModel):
+    v: SupportedTonconnectVersionEnum
+    id: str
+    r: str
+    ref: Optional[str]
 
     class Config:
         use_enum_values = True
-        validate_assignment = True
 
-    @property
-    def graphql_url(self):
-        if self.network == TonNetworkEnum.mainnet:
-            return settings.DAPP_MAINNET_GRAPHQL_URL
-        else:
-            return settings.DAPP_TESTNET_GRAPHQL_URL
-
-    @property
-    def broadcast_url(self):
-        if self.network == TonNetworkEnum.mainnet:
-            return settings.DAPP_MAINNET_BROADCAST_URL
-        else:
-            return settings.DAPP_TESTNET_BROADCAST_URL
+
+def get_network(param: Union[TransactionPayload]) -> TonNetworkEnum:
+    if param.network == TonconnectNetworkEnum.mainnet:
+        return TonNetworkEnum.mainnet
+    elif param.network == TonconnectNetworkEnum.testnet:
+        return TonNetworkEnum.testnet
+    else:
+        raise ValueError(f"Network {param.network} is not supported.")
```

### Comparing `tons-0.0.49/tons/config/_tons.py` & `tons-1.0.0/tons/config/_tons.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel, validator
 
 from tons import settings
 from tons.tonsdk.contract.wallet import WalletVersionEnum
+from tons.utils import storage
 
 
 class TonProviderEnum(str, Enum):
     dapp = "dapp"
 
 
 class TonsConfig(BaseModel):
     workdir: Optional[str]
     whitelist_path: Optional[str]
     keystore_name: Optional[str] = None
     provider: TonProviderEnum = TonProviderEnum.dapp
-    default_wallet_version: WalletVersionEnum = WalletVersionEnum.v3r2
+    default_wallet_version: WalletVersionEnum = WalletVersionEnum.v4r2
     warn_if_outdated: bool = True
+    sort_whitelist: bool = True
+    sort_keystore: bool = True
 
     class Config:
         use_enum_values = True
         validate_assignment = True
 
     @validator("workdir", always=True)
     def __validate_workdir(cls, v, values):
         if v:
             return v
 
-        return settings.CURRENT_WORKDIR
+        return storage.get_default_workdir()
 
     @validator("keystore_name", always=True)
     def __validate_keystore_name(cls, v, values):
         if v:
             if not v.endswith(".keystore"):
                 v += ".keystore"
```

### Comparing `tons-0.0.49/tons/tonclient/_exceptions.py` & `tons-1.0.0/tons/tonclient/_exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         if self.detail:
             error_msg += f" {self.detail}"
         self.error_msg = error_msg
 
     def __str__(self):
         return self.error_msg
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.error_msg}')"
+
 
 class TonContractUninitializedError(TonError):
     default_detail = "Contract is not initialized."
     default_code = -13
 
 
 class TonStackUnderflowError(TonError):
@@ -85,20 +88,22 @@
 
 class TonFatalError(TonError):
     default_detail = "Thrown by TVM in situations deemed impossible."
     default_code = 12
 
 
 class TonOutOfGasError(TonError):
-    default_detail = "Thrown by TVM when the remaining gas (gr) becomes negative. This exception usually cannot be caught and leads to an immediate termination of TVM."
+    default_detail = "Thrown by TVM when the remaining gas (gr) becomes negative. " \
+                     "This exception usually cannot be caught and leads to an immediate termination of TVM."
     default_code = 13
 
 
 class TonNetworkError(TonError):
-    default_detail = "Network problems. It may be caused by TON itself (e.g. testnet update). Make sure you have an internet connection and TON config is correct."
+    default_detail = "Network problems. It may be caused by TON itself (e.g. testnet update). " \
+                     "Make sure you have an internet connection and TON config is correct."
     default_code = 500
 
 
 class TonTooManyQueriesError(TonError):
     default_detail = "Requests limit reached. Obtain key or increase limit " \
                      "via a telegram bot: @tontech_dapp_bot (or @tontech_dapp_testnet_bot for testnet)"
     default_code = 429
```

### Comparing `tons-0.0.49/tons/tonclient/utils/_keystores/_backup.py` & `tons-1.0.0/tons/tonclient/utils/_keystores/_backup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional, Union, List, Dict
 
 from pydantic import BaseModel
 
 from tons import settings
-from tons.tonsdk.contract.wallet import WalletVersionEnum
+from tons.tonsdk.contract.wallet import WalletVersionEnum, WalletContract
 from tons.tonsdk.utils import Address
-from ._keystore import KeyStore
+from ._keystore import BaseKeyStore
 from ._record import Record
+from .._whitelist import WhitelistContact
 
 
 class TonCliRecordBackup(BaseModel):
     name: str
     comment: Optional[str] = ""
     config: str
     kind: str
@@ -22,32 +23,43 @@
         validate_assignment = True
         arbitrary_types_allowed = True
 
     def to_backup_record(self) -> Optional["RecordBackup"]:
         if not self.__supported_wallet():
             return None
 
+        version = self.__map_kind_to_version()
+        workchain = int(self.__map_config_to_workchain())
+
+        default_subwallet_id = WalletContract.default_subwallet_id(workchain, version)
+        subwallet_id = self.__map_config_to_subwallet_id()
+        subwallet_id = default_subwallet_id if subwallet_id is None else int(subwallet_id)
+
         return RecordBackup(name=self.name, address=self.address,
-                            version=self.__map_kind_to_version(),
-                            workchain=int(self.__map_config_to_workchain()),
-                            subwallet_id=int(self.__map_config_to_subwallet_id()),
+                            version=version,
+                            workchain=workchain,
+                            subwallet_id=subwallet_id,
                             mnemonics=" ".join(self.mnemonics), comment=self.comment)
 
     def __supported_wallet(self):
-        return self.kind in self.kind_version_map.keys()
+        return self.kind in self.kind_version_map
 
     def __map_kind_to_version(self):
-        return self.kind_version_map[self.kind]
+        return self.kind_version_map.get(self.kind, None)
 
     def __map_config_to_workchain(self):
         # "wc=0,walletId=698983191,pk=qweqweqwe"
         return self.config.split(",")[0].split("=")[1]
 
     def __map_config_to_subwallet_id(self):
-        return self.config.split(",")[1].split("=")[1]
+        temp = self.config.split("walletId=")
+        if len(temp) == 2:
+            return temp[1].split(",")[0]
+
+        return None
 
     @property
     def kind_version_map(self) -> Dict:
         return {
             "org.ton.wallets.v2": WalletVersionEnum.v2r1,
             "org.ton.wallets.v2.r2": WalletVersionEnum.v2r2,
             "org.ton.wallets.v3": WalletVersionEnum.v3r1,
@@ -81,46 +93,52 @@
             comment=record.comment,
         )
 
 
 class KeystoreBackup(BaseModel):
     version: int = settings.CURRENT_KEYSTORE_VERSION
     records: List[RecordBackup]
+    contacts: List[WhitelistContact] = []
 
     @classmethod
-    def backup_json(cls, keystore: KeyStore, filepath: str, password: str) -> Dict:
+    def backup_json(cls, keystore: BaseKeyStore) -> Dict:
         records: List[RecordBackup] = []
-        for record in keystore.records:
-            mnemonics = keystore.get_secret(record, password)
+        for record in keystore.get_records(False):
+            mnemonics = keystore.get_secret(record)
             records.append(RecordBackup.from_record(record, mnemonics))
 
-        return cls(records=records).dict()
+        return cls(records=records, contacts=keystore.contacts, version=keystore.version).dict()
 
     @classmethod
-    def restore_from_tons(cls, json_data: Dict) -> 'KeystoreBackup':
+    def restore_from_tons(cls, json_data: Union[Dict, List]) -> 'KeystoreBackup':
         records: List[RecordBackup] = []
-        # todo: check version and update records if required
+        contacts: List[WhitelistContact] = []
 
-        version = 1 if "version" not in json_data else json_data["version"]
+        version = 1 if isinstance(json_data, list) else json_data["version"]
 
         if version == 1:
-            version += 1
             raw_records = json_data
         else:
             raw_records = json_data['records']
 
+        raw_contacts = []
+        if version >= 4:
+            raw_contacts = json_data['contacts']
+
         for raw_record in raw_records:
             records.append(RecordBackup.parse_obj(raw_record))
 
-        assert version == settings.CURRENT_KEYSTORE_VERSION
-        return cls(records=records)
+        for raw_contact in raw_contacts:
+            contacts.append(WhitelistContact.parse_obj(raw_contact))
+
+        return cls(records=records, contacts=contacts, version=version)
 
     @classmethod
     def restore_from_ton_cli(cls, json_data: Dict) -> 'KeystoreBackup':
         records: List[RecordBackup] = []
         for raw_record in json_data:
             backup_record = TonCliRecordBackup.parse_obj(
                 raw_record).to_backup_record()
             if backup_record:
                 records.append(backup_record)
 
-        return cls(records=records)
+        return cls(records=records, contacts=[])
```

### Comparing `tons-0.0.49/tons/tonclient/utils/_keystores/_record.py` & `tons-1.0.0/tons/tonclient/utils/_keystores/_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,30 @@
 
 class Record(BaseModel):
     name: str
     address: Union[str, Address]
     version: WalletVersionEnum
     workchain: int
     subwallet_id: Optional[int]
-    public_key: str
     secret_key: str
     comment: Optional[str] = ""
 
     class Config:
         use_enum_values = True
         validate_assignment = True
         arbitrary_types_allowed = True
 
     @validator('address')
     def validate_address(cls, v, values, **kwargs):
-        if v:
-            if isinstance(v, Address):
-                return v.to_string(False, False, False)
-
-            try:
-                addr = Address(v)
-                return addr.to_string(False, False, False)
+        if isinstance(v, Address):
+            return v.to_string(False, False, False)
 
-            except InvalidAddressError as e:
-                raise ValueError(e)
+        try:
+            addr = Address(v)
+            return addr.to_string(False, False, False)
+
+        except InvalidAddressError as e:
+            raise ValueError(e)
 
     @property
-    def address_to_show(self):
+    def address_to_show(self) -> str:
         return Address(self.address).to_string(True, True, True)
```

### Comparing `tons-0.0.49/tons/tonsdk/boc/_cell.py` & `tons-1.0.0/tons/tonsdk/boc/_cell.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,304 +1,302 @@
 import copy
 import math
 from hashlib import sha256
+from typing import Dict, Tuple, List, Any, Union
 
 from ._bit_string import BitString
-from ..utils import concat_bytes, tree_walk, crc32c, read_n_bytes_uint_from_array, compare_bytes
+from ..utils import tree_walk, crc32c, read_n_bytes_uint_from_array
 
 
 class Cell:
-    REACH_BOC_MAGIC_PREFIX = bytes.fromhex('B5EE9C72')
+    REACH_BOC_MAGIC_PREFIX = bytes.fromhex('b5ee9c72')
     LEAN_BOC_MAGIC_PREFIX = bytes.fromhex('68ff65f3')
     LEAN_BOC_MAGIC_PREFIX_CRC = bytes.fromhex('acc3a728')
 
     def __init__(self):
         self.bits = BitString(1023)
-        self.refs = []
+        self._refs = []
         self.is_exotic = False
 
-    def __str__(self) -> str:
-        return "BITS: {}\nREFS: {}\nIS_EXOTIC: {}".format(self.bits, self.refs, self.is_exotic)
+    def __repr__(self):
+        return "<Cell refs_num: %d, %s>" % (len(self._refs), repr(self.bits))
 
-    def bytes_hash(self):
-        return bytes.fromhex(sha256(self.bytes_repr()).hexdigest())
+    def __bool__(self):
+        return bool(self.bits.cursor) or bool(self._refs)
 
-    def bytes_repr(self):
-        repr_array = []
-
-        repr_array.append(self.get_data_with_descriptors())
-
-        for r in self.refs:
+    @property
+    def refs(self) -> Tuple:
+        return tuple(self._refs)
+
+    def store_ref(self, ref: 'Cell'):
+        if len(self._refs) >= 4:
+            raise OverflowError("Number of refs cannot be greater than 4")
+        if isinstance(ref, Cell):
+            stack = [ref]
+            visited = set()
+            while len(stack) > 0:
+                cur_cell = stack.pop()
+                if cur_cell in visited:
+                    continue
+                visited.add(cur_cell)
+                if cur_cell == self:
+                    raise RecursionError("refs should not form a cyclic graph")
+                for _ref in cur_cell.refs:
+                    stack.append(_ref)
+        else:
+            # TODO: refactor this, only allow Cell type variable, forbid storing cell indices in refs
+            # raise TypeError("ref should be a Cell")
+            ...
+        self._refs.append(ref)
+
+    def bytes_hash(self) -> bytes:
+        return sha256(self.bytes_repr()).digest()
+
+    def bytes_repr(self) -> bytes:
+        repr_array = [self.get_data_with_descriptors()]
+        for r in self._refs:
             repr_array.append(r.get_max_depth_as_array())
-
-        for r in self.refs:
+        for r in self._refs:
             repr_array.append(r.bytes_hash())
 
-        x = bytes()
-        for r in repr_array:
-            x = concat_bytes(x, r)
-
-        return x
+        return b''.join(repr_array)
 
-    def write_cell(self, another_cell):
+    def write_cell(self, another_cell: 'Cell'):
         self.bits.write_bit_string(another_cell.bits)
-        self.refs += another_cell.refs
+        self._refs += another_cell.refs
 
-    def get_data_with_descriptors(self):
+    def get_data_with_descriptors(self) -> bytearray:
         d1 = self.get_refs_descriptor()
         d2 = self.get_bits_descriptor()
-        tuBits = self.bits.get_top_upped_array()
+        top_upped_bits = self.bits.get_top_upped_array()
 
-        return concat_bytes(concat_bytes(d1, d2), tuBits)
+        return d1 + d2 + top_upped_bits
 
-    def get_bits_descriptor(self):
+    def get_bits_descriptor(self) -> bytearray:
         d2 = bytearray([0])
-        d2[0] = math.ceil(self.bits.cursor / 8) + \
-                math.floor(self.bits.cursor / 8)
+        d2[0] = math.ceil(self.bits.cursor / 8) + math.floor(self.bits.cursor / 8)
         return d2
 
-    def get_refs_descriptor(self):
+    def get_refs_descriptor(self) -> bytearray:
         d1 = bytearray([0])
-        d1[0] = len(self.refs) + self.is_exotic * 8 + self.get_max_level() * 32
+        d1[0] = len(self._refs) + self.is_exotic * 8 + self.get_max_level() * 32
         return d1
 
-    def get_max_level(self):
-        # FIXME: looks strange! nothing happens here. Compare with get_max_depth.
+    def get_max_level(self) -> int:
+        if self.is_exotic:
+            raise NotImplementedError("Calculating max level for exotic cells is not implemented")
         max_level = 0
-        for r in self.refs:
+        for r in self._refs:
             r_max_level = r.get_max_level()
             if r_max_level > max_level:
                 max_level = r_max_level
         return max_level
 
-    def get_max_depth_as_array(self):
+    def get_max_depth_as_array(self) -> bytearray:
         max_depth = self.get_max_depth()
-        d = bytearray([0, 0])
-        d[1] = max_depth % 256
-        d[0] = math.floor(max_depth / 256)
-        return d
+        return bytearray([max_depth // 256, max_depth % 256])
 
-    def get_max_depth(self):
+    def get_max_depth(self) -> int:
         max_depth = 0
-        if len(self.refs) > 0:
-            for r in self.refs:
+        if len(self._refs) > 0:
+            for r in self._refs:
                 r_max_depth = r.get_max_depth()
                 if r_max_depth > max_depth:
                     max_depth = r_max_depth
             max_depth += 1
         return max_depth
 
     def tree_walk(self):
         return tree_walk(self, [], {})
 
-    def is_explicitly_stored_hashes(self):
-        return 0
+    def serialize_for_boc(self, cells_index: Dict) -> bytes:
+        repr_arr = [self.get_data_with_descriptors()]
 
-    def serialize_for_boc(self, cells_index, ref_size):
-        repr_arr = []
-
-        repr_arr.append(self.get_data_with_descriptors())
-        if self.is_explicitly_stored_hashes():
-            raise Exception("Cell hashes explicit storing is not implemented")
-
-        for ref in self.refs:
+        for ref in self._refs:
             ref_hash = ref.bytes_hash()
             ref_index_int = cells_index[ref_hash]
             ref_index_hex = format(ref_index_int, 'x')
             if len(ref_index_hex) % 2:
                 ref_index_hex = '0' + ref_index_hex
             reference = bytes.fromhex(ref_index_hex)
             repr_arr.append(reference)
 
-        x = b''
-        for data in repr_arr:
-            x = concat_bytes(x, data)
+        return b''.join(repr_arr)
 
-        return x
+    def boc_serialization_size(self, cells_index: Dict) -> int:
+        return len(self.serialize_for_boc(cells_index))
 
-    def boc_serialization_size(self, cells_index, ref_size):
-        return len(self.serialize_for_boc(cells_index, ref_size))
-
-    def to_boc(self, has_idx=True, hash_crc32=True, has_cache_bits=False, flags=0):
+    def to_boc(self, has_idx=True, hash_crc32=True, has_cache_bits=False, flags=0) -> bytearray:
         root_cell = copy.deepcopy(self)
 
         all_cells = root_cell.tree_walk()
         topological_order = all_cells[0]
         cells_index = all_cells[1]
 
         cells_num = len(topological_order)
         # Minimal number of bits to represent reference (unused?)
         s = len("{0:b}".format(cells_num))
         s_bytes = max(math.ceil(s / 8), 1)
         full_size = 0
-        size_index = []
-        for cell_info in topological_order:
-            size_index.append(full_size)
-            full_size += cell_info[1].boc_serialization_size(
-                cells_index, s_bytes)
+        cell_sizes = {}
+        for (_hash, subcell) in topological_order:
+            cell_sizes[_hash] = subcell.boc_serialization_size(cells_index)
+            full_size += cell_sizes[_hash]
 
         offset_bits = len("{0:b}".format(full_size))
         offset_bytes = max(math.ceil(offset_bits / 8), 1)
 
-        serialization = BitString(
-            (1023 + 32 * 4 + 32 * 3) * len(topological_order))
+        serialization = BitString((1023 + 32 * 4 + 32 * 3) * len(topological_order))
         serialization.write_bytes(Cell.REACH_BOC_MAGIC_PREFIX)
-        settings = bytes(''.join(['1' if i else '0' for i in [
-            has_idx, hash_crc32, has_cache_bits]]), 'utf-8')
+        settings = [bool(v) for v in (has_idx, hash_crc32, has_cache_bits)]
         serialization.write_bit_array(settings)
         serialization.write_uint(flags, 2)
         serialization.write_uint(s_bytes, 3)
         serialization.write_uint8(offset_bytes)
         serialization.write_uint(cells_num, s_bytes * 8)
         serialization.write_uint(1, s_bytes * 8)  # One root for now
         serialization.write_uint(0, s_bytes * 8)  # Complete BOCs only
         serialization.write_uint(full_size, offset_bytes * 8)
-        serialization.write_uint(0, s_bytes * 8)  # Root shoulh have index 0
+        serialization.write_uint(0, s_bytes * 8)  # Root should have index 0
 
         if has_idx:
-            for [cell_data, index] in topological_order:  # ?
-                serialization.write_uint(size_index[index], offset_bytes * 8)
+            for (_hash, subcell) in topological_order:
+                serialization.write_uint(cell_sizes[_hash], offset_bytes * 8)
 
         for cell_info in topological_order:
-            ref_cell_ser = cell_info[1].serialize_for_boc(cells_index, s_bytes)
+            ref_cell_ser = cell_info[1].serialize_for_boc(cells_index)
             serialization.write_bytes(ref_cell_ser)
 
         ser_arr = serialization.get_top_upped_array()
         if hash_crc32:
             ser_arr += crc32c(ser_arr)
 
         return ser_arr
 
+    def begin_parse(self):
+        from ._slice import Slice
+        return Slice(self)
+
     @staticmethod
-    def one_from_boc(serialized_boc):
+    def one_from_boc(serialized_boc: Union[str, bytes, bytearray]) -> 'Cell':
         cells = deserialize_boc(serialized_boc)
-
         if len(cells) != 1:
-            raise Exception("Expected 1 root cell")
-
+            raise ValueError("Expected 1 root cell")
         return cells[0]
 
 
-def deserialize_cell_data(cell_data, reference_index_size):
+def deserialize_cell_data(cell_data, reference_index_size) -> Tuple[Cell, bytes]:
     if len(cell_data) < 2:
-        raise Exception("Not enough bytes to encode cell descriptors")
+        raise ValueError("Not enough bytes to encode cell descriptors")
 
     d1, d2 = cell_data[0], cell_data[1]
     cell_data = cell_data[2:]
-    level = math.floor(d1 / 32)
     is_exotic = d1 & 8
     ref_num = d1 % 8
     data_bytes_size = math.ceil(d2 / 2)
-    fullfilled_bytes = not (d2 % 2)
+    fulfilled_bytes = not (d2 % 2)
 
     cell = Cell()
     cell.is_exotic = is_exotic
 
     if len(cell_data) < data_bytes_size + reference_index_size * ref_num:
-        raise Exception("Not enough bytes to encode cell data")
+        raise OverflowError("Not enough bytes to encode cell data")
 
-    cell.bits.set_top_upped_array(
-        bytearray(cell_data[:data_bytes_size]), fullfilled_bytes)
+    cell.bits = BitString.from_top_upped_array(bytearray(cell_data[:data_bytes_size]), fulfilled_bytes)
     cell_data = cell_data[data_bytes_size:]
     for r in range(ref_num):
-        cell.refs.append(read_n_bytes_uint_from_array(
+        # TODO: refactor this, cell indices should not be stored in the refs attribute
+        cell.store_ref(read_n_bytes_uint_from_array(
             reference_index_size, cell_data))
         cell_data = cell_data[reference_index_size:]
 
-    return {
-        "cell": cell,
-        "residue": cell_data
-    }
+    return cell, cell_data
 
 
-def parse_boc_header(serialized_boc):
+def parse_boc_header(serialized_boc) -> Dict[str, Any]:
     if len(serialized_boc) < 4 + 1:
-        raise Exception("Not enough bytes for magic prefix")
+        raise OverflowError("Not enough bytes for magic prefix")
 
     input_data = serialized_boc
     prefix = serialized_boc[:4]
     serialized_boc = serialized_boc[4:]
-    if compare_bytes(prefix, Cell.REACH_BOC_MAGIC_PREFIX):
+    if prefix == Cell.REACH_BOC_MAGIC_PREFIX:
         flags_byte = serialized_boc[0]
         has_idx = flags_byte & 128
         hash_crc32 = flags_byte & 64
         has_cache_bits = flags_byte & 32
         flags = (flags_byte & 16) * 2 + (flags_byte & 8)
         size_bytes = flags_byte % 8
-
-    if compare_bytes(prefix, Cell.LEAN_BOC_MAGIC_PREFIX):
+    elif prefix == Cell.LEAN_BOC_MAGIC_PREFIX:
         has_idx = 1
         hash_crc32 = 0
         has_cache_bits = 0
         flags = 0
         size_bytes = serialized_boc[0]
-
-    if compare_bytes(prefix, Cell.LEAN_BOC_MAGIC_PREFIX_CRC):
+    elif prefix == Cell.LEAN_BOC_MAGIC_PREFIX_CRC:
         has_idx = 1
         hash_crc32 = 1
         has_cache_bits = 0
         flags = 0
         size_bytes = serialized_boc[0]
+    else:
+        raise ValueError('Failed to parse boc header: unknown prefix')
 
     serialized_boc = serialized_boc[1:]
 
     if len(serialized_boc) < 1 + 5 * size_bytes:
-        raise Exception("Not enough bytes for encoding cells counters")
+        raise ValueError("Not enough bytes for encoding cells counters")
 
     offset_bytes = serialized_boc[0]
     serialized_boc = serialized_boc[1:]
-    cells_num = read_n_bytes_uint_from_array(
-        size_bytes, serialized_boc)
+    cells_num = read_n_bytes_uint_from_array(size_bytes, serialized_boc)
     serialized_boc = serialized_boc[size_bytes:]
-    roots_num = read_n_bytes_uint_from_array(
-        size_bytes, serialized_boc)
+    roots_num = read_n_bytes_uint_from_array(size_bytes, serialized_boc)
     serialized_boc = serialized_boc[size_bytes:]
-    absent_num = read_n_bytes_uint_from_array(
-        size_bytes, serialized_boc)
+    absent_num = read_n_bytes_uint_from_array(size_bytes, serialized_boc)
     serialized_boc = serialized_boc[size_bytes:]
-    tot_cells_size = read_n_bytes_uint_from_array(
-        offset_bytes, serialized_boc)
+    tot_cells_size = read_n_bytes_uint_from_array(offset_bytes, serialized_boc)
     serialized_boc = serialized_boc[offset_bytes:]
 
     if len(serialized_boc) < roots_num * size_bytes:
-        raise Exception("Not enough bytes for encoding root cells hashes")
+        raise ValueError("Not enough bytes for encoding root cells hashes")
 
     root_list = []
     for c in range(roots_num):
         root_list.append(read_n_bytes_uint_from_array(
             size_bytes, serialized_boc))
         serialized_boc = serialized_boc[size_bytes:]
 
     index = False
     if has_idx:
         index = []
         if len(serialized_boc) < offset_bytes * cells_num:
-            raise Exception("Not enough bytes for index encoding")
+            raise ValueError("Not enough bytes for index encoding")
         for c in range(cells_num):
             index.append(read_n_bytes_uint_from_array(
                 offset_bytes, serialized_boc))
             serialized_boc = serialized_boc[offset_bytes:]
 
     if len(serialized_boc) < tot_cells_size:
-        raise Exception("Not enough bytes for cells data")
+        raise ValueError("Not enough bytes for cells data")
     cells_data = serialized_boc[:tot_cells_size]
     serialized_boc = serialized_boc[tot_cells_size:]
 
     if hash_crc32:
         if len(serialized_boc) < 4:
-            raise Exception("Not enough bytes for crc32c hashsum")
+            raise ValueError("Not enough bytes for crc32c hashsum")
 
         length = len(input_data)
-        if not compare_bytes(crc32c(input_data[:length - 4]), serialized_boc[:4]):
-            raise Exception("Crc32c hashsum mismatch")
+        if crc32c(input_data[:length - 4]) != serialized_boc[:4]:
+            raise ValueError("Crc32c hashsum mismatch")
 
         serialized_boc = serialized_boc[4:]
 
     if len(serialized_boc):
-        raise Exception("Too much bytes in BoC serialization")
+        raise ValueError("Too much bytes in BoC serialization")
 
     return {
         'has_idx': has_idx,
         'hash_crc32': hash_crc32,
         'has_cache_bits': has_cache_bits,
         'flags': flags,
         'size_bytes': size_bytes,
@@ -309,33 +307,29 @@
         'tot_cells_size': tot_cells_size,
         'root_list': root_list,
         'index': index,
         'cells_data': cells_data,
     }
 
 
-def deserialize_boc(serialized_boc):
+def deserialize_boc(serialized_boc: Union[str, bytes, bytearray]) -> List[Cell]:
     if type(serialized_boc) == str:
         serialized_boc = bytes.fromhex(serialized_boc)
 
     header = parse_boc_header(serialized_boc)
     cells_data = header['cells_data']
     cells_array = []
 
     for ci in range(header["cells_num"]):
-        dd = deserialize_cell_data(cells_data, header["size_bytes"])
-        cells_data = dd["residue"]
-        cells_array.append(dd["cell"])
+        cell, cells_data = deserialize_cell_data(cells_data, header["size_bytes"])
+        cells_array.append(cell)
 
     for ci in reversed(range(header["cells_num"])):
         c = cells_array[ci]
         for ri in range(len(c.refs)):
+            # TODO: refactor this, cell indices should not be stored in the refs attribute
             r = c.refs[ri]
-            if (r < ci):
-                raise Exception("Topological order is broken")
-            c.refs[ri] = cells_array[r]
-
-    root_cells = []
-    for ri in header["root_list"]:
-        root_cells.append(cells_array[ri])
+            if r < ci:
+                raise AttributeError("Topological order is broken")
+            c._refs[ri] = cells_array[r]
 
-    return root_cells
+    return [cells_array[ri] for ri in header["root_list"]]
```

### Comparing `tons-0.0.49/tons/tonsdk/contract/__init__.py` & `tons-1.0.0/tons/tonsdk/contract/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC
+from typing import Optional, Union
 
 from ..boc import Cell
 from ..utils import Address
 
 
 class Contract(ABC):
     def __init__(self, **kwargs):
@@ -49,32 +50,40 @@
         message.bits.write_uint(2, 2)
         message.bits.write_address(Address(src) if src else None)
         message.bits.write_address(Address(dest))
         message.bits.write_grams(import_fee)
         return message
 
     @classmethod
-    def create_internal_message_header(cls, dest, grams=0, ihr_disabled=True,
-                                       bounce=None, bounced=False, src=None,
-                                       currency_collection=None, ihr_fees=0,
-                                       fwd_fees=0, created_lt=0, created_at=0):
+    def create_internal_message_header(cls,
+                                       dest: Address,
+                                       grams: int = 0,
+                                       ihr_disabled: bool = True,
+                                       bounce: Optional[bool] = None,
+                                       bounced: bool = False,
+                                       src: Optional[Union[Address, str]] = None,
+                                       currency_collection: Optional[bool] = None,
+                                       ihr_fees: int = 0,
+                                       fwd_fees: int = 0,
+                                       created_lt: int = 0,
+                                       created_at: int = 0):
         message = Cell()
         message.bits.write_bit(0)
         message.bits.write_bit(ihr_disabled)
 
         if bounce is not None:
             message.bits.write_bit(bounce)
         else:
             message.bits.write_bit(Address(dest).is_bounceable)
         message.bits.write_bit(bounced)
         message.bits.write_address(Address(src) if src else None)
         message.bits.write_address(Address(dest))
         message.bits.write_grams(grams)
         if currency_collection:
-            raise Exception("Currency collections are not implemented yet")
+            raise NotImplementedError("Currency collections are not implemented yet")
 
         message.bits.write_bit(bool(currency_collection))
         message.bits.write_grams(ihr_fees)
         message.bits.write_grams(fwd_fees)
         message.bits.write_uint(created_lt, 64)
         message.bits.write_uint(created_at, 32)
         return message
@@ -86,40 +95,38 @@
         if state_init:
             common_msg_info.bits.write_bit(1)
             if common_msg_info.bits.get_free_bits() - 1 >= state_init.bits.get_used_bits():
                 common_msg_info.bits.write_bit(0)
                 common_msg_info.write_cell(state_init)
             else:
                 common_msg_info.bits.write_bit(1)
-                common_msg_info.refs.append(state_init)
+                common_msg_info.store_ref(state_init)
         else:
             common_msg_info.bits.write_bit(0)
 
         if body:
             if common_msg_info.bits.get_free_bits() >= body.bits.get_used_bits():
                 common_msg_info.bits.write_bit(0)
                 common_msg_info.write_cell(body)
             else:
                 common_msg_info.bits.write_bit(1)
-                common_msg_info.refs.append(body)
+                common_msg_info.store_ref(body)
         else:
             common_msg_info.bits.write_bit(0)
 
         return common_msg_info
 
     def __create_state_init(self, code, data, library=None, split_depth=None, ticktock=None):
         if library or split_depth or ticktock:
-            raise Exception(
-                "Library/SplitDepth/Ticktock in state init is not implemented")
+            raise NotImplementedError("Library/SplitDepth/Ticktock in state init is not implemented")
 
         state_init = Cell()
-        settings = bytes(''.join(['1' if i else '0' for i in [bool(split_depth), bool(
-            ticktock), bool(code), bool(data), bool(library)]]), 'utf-8')
+        settings = [bool(split_depth), bool(ticktock), bool(code), bool(data), bool(library)]
         state_init.bits.write_bit_array(settings)
 
         if code:
-            state_init.refs.append(code)
+            state_init.store_ref(code)
         if data:
-            state_init.refs.append(data)
+            state_init.store_ref(data)
         if library:
-            state_init.refs.append(library)
+            state_init.store_ref(library)
         return state_init
```

### Comparing `tons-0.0.49/tons/tonsdk/contract/wallet/__init__.py` & `tons-1.0.0/tons/tonsdk/contract/wallet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-from enum import Enum
-from typing import List, Optional, Tuple, Set
+from typing import List, Optional, Tuple
 
-from ._wallet_contract import SendModeEnum
-from ._wallet_contract import WalletContract
+from ._wallet_contract import SendModeEnum, WalletContract, WalletVersionEnum, InternalMessage
 from ._wallet_contract_v2 import WalletV2ContractR1, WalletV2ContractR2
 from ._wallet_contract_v3 import WalletV3ContractR1, WalletV3ContractR2
 from ._wallet_contract_v4 import WalletV4ContractR1, WalletV4ContractR2
 from ...crypto import mnemonic_new, mnemonic_to_wallet_key, mnemonic_is_valid
 from ...crypto.exceptions import InvalidMnemonicsError
 
 
-class WalletVersionEnum(str, Enum):
-    v2r1 = 'v2r1'
-    v2r2 = 'v2r2'
-    v3r1 = 'v3r1'
-    v3r2 = 'v3r2'
-    v4r1 = 'v4r1'
-    v4r2 = 'v4r2'
-
-    @classmethod
-    def with_subwallet_id(cls) -> Set[str]:
-        return {cls.v3r1.value, cls.v3r2.value, cls.v4r1.value, cls.v4r2.value}
-
-
 class Wallets:
     default_version = WalletVersionEnum.v3r2
     ALL = {
         WalletVersionEnum.v2r1: WalletV2ContractR1,
         WalletVersionEnum.v2r2: WalletV2ContractR2,
         WalletVersionEnum.v3r1: WalletV3ContractR1,
         WalletVersionEnum.v3r2: WalletV3ContractR2,
         WalletVersionEnum.v4r1: WalletV4ContractR1,
         WalletVersionEnum.v4r2: WalletV4ContractR2,
     }
 
     @classmethod
     def create(cls, version: WalletVersionEnum, workchain: int,
-               subwallet_id: Optional[int] = None, password: Optional[str] = None) -> Tuple[
-        List[str], bytes, bytes, WalletContract]:
+               subwallet_id: Optional[int] = None, password: Optional[str] = None) \
+            -> Tuple[List[str], bytes, bytes, WalletContract]:
         """
         :rtype: (List[str](mnemonics), bytes(public_key), bytes(private_key), WalletContract(wallet))
         """
         mnemonics = mnemonic_new(password=password)
         pub_k, priv_k = mnemonic_to_wallet_key(mnemonics)
         wallet = cls.ALL[version](
             public_key=pub_k, private_key=priv_k, wc=workchain, subwallet_id=subwallet_id)
 
         return mnemonics, pub_k, priv_k, wallet
 
     @classmethod
     def from_mnemonics(cls, mnemonics: List[str], version: WalletVersionEnum = default_version,
-                       workchain: int = 0, subwallet_id: Optional[int] = None) -> Tuple[
-        List[str], bytes, bytes, WalletContract]:
+                       workchain: int = 0, subwallet_id: Optional[int] = None) \
+            -> Tuple[List[str], bytes, bytes, WalletContract]:
         """
         :rtype: (List[str](mnemonics), bytes(public_key), bytes(private_key), WalletContract(wallet))
         """
         if not mnemonic_is_valid(mnemonics):
             raise InvalidMnemonicsError()
 
         pub_k, priv_k = mnemonic_to_wallet_key(mnemonics)
@@ -64,15 +49,15 @@
 
         return mnemonics, pub_k, priv_k, wallet
 
     @classmethod
     def to_addr_pk(cls, mnemonics: List[str], version: WalletVersionEnum = default_version,
                    workchain: int = 0, subwallet_id: Optional[int] = None) -> Tuple[bytes, bytes]:
         """
-        :rtype: (bytes(addr), bytes(pk)
+        :rtype: (bytes(addr), bytes(pk))
         """
         _mnemonics, _pub_k, priv_k, wallet = cls.from_mnemonics(
             mnemonics, version, workchain, subwallet_id)
 
         return wallet.address.to_buffer(), priv_k[:32]
 
 
@@ -80,11 +65,12 @@
     'WalletV2ContractR1',
     'WalletV2ContractR2',
     'WalletV3ContractR1',
     'WalletV3ContractR2',
     'WalletV4ContractR1',
     'WalletV4ContractR2',
     'WalletContract',
+    'InternalMessage',
     'SendModeEnum',
     'WalletVersionEnum',
     'Wallets',
 ]
```

### Comparing `tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v2.py` & `tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v2.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,17 @@
             message.bits.write_uint(timestamp + 60, 32)
 
         return message
 
 
 class WalletV2ContractR1(WalletV2ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C724101010100570000AAFF0020DD2082014C97BA9730ED44D0D70B1FE0A4F2608308D71820D31FD31F01F823BBF263ED44D0D31FD3FFD15131BAF2A103F901541042F910F2A2F800029320D74A96D307D402FB00E8D1A4C8CB1FCBFFC9ED54A1370BB6"
+        self.code = "B5EE9C724101010100570000AAFF0020DD2082014C97BA9730ED44D0D70B1FE0A4F2608308D71820D31FD31F01F823BBF263ED44D0D31FD3FFD15131BAF2A103F901541042F910F2A2F800029320D74A96D307D402FB00E8D1A4C8CB1FCBFFC9ED54A1370BB6"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
 
 
 class WalletV2ContractR2(WalletV2ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C724101010100630000C2FF0020DD2082014C97BA218201339CBAB19C71B0ED44D0D31FD70BFFE304E0A4F2608308D71820D31FD31F01F823BBF263ED44D0D31FD3FFD15131BAF2A103F901541042F910F2A2F800029320D74A96D307D402FB00E8D1A4C8CB1FCBFFC9ED54044CD7A1"
+        self.code = "B5EE9C724101010100630000C2FF0020DD2082014C97BA218201339CBAB19C71B0ED44D0D31FD70BFFE304E0A4F2608308D71820D31FD31F01F823BBF263ED44D0D31FD3FFD15131BAF2A103F901541042F910F2A2F800029320D74A96D307D402FB00E8D1A4C8CB1FCBFFC9ED54044CD7A1"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
```

### Comparing `tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v3.py` & `tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 
 from ._wallet_contract import WalletContract
 from ...boc import Cell
-from ...utils._utils import default_subwallet_id
 
 
 class WalletV3ContractBase(WalletContract):
     def create_data_cell(self):
         cell = Cell()
         cell.bits.write_uint(0, 32)
         cell.bits.write_uint(self.options["subwallet_id"], 32)
@@ -26,21 +25,21 @@
 
         message.bits.write_uint(seqno, 32)
         return message
 
 
 class WalletV3ContractR1(WalletV3ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C724101010100620000C0FF0020DD2082014C97BA9730ED44D0D70B1FE0A4F2608308D71820D31FD31FD31FF82313BBF263ED44D0D31FD31FD3FFD15132BAF2A15144BAF2A204F901541055F910F2A3F8009320D74A96D307D402FB00E8D101A4C8CB1FCB1FCBFFC9ED543FBE6EE0"
+        self.code = "B5EE9C724101010100620000C0FF0020DD2082014C97BA9730ED44D0D70B1FE0A4F2608308D71820D31FD31FD31FF82313BBF263ED44D0D31FD31FD3FFD15132BAF2A15144BAF2A204F901541055F910F2A3F8009320D74A96D307D402FB00E8D101A4C8CB1FCB1FCBFFC9ED543FBE6EE0"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
         if "subwallet_id" not in self.options or self.options["subwallet_id"] is None:
-            self.options["subwallet_id"] = default_subwallet_id(self.options["wc"])
+            self.options["subwallet_id"] = self.default_subwallet_id(self.options["wc"])
 
 
 class WalletV3ContractR2(WalletV3ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C724101010100710000DEFF0020DD2082014C97BA218201339CBAB19F71B0ED44D0D31FD31F31D70BFFE304E0A4F2608308D71820D31FD31FD31FF82313BBF263ED44D0D31FD31FD3FFD15132BAF2A15144BAF2A204F901541055F910F2A3F8009320D74A96D307D402FB00E8D101A4C8CB1FCB1FCBFFC9ED5410BD6DAD"
+        self.code = "B5EE9C724101010100710000DEFF0020DD2082014C97BA218201339CBAB19F71B0ED44D0D31FD31F31D70BFFE304E0A4F2608308D71820D31FD31FD31FF82313BBF263ED44D0D31FD31FD3FFD15132BAF2A15144BAF2A204F901541055F910F2A3F8009320D74A96D307D402FB00E8D101A4C8CB1FCB1FCBFFC9ED5410BD6DAD"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
         if "subwallet_id" not in self.options or self.options["subwallet_id"] is None:
-            self.options["subwallet_id"] = default_subwallet_id(self.options["wc"])
+            self.options["subwallet_id"] = self.default_subwallet_id(self.options["wc"])
```

### Comparing `tons-0.0.49/tons/tonsdk/contract/wallet/_wallet_contract_v4.py` & `tons-1.0.0/tons/tonsdk/contract/wallet/_wallet_contract_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 
 from ._wallet_contract import WalletContract
 from ...boc import Cell
-from ...utils._utils import default_subwallet_id
 
 
 class WalletV4ContractBase(WalletContract):
     def create_data_cell(self):
         cell = Cell()
         cell.bits.write_uint(0, 32)
         cell.bits.write_uint(self.options["subwallet_id"], 32)
@@ -30,21 +29,21 @@
         if not without_op:
             message.bits.write_uint(0, 8)
         return message
 
 
 class WalletV4ContractR1(WalletV4ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C72410215010002F5000114FF00F4A413F4BCF2C80B010201200203020148040504F8F28308D71820D31FD31FD31F02F823BBF263ED44D0D31FD31FD3FFF404D15143BAF2A15151BAF2A205F901541064F910F2A3F80024A4C8CB1F5240CB1F5230CBFF5210F400C9ED54F80F01D30721C0009F6C519320D74A96D307D402FB00E830E021C001E30021C002E30001C0039130E30D03A4C8CB1F12CB1FCBFF1112131403EED001D0D3030171B0915BE021D749C120915BE001D31F218210706C7567BD228210626C6E63BDB022821064737472BDB0925F03E002FA403020FA4401C8CA07CBFFC9D0ED44D0810140D721F404305C810108F40A6FA131B3925F05E004D33FC8258210706C7567BA9131E30D248210626C6E63BAE30004060708020120090A005001FA00F404308210706C7567831EB17080185005CB0527CF165003FA02F40012CB69CB1F5210CB3F0052F8276F228210626C6E63831EB17080185005CB0527CF1624FA0214CB6A13CB1F5230CB3F01FA02F4000092821064737472BA8E3504810108F45930ED44D0810140D720C801CF16F400C9ED54821064737472831EB17080185004CB0558CF1622FA0212CB6ACB1FCB3F9410345F04E2C98040FB000201200B0C0059BD242B6F6A2684080A06B90FA0218470D4080847A4937D29910CE6903E9FF9837812801B7810148987159F31840201580D0E0011B8C97ED44D0D70B1F8003DB29DFB513420405035C87D010C00B23281F2FFF274006040423D029BE84C600201200F100019ADCE76A26840206B90EB85FFC00019AF1DF6A26840106B90EB858FC0006ED207FA00D4D422F90005C8CA0715CBFFC9D077748018C8CB05CB0222CF165005FA0214CB6B12CCCCC971FB00C84014810108F451F2A702006C810108D718C8542025810108F451F2A782106E6F746570748018C8CB05CB025004CF16821005F5E100FA0213CB6A12CB1FC971FB00020072810108D718305202810108F459F2A7F82582106473747270748018C8CB05CB025005CF16821005F5E100FA0214CB6A13CB1F12CB3FC973FB00000AF400C9ED5446A9F34F"
+        self.code = "B5EE9C72410215010002F5000114FF00F4A413F4BCF2C80B010201200203020148040504F8F28308D71820D31FD31FD31F02F823BBF263ED44D0D31FD31FD3FFF404D15143BAF2A15151BAF2A205F901541064F910F2A3F80024A4C8CB1F5240CB1F5230CBFF5210F400C9ED54F80F01D30721C0009F6C519320D74A96D307D402FB00E830E021C001E30021C002E30001C0039130E30D03A4C8CB1F12CB1FCBFF1112131403EED001D0D3030171B0915BE021D749C120915BE001D31F218210706C7567BD228210626C6E63BDB022821064737472BDB0925F03E002FA403020FA4401C8CA07CBFFC9D0ED44D0810140D721F404305C810108F40A6FA131B3925F05E004D33FC8258210706C7567BA9131E30D248210626C6E63BAE30004060708020120090A005001FA00F404308210706C7567831EB17080185005CB0527CF165003FA02F40012CB69CB1F5210CB3F0052F8276F228210626C6E63831EB17080185005CB0527CF1624FA0214CB6A13CB1F5230CB3F01FA02F4000092821064737472BA8E3504810108F45930ED44D0810140D720C801CF16F400C9ED54821064737472831EB17080185004CB0558CF1622FA0212CB6ACB1FCB3F9410345F04E2C98040FB000201200B0C0059BD242B6F6A2684080A06B90FA0218470D4080847A4937D29910CE6903E9FF9837812801B7810148987159F31840201580D0E0011B8C97ED44D0D70B1F8003DB29DFB513420405035C87D010C00B23281F2FFF274006040423D029BE84C600201200F100019ADCE76A26840206B90EB85FFC00019AF1DF6A26840106B90EB858FC0006ED207FA00D4D422F90005C8CA0715CBFFC9D077748018C8CB05CB0222CF165005FA0214CB6B12CCCCC971FB00C84014810108F451F2A702006C810108D718C8542025810108F451F2A782106E6F746570748018C8CB05CB025004CF16821005F5E100FA0213CB6A12CB1FC971FB00020072810108D718305202810108F459F2A7F82582106473747270748018C8CB05CB025005CF16821005F5E100FA0214CB6A13CB1F12CB3FC973FB00000AF400C9ED5446A9F34F"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
         if "subwallet_id" not in self.options or self.options["subwallet_id"] is None:
-            self.options["subwallet_id"] = default_subwallet_id(self.options["wc"])
+            self.options["subwallet_id"] = self.default_subwallet_id(self.options["wc"])
 
 
 class WalletV4ContractR2(WalletV4ContractBase):
     def __init__(self, **kwargs) -> None:
-        self.code = "B5EE9C72410214010002D4000114FF00F4A413F4BCF2C80B010201200203020148040504F8F28308D71820D31FD31FD31F02F823BBF264ED44D0D31FD31FD3FFF404D15143BAF2A15151BAF2A205F901541064F910F2A3F80024A4C8CB1F5240CB1F5230CBFF5210F400C9ED54F80F01D30721C0009F6C519320D74A96D307D402FB00E830E021C001E30021C002E30001C0039130E30D03A4C8CB1F12CB1FCBFF1011121302E6D001D0D3032171B0925F04E022D749C120925F04E002D31F218210706C7567BD22821064737472BDB0925F05E003FA403020FA4401C8CA07CBFFC9D0ED44D0810140D721F404305C810108F40A6FA131B3925F07E005D33FC8258210706C7567BA923830E30D03821064737472BA925F06E30D06070201200809007801FA00F40430F8276F2230500AA121BEF2E0508210706C7567831EB17080185004CB0526CF1658FA0219F400CB6917CB1F5260CB3F20C98040FB0006008A5004810108F45930ED44D0810140D720C801CF16F400C9ED540172B08E23821064737472831EB17080185005CB055003CF1623FA0213CB6ACB1FCB3FC98040FB00925F03E20201200A0B0059BD242B6F6A2684080A06B90FA0218470D4080847A4937D29910CE6903E9FF9837812801B7810148987159F31840201580C0D0011B8C97ED44D0D70B1F8003DB29DFB513420405035C87D010C00B23281F2FFF274006040423D029BE84C600201200E0F0019ADCE76A26840206B90EB85FFC00019AF1DF6A26840106B90EB858FC0006ED207FA00D4D422F90005C8CA0715CBFFC9D077748018C8CB05CB0222CF165005FA0214CB6B12CCCCC973FB00C84014810108F451F2A7020070810108D718FA00D33FC8542047810108F451F2A782106E6F746570748018C8CB05CB025006CF165004FA0214CB6A12CB1FCB3FC973FB0002006C810108D718FA00D33F305224810108F459F2A782106473747270748018C8CB05CB025005CF165003FA0213CB6ACB1F12CB3FC973FB00000AF400C9ED54696225E5"
+        self.code = "B5EE9C72410214010002D4000114FF00F4A413F4BCF2C80B010201200203020148040504F8F28308D71820D31FD31FD31F02F823BBF264ED44D0D31FD31FD3FFF404D15143BAF2A15151BAF2A205F901541064F910F2A3F80024A4C8CB1F5240CB1F5230CBFF5210F400C9ED54F80F01D30721C0009F6C519320D74A96D307D402FB00E830E021C001E30021C002E30001C0039130E30D03A4C8CB1F12CB1FCBFF1011121302E6D001D0D3032171B0925F04E022D749C120925F04E002D31F218210706C7567BD22821064737472BDB0925F05E003FA403020FA4401C8CA07CBFFC9D0ED44D0810140D721F404305C810108F40A6FA131B3925F07E005D33FC8258210706C7567BA923830E30D03821064737472BA925F06E30D06070201200809007801FA00F40430F8276F2230500AA121BEF2E0508210706C7567831EB17080185004CB0526CF1658FA0219F400CB6917CB1F5260CB3F20C98040FB0006008A5004810108F45930ED44D0810140D720C801CF16F400C9ED540172B08E23821064737472831EB17080185005CB055003CF1623FA0213CB6ACB1FCB3FC98040FB00925F03E20201200A0B0059BD242B6F6A2684080A06B90FA0218470D4080847A4937D29910CE6903E9FF9837812801B7810148987159F31840201580C0D0011B8C97ED44D0D70B1F8003DB29DFB513420405035C87D010C00B23281F2FFF274006040423D029BE84C600201200E0F0019ADCE76A26840206B90EB85FFC00019AF1DF6A26840106B90EB858FC0006ED207FA00D4D422F90005C8CA0715CBFFC9D077748018C8CB05CB0222CF165005FA0214CB6B12CCCCC973FB00C84014810108F451F2A7020070810108D718FA00D33FC8542047810108F451F2A782106E6F746570748018C8CB05CB025006CF165004FA0214CB6A12CB1FCB3FC973FB0002006C810108D718FA00D33F305224810108F459F2A782106473747270748018C8CB05CB025005CF165003FA0213CB6ACB1F12CB3FC973FB00000AF400C9ED54696225E5"  # noqa: E501
         kwargs["code"] = Cell.one_from_boc(self.code)
         super().__init__(**kwargs)
         if "subwallet_id" not in self.options or self.options["subwallet_id"] is None:
-            self.options["subwallet_id"] = default_subwallet_id(self.options["wc"])
+            self.options["subwallet_id"] = self.default_subwallet_id(self.options["wc"])
```

### Comparing `tons-0.0.49/tons/tonsdk/crypto/_mnemonic.py` & `tons-1.0.0/tons/tonsdk/crypto/_mnemonic.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 def mnemonic_to_entropy(mnemo_words: List[str], password: Optional[str] = None):
     # TODO: implement password
     sign = hmac.new((" ".join(mnemo_words)).encode(
         'utf-8'), bytes(0), hashlib.sha512).digest()
     return sign
 
 
-def mnemonic_to_seed(mnemo_words: List[str], seed: str, password: Optional[str] = None):
+def mnemonic_to_seed(mnemo_words: List[str], seed: bytes, password: Optional[str] = None):
     entropy = mnemonic_to_entropy(mnemo_words, password)
-    return hashlib.pbkdf2_hmac("sha512", entropy, seed, PBKDF_ITERATIONS)
+    return hashlib.pbkdf2_hmac("sha512", entropy, seed, PBKDF_ITERATIONS, dklen=64)
 
 
-def mnemonic_to_private_key(mnemo_words: List[str], password: Optional[str] = None) -> Tuple[
-    bytes, bytes]:
+def mnemonic_to_private_key(mnemo_words: List[str], password: Optional[str] = None) -> Tuple[bytes, bytes]:
     """
+    https://github.com/ton-blockchain/ton/blob/be9c34c62dbd5d46089a255db8bf52c600b08aa5/tonlib/tonlib/keys/Mnemonic.cpp#L64
+
     :rtype: (bytes(public_key), bytes(secret_key))
     """
     seed = mnemonic_to_seed(
         mnemo_words, 'TON default seed'.encode('utf-8'), password)
     return crypto_sign_seed_keypair(seed[:32])
```

### Comparing `tons-0.0.49/tons/tonsdk/crypto/_utils.py` & `tons-1.0.0/tons/tonsdk/crypto/_utils.py`

 * *Files identical despite different names*

### Comparing `tons-0.0.49/tons/tonsdk/crypto/bip39/_english.py` & `tons-1.0.0/tons/tonsdk/crypto/bip39/_english.py`

 * *Files identical despite different names*

### Comparing `tons-0.0.49/tons/tonsdk/provider/_address.py` & `tons-1.0.0/tons/tonsdk/provider/_address.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890_-')
 
 
 def is_int(x):
     try:
         int(x)
         return True
-    except:
+    except (TypeError, ValueError):
         return False
 
 
 def is_hex(x):
     try:
         int(x, 16)
         return True
-    except:
+    except (TypeError, ValueError):
         return False
 
 
 def calcCRC(message):
     poly = 0x1021
     reg = 0
     message += b'\x00\x00'
@@ -96,14 +96,15 @@
         workchain = address_bytes[1]
     hx = hex(int.from_bytes(address_bytes[2:-2], "big"))[2:]
     hx = (64 - len(hx)) * "0" + hx
     raw_form = str(workchain) + ":" + hx
     account = account_forms(raw_form, test_only)
     account['given_type'] = "friendly_" + \
                             ("bounceable" if bounceable else "non_bounceable")
+    account['urlsafe'] = urlsafe
     return account
 
 
 def detect_address(unknown_form):
     if is_hex(unknown_form):
         return account_forms("-1:" + unknown_form)
     elif (":" in unknown_form) and is_int(unknown_form.split(":")[0]) and is_hex(
```

### Comparing `tons-0.0.49/tons/tonsdk/provider/_utils/__init__.py` & `tons-1.0.0/tons/tonsdk/provider/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tons-0.0.49/tons/tonsdk/utils/__init__.py` & `tons-1.0.0/tons/tonsdk/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ._address import Address
-from ._currency import to_nano, from_nano, TonCurrencyEnum
+from ._currency import to_nano, from_nano, TonCurrencyEnum, ton_currency_decimal_context, setup_default_decimal_context
 from ._exceptions import InvalidAddressError
-from ._utils import concat_bytes, move_to_end, tree_walk, crc32c, \
-    crc16, read_n_bytes_uint_from_array, compare_bytes, sign_message, b64str_to_bytes, \
+from ._utils import move_to_end, tree_walk, crc32c, \
+    crc16, read_n_bytes_uint_from_array, sign_message, b64str_to_bytes, \
     b64str_to_hex, bytes_to_b64str
 
 __all__ = [
     'Address',
     'InvalidAddressError',
 
-    'concat_bytes',
     'move_to_end',
     'tree_walk',
     'crc32c',
     'crc16',
     'read_n_bytes_uint_from_array',
-    'compare_bytes',
     'sign_message',
     'b64str_to_bytes',
     'b64str_to_hex',
     'bytes_to_b64str',
 
     'to_nano',
     'from_nano',
     'TonCurrencyEnum',
+    'ton_currency_decimal_context',
+    'setup_default_decimal_context'
 ]
```

### Comparing `tons-0.0.49/tons/tonsdk/utils/_address.py` & `tons-1.0.0/tons/tonsdk/utils/_address.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import ctypes
+from typing import Union
 
 from ._exceptions import InvalidAddressError
 from ._utils import crc16, string_to_bytes
 
 
 def parse_friendly_address(addr_str):
     if len(addr_str) != 48:
@@ -21,15 +22,15 @@
     crc = data[34:36]
     calced_crc = crc16(addr)
     if not (calced_crc[0] == crc[0] and calced_crc[1] == crc[1]):
         raise InvalidAddressError("Wrong crc16 hashsum")
 
     tag = addr[0]
     is_test_only = False
-    is_bounceable = False
+
     if tag & Address.TEST_FLAG:
         is_test_only = True
         tag ^= Address.TEST_FLAG
     if (tag != Address.BOUNCEABLE_TAG) and (tag != Address.NON_BOUNCEABLE_TAG):
         raise InvalidAddressError("Unknown address tag")
 
     is_bounceable = tag == Address.BOUNCEABLE_TAG
@@ -51,15 +52,15 @@
 
 
 class Address:
     BOUNCEABLE_TAG = 0x11
     NON_BOUNCEABLE_TAG = 0x51
     TEST_FLAG = 0x80
 
-    def __init__(self, any_form):
+    def __init__(self, any_form: Union['Address', str]):
         if any_form is None:
             raise InvalidAddressError("Invalid address")
 
         if isinstance(any_form, Address):
             self.wc = any_form.wc
             self.hash_part = any_form.hash_part
             self.is_test_only = any_form.is_test_only
@@ -111,33 +112,50 @@
         if is_url_safe is None:
             is_url_safe = self.is_url_safe
         if is_bounceable is None:
             is_bounceable = self.is_bounceable
         if is_test_only is None:
             is_test_only = self.is_test_only
 
-        if not is_user_friendly:  # FIXME: ignores other flags here!
+        if not is_user_friendly:
             return f"{self.wc}:{self.hash_part.hex()}"
-        else:
-            tag = Address.BOUNCEABLE_TAG if is_bounceable else Address.NON_BOUNCEABLE_TAG
 
-            if is_test_only:
-                tag |= Address.TEST_FLAG
+        tag = Address.BOUNCEABLE_TAG if is_bounceable else Address.NON_BOUNCEABLE_TAG
 
-            addr = (ctypes.c_int8 * 34)()
-            addr[0] = tag
-            addr[1] = self.wc
-            addr[2:] = self.hash_part
-            address_with_checksum = (ctypes.c_uint8 * 36)()
-            address_with_checksum[:34] = addr
-            address_with_checksum[34:] = crc16(addr)
-
-            address_base_64 = base64.b64encode(
-                address_with_checksum).decode('utf-8')
-            if is_url_safe:
-                address_base_64 = address_base_64.replace(
-                    "+", '-').replace("/", '_')
+        if is_test_only:
+            tag |= Address.TEST_FLAG
 
-            return str(address_base_64)
+        addr = (ctypes.c_int8 * 34)()
+        addr[0] = tag
+        addr[1] = self.wc
+        addr[2:] = self.hash_part
+        address_with_checksum = (ctypes.c_uint8 * 36)()
+        address_with_checksum[:34] = addr
+        address_with_checksum[34:] = crc16(addr)
+
+        address_base_64 = base64.b64encode(address_with_checksum).decode('utf-8')
+        if is_url_safe:
+            address_base_64 = address_base_64.replace(
+                "+", '-').replace("/", '_')
+
+        return str(address_base_64)
 
     def to_buffer(self):
-        return self.hash_part + bytearray([self.wc, self.wc, self.wc, self.wc])
+        wc_32bit_signed = self.wc.to_bytes(length=4, byteorder='big', signed=True)
+        return self.hash_part + bytearray(wc_32bit_signed)
+
+    def to_mask(self, only_friendly=False):
+        if only_friendly:
+            addr_str = self.to_string(True)
+        else:
+            addr_str = self.to_string(True, True, True)
+        return f"{addr_str[:3]}..{addr_str[-3:]}"
+
+    @staticmethod
+    def raw_id(address: Union['Address', str]):
+        return Address(address).to_string(False, False, False)
+
+    def __eq__(self, other: Union['Address', str]):
+        return Address.raw_id(self) == Address.raw_id(other)
+
+    def __ne__(self, other: Union['Address', str]):
+        return not self == other
```

### Comparing `tons-0.0.49/tons/tonsdk/utils/_utils.py` & `tons-1.0.0/tons/tonsdk/utils/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 import struct
 
 import nacl
 from nacl.bindings import crypto_sign, crypto_sign_BYTES
 from nacl.signing import SignedMessage
 
 
-def concat_bytes(a, b):
-    return a + b  # ?
-
-
 def move_to_end(index_hashmap, topological_order_arr, target):
     target_index = index_hashmap[target]
     for k in index_hashmap.keys():
         if index_hashmap[k] > target_index:
             index_hashmap[k] -= 1
     index_hashmap[target] = len(topological_order_arr) - 1
     data = topological_order_arr.pop(target_index)  # ?
@@ -97,18 +93,14 @@
     for c in range(size_bytes):
         res *= 256
         res += uint8_array[c]  # must be uint8
 
     return res
 
 
-def compare_bytes(bytes_1, bytes_2):
-    return str(bytes_1) == str(bytes_2)  # why str?
-
-
 def string_to_bytes(string, size=1):  # ?
     if size == 1:
         buf = (ctypes.c_uint8 * len(string))()
     elif size == 2:
         buf = (ctypes.c_uint16 * len(string) * 2)()
     elif size == 4:
         buf = (ctypes.c_uint32 * len(string) * 4)()
@@ -142,11 +134,7 @@
     _hex = codecs.encode(_bytes, "hex")
     return codecs.decode(_hex, "utf-8")
 
 
 def bytes_to_b64str(bytes_arr):
     return codecs.decode(codecs.encode(
         bytes_arr, "base64"), 'utf-8').replace("\n", '')
-
-
-def default_subwallet_id(workchain: int) -> int:
-    return 698983191 + workchain
```

### Comparing `tons-0.0.49/tons/ui/direct_cli/_commands/_config_cmd.py` & `tons-1.0.0/tons/ui/direct_cli/_commands/_config_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,31 +39,32 @@
 @cli.command()
 @click.option('--list', is_flag=True, callback=__list_configs,
               expose_value=False, is_eager=True, help='Show configs values')
 @click.option('--current-setup', is_flag=True, callback=__current_setup,
               expose_value=False, is_eager=True, help='Show current configuration')
 @click.option('--global', '-g', 'config_location', flag_value=ConfigLocation.global_location.value,
               help='Work with a global config')
-@click.option('--local', '-l', 'config_location', default=True,
-              flag_value=ConfigLocation.local_location.value,
-              help='Work with the config in the current workdir. [default]')
+@click.option('--custom', '-c', 'config_location', default=True,
+              flag_value=ConfigLocation.custom_location.value,
+              help='Work with the custom config (./.tons/config.yaml or TONS_CONFIG_PATH env variable is specified) '
+                   '[default]')
 @click.option('--file', '-f', 'config_location', help='Specific config path', metavar='PATH')
 @click.option('--network', help='Setup providers to a provided network',
               type=click.Choice(TonNetworkEnum))
 @click.option('--unset', is_flag=True, default=False, help='Removes [NAME] from config')
 @click.argument('name', required=False)
 @click.argument('value', required=False)
 @click.pass_obj
 def config(shared_object: SharedObject, config_location: str, network: TonNetworkEnum, unset: bool,
            name: str, value: str):
     """
     Control config parameters (check README.md for all fields info)
     """
     if config_location is None:
-        config_location = settings.CURRENT_CONFIG_PATH
+        config_location = settings.current_config_path()
 
     if network:
         set_network(shared_object.config, config_location, network)
         return
     elif name is None:
         raise click.MissingParameter(name)
 
@@ -73,29 +74,27 @@
     else:
         if unset:
             unset_config_field(config_location, name)
         else:
             try:
                 update_config_field(config_location, name, value)
             except StorageError as e:
-                raise CustomClickException(e)
+                raise CustomClickException(repr(e))
             except ValidationError as e:
                 msg = f"'{e.errors()[0]['loc'][0]}' {e.errors()[0]['msg']} "
                 raise CustomClickException(msg)
-            except ValueError as e:
+            except ValueError:
                 raise CustomClickException(
                     "Incorrect field name. Choices are: {}".format(", ".join(Config.field_names())))
 
 
 def __show_value(config: Config, config_location: str, name: str):
     try:
         config_to_show = get_config(
             config_location) if config_location else config
     except StorageError as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     if config_to_show:
         field_val = config_to_show.get_nondefault_value(name)
         if field_val:
             click.echo(field_val)
-
-
```

### Comparing `tons-0.0.49/tons/ui/direct_cli/_commands/_dev_cmd.py` & `tons-1.0.0/tons/ui/direct_cli/_commands/_dev_cmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import importlib.util
+import os
 import sys
 
 import click
+from appdirs import user_config_dir
 
 from tons.tonclient import ton_exceptions_handler
 from tons.tonclient.utils import RecordDoesNotExistError, KeyStoreInvalidPasswordError
-from tons.tonsdk.contract.wallet import SendModeEnum, Wallets
+from tons.tonsdk.contract.wallet import SendModeEnum, Wallets, WalletVersionEnum, InternalMessage
+from tons.tonsdk.utils import Address, TonCurrencyEnum
 from ._base_cmd import cli
 from .._utils import CustomClickException, click_ton_exception_handler, \
-    click_echo_success, with_keystore, y_n_to_bool
+    click_echo_success, with_keystore
 from ..._utils import SharedObject
 
 
 # TODO: optimize code, this part was developed fast
 
 @cli.group()
 def dev():
@@ -21,49 +24,45 @@
     """
 
 
 @dev.command(context_settings=dict(
     ignore_unknown_options=True,
 ))
 @ton_exceptions_handler(click_ton_exception_handler)
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('python_script_path', required=True, type=click.Path(exists=True))
 @click.argument('method_to_call', required=True)
 @click.argument('from_wallet', required=True)
 @click.argument('amount', required=False, metavar='TON_COINS_NUM')
 @click.option('--wait', '-w', is_flag=True, help='Wait until transaction is committed', default=False)
-@click.option('--bounceable', default="y", type=click.Choice(["y", "n"]),
-              show_default=True, callback=y_n_to_bool,
-              help="Bounce back on errors. Should be 'n' to send money to an empty address")
 @click.option('--pay-gas-separately', default="y", type=click.Choice(["y", "n"]), show_default=True)
 @click.option('--ignore-errors', default="n", type=click.Choice(["y", "n"]), show_default=True,
               help='Bounce back if error occurs.')
 @click.option('--destroy-if-zero', default="n", type=click.Choice(["y", "n"]), show_default=True)
 @click.option('--transfer-all', default="n", type=click.Choice(["y", "n"]), show_default=True)
 @click.argument('custom_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_obj
 def send_internal(shared_object: SharedObject, from_wallet, python_script_path, method_to_call, amount,
-                  wait, bounceable, pay_gas_separately, ignore_errors, destroy_if_zero, transfer_all,
+                  wait, pay_gas_separately, ignore_errors, destroy_if_zero, transfer_all,
                   custom_args):
     """
     Generate internal message by METHOD_TO_CALL from PYTHON_SCRIPT_PATH
     and send it by selected FROM_WALLET wallet
     """
     if amount is None and not transfer_all:
         raise CustomClickException(
             "You must specify amount when you do not use --transfer-all flag.")
 
     try:
         record = shared_object.keystore.get_record_by_name(
             from_wallet, raise_none=True)
-        mnemonics = shared_object.keystore.get_secret(
-            record, shared_object.keystore_password).split(" ")
+        mnemonics = shared_object.keystore.get_secret(record).split(" ")
     except (RecordDoesNotExistError,
             KeyStoreInvalidPasswordError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     send_mode = 0
     if ignore_errors == "y":
         send_mode |= SendModeEnum.ignore_errors
     if pay_gas_separately == "y":
         send_mode |= SendModeEnum.pay_gas_separately
     if destroy_if_zero == "y":
@@ -76,17 +75,23 @@
 
     spec = importlib.util.spec_from_file_location("module.name", python_script_path)
     module = importlib.util.module_from_spec(spec)
     sys.modules["module.name"] = module
     spec.loader.exec_module(module)
     addr, state_init, body = getattr(module, method_to_call)(wallet, custom_args)
 
-    result = shared_object.ton_client.transfer(
-        wallet, addr, amount, body, send_mode, bounceable, wait, state_init)
+    messages = [InternalMessage(
+        to_addr=Address(addr),
+        amount=amount,
+        currency=TonCurrencyEnum.ton,
+        body=body,
+        state_init=state_init,
+    )]
 
+    _, result = shared_object.ton_client.transfer(wallet, messages, wait)
     click_echo_success(
         f"Internal message generated by {method_to_call} was sent to address {addr}. Result: {result}")
 
 
 @dev.command(context_settings=dict(
     ignore_unknown_options=True,
 ))
@@ -126,18 +131,70 @@
     click_echo_success(f"{result}")
 
 
 @dev.command(context_settings=dict(
     ignore_unknown_options=True,
 ))
 @ton_exceptions_handler(click_ton_exception_handler)
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('python_script_path', required=True, type=click.Path(exists=True))
 @click.argument('method_to_call', required=True)
 @click.argument('custom_args', nargs=-1, type=click.UNPROCESSED)
 @click.pass_obj
 def pass_forward(shared_object: SharedObject, python_script_path, method_to_call, custom_args):
+    """
+    Pass shared_object and all provided arguments to the python_script_path.method_to_call script
+    """
     spec = importlib.util.spec_from_file_location("module.name", python_script_path)
     module = importlib.util.module_from_spec(spec)
     sys.modules["module.name"] = module
     spec.loader.exec_module(module)
     getattr(module, method_to_call)(shared_object, custom_args)
+
+
+@dev.command()
+@with_keystore(sensitive_data=True)
+@click.argument('name', required=True)
+@click.option('--yes', '-y', 'is_sure', is_flag=True, help='Do not show the prompt')
+@click.pass_obj
+def replace_toncli_wallet(shared_object: SharedObject, name, is_sure: bool):
+    """
+    Replace standard toncli wallet
+    """
+    wallet_build_path = os.path.join(user_config_dir("toncli"), "wallet", "build")
+
+    if not is_sure:
+        click.confirm(
+            f'This command will replace .pk and .addr files inside {wallet_build_path} directory. '
+            f'Do you want to proceed?',
+            abort=True)
+
+    try:
+        record = shared_object.keystore.get_record_by_name(
+            name, raise_none=True)
+        mnemonics = shared_object.keystore.get_secret(record).split(" ")
+    except (RecordDoesNotExistError, KeyStoreInvalidPasswordError, OSError) as e:
+        raise CustomClickException(repr(e))
+
+    if record.subwallet_id != 0 or record.version != WalletVersionEnum.v3r2:
+        raise CustomClickException(f"Wallet '{name}' can not be used because "
+                                   f"toncli uses subwallet_id == 0 and wallet version == v3r2.")
+
+    wallet_pk = os.path.join(wallet_build_path, "contract.pk")
+    wallet_addr = os.path.join(wallet_build_path, "contract.addr")
+    wallet_contract_addr = os.path.join(wallet_build_path, "contract_address")
+    addr, pk = Wallets.to_addr_pk(mnemonics, record.version,
+                                  record.workchain, record.subwallet_id)
+
+    record_addr = Address(record.address)
+    with open(wallet_contract_addr, "w") as f:
+        f.write(f"{record_addr.to_string(False, False, False)} "
+                f"{record_addr.to_string(True, False, True)} "
+                f"{record_addr.to_string(True, False, False)} ")
+
+    with open(wallet_pk, "wb") as f:
+        f.write(pk)
+
+    with open(wallet_addr, "wb") as f:
+        f.write(addr)
+
+    click_echo_success("Wallet has been replaced.")
```

### Comparing `tons-0.0.49/tons/ui/direct_cli/_commands/_keystore_cmd.py` & `tons-1.0.0/tons/ui/direct_cli/_commands/_keystore_cmd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,134 @@
 import click
 
 from tons import settings
 from tons.tonclient.utils import KeyStoreAlreadyExistsError, KeyStoreInvalidPasswordError, \
     InvalidMnemonicsError
+from tons.tonclient.utils._keystores import KeyStoreTypeEnum, PasswordKeyStore
 from ._base_cmd import cli
-from .._utils import CustomClickException, with_keystores, with_keystore, click_echo_success
-from ..._utils import new_keystore_password_is_valid, SharedObject
+from .._utils import CustomClickException, with_keystores, with_keystore, click_echo_success, keystore_upgrade_message
+from ..._utils import SharedObject
 
 
 @cli.group()
 def keystore():
     """
     Operate with keystores
     """
 
 
-def __validate_password(ctx, param, value):
-    if not new_keystore_password_is_valid(value):
-        raise CustomClickException(
-            'password need to be at least 6 characters long')
-    return value
-
-
 @keystore.command()
 @with_keystores
 @click.argument('name', required=True)
-@click.password_option(default=settings.KEYSTORE_PASSWORD,
-                       confirmation_prompt=False, prompt=False if settings.KEYSTORE_PASSWORD else True,
-                       callback=__validate_password)
+@click.option('--keystore-type', '-t', default=KeyStoreTypeEnum.password.value, show_default=True,
+              type=click.Choice([KeyStoreTypeEnum.password]))
+@click.option("--password", default=settings.KEYSTORE_PASSWORD, show_default=False,
+              help='Required only for a "password" type keystore')
+@click.option("--pin", default=settings.YUBIKEY_PIN, show_default=False,
+              help='Required only for a "yubikey" type keystore')
 @click.pass_obj
-def new(shared_object: SharedObject, name, password):
+def new(shared_object: SharedObject, name, keystore_type, password, pin):
     """
     Create new .keystore file with a given name
     """
     try:
-        shared_object.keystores.create_new_keystore(name, password, save=True)
-    except KeyStoreAlreadyExistsError as e:
-        raise CustomClickException(e)
+        if keystore_type == KeyStoreTypeEnum.password:
+            if not password:
+                password = click.prompt("Password[]", hide_input=True)
+            shared_object.keystores.create_new_keystore(
+                name, keystore_type, secret=password,
+                save=True, )
+        elif keystore_type == KeyStoreTypeEnum.yubikey:
+            if not pin:
+                pin = click.prompt("Yubikey PIN[]", hide_input=True)
+            shared_object.keystores.create_new_keystore(
+                name, keystore_type, secret=pin,
+                save=True)
+    except (
+            KeyStoreAlreadyExistsError, KeyStoreInvalidPasswordError,
+            Exception) as e:  # fixme: specify exceptions from yubikey
+        raise CustomClickException(repr(e))
 
     click_echo_success(
         f"keystore {name} has been created. To use it run 'tons config tons.keystore_name {name}'.")
 
 
-@keystore.command()
+@keystore.command(name='list')
 @with_keystores
 @click.pass_obj
-def list(shared_object: SharedObject):
+def list_(shared_object: SharedObject):
     """
     List all .keystore files in a current keystore workdir
     """
-    for keystore in shared_object.keystores.keystore_paths.keys():
-        click.echo(keystore)
+    keystores = shared_object.keystores.load_all()
+
+    for keystore in keystores:
+        if keystore.has_been_upgraded:
+            click.echo(keystore_upgrade_message(keystore))
+        click.echo(keystore.pretty_string())
 
 
 @keystore.command()
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @with_keystores
 @click.argument('backup_file_path', required=True, type=click.Path(writable=True))
 @click.option('--yes', '-y', 'is_sure', is_flag=True, help='Do not show the prompt')
 @click.pass_obj
 def backup(shared_object: SharedObject, backup_file_path: str, is_sure: bool):
     """
     Backup the keystore into a specified file
     """
     if not is_sure:
         click.confirm(
-            f'Backup stores keys in UNENCRYPTED FORM. Are you sure want to export unencrypted keys to disk?',
+            'Backup stores keys in UNENCRYPTED FORM. Are you sure want to export unencrypted keys to disk?',
             abort=True)
     try:
         shared_object.keystores.backup_keystore(
-            shared_object.keystore, backup_file_path,
-            shared_object.keystore_password)
+            shared_object.keystore, backup_file_path)
     except (KeyStoreInvalidPasswordError, OSError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     click_echo_success(
         f"backup {backup_file_path} has been created from the keystore {shared_object.config.tons.keystore_name}")
 
 
 @keystore.command()
 @with_keystores
 @click.argument('name', required=True)
 @click.argument('backup_file_path', required=True, type=click.Path(exists=True, readable=True))
-@click.password_option(default=settings.KEYSTORE_PASSWORD,
-                       confirmation_prompt=False, prompt=False if settings.KEYSTORE_PASSWORD else True,
-                       callback=__validate_password)
+@click.option('--keystore-type', '-t', default=KeyStoreTypeEnum.password.value, show_default=True,
+              type=click.Choice([KeyStoreTypeEnum.password]))
+@click.option("--password", default=settings.KEYSTORE_PASSWORD, show_default=False,
+              help='Required only for a "password" type keystore')
+@click.option("--pin", default=settings.YUBIKEY_PIN, show_default=False,
+              help='Required only for a "yubikey" type keystore')
 @click.option('--from-ton-cli', 'from_ton_cli', is_flag=True, help='Restore from the ton-cli util')
 @click.pass_obj
-def restore(shared_object: SharedObject, name: str, backup_file_path: str, password: str,
-            from_ton_cli: bool):
+def restore(shared_object: SharedObject, name: str, backup_file_path: str, keystore_type,
+            password: str, pin: str, from_ton_cli: bool):
     """
     Restore the keystore from a specified file
     """
     try:
+        if keystore_type == KeyStoreTypeEnum.password:
+            if not password:
+                password = click.prompt("Password[]", hide_input=True)
+            PasswordKeyStore.validate_password(password)
+            secret = password
+        elif keystore_type == KeyStoreTypeEnum.yubikey:
+            if not pin:
+                pin = click.prompt("Yubikey PIN[]", hide_input=True)
+            secret = pin
+        else:
+            raise CustomClickException("Unknown keystore type.")
+
         if from_ton_cli:
             shared_object.keystores.restore_ton_cli_keystore(
-                name, backup_file_path, password)
+                name, backup_file_path, keystore_type, secret)
         else:
             shared_object.keystores.restore_tons_keystore(
-                name, backup_file_path, password)
-    except (InvalidMnemonicsError, KeyStoreAlreadyExistsError) as e:
-        raise CustomClickException(e)
+                name, backup_file_path, keystore_type, secret)
+
+    except (InvalidMnemonicsError, KeyStoreAlreadyExistsError, KeyStoreInvalidPasswordError) as e:
+        raise CustomClickException(repr(e))
 
     click_echo_success(f"keystore {name} has been restored.")
```

### Comparing `tons-0.0.49/tons/ui/direct_cli/_commands/_wallet_cmd.py` & `tons-1.0.0/tons/ui/direct_cli/_commands/_wallet_cmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,109 @@
 import os
+from typing import Optional
 
 import click
 
 from tons.tonclient import ton_exceptions_handler
+from tons.tonclient._client._base import AddressState
 from tons.tonclient.utils import RecordAlreadyExistsError, RecordDoesNotExistError, \
-    WhitelistContactDoesNotExistError, KeyStoreInvalidPasswordError, InvalidMnemonicsError
-from tons.tonsdk.contract.wallet import SendModeEnum, WalletVersionEnum, Wallets
+    WhitelistContactDoesNotExistError, KeyStoreInvalidPasswordError, InvalidMnemonicsError, KeyStoreDoesNotExistError
+from tons.tonsdk.boc import Cell
+from tons.tonsdk.contract.wallet import SendModeEnum, WalletVersionEnum, Wallets, WalletContract, InternalMessage
+from tons.tonsdk.crypto import mnemonic_to_wallet_key
+from tons.tonsdk.crypto._payload_encryption import encrypt_message
 from tons.tonsdk.utils import TonCurrencyEnum, Address
-from tons.tonsdk.utils._utils import default_subwallet_id
 from tons.utils import storage
 from ._base_cmd import cli
 from .._utils import CustomClickException, with_whitelist, with_keystore, click_ton_exception_handler, \
-    click_echo_success, y_n_to_bool
-from ..._utils import md_table, SharedObject, form_wallets_table
+    click_echo_success, y_n_to_bool, with_keystores, keystore_upgrade_message
+from ..._utils import SharedObject, form_wallets_table
 
 
-def __parse_subwallet_id_after_workchain(ctx, param, value):
-    version = ctx.params['version'] or ctx.obj.config.tons.default_wallet_version
-    if version in WalletVersionEnum.with_subwallet_id():
-        return default_subwallet_id(ctx.params['workchain']) if value is None else value
-
-    return None
+def __parse_subwallet_id_after_workchain(ctx: SharedObject, version: Optional[WalletVersionEnum], workchain: int,
+                                         subwallet_id: int):
+    if version is None:
+        version = ctx.config.tons.default_wallet_version
+    return WalletContract.default_subwallet_id(workchain, version) \
+        if subwallet_id is None else subwallet_id
 
 
 @cli.group()
 def wallet():
     """
     Operate with wallets
     """
 
 
 @wallet.command()
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @with_whitelist
 @click.argument('name', required=True)
 @click.option('--version', '-v', type=click.Choice(WalletVersionEnum))
 @click.option('--workchain', '-wc', default=0, show_default=True, type=int)
-@click.option('--subwallet-id', '-id', type=int, callback=__parse_subwallet_id_after_workchain,
+@click.option('--subwallet-id', '-id', type=int,
               help="Extra field for v3 and v4 versions. "
                    "Leave empty to use default 698983191 + workchain")
 @click.option('--comment', help='Extra information about the wallet')
-@click.option('--save-to-whitelist', 'contact_name', help='Contact name to save', metavar='NAME')
+@click.option('--save-to-whitelist', 'contact_name', help='Contact name to save to global whitelist', metavar='NAME')
 @click.pass_obj
-def create(shared_object: SharedObject, name: str, version: str, workchain: int, subwallet_id: int,
+def create(shared_object: SharedObject, name: str, version: WalletVersionEnum, workchain: int, subwallet_id: int,
            comment: str, contact_name: str):
     """
     Create wallet data and add it to the keystore
     """
+    subwallet_id = __parse_subwallet_id_after_workchain(shared_object, version, workchain,
+                                                        subwallet_id)
+
     if contact_name:
         contact = shared_object.whitelist.get_contact(contact_name)
         if contact is not None:
             raise CustomClickException(
                 f"Contact with the name '{contact_name}' already exists")
 
-    if not version:
+    if version is None:
         version = WalletVersionEnum(
             shared_object.config.tons.default_wallet_version)
 
     try:
-        mnemonics, pub_k, _priv_k, wallet = Wallets.create(version, workchain, subwallet_id)
-        shared_object.keystore.add_record(name, wallet.address,
-                                          pub_k.hex(), mnemonics, version,
-                                          workchain, subwallet_id, comment, save=True)
+        mnemonics, _, _, wallet_ = Wallets.create(version, workchain, subwallet_id)
+        shared_object.keystore.add_new_record(name, mnemonics, version,
+                                              workchain, subwallet_id, comment, save=True)
     except RecordAlreadyExistsError as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     if contact_name:
         shared_object.whitelist.add_contact(
-            contact_name, wallet.address.to_string(True), save=True)
+            contact_name, wallet_.address.to_string(True), save=True)
 
     click_echo_success(f"wallet {name} has been created.")
 
 
 @wallet.command()
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @with_whitelist
 @click.argument('name', required=True)
 @click.option('--name', '-n', 'new_name', help='New wallet name')
 @click.option('--comment', '-c', 'new_comment', help='New extra information about the wallet')
 @click.pass_obj
 def edit(shared_object: SharedObject, name: str, new_name: str, new_comment: str):
     """
     Edit wallet data in a keystore
     """
     try:
         shared_object.keystore.edit_record(
             name, new_name, new_comment, save=True)
-    except RecordDoesNotExistError as e:
-        raise CustomClickException(e)
+    except (RecordDoesNotExistError, RecordAlreadyExistsError) as e:
+        raise CustomClickException(repr(e))
 
     click_echo_success(f"wallet {name} has been edited.")
 
 
 @wallet.command()
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @with_whitelist
 @click.argument('name', required=True)
 @click.option('--yes', '-y', 'is_sure', is_flag=True, help='Do not show the prompt')
 @click.pass_obj
 def delete(shared_object: SharedObject, name: str, is_sure: bool):
     """
     Delete wallet data from a keystore
@@ -105,34 +111,34 @@
     if not is_sure:
         click.confirm(
             f'Are you sure you want to delete {name} wallet?', abort=True)
 
     try:
         shared_object.keystore.delete_record(name, save=True)
     except RecordDoesNotExistError as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     click_echo_success(f"wallet {name} has been deleted.")
 
 
 @wallet.command()
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @with_whitelist
 @click.argument('name', required=True)
 @click.option('--verbose', '-v', is_flag=True, help='Load info about wallet from TON network')
 @click.pass_obj
 def get(shared_object: SharedObject, name: str, verbose: bool):
     """
     Get all wallet data from a keystore
     """
     try:
         wallet_record = shared_object.keystore.get_record_by_name(
             name, raise_none=True)
     except RecordDoesNotExistError as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     addr = Address(wallet_record.address)
     if verbose:
         addr_info = shared_object.ton_client.get_address_information(
             wallet_record.address)
 
     click.echo(f"Raw address: {addr.to_string(False, False, False)}")
@@ -145,204 +151,301 @@
 
     if verbose:
         click.echo("--- Verbose wallet information ---")
         for k, v in addr_info.dict().items():
             click.echo(str(k) + ': ' + str(v))
 
 
-@wallet.command()
+@wallet.command(name='list')
 @ton_exceptions_handler(click_ton_exception_handler)
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @click.option('--currency', '-c', default=TonCurrencyEnum.ton, show_default=True,
               type=click.Choice(TonCurrencyEnum))
 @click.option('--verbose', '-v', 'verbose', is_flag=True, default=False,
               help="Extra information from TON")
 @click.pass_obj
-def list(shared_object: SharedObject, verbose: bool, currency: TonCurrencyEnum):
+def list_(shared_object: SharedObject, verbose: bool, currency: TonCurrencyEnum):
     """
-    Print all wallets info as a markdown table. 
+    Print all wallets info as a markdown table.
     You can output this command into .md file
     """
-    wallets = shared_object.keystore.records
+    wallets = shared_object.keystore.get_records(shared_object.config.tons.sort_keystore)
     wallet_infos = None
     if verbose:
         wallet_infos = shared_object.ton_client.get_addresses_information(
             [wallet.address for wallet in wallets], currency)
 
     table = form_wallets_table(wallets, verbose, wallet_infos, True)
 
     click.echo(table)
 
 
 @wallet.command()
-@with_keystore(password_required=False)
+@with_keystore(sensitive_data=False)
 @with_whitelist
 @click.argument('name', required=True)
 @click.argument('version', type=click.Choice(WalletVersionEnum))
 @click.argument('workchain', type=int)
 @click.argument('mnemonics')
-@click.option('--subwallet-id', '-id', type=int, callback=__parse_subwallet_id_after_workchain,
+@click.option('--subwallet-id', '-id', type=int,
               help="Extra field for v3 and v4 versions. "
                    "Leave empty to use default 698983191 + workchain")
 @click.option('--comment', help='Extra information about the wallet')
 @click.option('--save-to-whitelist', 'contact_name', help='Contact name to save', metavar='NAME')
 @click.pass_obj
 def import_from_mnemonics(shared_object: SharedObject, name: str, version: WalletVersionEnum,
                           workchain: int, mnemonics: str, subwallet_id: int, comment: str,
                           contact_name: str):
     """
     Create wallet data from mnemonics and add it to the keystore
     """
+    subwallet_id = __parse_subwallet_id_after_workchain(shared_object, version, workchain,
+                                                        subwallet_id)
     if contact_name:
         contact = shared_object.whitelist.get_contact(contact_name)
         if contact is not None:
             raise CustomClickException(
                 f"Contact with the name '{contact_name}' already exists")
 
     mnemonics = mnemonics.split(" ")
     try:
-        mnemonics, pub_k, _priv_k, wallet = Wallets.from_mnemonics(
-            mnemonics, version, workchain, subwallet_id)
-        shared_object.keystore.add_record(name, wallet.address,
-                                          pub_k.hex(), mnemonics, version,
-                                          workchain, subwallet_id, comment, save=True)
+        shared_object.keystore.add_new_record(name, mnemonics, version,
+                                              workchain, subwallet_id, comment, save=True)
     except (RecordAlreadyExistsError, InvalidMnemonicsError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     if contact_name:
         shared_object.whitelist.add_contact(
             contact_name, wallet.address.to_string(True), save=True)
 
     click_echo_success(f"wallet {name} has been imported.")
 
 
 @wallet.command()
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('name', required=True)
 @click.pass_obj
 def reveal(shared_object: SharedObject, name: str):
     """
     Echo mnemonics of a wallet by its name
     """
     try:
         record = shared_object.keystore.get_record_by_name(
             name, raise_none=True)
-        mnemonics = shared_object.keystore.get_secret(
-            record, shared_object.keystore_password)
+        mnemonics = shared_object.keystore.get_secret(record)
         click.echo(mnemonics)
 
     except (RecordDoesNotExistError, KeyStoreInvalidPasswordError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
 
 @wallet.command()
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('name', required=True)
 @click.argument('destination_dir', default=".", required=False, metavar='DESTINATION_DIR')
 @click.pass_obj
 def to_addr_pk(shared_object: SharedObject, name: str, destination_dir: str):
     """
     Export wallet to .pk and .addr file into a specified directory
     """
     try:
         record = shared_object.keystore.get_record_by_name(
             name, raise_none=True)
-        mnemonics = shared_object.keystore.get_secret(
-            record, shared_object.keystore_password).split(" ")
+        mnemonics = shared_object.keystore.get_secret(record).split(" ")
         addr, pk = Wallets.to_addr_pk(mnemonics, record.version,
                                       record.workchain, record.subwallet_id)
 
         addr_path = os.path.join(
             destination_dir, record.name + ".addr")
         pk_path = os.path.join(destination_dir, record.name + ".pk")
         storage.save_bytes(addr_path, addr)
         storage.save_bytes(pk_path, pk)
 
     except (RecordDoesNotExistError, KeyStoreInvalidPasswordError, OSError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
 
 @wallet.command()
 @ton_exceptions_handler(click_ton_exception_handler)
 @with_whitelist
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('name', required=True)
 @click.pass_obj
 def init(shared_object: SharedObject, name: str):
     """
     Initialize address as a wallet
     """
     try:
-        record = shared_object.keystore.get_record_by_name(
-            name, raise_none=True)
-        mnemonics = shared_object.keystore.get_secret(
-            record, shared_object.keystore_password).split(" ")
-    except (RecordDoesNotExistError, KeyStoreInvalidPasswordError) as e:
-        raise CustomClickException(e)
+        record = shared_object.keystore.get_record_by_name(name, raise_none=True)
+    except RecordDoesNotExistError as e:
+        raise CustomClickException(repr(e))
+
+    address_info = shared_object.ton_client.get_address_information(record.address)
+
+    if address_info.state == AddressState.active:
+        raise CustomClickException("Wallet is already active.")
+
+    if address_info.balance < (init_amount := WalletContract.init_amount(record.version)):
+        raise CustomClickException(
+            f"Insufficient amount, at least {init_amount} required.")
+
+    try:
+        mnemonics = shared_object.keystore.get_secret(record).split(" ")
+    except KeyStoreInvalidPasswordError as e:
+        raise CustomClickException(repr(e))
 
     _mnemonics, _pub_k, _priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
                                                                  record.workchain, record.subwallet_id)
 
-    result = shared_object.ton_client.deploy_wallet(wallet)
+    _, result = shared_object.ton_client.deploy_wallet(wallet)
 
     click_echo_success(result)
 
 
 @wallet.command()
 @ton_exceptions_handler(click_ton_exception_handler)
 @with_whitelist
-@with_keystore(password_required=True)
+@with_keystore(sensitive_data=True)
 @click.argument('from_wallet', required=True, metavar='WALLET_NAME')
 @click.argument('to_contact', required=True, metavar='CONTACT_NAME')
 @click.argument('amount', required=False, metavar='TON_COINS_NUM')
 @click.option('--message', '-m', help='Attach message to the transfer')
+@click.option('--encrypt-message', '-e', 'encrypt_message_flag', help='Encrypt message', is_flag=True, default=False)
 @click.option('--wait', '-w', is_flag=True, help='Wait until transaction is committed', default=False)
-@click.option('--bounceable', default="y", type=click.Choice(["y", "n"]),
-              show_default=True, callback=y_n_to_bool,
-              help="Bounce message back on errors. Should be 'n' to send money to an empty address")
 @click.option('--pay-gas-separately', default="y", type=click.Choice(["y", "n"]),
               show_default=True, callback=y_n_to_bool)
 @click.option('--ignore-errors', default="n", type=click.Choice(["y", "n"]), show_default=True,
               help='Bounce back if error occurs', callback=y_n_to_bool)
 @click.option('--destroy-if-zero', default="n", type=click.Choice(["y", "n"]),
               show_default=True, callback=y_n_to_bool)
 @click.option('--transfer-all', default="n", type=click.Choice(["y", "n"]),
               show_default=True, callback=y_n_to_bool)
+@click.option('--body', metavar='FILE', required=False, help="Path to a file containing the body (bag of cells)")
+@click.option('--state-init', metavar='FILE', required=False,
+              help='Path to a file containing the state init (bag of cells)')
 @click.pass_obj
-def transfer(shared_object: SharedObject, from_wallet, to_contact, amount, message, wait, bounceable,
-             pay_gas_separately, ignore_errors, destroy_if_zero, transfer_all):
+def transfer(shared_object: SharedObject, from_wallet, to_contact, amount, message, encrypt_message_flag, wait,
+             pay_gas_separately, ignore_errors, destroy_if_zero, transfer_all, body, state_init):
     """
     Transfer coins from your wallet to any address
     """
     if amount is None and not transfer_all:
         raise CustomClickException(
             "You must specify amount when you do not use --transfer-all flag.")
 
+    if (message is not None) and (body is not None):
+        raise CustomClickException("You cannot specify message and body at the same time.")
+
+    if body is not None:
+        try:
+            with open(body, 'rb') as file_obj:
+                body = file_obj.read()
+        except (FileNotFoundError, PermissionError, IsADirectoryError, OSError):
+            raise CustomClickException(f"Failed to open file: '{body}'")
+        try:
+            body = Cell.one_from_boc(body)
+        except Exception:
+            raise CustomClickException("Failed to parse body bag of cells")
+
+    if state_init is not None:
+        try:
+            with open(state_init, 'rb') as file_obj:
+                state_init = file_obj.read()
+        except (FileNotFoundError, PermissionError, IsADirectoryError, OSError):
+            raise CustomClickException(f"Failed to open file: '{state_init}'")
+        try:
+            state_init = Cell.one_from_boc(state_init)
+        except Exception:
+            raise CustomClickException("Failed to parse state init bag of cells")
+
     try:
         record = shared_object.keystore.get_record_by_name(
             from_wallet, raise_none=True)
-        mnemonics = shared_object.keystore.get_secret(
-            record, shared_object.keystore_password).split(" ")
-        contact = shared_object.whitelist.get_contact(
-            to_contact, raise_none=True)
+        mnemonics = shared_object.keystore.get_secret(record).split(" ")
+        contact = \
+            shared_object.whitelist.get_contact(to_contact) or \
+            shared_object.keystore.whitelist.get_contact(to_contact)
+
+        if contact is None:
+            raise WhitelistContactDoesNotExistError(f"Contact with the name {to_contact} does not exist")
     except (
             WhitelistContactDoesNotExistError, RecordDoesNotExistError,
             KeyStoreInvalidPasswordError) as e:
-        raise CustomClickException(e)
+        raise CustomClickException(repr(e))
 
     send_mode = 0
     if ignore_errors:
         send_mode |= SendModeEnum.ignore_errors
     if pay_gas_separately:
         send_mode |= SendModeEnum.pay_gas_separately
     if destroy_if_zero:
         send_mode |= SendModeEnum.destroy_account_if_zero
     if transfer_all:
         send_mode |= SendModeEnum.carry_all_remaining_balance
         amount = 0
 
-    _mnemonics, _pub_k, _priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
+    _mnemonics, pub_k, priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
                                                                  record.workchain, record.subwallet_id)
-    result = shared_object.ton_client.transfer(
-        wallet, contact.address, amount, message, send_mode, bounceable, wait)
 
+    if encrypt_message_flag:
+        if not message:
+            raise CustomClickException("Please specify message to encrypt (--message)")
+
+        receiver_info = shared_object.ton_client.get_address_information(contact.address)
+        if not receiver_info.can_receive_encrypted_payload:
+            raise CustomClickException("Contact cannot receive encrypted messages")
+
+        message = encrypt_message(message, pub_k, receiver_info.public_key, priv_k, wallet.address)
+
+    messages = [InternalMessage(
+        to_addr=Address(contact.address),
+        amount=amount,
+        currency=TonCurrencyEnum.ton,
+        body=message or body,
+        state_init=state_init,
+    )]
+
+    _, result = shared_object.ton_client.transfer(wallet, messages, wait)
     click_echo_success(result)
+
+
+@wallet.command()
+@ton_exceptions_handler(click_ton_exception_handler)
+@with_keystores
+@with_keystore(sensitive_data=True)
+@click.argument('wallet_name', type=str, required=True, )
+@click.argument('keystore_name_dst', metavar='KEYSTORE_DST', type=str, required=True)
+@click.option('--delete', '-d', 'remove_old', is_flag=True, default=False,
+              help='Remove wallet from the current keystore')
+@click.pass_obj
+def move(ctx: SharedObject, wallet_name: str, keystore_name_dst: str, remove_old: bool):
+    """
+    Move wallet to another keystore
+    """
+    keystore_src = ctx.keystore
+
+    try:
+        record = keystore_src.get_record_by_name(wallet_name, raise_none=True)
+    except RecordDoesNotExistError as e:
+        raise CustomClickException(repr(e))
+
+    try:
+        keystore_dst = ctx.keystores.get_keystore(keystore_name_dst,
+                                                  raise_none=True)
+    except KeyStoreDoesNotExistError as e:
+        raise CustomClickException(repr(e))
+
+    if keystore_dst.has_been_upgraded:
+        click.echo(keystore_upgrade_message(keystore_dst))
+
+    mnemonics = ctx.keystore.get_secret(record).split(" ")
+    try:
+        keystore_dst.add_new_record(record.name, mnemonics, record.version, record.workchain,
+                                    record.subwallet_id, record.comment, save=True)
+    except RecordAlreadyExistsError as e:
+        raise CustomClickException(repr(e))
+
+    if remove_old:
+        ctx.keystore.delete_record(record.name, save=True)
+
+    click_echo_success(f'Wallet \"{wallet_name}\" has been successfully {"moved" if remove_old else "copied"} '
+                       f'from {keystore_src.name} to {keystore_dst.name}')
```

### Comparing `tons-0.0.49/tons/ui/interactive_cli/_modified_inquirer/_text_render.py` & `tons-1.0.0/tons/ui/interactive_cli/_modified_inquirer/_text_render.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,53 @@
+from typing import Optional
+
 from inquirer import errors, Text
 from inquirer.render.console.base import BaseConsoleRender
 from readchar import key
 
+from ._utils import text_to_not_formatted_displayed_lines
+
 
 class ModifiedTextRender(BaseConsoleRender):
     title_inline = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.current = self.question.default or ""
         self.cursor_offset = 0
 
-    def get_current_value(self):
+    def get_current_value(self, console_render: 'ModifiedConsoleRender'):
         current = self.current
-        extra_len = len(self.question._message) + len("[?]  :")
-        diff = (extra_len + len(self.current)) - self.terminal.width
-        max_cursor_offset = self.terminal.width - extra_len
-        if diff > 0:
-            to_hide = diff
-            cursor_offset_from_beginning = len(self.current) - self.cursor_offset
-            if cursor_offset_from_beginning != 0:
-                to_replace = min(diff, cursor_offset_from_beginning)
-                current = current[to_replace:]
-                to_hide -= to_replace
-
-            if to_hide > 0:
-                current = current[:-to_hide]
-                diff -= to_hide
-
-        if diff >= 0 and self.cursor_offset > max_cursor_offset:
-            cursor_offset = max_cursor_offset
-            # if self.cursor_offset == 0:
-            #     cursor_offset = 0
-            # else:
-            #     cursor_offset = self.cursor_offset - diff if diff > 0 else self.cursor_offset
+        message = f"[?] {self.question._message}: {self.current}"
+        message_lines = text_to_not_formatted_displayed_lines(message, self.terminal.width)
+        cursor_x0 = cursor_x = len(message_lines[-1])
+        cursor_y0 = cursor_y = len(message_lines) - 1
+        cursor_offset = self.cursor_offset
+        while cursor_offset > 0:
+            cursor_x -= 1
+            if cursor_x < 0:
+                cursor_y -= 1
+                cursor_x = len(message_lines[cursor_y])-1
+            cursor_offset -= 1
+
+        cursor_delta_x = cursor_x - cursor_x0
+        cursor_delta_y = cursor_y - cursor_y0
+
+        if cursor_delta_x > 0:
+            current += self.terminal.move_right * cursor_delta_x
+        else:
+            current += self.terminal.move_left * (-cursor_delta_x)
+
+        if cursor_delta_y > 0:
+            current += self.terminal.move_down * cursor_delta_y
         else:
-            cursor_offset = self.cursor_offset
+            current += self.terminal.move_up * (-cursor_delta_y)
+        console_render._position += cursor_delta_y
 
-        return current + (self.terminal.move_left * cursor_offset)
-        # return self.current + (self.terminal.move_left * self.cursor_offset)
+        return current
 
     def process_input(self, pressed):
         if pressed == key.CTRL_C:
             raise KeyboardInterrupt()
 
         if pressed in (key.CR, key.LF, key.ENTER):
             raise errors.EndOfInput(self.current)
```

### Comparing `tons-0.0.49/tons/ui/interactive_cli/_sets/_keystore.py` & `tons-1.0.0/tons/ui/interactive_cli/_sets/_wallet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,297 +1,406 @@
+import decimal
 import os
 from collections import OrderedDict
+from copy import deepcopy
+from typing import OrderedDict as OrderedDictTyping
 
 import inquirer
 
-from tons.tonclient.utils import Whitelist, KeyStoreInvalidPasswordError
-from tons.tonsdk.contract.wallet import SendModeEnum, WalletVersionEnum, Wallets
+from tons.tonclient._client._base import AddressState
+from tons.tonsdk.contract.wallet import SendModeEnum, Wallets, WalletVersionEnum, WalletContract
+from tons.tonsdk.crypto._payload_encryption import encrypt_message
 from tons.tonsdk.utils import Address
+from tons.ui._utils import SharedObject, form_wallets_table
+from tons.ui.interactive_cli._sets._mixin import KeyStoreMixin
 from tons.utils import storage
-from ._base import BaseSet
-from .._modified_inquirer import TempText, ModifiedConfirm, RemovePrevAfterEnter
-from .._utils import echo_success, echo_error
-from .._validators import number_bigger_than_zero, valid_mnemonics, ignore_if_transfer_all
-from ..._utils import SharedObject, md_table, form_wallets_table
+from ._base import BaseSet, MenuItem
+from .._exceptions import InvalidBatchPattern
+from .._modified_inquirer import TempText, ModifiedConfirm, RemovePrevAfterEnter, ListWithFilter, terminal
+from .._utils import processing, echo_success, echo_error
+from .._validators import ignore_if_transfer_all, number_greater_than_or_equal_to_zero, non_empty_string, valid_mnemonics, \
+    integer_greater_than_zero
 
 
-class KeystoreSet(BaseSet):
-    def __init__(self, ctx: SharedObject, keystore_name: str) -> None:
+class WalletSet(BaseSet, KeyStoreMixin):
+    def __init__(self, ctx: SharedObject) -> None:
         super().__init__(ctx)
-        ctx.keystore = ctx.keystores.get_keystore(
-            keystore_name, raise_none=True)
-        ctx.whitelist = Whitelist(
-            ctx.config.tons.whitelist_path)
+        self._menu_message = f"Pick Wallet command [{self.ctx.keystore.name}]"
 
-    def _handlers(self) -> OrderedDict:
+    def _handlers(self) -> OrderedDictTyping[str, MenuItem]:
         ord_dict = OrderedDict()
-        ord_dict["List wallets"] = self._handle_list_wallets
-        ord_dict["Transfer"] = self._handle_transfer
-        ord_dict["Create wallet"] = self._handle_create_wallet
-        ord_dict["Init wallet"] = self._handle_init_wallet
-        ord_dict["Get wallet"] = self._handle_get_wallet
-        ord_dict["Edit wallet"] = self._handle_edit_wallet
-        ord_dict["Delete wallet"] = self._handle_delete_wallet
-        ord_dict["Reveal wallet mnemonics"] = self._handle_reveal_wallet_mnemonics
-        ord_dict["Import from mnemonics"] = self._handle_import_from_mnemonics
-        ord_dict["Wallet to .addr and .pk"] = self._handle_wallet_to_addr_pk
-        ord_dict["Backup keystore"] = self._handle_backup_keystore
-        ord_dict["Back"] = self._handle_exit
+        ord_dict[f"{terminal.underline}L{terminal.no_underline}ist"] = \
+            MenuItem(self._handle_list_wallets, "l")
+        ord_dict[f"{terminal.underline}T{terminal.no_underline}ransfer"] = \
+            MenuItem(self._handle_transfer, "t")
+        ord_dict[f"{terminal.underline}A{terminal.no_underline}dvanced Transfer"] = \
+            MenuItem(self._handle_advanced_transfer, "a")
+        ord_dict[f"{terminal.underline}C{terminal.no_underline}reate"] = \
+            MenuItem(self._handle_create_wallet, "c")
+        ord_dict[f"{terminal.underline}M{terminal.no_underline}ove"] = \
+            MenuItem(self._handle_move_wallet, "m")
+        ord_dict[f"{terminal.underline}I{terminal.no_underline}nit"] = \
+            MenuItem(self._handle_init_wallet, "i")
+        ord_dict[f"{terminal.underline}G{terminal.no_underline}et"] = \
+            MenuItem(self._handle_get_wallet, "g")
+        ord_dict[f"{terminal.underline}E{terminal.no_underline}dit"] = \
+            MenuItem(self._handle_edit_wallet, "e")
+        ord_dict[f"{terminal.underline}D{terminal.no_underline}elete"] = \
+            MenuItem(self._handle_delete_wallet, "d")
+        ord_dict[f"{terminal.underline}R{terminal.no_underline}eveal mnemonics"] = \
+            MenuItem(self._handle_reveal_wallet_mnemonics, "r")
+        ord_dict[f"{terminal.underline}F{terminal.no_underline}rom mnemonics"] = \
+            MenuItem(self._handle_import_from_mnemonics, "f")
+        ord_dict[f"T{terminal.underline}o{terminal.no_underline} .addr and .pk"] = \
+            MenuItem(self._handle_wallet_to_addr_pk, "o")
+        ord_dict[f"{terminal.underline}B{terminal.no_underline}ack"] = \
+            MenuItem(self._handle_exit, "b")
+
         return ord_dict
 
     def _handle_list_wallets(self):
         questions = [
             ModifiedConfirm(
                 "verbose", message='Show verbose information?', default=True),
         ]
         verbose = self._prompt(questions)["verbose"]
 
-        with self._processing():
-            wallets = self.ctx.keystore.records
+        with processing():
             wallet_infos = None
+            records = self.ctx.keystore.get_records(self.ctx.config.tons.sort_keystore)
             if verbose:
                 wallet_infos = self.ctx.ton_client.get_addresses_information(
-                    [wallet.address for wallet in wallets])
-
-            table = form_wallets_table(wallets, verbose, wallet_infos, True)
+                    [record.address for record in records])
+            table = form_wallets_table(records, verbose, wallet_infos, True)
 
-        echo_success(table.get_string(), only_msg=True)
+        echo_success(table, only_msg=True)
 
     def _handle_transfer(self):
-        from_wallet = self.__select_wallet_or_false("Transfer from")
-        if not from_wallet:
+        self.__handle_transfer(is_simple=True)
+
+    def _handle_advanced_transfer(self):
+        self.__handle_transfer(is_simple=False)
+
+    def __handle_transfer(self, is_simple):
+        from_wallet = self.select_wallet("Transfer from", verbose=True)
+        if from_wallet is None:
             return
 
         record = self.ctx.keystore.get_record_by_name(
             from_wallet, raise_none=True)
 
-        to_contact = self.__select_contact_or_false("Send to")
-        if not to_contact:
+        contact = self.select_contact("Send to", show_balance=True)
+        if contact is None:
             return
 
-        contact = self.ctx.whitelist.get_contact(to_contact, raise_none=True)
-
-        with self._processing():
+        with processing():
             contact_info = self.ctx.ton_client.get_address_information(contact.address)
-        bounceable = True
-        if contact_info.state != "Active":
-            bounceable = False
+
+        if contact_info.state != AddressState.active:
             is_sure = self._prompt([
                 ModifiedConfirm(
-                    "is_sure", message="Sending to not an active address. Send anyway?", default=False),
+                    "is_sure", message="Sending to not active address. Send anyway?", default=False),
             ])["is_sure"]
             if not is_sure:
                 echo_success("Action canceled.")
                 return
 
         questions = [
             ModifiedConfirm("transfer_all", message='Transfer all remaining coins?',
-                            default=False),
+                            default=False, ignore=is_simple),
             inquirer.Text("amount", message='Amount in TON coins to transfer',
                           ignore=ignore_if_transfer_all,
-                          validate=number_bigger_than_zero),
+                          validate=number_greater_than_or_equal_to_zero),
             ModifiedConfirm(
-                "destroy_if_zero", message='Destroy if balance becomes zero?', default=False),
+                "destroy_if_zero", message='Destroy if balance becomes zero?',
+                default=False, ignore=is_simple),
             inquirer.Text(
-                "message", message='Message (press \'Enter\' to skip)'),
+                "message", message='Message (press \'Enter\' to skip)', default=contact.default_message),
+            ModifiedConfirm("encrypt_payload", message='Encrypt payload?',
+                            default=False, ignore=is_simple or (not contact_info.can_receive_encrypted_payload)
+            ),
             ModifiedConfirm(
                 "wait_for_result", message="Wait until transaction will be completed?", default=True),
         ]
         ans = self._prompt(questions)
         transfer_all = ans["transfer_all"]
-        amount = 0 if transfer_all else float(ans["amount"])
+        amount = 0 if transfer_all else decimal.Decimal(ans["amount"])
         message = ans["message"]
         destroy_if_zero = ans["destroy_if_zero"]
         wait_for_result = ans["wait_for_result"]
+        encrypt_payload = ans["encrypt_payload"]
+
         send_mode = SendModeEnum.ignore_errors | SendModeEnum.pay_gas_separately
         if destroy_if_zero:
             send_mode |= SendModeEnum.destroy_account_if_zero
         if transfer_all:
             send_mode |= SendModeEnum.carry_all_remaining_balance
 
-        mnemonics = self.__get_mnemonics(record)
+        mnemonics = self.get_mnemonics(record)
 
-        with self._processing():
-            _mnemonics, _pub_k, _priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
+        with processing():
+            _mnemonics, pub_k, priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
                                                                          record.workchain,
                                                                          record.subwallet_id)
 
-            result = self.ctx.ton_client.transfer(
-                wallet, contact.address, amount, message, send_mode, bounceable, wait_for_result)
+            if encrypt_payload:
+                if not contact_info.can_receive_encrypted_payload:
+                    echo_error(f"Contact cannot receive encrypted messages")
+                    return
+
+                message = encrypt_message(message, pub_k, contact_info.public_key, priv_k, wallet.address)
+
+            task_id = self.ctx.background_task_manager.transfer_task(from_wallet=wallet,
+                                                                     to_addr=contact.address,
+                                                                     amount=amount,
+                                                                     payload=message,
+                                                                     send_mode=send_mode
+                                                                     )
+        if not wait_for_result:
+            echo_success('Task has been added to the queue.')
+            return
 
-        echo_success(str(result))
+        self._wait_for_result_and_echo(task_id)
 
     def _handle_create_wallet(self):
         questions = [
             inquirer.List(
-                "single", message="Choose option", choices=["Single", "Batch"],
+                "is_single", message="Choose option", choices=["Single", "Batch"],
                 carousel=True),
             inquirer.List(
                 "version", message='Wallet version', choices=[e.value for e in WalletVersionEnum],
                 carousel=True, default=self.ctx.config.tons.default_wallet_version),
             inquirer.Text(
                 "workchain", message='Workchain', default="0"),
         ]
         ans = self._prompt(questions)
-        is_single = ans["single"] == "Single"
+        is_single = ans["is_single"] == "Single"
         version = WalletVersionEnum(ans["version"])
         workchain = int(ans["workchain"])
 
         if is_single:
             questions = [
-                inquirer.Text("name", message='Wallet name'),
+                inquirer.Text("name", message='Wallet name', validate=non_empty_string),
                 inquirer.Text(
                     "comment", message='Wallet description (leave blank to skip)'),
             ]
             ans = self._prompt(questions)
             name = ans["name"]
             comment = ans["comment"]
-            questions = [
-                inquirer.Text(
-                    "contact_name", message='Enter name to save to whitelist (blank to skip)',
-                    default=name),
-            ]
-            contact_name = self._prompt(questions)["contact_name"]
-
-            wallets_to_create = [(name, comment, contact_name)]
+            wallets_to_create = [(name, comment)]
 
         else:
-            questions = [
-                inquirer.Text("number_of_wallets",
-                              message="Number of wallets to create"),
-                inquirer.Text(
-                    "prefix", message='Wallet name prefix (e.g. employee)'),
-                inquirer.Text(
-                    "comment", message='Overall wallets description (leave blank to skip)'),
-                ModifiedConfirm(
-                    "add_all_to_whitelist", message='Add all wallets to whitelist?', default=True),
-            ]
-            ans = self._prompt(questions)
-            number_of_wallets = int(ans["number_of_wallets"])
-            prefix = ans["prefix"] + "_"
-            comment = ans["comment"]
-            add_all_to_whitelist = ans["add_all_to_whitelist"]
-
-            num_of_existing = sum(record.name.startswith(prefix)
-                                  for record in self.ctx.keystore.records)
-            existing_leading_zeros = len(str(num_of_existing))
-            new_leading_zeros = len(str(number_of_wallets + num_of_existing))
-
-            if new_leading_zeros != existing_leading_zeros:
-                zeros_dif = new_leading_zeros - existing_leading_zeros
-                replace_with = "_" + ("0" * zeros_dif)
-                for record in self.ctx.keystore.records:
-                    if record.name.startswith(prefix):
-                        record.name = record.name.replace("_", replace_with)
-                for contact in self.ctx.whitelist.contacts:
-                    if contact.name.startswith(prefix):
-                        contact.name = contact.name.replace("_", replace_with)
+            batch_type = self._prompt([
+                inquirer.List(
+                    "batch_type", message="Batch type",
+                    choices=["Number of wallets by prefix",
+                             "Pattern (e.g. 'My Brand [001..087] Wallet')"],
+                    carousel=True),
+            ])["batch_type"]
 
             wallets_to_create = []
-            i = 1
-            while len(wallets_to_create) < number_of_wallets:
-                wallet_name_unique = False
-                new_name = None
-                contact_name = ""
-                while not wallet_name_unique:
-                    new_name = f"{prefix}{str(i).zfill(new_leading_zeros)}"
-                    i += 1
-                    if add_all_to_whitelist:
-                        contact_name = new_name
-                        if self.ctx.whitelist.get_contact(contact_name) is not None:
+
+            if batch_type == "Pattern (e.g. 'My Brand [001..087] Wallet')":
+                questions = [
+                    inquirer.Text(
+                        "pattern", message="Pattern"),
+                    inquirer.Text(
+                        "comment", message='Overall wallets description (leave blank to skip)'),
+                ]
+                ans = self._prompt(questions)
+                pattern = ans["pattern"]
+                comment = ans["comment"]
+
+                splitted = pattern.split("[")
+                if len(splitted) != 2:
+                    raise InvalidBatchPattern("Invalid pattern. It must include only one '[' bracket")
+
+                right_splitted = splitted[1].split("]")
+                if len(splitted[0].split("]")) != 1 or len(right_splitted) != 2:
+                    raise InvalidBatchPattern("Invalid pattern. It must include only one ']' bracket")
+
+                pattern_range = right_splitted[0]
+                range_idxes = pattern_range.split("..")
+                if len(range_idxes) != 2:
+                    raise InvalidBatchPattern("Invalid pattern. Wallets range support only X..Y format")
+
+                if len(range_idxes[0]) != len(range_idxes[1]):
+                    raise InvalidBatchPattern("Invalid pattern. Dimensions of the X and Y must coincide")
+
+                x = int(range_idxes[0])
+                y = int(range_idxes[1])
+                dimension = len(range_idxes[0])
+                if y < x:
+                    raise InvalidBatchPattern("Invalid pattern. "
+                                              "Left value must be bigger than right value")
+                if x <= 0:
+                    raise InvalidBatchPattern("Invalid pattern. "
+                                              "Left value must be bigger than 0")
+
+                name_left_part = splitted[0]
+                name_right_part = right_splitted[1]
+
+                for num in range(x, y + 1):
+                    number = str(num).zfill(dimension)
+                    wallets_to_create.append((f"{name_left_part}{number}{name_right_part}", comment))
+
+            else:
+                questions = [
+                    inquirer.Text("number_of_wallets",
+                                  message="Number of wallets to create",
+                                  validate=integer_greater_than_zero),
+                    inquirer.Text(
+                        "prefix", message='Wallet name prefix (e.g. employee_)'),
+                    inquirer.Text(
+                        "comment", message='Overall wallets description (leave blank to skip)'),
+                ]
+                ans = self._prompt(questions)
+                number_of_wallets = int(ans["number_of_wallets"])
+                prefix = ans["prefix"]
+                comment = ans["comment"]
+
+                for record in self.ctx.keystore.get_records(self.ctx.config.tons.sort_keystore):
+                    if record.name.startswith(prefix):
+                        name = record.name[len(prefix):]
+                        try:
+                            int(name)
+                            echo_error(f"Wallets with the prefix '{prefix}' already exist")
+                            return
+
+                        except ValueError:
+                            pass
+                leading_zeros = len(str(number_of_wallets))
+                i = 1
+                while len(wallets_to_create) < number_of_wallets:
+                    wallet_name_unique = False
+                    new_name = None
+                    while not wallet_name_unique:
+                        new_name = f"{prefix}{str(i).zfill(leading_zeros)}"
+                        i += 1
+                        if self.ctx.keystore.get_record_by_name(new_name) is not None:
                             continue
-                    if self.ctx.keystore.get_record_by_name(new_name) is not None:
-                        continue
-                    wallet_name_unique = True
-
-                wallets_to_create.append(
-                    (new_name, comment, contact_name))
-
-        with self._processing():
-            records_before = self.ctx.keystore.records
-            contacts_before = self.ctx.whitelist.contacts
-            try:
-                for wallet_name, comment, contact_name in wallets_to_create:
-                    if contact_name:
-                        contact = self.ctx.whitelist.get_contact(contact_name)
-                        if contact is not None:
-                            raise Exception(
-                                f"Contact with the name '{contact_name}' already exists")
-
-                    mnemonics, pub_k, _priv_k, wallet = Wallets.create(
-                        version, workchain)
-                    self.ctx.keystore.add_record(wallet_name, wallet.address,
-                                                 pub_k.hex(), mnemonics, version,
-                                                 workchain, None, comment, save=False)
-
-                    if contact_name:
-                        self.ctx.whitelist.add_contact(
-                            contact_name, wallet.address.to_string(True), save=False)
+                        wallet_name_unique = True
+
+                    wallets_to_create.append((new_name, comment))
 
+        if not is_single:
+            msg = f"Create '{wallets_to_create[0][0]}'-'{wallets_to_create[-1][0]}' wallets?"
+            is_sure = self._prompt([
+                ModifiedConfirm(
+                    "is_sure", message=msg,
+                    default=True), ])["is_sure"]
+            if not is_sure:
+                echo_success("Action canceled.")
+                return
+
+        with processing():
+            records_before = deepcopy(self.ctx.keystore._records)
+            subwallet_id = WalletContract.default_subwallet_id(workchain, version)
+            try:
+                for wallet_name, comment in wallets_to_create:
+                    mnemonics, _, _, _ = Wallets.create(version, workchain, subwallet_id)
+                    self.ctx.keystore.add_new_record(wallet_name, mnemonics, version,
+                                                     workchain, subwallet_id, comment, save=False)
                 self.ctx.keystore.save()
             except Exception:
                 # error during add or keystore save. No files have been changed. Only in-memory.
-                self.ctx.keystore.records = records_before
-                self.ctx.whitelist.contacts = contacts_before
+                self.ctx.keystore._records = records_before
                 raise
 
-            else:
-                # keystore has been saved successfully. whitelist has new records in-memory.
-                try:
-                    self.ctx.whitelist.save()
-                except Exception:
-                    # error during whitelist save. Change its in-memory contacts
-                    # and re-save keystore with old records
-                    self.ctx.whitelist.contacts = contacts_before
-                    self.ctx.keystore.records = records_before
-                    self.ctx.keystore.save()
-                    raise
+        echo_success()
+
+    def _handle_move_wallet(self):
+        wallet_name = self.select_wallet("Move wallet")
+        if wallet_name is None:
+            return
+        record = self.ctx.keystore.get_record_by_name(wallet_name, raise_none=True)
+
+        choose_from = [keystore_name for keystore_name in self.ctx.keystores.keystore_paths.keys()
+                       if keystore_name != self.ctx.keystore.name]
+
+        questions = [
+            ListWithFilter(
+                "move_to",
+                message="Move to",
+                choices=choose_from,
+                carousel=True
+            ),
+            ModifiedConfirm(
+                "remove_old", message="Remove wallet from the current keystore?", default=False),
+        ]
+        ans = self._prompt(questions)
+        move_to = ans["move_to"]
+        remove_old = ans["remove_old"]
+
+        keystore_to_move_in = self.ctx.keystores.get_keystore(move_to,
+                                                              raise_none=True)
+        self.unlock_keystore(keystore_to_move_in)
+        mnemonics = self.get_mnemonics(record)
+        keystore_to_move_in.add_new_record(record.name, mnemonics, record.version, record.workchain,
+                                           record.subwallet_id, record.comment, save=True)
+
+        if remove_old:
+            self.ctx.keystore.delete_record(record.name, save=True)
 
         echo_success()
 
     def _handle_init_wallet(self):
-        wallet_name_to_init = self.__select_wallet_or_false("Wallet to init")
-        if wallet_name_to_init == False:
+        wallet_name_to_init = self.select_wallet("Wallet to init")
+        if wallet_name_to_init is None:
             return
         questions = [
             ModifiedConfirm(
                 "wait_for_result", message="Wait until transaction will be completed?", default=True),
         ]
         ans = self._prompt(questions)
         wait_for_result = ans["wait_for_result"]
-        record = self.ctx.keystore.get_record_by_name(
-            wallet_name_to_init, raise_none=True)
-        mnemonics = self.__get_mnemonics(record)
+        record = self.ctx.keystore.get_record_by_name(wallet_name_to_init, raise_none=True)
+
+        with processing():
+            address_info = self.ctx.ton_client.get_address_information(record.address)
+
+        if address_info.state == AddressState.active:
+            echo_error("Wallet is already active.")
+            return
+        if address_info.balance < (init_amount := WalletContract.init_amount(record.version)):
+            echo_error(f"Insufficient amount, at least {init_amount} required.")
+            return
+
+        mnemonics = self.get_mnemonics(record)
         _mnemonics, _pub_k, _priv_k, wallet = Wallets.from_mnemonics(mnemonics, record.version,
                                                                      record.workchain,
                                                                      record.subwallet_id)
 
-        with self._processing():
-            result = self.ctx.ton_client.deploy_wallet(wallet, wait_for_result)
-        echo_success(str(result))
+        with processing():
+            task_id = self.ctx.background_task_manager.deploy_wallet_task(wallet)
+
+        if not wait_for_result:
+            echo_success("Transaction has been queued.")
+            return
+
+        self._wait_for_result_and_echo(task_id)
 
     def _handle_get_wallet(self):
-        wallet_name = self.__select_wallet_or_false("Get wallet")
-        if wallet_name == False:
+        wallet_name = self.select_wallet("Get wallet")
+        if wallet_name is None:
             return
 
-        wallet = self.ctx.keystore.get_record_by_name(
-            wallet_name, raise_none=True)
+        wallet = self.ctx.keystore.get_record_by_name(wallet_name, raise_none=True)
 
         questions = [
             ModifiedConfirm(
                 "verbose", message='Show balances?', default=True),
         ]
         verbose = self._prompt(questions)["verbose"]
 
         addr = Address(wallet.address)
 
         if verbose:
-            addr_info = self.ctx.ton_client.get_address_information(
-                wallet.address)
+            with processing():
+                addr_info = self.ctx.ton_client.get_address_information(wallet.address)
 
         echo_success(
             f"Raw address: {addr.to_string(False, False, False)}", True)
         echo_success(
             f"Nonbounceable address: {addr.to_string(True, True, False)}", True)
         echo_success(
             f"Bounceable address: {addr.to_string(True, True, True)}", True)
@@ -299,262 +408,130 @@
         echo_success(f"Workchain: {wallet.workchain}", True)
         echo_success(f"Subwallet id: {wallet.subwallet_id}", True)
         echo_success(f"Comment: {wallet.comment}", True)
 
         if verbose:
             echo_success("--- Verbose wallet information ---", True)
             for k, v in addr_info.dict().items():
+                if isinstance(v, AddressState):
+                    v = v.value
                 echo_success(str(k) + ': ' + str(v), True)
 
     def _handle_edit_wallet(self):
-        wallet_name = self.__select_wallet_or_false("Edit wallet")
-        if wallet_name == False:
+        wallet_name = self.select_wallet("Edit wallet")
+        if wallet_name is None:
             return
 
-        record = self.ctx.keystore.get_record_by_name(wallet_name)
-        contact = self.ctx.whitelist.get_contact_by_address(
-            Address(record.address).to_string(True, True, True))
-
         new_name = self._select_wallet_available_name(wallet_name)
+        if new_name is None:
+            return
+
         new_comment = self._prompt([
             inquirer.Text(
                 "new_comment", message='New wallet description (leave blank to skip)'),
         ])["new_comment"]
 
         self.ctx.keystore.edit_record(
             wallet_name, new_name, new_comment, save=True)
 
-        if new_name is not None and contact is not None:
-            want_to_edit = self._prompt([
-                ModifiedConfirm(
-                    "want_to_edit",
-                    message='Edit whitelist contact name with the same address?',
-                    default=True),
-            ])["want_to_edit"]
-
-            if want_to_edit:
-                new_contact_name = self._select_whitelist_available_name(contact.name, new_name)
-                if new_contact_name is not None:
-                    self.ctx.whitelist.edit_contact(contact.name, new_contact_name)
-
         echo_success()
 
     def _handle_delete_wallet(self):
-        questions = [
-            inquirer.List(
-                "single", message="Choose option", choices=["Single", "Batch"],
-                carousel=True),
-        ]
-        is_single = self._prompt(questions)["single"] == "Single"
-        if is_single:
-            wallet_name = self.__select_wallet_or_false("Delete wallet")
-            if wallet_name == False:
-                return
-            confirm_phrase = f'Are you sure you want to delete {wallet_name} wallet?'
-            names_to_delete = [wallet_name]
+        wallet_name = self.select_wallet("Delete wallet")
+        if wallet_name is None:
+            return
 
-        else:
-            questions = [
-                inquirer.Text(
-                    "prefix", message="Etner wallet prefix to delete (e.g. employee)"),
-            ]
-            prefix = self._prompt(questions)["prefix"] + "_"
-            confirm_phrase = f'Are you sure you want to delete all wallets with {prefix} prefix?'
-            names_to_delete = [
-                record.name for record in self.ctx.keystore.records if record.name.startswith(prefix)]
+        confirm_phrase = f'Are you sure you want to delete {wallet_name} wallet?'
+        names_to_delete = [wallet_name]
 
         is_sure = self._prompt([
             ModifiedConfirm(
                 "is_sure", message=confirm_phrase, default=False),
         ])["is_sure"]
         if not is_sure:
             echo_success("Action canceled.", True)
             return
 
-        delete_whitelist = self._prompt([
-            ModifiedConfirm(
-                "delete_whitelist",
-                message="Do you want to delete whitelist contacts with deleted wallets' addresses?",
-                default=True)
-        ])["delete_whitelist"]
-
-        records_before = self.ctx.keystore.records
-        contacts_before = self.ctx.whitelist.contacts
+        records_before = deepcopy(self.ctx.keystore._records)
         for name in names_to_delete:
-            deleted_record = self.ctx.keystore.delete_record(name, save=False)
-            if delete_whitelist:
-                contact = self.ctx.whitelist.get_contact_by_address(
-                    Address(deleted_record.address).to_string(True, True, True))
-                if contact is not None:
-                    self.ctx.whitelist.delete_contact(contact, save=False)
+            self.ctx.keystore.delete_record(name, save=False)
+
         try:
             self.ctx.keystore.save()
         except Exception:
-            self.ctx.keystore.records = records_before
-            if delete_whitelist:
-                self.ctx.whitelist.contacts = contacts_before
+            self.ctx.keystore._records = records_before
             raise
 
-        else:
-            try:
-                if delete_whitelist:
-                    self.ctx.whitelist.save()
-            except Exception:
-                self.ctx.keystore.records = records_before
-                self.ctx.keystore.save()
-                self.ctx.whitelist.contacts = contacts_before
-                raise
-
         echo_success()
 
     def _handle_reveal_wallet_mnemonics(self):
-        wallet_name = self.__select_wallet_or_false("Wallet to reveal")
-        if wallet_name == False:
+        wallet_name = self.select_wallet("Wallet to reveal")
+        if wallet_name is None:
             return
 
         record = self.ctx.keystore.get_record_by_name(
             wallet_name, raise_none=True)
-        mnemonics = self.__get_mnemonics(record)
+        mnemonics = self.get_mnemonics(record)
 
+        text_to_erase = ""
         for i in range(4):
-            echo_success(" ".join(mnemonics[i * 6:i * 6 + 6]), only_msg=True)
+            mnemonics_row = " ".join(mnemonics[i * 6:i * 6 + 6])
+            echo_success(mnemonics_row, only_msg=True)
+            text_to_erase += f"{mnemonics_row}\n"
 
         self._prompt([
-            RemovePrevAfterEnter("_", message="Press 'Enter' to remove mnemonics from the screen")
+            RemovePrevAfterEnter("_",
+                                 text_to_erase=text_to_erase,
+                                 message="Press 'Enter' to remove mnemonics from the screen")
         ])
 
     def _handle_import_from_mnemonics(self):
-        mnemonic = self._prompt([TempText("mnemonics", message="Mnemonic words (splited by space)",
-                                          validate=valid_mnemonics)])["mnemonics"].split(" ")
+        mnemonics = self._prompt([TempText("mnemonics", message="Mnemonic words (separated by spaces)",
+                                           validate=valid_mnemonics)])["mnemonics"].split(" ")
 
         questions = [
             inquirer.List(
                 "version", message='Wallet version', choices=[e.value for e in WalletVersionEnum],
                 carousel=True, default=self.ctx.config.tons.default_wallet_version),
             inquirer.Text(
                 "workchain", message='Workchain', default="0"),
             inquirer.Text("name", message='Wallet name')
         ]
         ans = self._prompt(questions)
         version = WalletVersionEnum(ans["version"])
         workchain = int(ans["workchain"])
-
-        mnemonics, pub_k, _priv_k, wallet = Wallets.from_mnemonics(
-            mnemonic, version, workchain)
-
-        name = self._prompt([inquirer.Text("name", message='Wallet name')])["name"]
+        name = ans["name"]
 
         questions = [
             inquirer.Text(
-                "comment", message='Wallet description (leave blank to skip)'),
-            inquirer.Text(
-                "contact_name", message='Enter name to save to whitelist (blank to skip)', default=name),
+                "comment", message='Wallet description (leave blank to skip)')
         ]
         ans = self._prompt(questions)
         comment = ans["comment"]
-        contact_name = ans["contact_name"]
-
-        if contact_name:
-            contact = self.ctx.whitelist.get_contact(contact_name)
-            if contact is not None:
-                raise Exception(
-                    f"Contact with the name '{contact_name}' already exists")
-
-        self.ctx.keystore.add_record(name, wallet.address,
-                                     pub_k.hex(), mnemonics, version,
-                                     workchain, None, comment, save=True)
-
-        if contact_name:
-            self.ctx.whitelist.add_contact(
-                contact_name, wallet.address.to_string(True), save=True)
+        subwallet_id = WalletContract.default_subwallet_id(workchain, version)
+        self.ctx.keystore.add_new_record(name, mnemonics, version,
+                                         workchain, subwallet_id, comment, save=True)
 
         echo_success()
 
     def _handle_wallet_to_addr_pk(self):
-        wallet_name = self.__select_wallet_or_false("Wallet to use")
-        if wallet_name == False:
+        wallet_name = self.select_wallet("Wallet to use")
+        if wallet_name is None:
             return
         questions = [
             inquirer.Text("destination_dir",
                           message='Directory path to export into'),
         ]
         ans = self._prompt(questions)
         destination_dir = ans["destination_dir"]
 
         record = self.ctx.keystore.get_record_by_name(
             wallet_name, raise_none=True)
-        mnemonics = self.__get_mnemonics(record)
+        mnemonics = self.get_mnemonics(record)
         addr, pk = Wallets.to_addr_pk(mnemonics, record.version,
                                       record.workchain, record.subwallet_id)
         addr_path = os.path.join(
             destination_dir, record.name + ".addr")
         pk_path = os.path.join(destination_dir, record.name + ".pk")
         storage.save_bytes(addr_path, addr)
         storage.save_bytes(pk_path, pk)
         echo_success()
-
-    def _handle_backup_keystore(self):
-        questions = [
-            inquirer.Text("backup_file_path", message='Backup filepath'),
-            ModifiedConfirm(
-                "is_sure",
-                message='Backup stores keys in UNENCRYPTED FORM. Are you sure want to export unencrypted keys to disk?',
-                default=False),
-            inquirer.Password("keystore_password",
-                              message='Keystore password'),
-        ]
-        ans = self._prompt(questions)
-        backup_file_path = ans["backup_file_path"]
-        keystore_password = ans["keystore_password"]
-        is_sure = ans["is_sure"]
-
-        if not is_sure:
-            echo_success("Action canceled.", True)
-            return
-
-        self.ctx.keystores.backup_keystore(self.ctx.keystore, backup_file_path, keystore_password)
-
-        echo_success()
-
-    def __select_wallet_or_false(self, message):
-        if self.ctx.keystore.records:
-            questions = [
-                inquirer.List(
-                    "wallet",
-                    message=message,
-                    choices=[record.name for record in self.ctx.keystore.records],
-                    carousel=True
-                )
-            ]
-            return self._prompt(questions)["wallet"]
-
-        echo_success("You do not have any wallets yet.")
-        return False
-
-    def __select_contact_or_false(self, message):
-        if self.ctx.whitelist.contacts:
-            questions = [
-                inquirer.List(
-                    "contact",
-                    message=message,
-                    choices=[
-                        record.name for record in self.ctx.whitelist.contacts],
-                    carousel=True
-                )
-            ]
-            return self._prompt(questions)["contact"]
-
-        echo_success("You do not have any contacts yet.")
-        return False
-
-    def __get_mnemonics(self, record):
-        while True:
-            questions = [
-                inquirer.Password("keystore_password", message='Keystore password'),
-            ]
-            keystore_password = self._prompt(questions)["keystore_password"]
-
-            try:
-                return self.ctx.keystore.get_secret(record, keystore_password).split(" ")
-            except KeyStoreInvalidPasswordError as e:
-                echo_error(str(e))
-                continue
```

### Comparing `tons-0.0.49/tons.egg-info/SOURCES.txt` & `tons-1.0.0/tons.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,83 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_settings.py
 tons/__init__.py
 tons/settings.py
 tons/version.py
 tons.egg-info/PKG-INFO
 tons.egg-info/SOURCES.txt
 tons.egg-info/dependency_links.txt
 tons.egg-info/entry_points.txt
 tons.egg-info/not-zip-safe
 tons.egg-info/requires.txt
 tons.egg-info/top_level.txt
 tons/config/__init__.py
 tons/config/_config.py
+tons/config/_dns.py
 tons/config/_exceptions.py
+tons/config/_jetton.py
 tons/config/_tons.py
 tons/config/_provider/__init__.py
 tons/config/_provider/_dapp.py
 tons/tonclient/__init__.py
 tons/tonclient/_exceptions.py
 tons/tonclient/_client/__init__.py
 tons/tonclient/_client/_base.py
 tons/tonclient/_client/_dapp/__init__.py
+tons/tonclient/_client/_dapp/_daemon.py
 tons/tonclient/_client/_dapp/_dapp.py
 tons/tonclient/_client/_dapp/_queries.py
 tons/tonclient/utils/__init__.py
 tons/tonclient/utils/_exceptions.py
 tons/tonclient/utils/_whitelist.py
 tons/tonclient/utils/_keystores/__init__.py
 tons/tonclient/utils/_keystores/_backup.py
-tons/tonclient/utils/_keystores/_keystore.py
+tons/tonclient/utils/_keystores/_crypto.py
 tons/tonclient/utils/_keystores/_record.py
+tons/tonclient/utils/_keystores/_keystore/__init__.py
+tons/tonclient/utils/_keystores/_keystore/_base.py
+tons/tonclient/utils/_keystores/_keystore/_password.py
+tons/tonclient/utils/_keystores/_keystore/_yubikey.py
+tons/tonclient/utils/_tonconnect/__init__.py
+tons/tonclient/utils/_tonconnect/_handlers.py
+tons/tonclient/utils/_tonconnect/_models.py
+tons/tonclient/utils/_tonconnect/_utils.py
 tons/tonsdk/__init__.py
 tons/tonsdk/_exceptions.py
 tons/tonsdk/boc/__init__.py
 tons/tonsdk/boc/_bit_string.py
+tons/tonsdk/boc/_builder.py
 tons/tonsdk/boc/_cell.py
+tons/tonsdk/boc/_dict_builder.py
+tons/tonsdk/boc/_slice.py
+tons/tonsdk/boc/dict/__init__.py
+tons/tonsdk/boc/dict/find_common_prefix.py
+tons/tonsdk/boc/dict/serialize_dict.py
 tons/tonsdk/contract/__init__.py
+tons/tonsdk/contract/token/__init__.py
+tons/tonsdk/contract/token/ft/__init__.py
+tons/tonsdk/contract/token/ft/jetton_minter.py
+tons/tonsdk/contract/token/ft/jetton_wallet.py
+tons/tonsdk/contract/token/nft/__init__.py
+tons/tonsdk/contract/token/nft/nft_collection.py
+tons/tonsdk/contract/token/nft/nft_item.py
+tons/tonsdk/contract/token/nft/nft_sale.py
+tons/tonsdk/contract/token/nft/nft_utils.py
 tons/tonsdk/contract/wallet/__init__.py
 tons/tonsdk/contract/wallet/_wallet_contract.py
 tons/tonsdk/contract/wallet/_wallet_contract_v2.py
 tons/tonsdk/contract/wallet/_wallet_contract_v3.py
 tons/tonsdk/contract/wallet/_wallet_contract_v4.py
 tons/tonsdk/crypto/__init__.py
-tons/tonsdk/crypto/_keystore.py
 tons/tonsdk/crypto/_mnemonic.py
+tons/tonsdk/crypto/_payload_encryption.py
 tons/tonsdk/crypto/_settings.py
 tons/tonsdk/crypto/_utils.py
 tons/tonsdk/crypto/exceptions.py
 tons/tonsdk/crypto/bip39/__init__.py
 tons/tonsdk/crypto/bip39/_english.py
 tons/tonsdk/provider/__init__.py
 tons/tonsdk/provider/_address.py
@@ -59,41 +86,62 @@
 tons/tonsdk/provider/dapp/__init__.py
 tons/tonsdk/provider/dapp/_client.py
 tons/tonsdk/utils/__init__.py
 tons/tonsdk/utils/_address.py
 tons/tonsdk/utils/_currency.py
 tons/tonsdk/utils/_exceptions.py
 tons/tonsdk/utils/_utils.py
+tons/tonsdk/utils/tonconnect/__init__.py
+tons/tonsdk/utils/tonconnect/_bridge.py
+tons/tonsdk/utils/tonconnect/_session.py
+tons/tonsdk/utils/tonconnect/requests_responses/__init__.py
+tons/tonsdk/utils/tonconnect/requests_responses/_app.py
+tons/tonsdk/utils/tonconnect/requests_responses/_common.py
+tons/tonsdk/utils/tonconnect/requests_responses/_wallet.py
 tons/ui/__init__.py
+tons/ui/_background.py
 tons/ui/_utils.py
 tons/ui/direct_cli/__init__.py
 tons/ui/direct_cli/_utils.py
 tons/ui/direct_cli/_commands/__init__.py
 tons/ui/direct_cli/_commands/_base_cmd.py
 tons/ui/direct_cli/_commands/_config_cmd.py
 tons/ui/direct_cli/_commands/_contract_cmd.py
 tons/ui/direct_cli/_commands/_dev_cmd.py
+tons/ui/direct_cli/_commands/_dns_cmd.py
 tons/ui/direct_cli/_commands/_keystore_cmd.py
+tons/ui/direct_cli/_commands/_tonconnect.py
 tons/ui/direct_cli/_commands/_wallet_cmd.py
 tons/ui/direct_cli/_commands/_whitelist_cmd.py
 tons/ui/gui/__init__.py
+tons/ui/gui/_sets/__init__.py
 tons/ui/interactive_cli/__init__.py
 tons/ui/interactive_cli/_exceptions.py
 tons/ui/interactive_cli/_utils.py
 tons/ui/interactive_cli/_validators.py
 tons/ui/interactive_cli/_modified_inquirer/__init__.py
 tons/ui/interactive_cli/_modified_inquirer/_confirm_render.py
+tons/ui/interactive_cli/_modified_inquirer/_list_with_filter_render.py
+tons/ui/interactive_cli/_modified_inquirer/_menu_with_hotkeys.py
 tons/ui/interactive_cli/_modified_inquirer/_prompt.py
 tons/ui/interactive_cli/_modified_inquirer/_render.py
 tons/ui/interactive_cli/_modified_inquirer/_text_render.py
 tons/ui/interactive_cli/_modified_inquirer/_theme.py
+tons/ui/interactive_cli/_modified_inquirer/_utils.py
 tons/ui/interactive_cli/_sets/__init__.py
 tons/ui/interactive_cli/_sets/_base.py
 tons/ui/interactive_cli/_sets/_config.py
+tons/ui/interactive_cli/_sets/_config_advanced.py
+tons/ui/interactive_cli/_sets/_dns.py
 tons/ui/interactive_cli/_sets/_entrypoint.py
+tons/ui/interactive_cli/_sets/_jetton.py
 tons/ui/interactive_cli/_sets/_keystore.py
 tons/ui/interactive_cli/_sets/_keystores.py
+tons/ui/interactive_cli/_sets/_mixin.py
+tons/ui/interactive_cli/_sets/_tonconnect.py
+tons/ui/interactive_cli/_sets/_wallet.py
 tons/ui/interactive_cli/_sets/_whitelist.py
 tons/utils/__init__.py
 tons/utils/exceptions.py
+tons/utils/spinner.py
 tons/utils/storage.py
 tons/utils/versioning.py
```

