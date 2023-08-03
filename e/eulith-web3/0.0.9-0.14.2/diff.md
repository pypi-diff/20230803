# Comparing `tmp/eulith_web3-0.0.9.tar.gz` & `tmp/eulith_web3-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulith_web3-0.0.9.tar", last modified: Wed Dec 28 04:09:31 2022, max compression
+gzip compressed data, was "eulith_web3-0.14.2.tar", last modified: Thu Aug  3 15:31:21 2023, max compression
```

## Comparing `eulith_web3-0.0.9.tar` & `eulith_web3-0.14.2.tar`

### file list

```diff
@@ -1,26 +1,127 @@
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.614918 eulith_web3-0.0.9/
--rw-r--r--   0 kristian   (501) staff       (20)     1073 2022-10-20 18:39:39.000000 eulith_web3-0.0.9/LICENSE
--rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-28 04:09:31.614772 eulith_web3-0.0.9/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)       75 2022-12-11 23:44:03.000000 eulith_web3-0.0.9/README.md
--rw-r--r--   0 kristian   (501) staff       (20)      618 2022-12-28 04:09:22.000000 eulith_web3-0.0.9/pyproject.toml
--rw-r--r--   0 kristian   (501) staff       (20)       38 2022-12-28 04:09:31.614957 eulith_web3-0.0.9/setup.cfg
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.610431 eulith_web3-0.0.9/src/
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.613113 eulith_web3-0.0.9/src/eulith_web3/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2022-10-20 22:32:35.000000 eulith_web3-0.0.9/src/eulith_web3/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     4809 2022-10-20 22:32:35.000000 eulith_web3-0.0.9/src/eulith_web3/asn_dump.py
--rw-r--r--   0 kristian   (501) staff       (20)     5015 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/binding_generator.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.614426 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     5064 2022-12-09 21:02:11.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/i_e_r_c20.py
--rw-r--r--   0 kristian   (501) staff       (20)     5993 2022-12-23 23:27:12.000000 eulith_web3-0.0.9/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
--rw-r--r--   0 kristian   (501) staff       (20)     1732 2022-12-23 23:27:12.000000 eulith_web3-0.0.9/src/eulith_web3/erc20.py
--rw-r--r--   0 kristian   (501) staff       (20)    13056 2022-12-28 04:07:53.000000 eulith_web3-0.0.9/src/eulith_web3/eulith_web3.py
--rw-r--r--   0 kristian   (501) staff       (20)     2315 2022-11-05 20:26:56.000000 eulith_web3-0.0.9/src/eulith_web3/fireblocks.py
--rw-r--r--   0 kristian   (501) staff       (20)     2140 2022-11-05 20:26:56.000000 eulith_web3-0.0.9/src/eulith_web3/kms.py
--rw-r--r--   0 kristian   (501) staff       (20)     5131 2022-12-28 03:42:22.000000 eulith_web3-0.0.9/src/eulith_web3/signing.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2022-12-28 04:09:31.613846 eulith_web3-0.0.9/src/eulith_web3.egg-info/
--rw-r--r--   0 kristian   (501) staff       (20)      475 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)      603 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/SOURCES.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/dependency_links.txt
--rw-r--r--   0 kristian   (501) staff       (20)       79 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/requires.txt
--rw-r--r--   0 kristian   (501) staff       (20)       12 2022-12-28 04:09:31.000000 eulith_web3-0.0.9/src/eulith_web3.egg-info/top_level.txt
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.939554 eulith_web3-0.14.2/
+-rw-r--r--   0 kristian   (501) staff       (20)    19298 2023-05-10 17:26:21.000000 eulith_web3-0.14.2/LICENSE
+-rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:31:21.939405 eulith_web3-0.14.2/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)      483 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/README.md
+-rw-r--r--   0 kristian   (501) staff       (20)      670 2023-08-03 15:31:10.000000 eulith_web3-0.14.2/pyproject.toml
+-rw-r--r--   0 kristian   (501) staff       (20)       38 2023-08-03 15:31:21.939602 eulith_web3-0.14.2/setup.cfg
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.902918 eulith_web3-0.14.2/src/
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.911368 eulith_web3-0.14.2/src/eulith_web3/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2022-10-20 22:32:35.000000 eulith_web3-0.14.2/src/eulith_web3/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2598 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/ace.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5059 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/asn_dump.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11825 2023-08-03 01:10:39.000000 eulith_web3-0.14.2/src/eulith_web3/binding_generator.py
+-rw-r--r--   0 kristian   (501) staff       (20)      181 2023-05-11 20:44:47.000000 eulith_web3-0.14.2/src/eulith_web3/common.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.919855 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-20 01:40:58.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/__init__.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.920843 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4338 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_booster.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1868 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7615 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_reward_staking.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9343 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_rewards.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.923163 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24465 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24149 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    26614 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27226 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    26616 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27228 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15565 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py
+-rw-r--r--   0 kristian   (501) staff       (20)    28229 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.926415 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10030 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11100 2023-05-15 20:04:29.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_order_book.py
+-rw-r--r--   0 kristian   (501) staff       (20)    22721 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_position_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13989 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reader.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4360 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10396 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6133 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    55194 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11712 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10873 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5283 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c20.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8379 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10077 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9891 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10450 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6646 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24838 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_lending_pool.py
+-rw-r--r--   0 kristian   (501) staff       (20)    25872 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1686 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2772 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_payments.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1764 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_pool_initializer.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6227 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_swap_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24033 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.934523 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-06 22:33:30.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      166 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/approx_params.py
+-rw-r--r--   0 kristian   (501) staff       (20)      106 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/call3.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3166 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2871 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27755 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py
+-rw-r--r--   0 kristian   (501) staff       (20)    14201 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3251 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6688 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11760 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15386 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    69987 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7648 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1817 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2103 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18782 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2256 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11520 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2535 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18706 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2162 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18802 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py
+-rw-r--r--   0 kristian   (501) staff       (20)      108 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/multi_approval.py
+-rw-r--r--   0 kristian   (501) staff       (20)      148 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/swap_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      256 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/token_input.py
+-rw-r--r--   0 kristian   (501) staff       (20)      261 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/token_output.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.934913 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-26 00:24:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    78604 2023-08-03 01:10:39.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/i_safe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6358 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1478 2023-03-21 02:59:35.000000 eulith_web3-0.14.2/src/eulith_web3/curve.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3651 2023-05-15 20:04:29.000000 eulith_web3-0.14.2/src/eulith_web3/erc20.py
+-rw-r--r--   0 kristian   (501) staff       (20)    89891 2023-08-01 19:26:04.000000 eulith_web3-0.14.2/src/eulith_web3/eulith_web3.py
+-rw-r--r--   0 kristian   (501) staff       (20)      543 2023-05-15 21:44:45.000000 eulith_web3-0.14.2/src/eulith_web3/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2345 2023-05-10 03:38:33.000000 eulith_web3-0.14.2/src/eulith_web3/fireblocks.py
+-rw-r--r--   0 kristian   (501) staff       (20)    28892 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/gmx.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2127 2023-05-10 04:03:27.000000 eulith_web3-0.14.2/src/eulith_web3/kms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2305 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/ledger.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938031 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 03:38:33.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3935 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/account.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6647 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/comms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2325 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/constants.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3929 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5230 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/messages.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27686 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/objects.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11098 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/transactions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6807 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6961 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/pendle.py
+-rw-r--r--   0 kristian   (501) staff       (20)      935 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/requests.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938411 eulith_web3-0.14.2/src/eulith_web3/safe_utils/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 04:36:00.000000 eulith_web3-0.14.2/src/eulith_web3/safe_utils/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1512 2023-05-10 04:41:15.000000 eulith_web3-0.14.2/src/eulith_web3/safe_utils/transaction_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      500 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/signer.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7379 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/signing.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1207 2023-01-09 03:56:23.000000 eulith_web3-0.14.2/src/eulith_web3/swap.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4152 2023-06-03 21:04:08.000000 eulith_web3-0.14.2/src/eulith_web3/trezor.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6190 2023-06-26 18:01:37.000000 eulith_web3-0.14.2/src/eulith_web3/uniswap.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8055 2023-07-13 16:28:28.000000 eulith_web3-0.14.2/src/eulith_web3/websocket.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1511 2023-07-19 16:02:43.000000 eulith_web3-0.14.2/src/eulith_web3/whitelists.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.912217 eulith_web3-0.14.2/src/eulith_web3.egg-info/
+-rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)     5315 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      121 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/requires.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       29 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/top_level.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      244 2023-08-02 21:50:32.000000 eulith_web3-0.14.2/src/generate.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5922 2023-08-03 00:54:36.000000 eulith_web3-0.14.2/src/scratch.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938675 eulith_web3-0.14.2/tests/
+-rw-r--r--   0 kristian   (501) staff       (20)     1573 2023-05-15 21:47:40.000000 eulith_web3-0.14.2/tests/test_guard.py
```

### Comparing `eulith_web3-0.0.9/pyproject.toml` & `eulith_web3-0.14.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 [build-system]
   build-backend = "setuptools.build_meta"
   requires = ["setuptools", "wheel"]
 
 [project]
   classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
