# Comparing `tmp/moneyonchain_prices_source-0.6.6b6.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.6b6.tar", last modified: Fri Jul 28 17:11:13 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b7.tar", last modified: Thu Aug  3 13:16:38 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.6b6.tar` & `moneyonchain_prices_source-0.6.6b7.tar`

### file list

```diff
@@ -1,115 +1,117 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2023-07-28 16:02:42.000000 moneyonchain_prices_source-0.6.6b6/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.897980 moneyonchain_prices_source-0.6.6b6/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-07-26 17:12:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2023-07-28 15:37:53.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3101 2023-07-27 12:10:08.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.897980 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2312 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.913979 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5000 2023-07-26 17:37:06.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-28 16:25:00.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-28 17:10:06.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b6/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4666 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-28 17:11:13.000000 moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-28 17:11:13.917979 moneyonchain_prices_source-0.6.6b6/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1868 2023-07-28 17:07:59.000000 moneyonchain_prices_source-0.6.6b6/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.716544 moneyonchain_prices_source-0.6.6b7/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.668544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-07-26 17:12:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3101 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.672544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2377 2023-08-03 12:28:17.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-08-02 20:35:41.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5153 2023-08-03 11:58:32.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13875 2023-08-02 20:44:38.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1825 2023-08-03 12:16:49.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-08-02 21:03:56.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2023-08-03 12:05:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-08-02 20:35:42.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-08-03 11:55:27.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2023-07-24 16:24:11.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b7/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-08-03 13:16:38.712544 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4787 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4767 2023-08-03 13:16:38.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-08-03 13:16:37.000000 moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-08-03 13:16:38.716544 moneyonchain_prices_source-0.6.6b7/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1868 2023-07-28 18:46:05.000000 moneyonchain_prices_source-0.6.6b7/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.6b6/PKG-INFO` & `moneyonchain_prices_source-0.6.6b7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.6.6b6
+Version: 0.6.6b7
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # **MoC prices source**
         
@@ -32,15 +32,15 @@
         >>> get_price(BTC_USD)
         Decimal('29395.82')
         >>> 
         ```
         
         And that's it!
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b6)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b7)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b6)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b7)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `moneyonchain_prices_source-0.6.6b6/README.md` & `moneyonchain_prices_source-0.6.6b7/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/computed_pairs.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/data/weighing.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'rif_btc_mp1p_binance'": '1', "'rif_usdt_mp1p_binance'": '1'}*

```diff
@@ -26,16 +26,18 @@
     "eth_btc_kraken": 0.25,
     "gas_btc_rsk": 1,
     "moc_btc_sovryn": 1,
     "rif_btc_binance": 1,
     "rif_btc_bithumbpro": 0,
     "rif_btc_coingecko": 0,
     "rif_btc_mexc": 0,
+    "rif_btc_mp1p_binance": 1,
     "rif_btc_sovryn": 0,
     "rif_usdt_binance": 1,
+    "rif_usdt_mp1p_binance": 1,
     "usd_ars_ambito": 0.09,
     "usd_ars_ccb_emdx": 0,
     "usd_ars_ccb_rofex": 1,
     "usd_ars_ccl_ambito": 0.09,
     "usd_ars_ccl_coinmonitor": 0.09,
     "usd_ars_ccl_criptoya": 0.09,
     "usd_ars_ccl_cronista": 0.09,
```

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/coins.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,20 +121,22 @@
     def __hash__(self):
         return hash(str(self))
 
 
 BTC_USD         = CoinPair(BTC,  USD)
 BTC_ARS         = CoinPair(BTC,  ARS)
 RIF_BTC         = CoinPair(RIF,  BTC)
+RIF_BTC_MP1P    = CoinPair(RIF,  BTC, "mp1%") # To move the price 1 percent
 RIF_USD         = CoinPair(RIF,  USD) # Leave this as legacy
 RIF_USD_B       = CoinPair(RIF,  USD, "B") # Passing through Bitcoin
 RIF_USD_T       = CoinPair(RIF,  USD, "T") # Passing through Tether
 RIF_USD_TB      = CoinPair(RIF,  USD, "TB") # Passing through Tether & Bitcoin
 RIF_USD_WMTB    = CoinPair(RIF,  USD, "WMTB") # Passing through Tether & Bitcoin usinng weighted_median
 RIF_USDT        = CoinPair(RIF,  USDT)
+RIF_USDT_MP1P   = CoinPair(RIF,  USDT, "mp1%") # To move the price 1 percent
 MOC_BTC         = CoinPair(MOC,  BTC)
 MOC_USD         = CoinPair(MOC,  USD)
 ETH_BTC         = CoinPair(ETH,  BTC)
 ETH_USD         = CoinPair(ETH,  USD)
 BTC_USDT        = CoinPair(BTC,  USDT)
 USDT_USD        = CoinPair(USDT, USD)
 USDT_USD_B      = CoinPair(USDT, USD, "B") # Passing through Bitcoin
```

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/engine_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,16 +403,17 @@
         return data
 
 
 class BaseWithFailover(Base):
 
     _uri_failover = None
 
-    def __call__(self):
-        start_time = datetime.datetime.now()
+    def __call__(self, start_time=None):
+        if start_time is None:
+            start_time = datetime.datetime.now()
         ok = Base.__call__(self, start_time)
         if self._uri_failover and not ok:
             uri_failover, uri = self._uri_failover, self._uri
             self._uri_failover, self._uri =  uri, uri_failover
             ok = Base.__call__(self, start_time)
         return ok
```

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/engines/usdt_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b7/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.6.6b6
+Version: 0.6.6b7
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # **MoC prices source**
         
@@ -32,15 +32,15 @@
         >>> get_price(BTC_USD)
         Decimal('29395.82')
         >>> 
         ```
         
         And that's it!
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b6)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b7)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b6)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.6.6b7)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b6/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.6.6b7/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `moneyonchain_prices_source-0.6.6b6/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b7/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,19 @@
 moc_prices_source/engines/rif_btc_binance.py
 moc_prices_source/engines/rif_btc_bitfinex.py
 moc_prices_source/engines/rif_btc_bithumbpro.py
 moc_prices_source/engines/rif_btc_coinbene.py
 moc_prices_source/engines/rif_btc_coingecko.py
 moc_prices_source/engines/rif_btc_kucoin.py
 moc_prices_source/engines/rif_btc_mexc.py
+moc_prices_source/engines/rif_btc_mp1p_binance.py
 moc_prices_source/engines/rif_btc_mxc.py
 moc_prices_source/engines/rif_btc_sovryn.py
 moc_prices_source/engines/rif_usdt_binance.py
+moc_prices_source/engines/rif_usdt_mp1p_binance.py
 moc_prices_source/engines/usd_ars_ambito.py
 moc_prices_source/engines/usd_ars_ccb_emdx.py
 moc_prices_source/engines/usd_ars_ccb_rofex.py
 moc_prices_source/engines/usd_ars_ccl_ambito.py
 moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
 moc_prices_source/engines/usd_ars_ccl_criptoya.py
 moc_prices_source/engines/usd_ars_ccl_cronista.py
```

### Comparing `moneyonchain_prices_source-0.6.6b6/setup.py` & `moneyonchain_prices_source-0.6.6b7/setup.py`

 * *Files identical despite different names*

