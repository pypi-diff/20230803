# Comparing `tmp/moneyonchain_prices_source-0.6.6b7.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.6b7.tar", last modified: Thu Aug  3 13:16:38 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b8.tar", last modified: Thu Aug  3 17:42:18 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.6b7.tar` & `moneyonchain_prices_source-0.6.6b8.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.716544 moneyonchain_prices_source-0.6.6b7/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.668544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-07-26 17:12:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3101 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.672544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2377 2023-08-03 12:28:17.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5153 2023-08-03 11:58:32.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13875 2023-08-02 20:44:38.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1825 2023-08-03 12:16:49.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-08-02 21:03:56.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2023-08-03 12:05:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-08-03 11:55:27.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4767 2023-08-03 13:16:38.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-08-03 13:16:38.716544 moneyonchain_prices_source-0.6.6b7/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1868 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 17:42:18.340403 moneyonchain_prices_source-0.6.6b8/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3784 2023-08-03 17:42:18.340403 moneyonchain_prices_source-0.6.6b8/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 17:42:18.328402 moneyonchain_prices_source-0.6.6b8/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3101 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 17:42:18.328402 moneyonchain_prices_source-0.6.6b8/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2377 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 17:42:18.336403 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5153 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13875 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-06-12 23:13:25.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2023-08-03 17:23:24.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-06-12 23:14:40.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-06-12 21:21:22.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_usdt_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2022-10-13 14:25:37.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2022-10-13 14:12:43.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-08-03 17:24:26.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-10-04 17:25:42.000000 moneyonchain_prices_source-0.6.6b8/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 17:42:18.340403 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3784 2023-08-03 17:42:18.000000 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4767 2023-08-03 17:42:18.000000 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-08-03 17:42:18.000000 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-08-03 17:42:18.000000 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-08-03 17:42:18.000000 moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-08-03 17:42:18.340403 moneyonchain_prices_source-0.6.6b8/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1868 2023-08-03 17:21:32.000000 moneyonchain_prices_source-0.6.6b8/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.6b7/README.md` & `moneyonchain_prices_source-0.6.6b8/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/computed_pairs.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/data/weighing.json`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mp1p_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mp1p_binance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from engine_base import BaseWithFailover, RIF_BTC_MP1P
-from rif_usdt_binance import Engine as RifUsdtEngine
+from rif_btc_binance import Engine as RifBtcEngine
 from decimal import Decimal
 
 base_uri = "https://{}/api/v3/depth?symbol=RIFBTC"
 factor = 0.01
 
 class Engine(BaseWithFailover):
 
@@ -13,15 +13,15 @@
     _uri_failover = base_uri.format("moc-proxy-api-binance.moneyonchain.com")
     _coinpair     = RIF_BTC_MP1P
     _max_time_without_price_change = 0 # zero means infinity
 
 
 
     def __call__(self):
-        price_engine = RifUsdtEngine()
+        price_engine = RifBtcEngine()
         ok = price_engine()
         self._error = price_engine.error
         self.base_price = price_engine.price
         if ok:
             ok = BaseWithFailover.__call__(self)
         return ok
```

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/rif_usdt_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b8/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b8/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b7/setup.py` & `moneyonchain_prices_source-0.6.6b8/setup.py`

 * *Files identical despite different names*