-  dependencies = ["web3 >= 5.31.1", "boto3", "asn1", "uuid", "requests", "hexbytes", "cytoolz", "botocore", "fireblocks-sdk"]
+  dependencies = ["web3 >= 5.31.1", "boto3", "asn1", "uuid", "requests", "hexbytes", "cytoolz", "botocore", "fireblocks-sdk", "websocket-client", "ledgerblue", "eulith-trezor"]
   description = "A Web3.py compatible wrapper library for Eulith clients"
   name = "eulith_web3"
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.9"
+  version = "0.14.2"
 
   [[project.authors]]
     email = "kristian@eulith.com"
     name = "Eulith Team"
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/asn_dump.py` & `eulith_web3-0.14.2/src/eulith_web3/asn_dump.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 from builtins import open, bytes, str
 import sys
 import base64
 import binascii
 
 import asn1
-import optparse
 
 
 def read_pem(input_file):
-    """Read PEM formatted input."""
+    """
+    Reads PEM formatted input like private keys and public keys used for SSL/TLS encryption, and X.509/SSL certificates.
+    original file can be found here: https://github.com/andrivet/python-asn1/blob/master/examples/dump.py
+    """
+
     data = []
     state = 0
     for line in input_file:
         if state == 0:
             if line.startswith('-----BEGIN'):
                 state = 1
         elif state == 1:
@@ -34,14 +37,15 @@
             break
     if state != 2:
         raise ValueError('No PEM encoded input found')
     data = ''.join(data)
     return base64.b64decode(data)
 
 
+# maps ASN.1 tag IDs to string names to convert between abstract syntax notation 1
 tag_id_to_string_map = {
     asn1.Numbers.Boolean: "BOOLEAN",
     asn1.Numbers.Integer: "INTEGER",
     asn1.Numbers.BitString: "BIT STRING",
     asn1.Numbers.OctetString: "OCTET STRING",
     asn1.Numbers.Null: "NULL",
     asn1.Numbers.ObjectIdentifier: "OBJECT",
@@ -50,21 +54,23 @@
     asn1.Numbers.UTCTime: "UTCTIME",
     asn1.Numbers.GeneralizedTime: "GENERALIZED TIME",
     asn1.Numbers.Enumerated: "ENUMERATED",
     asn1.Numbers.Sequence: "SEQUENCE",
     asn1.Numbers.Set: "SET"
 }
 
+# maps ASN.1 class IDs to string names
 class_id_to_string_map = {
     asn1.Classes.Universal: "U",
     asn1.Classes.Application: "A",
     asn1.Classes.Context: "C",
     asn1.Classes.Private: "P"
 }
 
+# maps object IDs to string names
 object_id_to_string_map = {
     "1.2.840.113549.1.1.1": "rsaEncryption",
     "1.2.840.113549.1.1.5": "sha1WithRSAEncryption",
 
     "1.3.6.1.5.5.7.1.1": "authorityInfoAccess",
 
     "2.5.4.3": "commonName",
@@ -95,22 +101,20 @@
     "2.5.29.35": "X509v3 Authority Key Identifier",
     "2.5.29.36": "X509v3 Policy Constraints",
     "2.5.29.37": "X509v3 Extended Key Usage"
 }
 
 
 def tag_id_to_string(identifier):
