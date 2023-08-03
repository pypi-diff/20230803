# Comparing `tmp/eulith_web3-0.14.2.tar.gz` & `tmp/eulith_web3-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulith_web3-0.14.2.tar", last modified: Thu Aug  3 15:31:21 2023, max compression
+gzip compressed data, was "eulith_web3-0.14.3.tar", last modified: Thu Aug  3 15:34:56 2023, max compression
```

## Comparing `eulith_web3-0.14.2.tar` & `eulith_web3-0.14.3.tar`

### file list

```diff
@@ -1,127 +1,125 @@
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.939554 eulith_web3-0.14.2/
--rw-r--r--   0 kristian   (501) staff       (20)    19298 2023-05-10 17:26:21.000000 eulith_web3-0.14.2/LICENSE
--rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:31:21.939405 eulith_web3-0.14.2/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)      483 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/README.md
--rw-r--r--   0 kristian   (501) staff       (20)      670 2023-08-03 15:31:10.000000 eulith_web3-0.14.2/pyproject.toml
--rw-r--r--   0 kristian   (501) staff       (20)       38 2023-08-03 15:31:21.939602 eulith_web3-0.14.2/setup.cfg
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.902918 eulith_web3-0.14.2/src/
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.911368 eulith_web3-0.14.2/src/eulith_web3/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2022-10-20 22:32:35.000000 eulith_web3-0.14.2/src/eulith_web3/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     2598 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/ace.py
--rw-r--r--   0 kristian   (501) staff       (20)     5059 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/asn_dump.py
--rw-r--r--   0 kristian   (501) staff       (20)    11825 2023-08-03 01:10:39.000000 eulith_web3-0.14.2/src/eulith_web3/binding_generator.py
--rw-r--r--   0 kristian   (501) staff       (20)      181 2023-05-11 20:44:47.000000 eulith_web3-0.14.2/src/eulith_web3/common.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.919855 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-20 01:40:58.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/__init__.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.920843 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     4338 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_booster.py
--rw-r--r--   0 kristian   (501) staff       (20)     1868 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
--rw-r--r--   0 kristian   (501) staff       (20)     7615 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_reward_staking.py
--rw-r--r--   0 kristian   (501) staff       (20)     9343 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_rewards.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.923163 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    24465 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py
--rw-r--r--   0 kristian   (501) staff       (20)    24149 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    26614 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py
--rw-r--r--   0 kristian   (501) staff       (20)    27226 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    26616 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py
--rw-r--r--   0 kristian   (501) staff       (20)    27228 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)    15565 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py
--rw-r--r--   0 kristian   (501) staff       (20)    28229 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.926415 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    10030 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)    11100 2023-05-15 20:04:29.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_order_book.py
--rw-r--r--   0 kristian   (501) staff       (20)    22721 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_position_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    13989 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reader.py
--rw-r--r--   0 kristian   (501) staff       (20)     4360 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    10396 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py
--rw-r--r--   0 kristian   (501) staff       (20)     6133 2023-04-02 23:46:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    55194 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault.py
--rw-r--r--   0 kristian   (501) staff       (20)    11712 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py
--rw-r--r--   0 kristian   (501) staff       (20)    10873 2023-03-30 16:24:00.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py
--rw-r--r--   0 kristian   (501) staff       (20)     5283 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c20.py
--rw-r--r--   0 kristian   (501) staff       (20)     8379 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721.py
--rw-r--r--   0 kristian   (501) staff       (20)    10077 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py
--rw-r--r--   0 kristian   (501) staff       (20)     9891 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py
--rw-r--r--   0 kristian   (501) staff       (20)    10450 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py
--rw-r--r--   0 kristian   (501) staff       (20)     6646 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
--rw-r--r--   0 kristian   (501) staff       (20)    24838 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_lending_pool.py
--rw-r--r--   0 kristian   (501) staff       (20)    25872 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)     1686 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py
--rw-r--r--   0 kristian   (501) staff       (20)     2772 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_payments.py
--rw-r--r--   0 kristian   (501) staff       (20)     1764 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_pool_initializer.py
--rw-r--r--   0 kristian   (501) staff       (20)     6227 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_swap_router.py
--rw-r--r--   0 kristian   (501) staff       (20)    24033 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.934523 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-06 22:33:30.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)      166 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/approx_params.py
--rw-r--r--   0 kristian   (501) staff       (20)      106 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/call3.py
--rw-r--r--   0 kristian   (501) staff       (20)     3166 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py
--rw-r--r--   0 kristian   (501) staff       (20)     2871 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py
--rw-r--r--   0 kristian   (501) staff       (20)    27755 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py
--rw-r--r--   0 kristian   (501) staff       (20)    14201 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py
--rw-r--r--   0 kristian   (501) staff       (20)     3251 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py
--rw-r--r--   0 kristian   (501) staff       (20)     6688 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py
--rw-r--r--   0 kristian   (501) staff       (20)    11760 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py
--rw-r--r--   0 kristian   (501) staff       (20)    15386 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py
--rw-r--r--   0 kristian   (501) staff       (20)    69987 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py
--rw-r--r--   0 kristian   (501) staff       (20)     7648 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py
--rw-r--r--   0 kristian   (501) staff       (20)     1817 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py
--rw-r--r--   0 kristian   (501) staff       (20)     2103 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py
--rw-r--r--   0 kristian   (501) staff       (20)    18782 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market.py
--rw-r--r--   0 kristian   (501) staff       (20)     2256 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py
--rw-r--r--   0 kristian   (501) staff       (20)    11520 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py
--rw-r--r--   0 kristian   (501) staff       (20)     2535 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py
--rw-r--r--   0 kristian   (501) staff       (20)    18706 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py
--rw-r--r--   0 kristian   (501) staff       (20)     2162 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py
--rw-r--r--   0 kristian   (501) staff       (20)    18802 2023-04-09 00:27:11.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py
--rw-r--r--   0 kristian   (501) staff       (20)      108 2023-04-07 03:16:15.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/multi_approval.py
--rw-r--r--   0 kristian   (501) staff       (20)      148 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/swap_data.py
--rw-r--r--   0 kristian   (501) staff       (20)      256 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/token_input.py
--rw-r--r--   0 kristian   (501) staff       (20)      261 2023-04-09 00:29:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/token_output.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.934913 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-26 00:24:28.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)    78604 2023-08-03 01:10:39.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/i_safe.py
--rw-r--r--   0 kristian   (501) staff       (20)     6358 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
--rw-r--r--   0 kristian   (501) staff       (20)     1478 2023-03-21 02:59:35.000000 eulith_web3-0.14.2/src/eulith_web3/curve.py
--rw-r--r--   0 kristian   (501) staff       (20)     3651 2023-05-15 20:04:29.000000 eulith_web3-0.14.2/src/eulith_web3/erc20.py
--rw-r--r--   0 kristian   (501) staff       (20)    89891 2023-08-01 19:26:04.000000 eulith_web3-0.14.2/src/eulith_web3/eulith_web3.py
--rw-r--r--   0 kristian   (501) staff       (20)      543 2023-05-15 21:44:45.000000 eulith_web3-0.14.2/src/eulith_web3/exceptions.py
--rw-r--r--   0 kristian   (501) staff       (20)     2345 2023-05-10 03:38:33.000000 eulith_web3-0.14.2/src/eulith_web3/fireblocks.py
--rw-r--r--   0 kristian   (501) staff       (20)    28892 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/gmx.py
--rw-r--r--   0 kristian   (501) staff       (20)     2127 2023-05-10 04:03:27.000000 eulith_web3-0.14.2/src/eulith_web3/kms.py
--rw-r--r--   0 kristian   (501) staff       (20)     2305 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/ledger.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938031 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 03:38:33.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     3935 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/account.py
--rw-r--r--   0 kristian   (501) staff       (20)     6647 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/comms.py
--rw-r--r--   0 kristian   (501) staff       (20)     2325 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/constants.py
--rw-r--r--   0 kristian   (501) staff       (20)     3929 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/exceptions.py
--rw-r--r--   0 kristian   (501) staff       (20)     5230 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/messages.py
--rw-r--r--   0 kristian   (501) staff       (20)    27686 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/objects.py
--rw-r--r--   0 kristian   (501) staff       (20)    11098 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/transactions.py
--rw-r--r--   0 kristian   (501) staff       (20)     6807 2023-05-10 17:27:12.000000 eulith_web3-0.14.2/src/eulith_web3/ledger_interface/utils.py
--rw-r--r--   0 kristian   (501) staff       (20)     6961 2023-07-28 15:05:53.000000 eulith_web3-0.14.2/src/eulith_web3/pendle.py
--rw-r--r--   0 kristian   (501) staff       (20)      935 2023-02-23 17:03:31.000000 eulith_web3-0.14.2/src/eulith_web3/requests.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938411 eulith_web3-0.14.2/src/eulith_web3/safe_utils/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 04:36:00.000000 eulith_web3-0.14.2/src/eulith_web3/safe_utils/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     1512 2023-05-10 04:41:15.000000 eulith_web3-0.14.2/src/eulith_web3/safe_utils/transaction_data.py
--rw-r--r--   0 kristian   (501) staff       (20)      500 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/signer.py
--rw-r--r--   0 kristian   (501) staff       (20)     7379 2023-05-20 18:29:54.000000 eulith_web3-0.14.2/src/eulith_web3/signing.py
--rw-r--r--   0 kristian   (501) staff       (20)     1207 2023-01-09 03:56:23.000000 eulith_web3-0.14.2/src/eulith_web3/swap.py
--rw-r--r--   0 kristian   (501) staff       (20)     4152 2023-06-03 21:04:08.000000 eulith_web3-0.14.2/src/eulith_web3/trezor.py
--rw-r--r--   0 kristian   (501) staff       (20)     6190 2023-06-26 18:01:37.000000 eulith_web3-0.14.2/src/eulith_web3/uniswap.py
--rw-r--r--   0 kristian   (501) staff       (20)     8055 2023-07-13 16:28:28.000000 eulith_web3-0.14.2/src/eulith_web3/websocket.py
--rw-r--r--   0 kristian   (501) staff       (20)     1511 2023-07-19 16:02:43.000000 eulith_web3-0.14.2/src/eulith_web3/whitelists.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.912217 eulith_web3-0.14.2/src/eulith_web3.egg-info/
--rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)     5315 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/SOURCES.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/dependency_links.txt
--rw-r--r--   0 kristian   (501) staff       (20)      121 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/requires.txt
--rw-r--r--   0 kristian   (501) staff       (20)       29 2023-08-03 15:31:21.000000 eulith_web3-0.14.2/src/eulith_web3.egg-info/top_level.txt
--rw-r--r--   0 kristian   (501) staff       (20)      244 2023-08-02 21:50:32.000000 eulith_web3-0.14.2/src/generate.py
--rw-r--r--   0 kristian   (501) staff       (20)     5922 2023-08-03 00:54:36.000000 eulith_web3-0.14.2/src/scratch.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:31:21.938675 eulith_web3-0.14.2/tests/
--rw-r--r--   0 kristian   (501) staff       (20)     1573 2023-05-15 21:47:40.000000 eulith_web3-0.14.2/tests/test_guard.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.213620 eulith_web3-0.14.3/
+-rw-r--r--   0 kristian   (501) staff       (20)    19298 2023-05-10 17:26:21.000000 eulith_web3-0.14.3/LICENSE
+-rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:34:56.213459 eulith_web3-0.14.3/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)      483 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/README.md
+-rw-r--r--   0 kristian   (501) staff       (20)      670 2023-08-03 15:34:47.000000 eulith_web3-0.14.3/pyproject.toml
+-rw-r--r--   0 kristian   (501) staff       (20)       38 2023-08-03 15:34:56.213671 eulith_web3-0.14.3/setup.cfg
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.177634 eulith_web3-0.14.3/src/
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.186540 eulith_web3-0.14.3/src/eulith_web3/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2022-10-20 22:32:35.000000 eulith_web3-0.14.3/src/eulith_web3/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2598 2023-07-28 15:05:53.000000 eulith_web3-0.14.3/src/eulith_web3/ace.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5059 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/asn_dump.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11825 2023-08-03 01:10:39.000000 eulith_web3-0.14.3/src/eulith_web3/binding_generator.py
+-rw-r--r--   0 kristian   (501) staff       (20)      181 2023-05-11 20:44:47.000000 eulith_web3-0.14.3/src/eulith_web3/common.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.191882 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-20 01:40:58.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/__init__.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.193268 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4338 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_booster.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1868 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7615 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_reward_staking.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9343 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_rewards.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.195789 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24465 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24149 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    26614 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27226 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    26616 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27228 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15565 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py
+-rw-r--r--   0 kristian   (501) staff       (20)    28229 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.199672 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10030 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11100 2023-05-15 20:04:29.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_order_book.py
+-rw-r--r--   0 kristian   (501) staff       (20)    22721 2023-04-02 23:46:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_position_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13989 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reader.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4360 2023-04-02 23:46:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reward_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10396 2023-04-02 23:46:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6133 2023-04-02 23:46:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    55194 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11712 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10873 2023-03-30 16:24:00.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5283 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c20.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8379 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10077 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9891 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10450 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6646 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24838 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_lending_pool.py
+-rw-r--r--   0 kristian   (501) staff       (20)    25872 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1686 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2772 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_periphery_payments.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1764 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_pool_initializer.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6227 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_swap_router.py
+-rw-r--r--   0 kristian   (501) staff       (20)    24033 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.208151 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-06 22:33:30.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)      166 2023-04-07 03:16:15.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/approx_params.py
+-rw-r--r--   0 kristian   (501) staff       (20)      106 2023-04-07 03:16:15.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/call3.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3166 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2871 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27755 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py
+-rw-r--r--   0 kristian   (501) staff       (20)    14201 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3251 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6688 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11760 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15386 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    69987 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7648 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1817 2023-04-07 03:16:15.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2103 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18782 2023-04-07 03:16:15.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_market.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2256 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11520 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2535 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18706 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2162 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18802 2023-04-09 00:27:11.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py
+-rw-r--r--   0 kristian   (501) staff       (20)      108 2023-04-07 03:16:15.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/multi_approval.py
+-rw-r--r--   0 kristian   (501) staff       (20)      148 2023-04-09 00:29:28.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/swap_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      256 2023-04-09 00:29:28.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/token_input.py
+-rw-r--r--   0 kristian   (501) staff       (20)      261 2023-04-09 00:29:28.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/token_output.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.209023 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/safe/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-04-26 00:24:28.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/safe/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)    78604 2023-08-03 01:10:39.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/safe/i_safe.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6358 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/contract_bindings/w_e_t_h_interface.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1478 2023-03-21 02:59:35.000000 eulith_web3-0.14.3/src/eulith_web3/curve.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3651 2023-05-15 20:04:29.000000 eulith_web3-0.14.3/src/eulith_web3/erc20.py
+-rw-r--r--   0 kristian   (501) staff       (20)    89891 2023-08-01 19:26:04.000000 eulith_web3-0.14.3/src/eulith_web3/eulith_web3.py
+-rw-r--r--   0 kristian   (501) staff       (20)      543 2023-05-15 21:44:45.000000 eulith_web3-0.14.3/src/eulith_web3/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2345 2023-05-10 03:38:33.000000 eulith_web3-0.14.3/src/eulith_web3/fireblocks.py
+-rw-r--r--   0 kristian   (501) staff       (20)    28892 2023-07-28 15:05:53.000000 eulith_web3-0.14.3/src/eulith_web3/gmx.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2127 2023-05-10 04:03:27.000000 eulith_web3-0.14.3/src/eulith_web3/kms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2305 2023-05-20 18:29:54.000000 eulith_web3-0.14.3/src/eulith_web3/ledger.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.212304 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 03:38:33.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3935 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/account.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6647 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/comms.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2325 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/constants.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3929 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5230 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/messages.py
+-rw-r--r--   0 kristian   (501) staff       (20)    27686 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/objects.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11098 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/transactions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6807 2023-05-10 17:27:12.000000 eulith_web3-0.14.3/src/eulith_web3/ledger_interface/utils.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6961 2023-07-28 15:05:53.000000 eulith_web3-0.14.3/src/eulith_web3/pendle.py
+-rw-r--r--   0 kristian   (501) staff       (20)      935 2023-02-23 17:03:31.000000 eulith_web3-0.14.3/src/eulith_web3/requests.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.212725 eulith_web3-0.14.3/src/eulith_web3/safe_utils/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-10 04:36:00.000000 eulith_web3-0.14.3/src/eulith_web3/safe_utils/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1512 2023-05-10 04:41:15.000000 eulith_web3-0.14.3/src/eulith_web3/safe_utils/transaction_data.py
+-rw-r--r--   0 kristian   (501) staff       (20)      500 2023-05-20 18:29:54.000000 eulith_web3-0.14.3/src/eulith_web3/signer.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7379 2023-05-20 18:29:54.000000 eulith_web3-0.14.3/src/eulith_web3/signing.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1207 2023-01-09 03:56:23.000000 eulith_web3-0.14.3/src/eulith_web3/swap.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4152 2023-06-03 21:04:08.000000 eulith_web3-0.14.3/src/eulith_web3/trezor.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6190 2023-06-26 18:01:37.000000 eulith_web3-0.14.3/src/eulith_web3/uniswap.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8055 2023-07-13 16:28:28.000000 eulith_web3-0.14.3/src/eulith_web3/websocket.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1511 2023-07-19 16:02:43.000000 eulith_web3-0.14.3/src/eulith_web3/whitelists.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.187372 eulith_web3-0.14.3/src/eulith_web3.egg-info/
+-rw-r--r--   0 kristian   (501) staff       (20)      884 2023-08-03 15:34:56.000000 eulith_web3-0.14.3/src/eulith_web3.egg-info/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)     5284 2023-08-03 15:34:56.000000 eulith_web3-0.14.3/src/eulith_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2023-08-03 15:34:56.000000 eulith_web3-0.14.3/src/eulith_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      121 2023-08-03 15:34:56.000000 eulith_web3-0.14.3/src/eulith_web3.egg-info/requires.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       12 2023-08-03 15:34:56.000000 eulith_web3-0.14.3/src/eulith_web3.egg-info/top_level.txt
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-08-03 15:34:56.213005 eulith_web3-0.14.3/tests/
+-rw-r--r--   0 kristian   (501) staff       (20)     1573 2023-05-15 21:47:40.000000 eulith_web3-0.14.3/tests/test_guard.py
```

### Comparing `eulith_web3-0.14.2/LICENSE` & `eulith_web3-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/PKG-INFO` & `eulith_web3-0.14.3/src/eulith_web3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eulith_web3
-Version: 0.14.2
+Name: eulith-web3
+Version: 0.14.3
 Summary: A Web3.py compatible wrapper library for Eulith clients
 Author-email: Eulith Team <kristian@eulith.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eulith_web3-0.14.2/pyproject.toml` & `eulith_web3-0.14.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 [project]
   classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
   dependencies = ["web3 >= 5.31.1", "boto3", "asn1", "uuid", "requests", "hexbytes", "cytoolz", "botocore", "fireblocks-sdk", "websocket-client", "ledgerblue", "eulith-trezor"]
   description = "A Web3.py compatible wrapper library for Eulith clients"
   name = "eulith_web3"
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.14.2"
+  version = "0.14.3"
 
   [[project.authors]]
     email = "kristian@eulith.com"
     name = "Eulith Team"
```

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ace.py` & `eulith_web3-0.14.3/src/eulith_web3/ace.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/asn_dump.py` & `eulith_web3-0.14.3/src/eulith_web3/asn_dump.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/binding_generator.py` & `eulith_web3-0.14.3/src/eulith_web3/binding_generator.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_booster.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_booster.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_convex_deposits.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_reward_staking.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_reward_staking.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/convex/i_rewards.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/convex/i_rewards.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_crv_gauge.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_ldo_gauge.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_eth_matic_gauge.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_three_pool.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/curve/curve_v2_tri_crypto.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_glp_manager.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_order_book.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_order_book.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_position_router.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_position_router.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reader.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reader.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_router.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reward_router.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_reward_tracker.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_router.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_router.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault_price_feed.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/gmx/i_vault_utils.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c20.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c20.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_enumerable.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_metadata.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c721_permit.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_e_r_c_detailed.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_lending_pool.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_lending_pool.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_nonfungible_position_manager.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_periphery_immutable_state.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_periphery_payments.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_periphery_payments.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_pool_initializer.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_pool_initializer.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_swap_router.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_swap_router.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/i_uniswap_v3_pool.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_diamond_loupe.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_e_r_c20_permit.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_add_remove_liq.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_mint_redeem.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_misc.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_storage_static.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_p_t.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_action_swap_y_t.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_all_action.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_bulk_seller.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_gauge.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_interest_manager_y_t.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_market.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_market_swap_callback.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_principal_token.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_swap_aggregator.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_p_yield_token.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_reward_manager.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/pendle/i_standardized_yield.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/safe/i_safe.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/safe/i_safe.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/contract_bindings/w_e_t_h_interface.py` & `eulith_web3-0.14.3/src/eulith_web3/contract_bindings/w_e_t_h_interface.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/curve.py` & `eulith_web3-0.14.3/src/eulith_web3/curve.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/erc20.py` & `eulith_web3-0.14.3/src/eulith_web3/erc20.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/eulith_web3.py` & `eulith_web3-0.14.3/src/eulith_web3/eulith_web3.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/exceptions.py` & `eulith_web3-0.14.3/src/eulith_web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/fireblocks.py` & `eulith_web3-0.14.3/src/eulith_web3/fireblocks.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/gmx.py` & `eulith_web3-0.14.3/src/eulith_web3/gmx.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/kms.py` & `eulith_web3-0.14.3/src/eulith_web3/kms.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/account.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/account.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/comms.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/comms.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/constants.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/constants.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/exceptions.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/messages.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/messages.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/objects.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/objects.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/transactions.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/transactions.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/ledger_interface/utils.py` & `eulith_web3-0.14.3/src/eulith_web3/ledger_interface/utils.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/pendle.py` & `eulith_web3-0.14.3/src/eulith_web3/pendle.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/requests.py` & `eulith_web3-0.14.3/src/eulith_web3/requests.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/safe_utils/transaction_data.py` & `eulith_web3-0.14.3/src/eulith_web3/safe_utils/transaction_data.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/signing.py` & `eulith_web3-0.14.3/src/eulith_web3/signing.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/swap.py` & `eulith_web3-0.14.3/src/eulith_web3/swap.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/trezor.py` & `eulith_web3-0.14.3/src/eulith_web3/trezor.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/uniswap.py` & `eulith_web3-0.14.3/src/eulith_web3/uniswap.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/websocket.py` & `eulith_web3-0.14.3/src/eulith_web3/websocket.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3/whitelists.py` & `eulith_web3-0.14.3/src/eulith_web3/whitelists.py`

 * *Files identical despite different names*

### Comparing `eulith_web3-0.14.2/src/eulith_web3.egg-info/PKG-INFO` & `eulith_web3-0.14.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eulith-web3
-Version: 0.14.2
+Name: eulith_web3
+Version: 0.14.3
 Summary: A Web3.py compatible wrapper library for Eulith clients
 Author-email: Eulith Team <kristian@eulith.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `eulith_web3-0.14.2/src/eulith_web3.egg-info/SOURCES.txt` & `eulith_web3-0.14.3/src/eulith_web3.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-src/generate.py
-src/scratch.py
 src/eulith_web3/__init__.py
 src/eulith_web3/ace.py
 src/eulith_web3/asn_dump.py
 src/eulith_web3/binding_generator.py
 src/eulith_web3/common.py
 src/eulith_web3/curve.py
 src/eulith_web3/erc20.py
```

### Comparing `eulith_web3-0.14.2/tests/test_guard.py` & `eulith_web3-0.14.3/tests/test_guard.py`

 * *Files identical despite different names*