-    """Return a string representation of a ASN.1 id."""
     if identifier in tag_id_to_string_map:
         return tag_id_to_string_map[identifier]
     return '{:#02x}'.format(identifier)
 
 
 def class_id_to_string(identifier):
-    """Return a string representation of an ASN.1 class."""
     if identifier in class_id_to_string_map:
         return class_id_to_string_map[identifier]
     raise ValueError('Illegal class: {:#02x}'.format(identifier))
 
 
 def object_identifier_to_string(identifier):
     if identifier in object_id_to_string_map:
@@ -125,21 +129,21 @@
         return '0x' + str(binascii.hexlify(value).upper())
     elif isinstance(value, str):
         return value
     else:
         return repr(value)
 
 
-def pretty_print(input_stream, output_stream = sys.stdout, indent=0):
-    """Pretty print ASN.1 data."""
+def pretty_print(input_stream, output_stream=sys.stdout, indent=0):
     while not input_stream.eof():
         tag = input_stream.peek()
         if tag.typ == asn1.Types.Primitive:
             tag, value = input_stream.read()
             output_stream.write(' ' * indent)
-            output_stream.write('[{}] {}: {}\n'.format(class_id_to_string(tag.cls), tag_id_to_string(tag.nr), value_to_string(tag.nr, value)))
+            output_stream.write('[{}] {}: {}\n'.format(class_id_to_string(tag.cls), tag_id_to_string(tag.nr),
+                                                       value_to_string(tag.nr, value)))
         elif tag.typ == asn1.Types.Constructed:
             output_stream.write(' ' * indent)
             output_stream.write('[{}] {}\n'.format(class_id_to_string(tag.cls), tag_id_to_string(tag.nr)))
             input_stream.enter()
             pretty_print(input_stream, output_stream, indent + 2)
             input_stream.leave()
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/contract_bindings/i_e_r_c20.py` & `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c20.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
         return c.functions.allowance(owner, spender).call()
 
-    def approve(self, spender: str, amount: int) -> TxParams:
+    def approve(self, spender: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.approve(spender, amount).build_transaction()
+        return c.functions.approve(spender, amount).build_transaction(override_tx_parameters)
 
     def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
         return c.functions.balanceOf(account).call()
@@ -45,20 +45,20 @@
     def total_supply(self) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
         return c.functions.totalSupply().call()
 
-    def transfer(self, to: str, amount: int) -> TxParams:
+    def transfer(self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.transfer(to, amount).build_transaction()
+        return c.functions.transfer(to, amount).build_transaction(override_tx_parameters)
 
-    def transfer_from(self, _from: str, to: str, amount: int) -> TxParams:
+    def transfer_from(self, _from: str, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.transferFrom(_from, to, amount).build_transaction()
+        return c.functions.transferFrom(_from, to, amount).build_transaction(override_tx_parameters)
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/contract_bindings/w_e_t_h_interface.py` & `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Optional, Union
 from eth_typing import Address, ChecksumAddress
-from web3 import Web3
 from web3.types import TxParams
+from web3 import Web3
 
 
 class ContractAddressNotSet(Exception):
     pass
 
 
-class WETHInterface:
+class IERCDetailed:
     def __init__(self, web3: Web3, contract_address: Optional[Union[Address, ChecksumAddress]] = None):
         self.address: Optional[Union[Address, ChecksumAddress]] = contract_address
-        self.abi = [{'anonymous': False, 'inputs': [{'indexed': True, 'internalType': 'address', 'name': 'owner', 'type': 'address'}, {'indexed': True, 'internalType': 'address', 'name': 'spender', 'type': 'address'}, {'indexed': False, 'internalType': 'uint256', 'name': 'value', 'type': 'uint256'}], 'name': 'Approval', 'type': 'event'}, {'anonymous': False, 'inputs': [{'indexed': True, 'internalType': 'address', 'name': 'from', 'type': 'address'}, {'indexed': True, 'internalType': 'address', 'name': 'to', 'type': 'address'}, {'indexed': False, 'internalType': 'uint256', 'name': 'value', 'type': 'uint256'}], 'name': 'Transfer', 'type': 'event'}, {'inputs': [{'internalType': 'address', 'name': 'owner', 'type': 'address'}, {'internalType': 'address', 'name': 'spender', 'type': 'address'}], 'name': 'allowance', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'spender', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'approve', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'account', 'type': 'address'}], 'name': 'balanceOf', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [], 'name': 'deposit', 'outputs': [], 'stateMutability': 'payable', 'type': 'function'}, {'inputs': [], 'name': 'totalSupply', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'to', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'transfer', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'from', 'type': 'address'}, {'internalType': 'address', 'name': 'to', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'transferFrom', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}, {'inputs': [{'internalType': 'uint256', 'name': 'wad', 'type': 'uint256'}], 'name': 'withdraw', 'outputs': [], 'stateMutability': 'nonpayable', 'type': 'function'}]
+        self.abi = [{'anonymous': False, 'inputs': [{'indexed': True, 'internalType': 'address', 'name': 'owner', 'type': 'address'}, {'indexed': True, 'internalType': 'address', 'name': 'spender', 'type': 'address'}, {'indexed': False, 'internalType': 'uint256', 'name': 'value', 'type': 'uint256'}], 'name': 'Approval', 'type': 'event'}, {'anonymous': False, 'inputs': [{'indexed': True, 'internalType': 'address', 'name': 'from', 'type': 'address'}, {'indexed': True, 'internalType': 'address', 'name': 'to', 'type': 'address'}, {'indexed': False, 'internalType': 'uint256', 'name': 'value', 'type': 'uint256'}], 'name': 'Transfer', 'type': 'event'}, {'inputs': [{'internalType': 'address', 'name': 'owner', 'type': 'address'}, {'internalType': 'address', 'name': 'spender', 'type': 'address'}], 'name': 'allowance', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'spender', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'approve', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'account', 'type': 'address'}], 'name': 'balanceOf', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [], 'name': 'decimals', 'outputs': [{'internalType': 'uint8', 'name': '', 'type': 'uint8'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [], 'name': 'name', 'outputs': [{'internalType': 'string', 'name': '', 'type': 'string'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [], 'name': 'symbol', 'outputs': [{'internalType': 'string', 'name': '', 'type': 'string'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [], 'name': 'totalSupply', 'outputs': [{'internalType': 'uint256', 'name': '', 'type': 'uint256'}], 'stateMutability': 'view', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'to', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'transfer', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}, {'inputs': [{'internalType': 'address', 'name': 'from', 'type': 'address'}, {'internalType': 'address', 'name': 'to', 'type': 'address'}, {'internalType': 'uint256', 'name': 'amount', 'type': 'uint256'}], 'name': 'transferFrom', 'outputs': [{'internalType': 'bool', 'name': '', 'type': 'bool'}], 'stateMutability': 'nonpayable', 'type': 'function'}]
         self.bytecode = ''
         self.w3 = web3
             
     def deploy(self):
         contract = self.w3.eth.contract(abi=self.abi, bytecode=self.bytecode)
         tx_hash = contract.constructor().transact()
         tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
@@ -24,55 +24,62 @@
     def allowance(self, owner: str, spender: str) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
         return c.functions.allowance(owner, spender).call()
 
-    def approve(self, spender: str, amount: int) -> TxParams:
+    def approve(self, spender: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.approve(spender, amount).build_transaction()
+        return c.functions.approve(spender, amount).build_transaction(override_tx_parameters)
 
     def balance_of(self, account: str) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
         return c.functions.balanceOf(account).call()
 
-    def deposit(self) -> TxParams:
+    def decimals(self) -> int:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.deposit().build_transaction()
+        return c.functions.decimals().call()
 
-    def total_supply(self) -> int:
+    def name(self) -> str:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.totalSupply().call()
+        return c.functions.name().call()
 
-    def transfer(self, to: str, amount: int) -> TxParams:
+    def symbol(self) -> str:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.transfer(to, amount).build_transaction()
+        return c.functions.symbol().call()
+
+    def total_supply(self) -> int:
+        if not self.address:
+            raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
+        c = self.w3.eth.contract(address=self.address, abi=self.abi)
+                    
+        return c.functions.totalSupply().call()
 
-    def transfer_from(self, _from: str, to: str, amount: int) -> TxParams:
+    def transfer(self, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.transferFrom(_from, to, amount).build_transaction()
+        return c.functions.transfer(to, amount).build_transaction(override_tx_parameters)
 
-    def withdraw(self, wad: int) -> TxParams:
+    def transfer_from(self, _from: str, to: str, amount: int, override_tx_parameters: Optional[TxParams] = None) -> TxParams:
         if not self.address:
             raise ContractAddressNotSet("you must either deploy or initialize the contract with an address")
         c = self.w3.eth.contract(address=self.address, abi=self.abi)
                     
-        return c.functions.withdraw(wad).build_transaction()
+        return c.functions.transferFrom(_from, to, amount).build_transaction(override_tx_parameters)
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/fireblocks.py` & `eulith_web3-0.14.2/src/eulith_web3/fireblocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from eth_keys.backends import NativeECCBackend, BaseECCBackend
 from eth_keys.datatypes import PublicKey, Signature
 from eth_utils import big_endian_to_int
 from fireblocks_sdk import FireblocksSDK, RawMessage, UnsignedMessage
 
 from hexbytes import HexBytes
 
-from eulith_web3.signing import Signer, SigningException
+from eulith_web3.signing import SigningException
+from eulith_web3.signer import Signer
 
 logger = logging.getLogger(__name__)
 
 ALGO: str = 'MPC_ECDSA_SECP256K1'
 COMPRESSED: int = 0
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/kms.py` & `eulith_web3-0.14.2/src/eulith_web3/kms.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import Any
 
 import asn1
 from botocore.exceptions import ClientError
 from eth_keys.backends import BaseECCBackend, NativeECCBackend
 from eth_keys.datatypes import PublicKey
 
-from eulith_web3.signing import Signer, recover_v
+from eulith_web3.signing import recover_v
+from eulith_web3.signer import Signer
 from eth_keys.datatypes import Signature
 
 
 class KmsSigner(Signer):
     def __init__(self, kms_client: Any, key_id: str, backend: BaseECCBackend = NativeECCBackend):
         self.key_id = key_id
         self.client = kms_client
@@ -26,15 +27,15 @@
         pk_bytes = self.decode_pk(key['PublicKey'])
         self.public_address = PublicKey(pk_bytes, backend).to_checksum_address()
 
     @property
     def address(self):
         return self.public_address
 
-    def sign_msg_hash(self, message_hash: bytes) -> 'Signature':
+    def sign_msg_hash(self, message_hash: bytes) -> Signature:
         der_sig = self.client.sign(KeyId=self.key_id, Message=message_hash, MessageType="DIGEST",
                                    SigningAlgorithm="ECDSA_SHA_256")
         decoder = asn1.Decoder()
         decoder.start(der_sig['Signature'])
         decoder.enter()
         _, r = decoder.read()
         _, s = decoder.read()
@@ -55,10 +56,8 @@
     def decode_pk(pk_bytes) -> bytes:
         decoder = asn1.Decoder()
         decoder.start(pk_bytes)
         decoder.enter()
         decoder.enter()
         decoder.leave()
         tag, value = decoder.read()
-        pprint(tag)
-        pprint(value)
-        return value[1:]
+        return value[1:]
```

### Comparing `eulith_web3-0.0.9/src/eulith_web3/signing.py` & `eulith_web3-0.14.2/src/eulith_web3/signing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable, Mapping,
 )
-import logging
+
 from cytoolz import dissoc
-from eth_account._utils.signing import sign_transaction_dict
+from eth_account._utils.legacy_transactions import serializable_unsigned_transaction_from_dict, UnsignedTransaction, \
+    Transaction, encode_transaction
+from eth_account._utils.signing import sign_transaction_dict, to_eth_v
+from eth_account._utils.typed_transactions import TypedTransaction
 from eth_account.datastructures import SignedTransaction
 from eth_keys.backends import NativeECCBackend, BaseECCBackend
 from eth_keys.datatypes import PrivateKey, Signature
-from eth_utils import keccak
 from eth_utils.toolz import (
     compose,
 )
 from hexbytes import HexBytes
 from web3._utils.method_formatters import (
     STANDARD_NORMALIZERS,
 )
@@ -28,14 +31,16 @@
 from web3.types import (
     Middleware,
     RPCEndpoint,
     RPCResponse,
     TxParams,
 )
 
+from eulith_web3.signer import Signer
+
 if TYPE_CHECKING:
     from web3 import Web3  # noqa: F401
 
 logger = logging.getLogger(__name__)
 
 
 class SigningException(Exception):
@@ -47,27 +52,41 @@
 
     Converts bytes to hex strings and other types that can be passed to the underlying layers.
     Also has the effect of normalizing 'from' for easier comparisons.
     """
     return apply_abi_formatters_to_dict(STANDARD_NORMALIZERS, TRANSACTION_PARAMS_ABIS, transaction)
 
 
+def normalize_s(s: int) -> int:
+    """
+    Eth expects signatures in canonical form to avoid replay attacks.
+
+    :param s: Signature's s value
+    :return:  Normalized s value
+    """
+    n = 115792089237316195423570985008687907852837564279074904382605163141518161494337
+    if s > n // 2:
+        s = n - s
+    return s
+
+
 def recover_v(r: int, s: int, message_hash: bytes, address: str, backend: BaseECCBackend) -> Signature:
+    s = normalize_s(s)
     sig0 = Signature(vrs=(0, r, s), backend=backend)
     if sig0.recover_public_key_from_msg_hash(message_hash).to_checksum_address() == address:
         return sig0
     sig1 = Signature(vrs=(1, r, s), backend=backend)
     if sig1.recover_public_key_from_msg_hash(message_hash).to_checksum_address() == address:
         return sig1
     raise SigningException("Could not determine v")
 
 
 # signer has two functions: address, sign_msg_hash
 #    def sign_msg_hash(self, message_hash: bytes) -> 'Signature':
-def sign_transaction(transaction_dict, signer) -> SignedTransaction:
+def sign_transaction(transaction_dict, signer: Signer) -> SignedTransaction:
     if not isinstance(transaction_dict, Mapping):
         raise TypeError("transaction_dict must be dict-like, got %r" % transaction_dict)
 
     # allow from field, *only* if it matches the private key
     if 'from' in transaction_dict:
         if transaction_dict['from'] == signer.address:
             sanitized_transaction = dissoc(transaction_dict, 'from')
@@ -75,66 +94,84 @@
             raise TypeError("from field must match key's %s, but it was %s" % (
                 signer.address,
                 transaction_dict['from'],
             ))
     else:
         sanitized_transaction = transaction_dict
 
-    # sign transaction
     (
         v,
         r,
         s,
         encoded_transaction,
+        transaction_hash
     ) = sign_transaction_dict(signer, sanitized_transaction)
-    transaction_hash = keccak(encoded_transaction)
 
     return SignedTransaction(
         rawTransaction=HexBytes(encoded_transaction),
         hash=HexBytes(transaction_hash),
         r=r,
         s=s,
         v=v,
     )
 
 
-class Signer:
-    def address(self) -> str:
-        pass
+def sign_transaction_dict(eth_key: Signer, transaction_dict):
+    # generate RLP-serializable transaction, with defaults filled
+    unsigned_transaction = serializable_unsigned_transaction_from_dict(transaction_dict)
+    transaction_hash = unsigned_transaction.hash()
+
+    # detect chain
+    if isinstance(unsigned_transaction, UnsignedTransaction):
+        signature = eth_key.sign_transaction(unsigned_transaction, transaction_hash)
+        (v_raw, r, s) = signature.vrs
+        v = to_eth_v(v_raw, None)
+    elif isinstance(unsigned_transaction, Transaction):
+        chain_id = unsigned_transaction.v
+
+        signature = eth_key.sign_transaction(unsigned_transaction, transaction_hash)
+        (v_raw, r, s) = signature.vrs
+        v = to_eth_v(v_raw, chain_id)
+    elif isinstance(unsigned_transaction, TypedTransaction):
+        # Each transaction type dictates its payload, and consequently,
+        # all the funky logic around the `v` signature field is both obsolete &&
+        # incorrect. We want to obtain the raw `v` and delegate
+        # to the transaction type itself.
+        (v, r, s) = eth_key.sign_transaction(unsigned_transaction, transaction_hash).vrs
+    else:
+        # Cannot happen, but better for code to be defensive + self-documenting.
+        raise TypeError("unknown Transaction object: %s" % type(unsigned_transaction))
 
-    def sign_msg_hash(self, message_hash: bytes) -> 'Signature':
-        pass
+    # serialize transaction with rlp
+    encoded_transaction = encode_transaction(unsigned_transaction, vrs=(v, r, s))
+
+    return v, r, s, encoded_transaction, transaction_hash
 
 
 class LocalSigner(Signer):
     def __init__(self, private_key, backend: BaseECCBackend = NativeECCBackend):
         self.private_key = PrivateKey(HexBytes(private_key), backend)
         self.address = self.private_key.public_key.to_checksum_address()
 
     def address(self) -> str:
         return self.address
 
-    def sign_msg_hash(self, message_hash: bytes) -> 'Signature':
+    def sign_msg_hash(self, message_hash: bytes) -> Signature:
         return self.private_key.sign_msg_hash(message_hash)
 
 
-def construct_signing_middleware(
-        account: Signer
-) -> Middleware:
-    """Capture transactions sign and send as raw transactions
-
-
-    Keyword arguments:
-    private_key_or_account -- A single private key or a tuple,
-    list or set of private keys. Keys can be any of the following formats:
-      - An eth_account.LocalAccount object
-      - An eth_keys.PrivateKey object
-      - A raw private key as a hex string or byte string
+def construct_signing_middleware(account: Signer) -> Middleware:
     """
+    Wrap signature source in middleware to allow for automatic signing when necessary for transactions
+    being signed and sent directly to the network (as opposed to an atomic transaction, which gets sent
+    unsigned to the Eulith server).
 
+    :param account: The LocalSigner, KMSSigner, or FireblocksSigner for your wallet
+    :type account: Signer
+    """
     acct = account
 
     def sign_and_send_raw_middleware(
             make_request: Callable[[RPCEndpoint, Any], Any], w3: "Web3"
     ) -> Callable[[RPCEndpoint, Any], RPCResponse]:
         format_and_fill_tx = compose(
             format_transaction,
@@ -155,10 +192,22 @@
             raw_tx = sign_transaction(transaction, acct).rawTransaction
 
             return make_request(
                 RPCEndpoint("eth_sendRawTransaction"),
                 [raw_tx])
 
         return middleware
+
     smw = sign_and_send_raw_middleware
     smw.address = account.address
+    smw.signer = acct
+
     return smw
+
+
+def normalize_signature(signature: Signature) -> str:
+    """
+    Normalize the signature to a string, for instance for serialization for an RPC method.
+    """
+    compatible_v = signature.v + 27
+    last_two_chars = hex(compatible_v)[-2:]
+    return str(signature)[:-2] + last_two_chars
```

