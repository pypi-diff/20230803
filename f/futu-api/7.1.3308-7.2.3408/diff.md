# Comparing `tmp/futu-api-7.1.3308.tar.gz` & `tmp/futu-api-7.2.3408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futu-api-7.1.3308.tar", last modified: Thu Feb 23 07:52:01 2023, max compression
+gzip compressed data, was "futu-api-7.2.3408.tar", last modified: Thu Aug  3 08:47:47 2023, max compression
```

## Comparing `futu-api-7.1.3308.tar` & `futu-api-7.2.3408.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.823069 futu-api-7.1.3308/
--rw-rw-rw-   0        0        0    11547 2022-09-16 08:53:29.000000 futu-api-7.1.3308/LICENSE
--rw-rw-rw-   0        0        0      252 2022-09-16 08:53:29.000000 futu-api-7.1.3308/MANIFEST.in
--rw-rw-rw-   0        0        0     8202 2023-02-23 07:52:01.822071 futu-api-7.1.3308/PKG-INFO
--rw-rw-rw-   0        0        0     7834 2022-09-29 02:08:19.000000 futu-api-7.1.3308/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.684440 futu-api-7.1.3308/futu/
--rw-rw-rw-   0        0        0       10 2023-02-23 07:49:55.000000 futu-api-7.1.3308/futu/VERSION.txt
--rw-rw-rw-   0        0        0     4815 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.699400 futu-api-7.1.3308/futu/common/
--rw-rw-rw-   0        0        0     2692 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/__init__.py
--rw-rw-rw-   0        0        0      816 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/callback_executor.py
--rw-rw-rw-   0        0        0     1152 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/common/comm_add_path.py
--rw-rw-rw-   0        0        0     5165 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/conn_mng.py
--rw-rw-rw-   0        0        0   130028 2022-10-12 02:40:47.000000 futu-api-7.1.3308/futu/common/constant.py
--rw-rw-rw-   0        0        0     1772 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/diag.py
--rw-rw-rw-   0        0        0     1976 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/err.py
--rw-rw-rw-   0        0        0     9953 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/ft_logger.py
--rw-rw-rw-   0        0        0     2981 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/handler_context.py
--rw-rw-rw-   0        0        0    23761 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/network_manager.py
--rw-rw-rw-   0        0        0    20010 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/open_context_base.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.790157 futu-api-7.1.3308/futu/common/pb/
--rw-rw-rw-   0        0        0    12889 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Common_pb2.py
--rw-rw-rw-   0        0        0    26025 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/GetDelayStatistics_pb2.py
--rw-rw-rw-   0        0        0    14101 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/GetGlobalState_pb2.py
--rw-rw-rw-   0        0        0    21325 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/GetUserInfo_pb2.py
--rw-rw-rw-   0        0        0    11456 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/InitConnect_pb2.py
--rw-rw-rw-   0        0        0     6839 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/KeepAlive_pb2.py
--rw-rw-rw-   0        0        0    28183 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Notify_pb2.py
--rw-rw-rw-   0        0        0   173802 2022-10-12 02:40:47.000000 futu-api-7.1.3308/futu/common/pb/Qot_Common_pb2.py
--rw-rw-rw-   0        0        0     7362 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetBasicQot_pb2.py
--rw-rw-rw-   0        0        0     8305 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetBroker_pb2.py
--rw-rw-rw-   0        0        0    11466 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetCapitalDistribution_pb2.py
--rw-rw-rw-   0        0        0    13739 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetCapitalFlow_pb2.py
--rw-rw-rw-   0        0        0    19445 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetCodeChange_pb2.py
--rw-rw-rw-   0        0        0    17850 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetFutureInfo_pb2.py
--rw-rw-rw-   0        0        0    16986 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py
--rw-rw-rw-   0        0        0    11145 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetHistoryKL_pb2.py
--rw-rw-rw-   0        0        0     9419 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetHoldingChangeList_pb2.py
--rw-rw-rw-   0        0        0    28489 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetIpoList_pb2.py
--rw-rw-rw-   0        0        0     8802 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetKL_pb2.py
--rw-rw-rw-   0        0        0     9565 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetMarketState_pb2.py
--rw-rw-rw-   0        0        0    23483 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetOptionChain_pb2.py
--rw-rw-rw-   0        0        0    10797 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py
--rw-rw-rw-   0        0        0    10581 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetOrderBook_pb2.py
--rw-rw-rw-   0        0        0     9371 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetOwnerPlate_pb2.py
--rw-rw-rw-   0        0        0     8305 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetPlateSecurity_pb2.py
--rw-rw-rw-   0        0        0     7643 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetPlateSet_pb2.py
--rw-rw-rw-   0        0        0    13090 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetPriceReminder_pb2.py
--rw-rw-rw-   0        0        0     7651 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetRT_pb2.py
--rw-rw-rw-   0        0        0     8949 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetReference_pb2.py
--rw-rw-rw-   0        0        0     9114 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetRehab_pb2.py
--rw-rw-rw-   0        0        0    73561 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py
--rw-rw-rw-   0        0        0     8230 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetStaticInfo_pb2.py
--rw-rw-rw-   0        0        0     8068 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetSubInfo_pb2.py
--rw-rw-rw-   0        0        0    11590 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetSuspend_pb2.py
--rw-rw-rw-   0        0        0     8170 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetTicker_pb2.py
--rw-rw-rw-   0        0        0    10348 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py
--rw-rw-rw-   0        0        0     7403 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetUserSecurity_pb2.py
--rw-rw-rw-   0        0        0    41430 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_GetWarrant_pb2.py
--rw-rw-rw-   0        0        0     9314 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_ModifyUserSecurity_pb2.py
--rw-rw-rw-   0        0        0     8457 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_RegQotPush_pb2.py
--rw-rw-rw-   0        0        0    10539 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py
--rw-rw-rw-   0        0        0    11678 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_RequestHistoryKL_pb2.py
--rw-rw-rw-   0        0        0     7352 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_RequestRehab_pb2.py
--rw-rw-rw-   0        0        0    10735 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_RequestTradeDate_pb2.py
--rw-rw-rw-   0        0        0    11792 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_SetPriceReminder_pb2.py
--rw-rw-rw-   0        0        0    75774 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_StockFilter_pb2.py
--rw-rw-rw-   0        0        0     9912 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_Sub_pb2.py
--rw-rw-rw-   0        0        0     5003 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateBasicQot_pb2.py
--rw-rw-rw-   0        0        0     5981 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateBroker_pb2.py
--rw-rw-rw-   0        0        0     6135 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateKL_pb2.py
--rw-rw-rw-   0        0        0     7861 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateOrderBook_pb2.py
--rw-rw-rw-   0        0        0    10066 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdatePriceReminder_pb2.py
--rw-rw-rw-   0        0        0     5362 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateRT_pb2.py
--rw-rw-rw-   0        0        0     5448 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Qot_UpdateTicker_pb2.py
--rw-rw-rw-   0        0        0     7519 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/TestCmd_pb2.py
--rw-rw-rw-   0        0        0    85604 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_Common_pb2.py
--rw-rw-rw-   0        0        0     8030 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetAccList_pb2.py
--rw-rw-rw-   0        0        0     8526 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetFunds_pb2.py
--rw-rw-rw-   0        0        0     8747 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py
--rw-rw-rw-   0        0        0     9051 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetHistoryOrderList_pb2.py
--rw-rw-rw-   0        0        0    15027 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetMarginRatio_pb2.py
--rw-rw-rw-   0        0        0    10745 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py
--rw-rw-rw-   0        0        0     8963 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetOrderFillList_pb2.py
--rw-rw-rw-   0        0        0     9249 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetOrderList_pb2.py
--rw-rw-rw-   0        0        0     9803 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_GetPositionList_pb2.py
--rw-rw-rw-   0        0        0    13065 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_ModifyOrder_pb2.py
--rw-rw-rw-   0        0        0     5205 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_Notify_pb2.py
--rw-rw-rw-   0        0        0    14257 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_PlaceOrder_pb2.py
--rw-rw-rw-   0        0        0     9108 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_ReconfirmOrder_pb2.py
--rw-rw-rw-   0        0        0     6604 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_SubAccPush_pb2.py
--rw-rw-rw-   0        0        0     7445 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_UnlockTrade_pb2.py
--rw-rw-rw-   0        0        0     5505 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_UpdateOrderFill_pb2.py
--rw-rw-rw-   0        0        0     5403 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Trd_UpdateOrder_pb2.py
--rw-rw-rw-   0        0        0     9612 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/Verification_pb2.py
--rw-rw-rw-   0        0        0       67 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/__init__.py
--rwxrwxrwx   0        0        0      213 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/build.bat
--rwxrwxrwx   0        0        0      130 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pb/generate_python.bat
--rw-rw-rw-   0        0        0     4937 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/pbjson.py
--rw-rw-rw-   0        0        0     7820 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/sys_config.py
--rw-rw-rw-   0        0        0    27105 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.798136 futu-api-7.1.3308/futu/examples/
--rw-rw-rw-   0        0        0       27 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/__init__.py
--rw-rw-rw-   0        0        0     1785 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/get_mkt_snapshot_demo.py
--rw-rw-rw-   0        0        0     6608 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/macd_strategy.py
--rw-rw-rw-   0        0        0    12064 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/quote_and_trade_demo.py
--rw-rw-rw-   0        0        0     2866 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/quote_push.py
--rw-rw-rw-   0        0        0     2151 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/simple_filter_demo.py
--rw-rw-rw-   0        0        0     3711 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/examples/stocksell_demo.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.806114 futu-api-7.1.3308/futu/quote/
--rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/quote/__init__.py
--rw-rw-rw-   0        0        0   127218 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/open_quote_context.py
--rw-rw-rw-   0        0        0    17142 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/quote_get_warrant.py
--rw-rw-rw-   0        0        0   130710 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/quote_query.py
--rw-rw-rw-   0        0        0    13150 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/quote_response_handler.py
--rw-rw-rw-   0        0        0    31564 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/quote_stockfilter_info.py
--rw-rw-rw-   0        0        0     5182 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/quote/quote_tool.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.811101 futu-api-7.1.3308/futu/tools/
--rw-rw-rw-   0        0        0     7966 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/tools/Common.proto.json
--rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/tools/__init__.py
--rw-rw-rw-   0        0        0      354 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/tools/auto_generate.py
--rw-rw-rw-   0        0        0    31193 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/tools/generate_code.py
--rw-rw-rw-   0        0        0     1976 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/tools/load_template.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.817086 futu-api-7.1.3308/futu/trade/
--rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.1.3308/futu/trade/__init__.py
--rw-rw-rw-   0        0        0    38869 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/trade/open_trade_context.py
--rw-rw-rw-   0        0        0    36121 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/trade/trade_query.py
--rw-rw-rw-   0        0        0     1804 2022-09-29 02:08:19.000000 futu-api-7.1.3308/futu/trade/trade_response_handler.py
-drwxrwxrwx   0        0        0        0 2023-02-23 07:52:01.821075 futu-api-7.1.3308/futu_api.egg-info/
--rw-rw-rw-   0        0        0     8202 2023-02-23 07:52:01.000000 futu-api-7.1.3308/futu_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4289 2023-02-23 07:52:01.000000 futu-api-7.1.3308/futu_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 07:52:01.000000 futu-api-7.1.3308/futu_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-02-23 07:52:01.000000 futu-api-7.1.3308/futu_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-23 07:52:01.000000 futu-api-7.1.3308/futu_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2022-09-29 02:08:19.000000 futu-api-7.1.3308/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 07:52:01.823069 futu-api-7.1.3308/setup.cfg
--rw-rw-rw-   0        0        0     1788 2022-09-29 02:08:19.000000 futu-api-7.1.3308/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.548115 futu-api-7.2.3408/
+-rw-rw-rw-   0        0        0    11547 2022-09-16 08:53:29.000000 futu-api-7.2.3408/LICENSE
+-rw-rw-rw-   0        0        0      252 2022-09-16 08:53:29.000000 futu-api-7.2.3408/MANIFEST.in
+-rw-rw-rw-   0        0        0     8202 2023-08-03 08:47:47.547118 futu-api-7.2.3408/PKG-INFO
+-rw-rw-rw-   0        0        0     7834 2022-09-29 02:08:19.000000 futu-api-7.2.3408/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.294813 futu-api-7.2.3408/futu/
+-rw-rw-rw-   0        0        0       10 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/VERSION.txt
+-rw-rw-rw-   0        0        0     4815 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.320716 futu-api-7.2.3408/futu/common/
+-rw-rw-rw-   0        0        0     2692 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/__init__.py
+-rw-rw-rw-   0        0        0      816 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/callback_executor.py
+-rw-rw-rw-   0        0        0     1152 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/common/comm_add_path.py
+-rw-rw-rw-   0        0        0     5165 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/conn_mng.py
+-rw-rw-rw-   0        0        0   130287 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/constant.py
+-rw-rw-rw-   0        0        0     1772 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/diag.py
+-rw-rw-rw-   0        0        0     1976 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/err.py
+-rw-rw-rw-   0        0        0     9953 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/ft_logger.py
+-rw-rw-rw-   0        0        0     2981 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/handler_context.py
+-rw-rw-rw-   0        0        0    23761 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/network_manager.py
+-rw-rw-rw-   0        0        0    20010 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/open_context_base.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.484284 futu-api-7.2.3408/futu/common/pb/
+-rw-rw-rw-   0        0        0    12889 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Common_pb2.py
+-rw-rw-rw-   0        0        0    26025 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/GetDelayStatistics_pb2.py
+-rw-rw-rw-   0        0        0    14101 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/GetGlobalState_pb2.py
+-rw-rw-rw-   0        0        0    22527 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/GetUserInfo_pb2.py
+-rw-rw-rw-   0        0        0    11456 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/InitConnect_pb2.py
+-rw-rw-rw-   0        0        0     6839 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/KeepAlive_pb2.py
+-rw-rw-rw-   0        0        0    31199 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Notify_pb2.py
+-rw-rw-rw-   0        0        0   174207 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_Common_pb2.py
+-rw-rw-rw-   0        0        0     7362 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetBasicQot_pb2.py
+-rw-rw-rw-   0        0        0     8706 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetBroker_pb2.py
+-rw-rw-rw-   0        0        0    11466 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetCapitalDistribution_pb2.py
+-rw-rw-rw-   0        0        0    13739 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetCapitalFlow_pb2.py
+-rw-rw-rw-   0        0        0    19445 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetCodeChange_pb2.py
+-rw-rw-rw-   0        0        0    17850 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetFutureInfo_pb2.py
+-rw-rw-rw-   0        0        0    16986 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py
+-rw-rw-rw-   0        0        0    11145 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetHistoryKL_pb2.py
+-rw-rw-rw-   0        0        0     9419 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetHoldingChangeList_pb2.py
+-rw-rw-rw-   0        0        0    28489 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetIpoList_pb2.py
+-rw-rw-rw-   0        0        0     9199 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetKL_pb2.py
+-rw-rw-rw-   0        0        0     9565 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetMarketState_pb2.py
+-rw-rw-rw-   0        0        0    23483 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetOptionChain_pb2.py
+-rw-rw-rw-   0        0        0    10797 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py
+-rw-rw-rw-   0        0        0    10985 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetOrderBook_pb2.py
+-rw-rw-rw-   0        0        0     9791 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetOwnerPlate_pb2.py
+-rw-rw-rw-   0        0        0     8305 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetPlateSecurity_pb2.py
+-rw-rw-rw-   0        0        0     7643 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetPlateSet_pb2.py
+-rw-rw-rw-   0        0        0    13515 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetPriceReminder_pb2.py
+-rw-rw-rw-   0        0        0     8048 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetRT_pb2.py
+-rw-rw-rw-   0        0        0     8949 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetReference_pb2.py
+-rw-rw-rw-   0        0        0     9114 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetRehab_pb2.py
+-rw-rw-rw-   0        0        0    73985 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py
+-rw-rw-rw-   0        0        0     8230 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetStaticInfo_pb2.py
+-rw-rw-rw-   0        0        0     8068 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetSubInfo_pb2.py
+-rw-rw-rw-   0        0        0    11590 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetSuspend_pb2.py
+-rw-rw-rw-   0        0        0     8571 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetTicker_pb2.py
+-rw-rw-rw-   0        0        0    10348 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py
+-rw-rw-rw-   0        0        0     7403 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetUserSecurity_pb2.py
+-rw-rw-rw-   0        0        0    41430 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_GetWarrant_pb2.py
+-rw-rw-rw-   0        0        0     9314 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_ModifyUserSecurity_pb2.py
+-rw-rw-rw-   0        0        0     8457 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_RegQotPush_pb2.py
+-rw-rw-rw-   0        0        0    10959 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py
+-rw-rw-rw-   0        0        0    12086 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_RequestHistoryKL_pb2.py
+-rw-rw-rw-   0        0        0     7352 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_RequestRehab_pb2.py
+-rw-rw-rw-   0        0        0    10735 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_RequestTradeDate_pb2.py
+-rw-rw-rw-   0        0        0    11792 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_SetPriceReminder_pb2.py
+-rw-rw-rw-   0        0        0    75774 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_StockFilter_pb2.py
+-rw-rw-rw-   0        0        0     9912 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_Sub_pb2.py
+-rw-rw-rw-   0        0        0     5003 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateBasicQot_pb2.py
+-rw-rw-rw-   0        0        0     6385 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateBroker_pb2.py
+-rw-rw-rw-   0        0        0     6542 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateKL_pb2.py
+-rw-rw-rw-   0        0        0     8268 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateOrderBook_pb2.py
+-rw-rw-rw-   0        0        0    10479 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdatePriceReminder_pb2.py
+-rw-rw-rw-   0        0        0     5762 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateRT_pb2.py
+-rw-rw-rw-   0        0        0     5852 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Qot_UpdateTicker_pb2.py
+-rw-rw-rw-   0        0        0     7519 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/TestCmd_pb2.py
+-rw-rw-rw-   0        0        0    85996 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/Trd_Common_pb2.py
+-rw-rw-rw-   0        0        0     8030 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetAccList_pb2.py
+-rw-rw-rw-   0        0        0     8526 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetFunds_pb2.py
+-rw-rw-rw-   0        0        0     8747 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py
+-rw-rw-rw-   0        0        0     9051 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetHistoryOrderList_pb2.py
+-rw-rw-rw-   0        0        0    15027 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetMarginRatio_pb2.py
+-rw-rw-rw-   0        0        0    10745 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py
+-rw-rw-rw-   0        0        0     8963 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetOrderFillList_pb2.py
+-rw-rw-rw-   0        0        0     9249 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetOrderList_pb2.py
+-rw-rw-rw-   0        0        0     9803 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_GetPositionList_pb2.py
+-rw-rw-rw-   0        0        0    13065 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_ModifyOrder_pb2.py
+-rw-rw-rw-   0        0        0     5205 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_Notify_pb2.py
+-rw-rw-rw-   0        0        0    14257 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_PlaceOrder_pb2.py
+-rw-rw-rw-   0        0        0     9108 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_ReconfirmOrder_pb2.py
+-rw-rw-rw-   0        0        0     6604 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_SubAccPush_pb2.py
+-rw-rw-rw-   0        0        0     7445 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_UnlockTrade_pb2.py
+-rw-rw-rw-   0        0        0     5505 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_UpdateOrderFill_pb2.py
+-rw-rw-rw-   0        0        0     5403 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Trd_UpdateOrder_pb2.py
+-rw-rw-rw-   0        0        0     6800 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/common/pb/UsedQuota_pb2.py
+-rw-rw-rw-   0        0        0     9612 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/Verification_pb2.py
+-rw-rw-rw-   0        0        0       67 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/__init__.py
+-rwxrwxrwx   0        0        0      213 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/build.bat
+-rwxrwxrwx   0        0        0      130 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pb/generate_python.bat
+-rw-rw-rw-   0        0        0     4937 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/pbjson.py
+-rw-rw-rw-   0        0        0     7820 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/sys_config.py
+-rw-rw-rw-   0        0        0    27105 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.499245 futu-api-7.2.3408/futu/examples/
+-rw-rw-rw-   0        0        0       27 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/__init__.py
+-rw-rw-rw-   0        0        0     1785 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/get_mkt_snapshot_demo.py
+-rw-rw-rw-   0        0        0     6608 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/macd_strategy.py
+-rw-rw-rw-   0        0        0    12064 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/quote_and_trade_demo.py
+-rw-rw-rw-   0        0        0     2866 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/quote_push.py
+-rw-rw-rw-   0        0        0     2151 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/simple_filter_demo.py
+-rw-rw-rw-   0        0        0     3711 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/examples/stocksell_demo.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.516199 futu-api-7.2.3408/futu/quote/
+-rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/quote/__init__.py
+-rw-rw-rw-   0        0        0   127328 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/quote/open_quote_context.py
+-rw-rw-rw-   0        0        0    17142 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/quote/quote_get_warrant.py
+-rw-rw-rw-   0        0        0   131895 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/quote/quote_query.py
+-rw-rw-rw-   0        0        0    13197 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/quote/quote_response_handler.py
+-rw-rw-rw-   0        0        0    31564 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/quote/quote_stockfilter_info.py
+-rw-rw-rw-   0        0        0     5182 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/quote/quote_tool.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.526173 futu-api-7.2.3408/futu/tools/
+-rw-rw-rw-   0        0        0     7966 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/tools/Common.proto.json
+-rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/tools/__init__.py
+-rw-rw-rw-   0        0        0      354 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/tools/auto_generate.py
+-rw-rw-rw-   0        0        0    31193 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/tools/generate_code.py
+-rw-rw-rw-   0        0        0     1976 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/tools/load_template.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.534153 futu-api-7.2.3408/futu/trade/
+-rw-rw-rw-   0        0        0        0 2022-09-16 08:53:29.000000 futu-api-7.2.3408/futu/trade/__init__.py
+-rw-rw-rw-   0        0        0    38906 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/trade/open_trade_context.py
+-rw-rw-rw-   0        0        0    36430 2023-08-01 01:47:42.000000 futu-api-7.2.3408/futu/trade/trade_query.py
+-rw-rw-rw-   0        0        0     1804 2022-09-29 02:08:19.000000 futu-api-7.2.3408/futu/trade/trade_response_handler.py
+drwxrwxrwx   0        0        0        0 2023-08-03 08:47:47.545124 futu-api-7.2.3408/futu_api.egg-info/
+-rw-rw-rw-   0        0        0     8202 2023-08-03 08:47:46.000000 futu-api-7.2.3408/futu_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4321 2023-08-03 08:47:47.000000 futu-api-7.2.3408/futu_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 08:47:46.000000 futu-api-7.2.3408/futu_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-08-03 08:47:46.000000 futu-api-7.2.3408/futu_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 08:47:46.000000 futu-api-7.2.3408/futu_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       61 2023-08-01 01:47:42.000000 futu-api-7.2.3408/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 08:47:47.548115 futu-api-7.2.3408/setup.cfg
+-rw-rw-rw-   0        0        0     1788 2023-08-01 01:47:42.000000 futu-api-7.2.3408/setup.py
```

### Comparing `futu-api-7.1.3308/LICENSE` & `futu-api-7.2.3408/LICENSE`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/PKG-INFO` & `futu-api-7.2.3408/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futu-api
-Version: 7.1.3308
+Version: 7.2.3408
 Summary: Futu Quantitative Trading API
 Home-page: https://github.com/FutunnOpen/py-futu-api
 Author: Futu, Inc.
 Author-email: ftdev@futunn.com
 License: Apache License 2.0
 Keywords: Futu HK/US Stock Quant Trading API
 Platform: UNKNOWN
```

### Comparing `futu-api-7.1.3308/README.md` & `futu-api-7.2.3408/README.md`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/__init__.py` & `futu-api-7.2.3408/futu/__init__.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/__init__.py` & `futu-api-7.2.3408/futu/common/__init__.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/callback_executor.py` & `futu-api-7.2.3408/futu/common/callback_executor.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/comm_add_path.py` & `futu-api-7.2.3408/futu/common/comm_add_path.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/conn_mng.py` & `futu-api-7.2.3408/futu/common/conn_mng.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/constant.py` & `futu-api-7.2.3408/futu/common/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,24 +929,26 @@
     NONE = "N/A"
     GTW_EVENT = "GTW_EVENT"
     PROGRAM_STATUS = "PROGRAM_STATUS"
     CONN_STATUS = "CONN_STATUS"
     QOT_RIGHT = "QOT_RIGHT"
     API_LEVEL = "API_LEVEL"
     API_QUOTA = "API_QUOTA"
+    USED_QUOTA = "USED_QUOTA"
 
     def load_dic(self):
         return {
             self.NONE: Notify_pb2.NotifyType_None,
             self.GTW_EVENT: Notify_pb2.NotifyType_GtwEvent,
             self.PROGRAM_STATUS: Notify_pb2.NotifyType_ProgramStatus,
             self.CONN_STATUS: Notify_pb2.NotifyType_ConnStatus,
             self.QOT_RIGHT: Notify_pb2.NotifyType_QotRight,
             self.API_LEVEL: Notify_pb2.NotifyType_APILevel,
             self.API_QUOTA: Notify_pb2.NotifyType_APIQuota,
+            self.USED_QUOTA: Notify_pb2.NotifyType_UsedQuota,
         }
 
 class GtwEventType(FtEnum):
     """
     网关异步通知类型定义
     ..  py:class:: GtwEventType
      ..  py:attribute:: LocalCfgLoadFailed
@@ -2415,23 +2417,25 @@
 class Currency(FtEnum):
     NONE = 'N/A' # 未知
     HKD = 'HKD'  # 港币
     USD = 'USD'  # 美元
     CNH = 'CNH'  # 离岸人民币
     JPY = 'JPY'  # 日元
     SGD = 'SGD'  # 新元
+    AUD = 'AUD'  # 澳元
 
     def load_dic(self):
         return {
             self.NONE: Trd_Common_pb2.Currency_Unknown,
             self.HKD: Trd_Common_pb2.Currency_HKD,
             self.USD: Trd_Common_pb2.Currency_USD,
             self.CNH: Trd_Common_pb2.Currency_CNH,
             self.JPY: Trd_Common_pb2.Currency_JPY,
-            self.SGD: Trd_Common_pb2.Currency_SGD
+            self.SGD: Trd_Common_pb2.Currency_SGD,
+            self.AUD: Trd_Common_pb2.Currency_AUD
         }
 
 class CltRiskLevel(FtEnum):
     NONE = 'N/A'    # 未知
     SAFE = 'SAFE'   # 安全
     WARNING = 'WARNING'     # 预警
     DANGER = 'DANGER'       # 危险
@@ -2680,21 +2684,23 @@
 
 # 券商
 class SecurityFirm(FtEnum):
     NONE = 'N/A'
     FUTUSECURITIES = 'FUTUSECURITIES'
     FUTUINC = 'FUTUINC'
     FUTUSG = 'FUTUSG'
+    FUTUAU = 'FUTUAU'
 
     def load_dic(self):
         return {
             self.NONE: Trd_Common_pb2.SecurityFirm_Unknown,
             self.FUTUSECURITIES: Trd_Common_pb2.SecurityFirm_FutuSecurities,
             self.FUTUINC: Trd_Common_pb2.SecurityFirm_FutuInc,
-            self.FUTUSG: Trd_Common_pb2.SecurityFirm_FutuSG
+            self.FUTUSG: Trd_Common_pb2.SecurityFirm_FutuSG,
+            self.FUTUAU: Trd_Common_pb2.SecurityFirm_FutuAU,
         }
 
 # 模拟交易账号类型
 class SimAccType(FtEnum):
     NONE = 'N/A'
     STOCK = 'STOCK'
     OPTION = 'OPTION'
```

### Comparing `futu-api-7.1.3308/futu/common/diag.py` & `futu-api-7.2.3408/futu/common/diag.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/err.py` & `futu-api-7.2.3408/futu/common/err.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/ft_logger.py` & `futu-api-7.2.3408/futu/common/ft_logger.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/handler_context.py` & `futu-api-7.2.3408/futu/common/handler_context.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/network_manager.py` & `futu-api-7.2.3408/futu/common/network_manager.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/open_context_base.py` & `futu-api-7.2.3408/futu/common/open_context_base.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Common_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/GetDelayStatistics_pb2.py` & `futu-api-7.2.3408/futu/common/pb/GetDelayStatistics_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/GetGlobalState_pb2.py` & `futu-api-7.2.3408/futu/common/pb/GetGlobalState_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/GetUserInfo_pb2.py` & `futu-api-7.2.3408/futu/common/pb/GetUserInfo_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Common_pb2 as Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='GetUserInfo.proto',
   package='GetUserInfo',
   syntax='proto2',
-  serialized_pb=_b('\n\x11GetUserInfo.proto\x12\x0bGetUserInfo\x1a\x0c\x43ommon.proto\"\x13\n\x03\x43\x32S\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\"\xbe\x05\n\x03S2C\x12\x10\n\x08nickName\x18\x01 \x01(\t\x12\x11\n\tavatarUrl\x18\x02 \x01(\t\x12\x10\n\x08\x61piLevel\x18\x03 \x01(\t\x12\x12\n\nhkQotRight\x18\x04 \x01(\x05\x12\x12\n\nusQotRight\x18\x05 \x01(\x05\x12\x12\n\ncnQotRight\x18\x06 \x01(\x05\x12\x1d\n\x15isNeedAgreeDisclaimer\x18\x07 \x01(\x08\x12\x0e\n\x06userID\x18\x08 \x01(\x03\x12\x12\n\nupdateType\x18\t \x01(\x05\x12\x0e\n\x06webKey\x18\n \x01(\t\x12\x16\n\x0ewebJumpUrlHead\x18\x12 \x01(\t\x12\x18\n\x10hkOptionQotRight\x18\x0b \x01(\x05\x12\x1b\n\x13hasUSOptionQotRight\x18\x0c \x01(\x08\x12\x18\n\x10hkFutureQotRight\x18\r \x01(\x05\x12\x10\n\x08subQuota\x18\x0e \x01(\x05\x12\x16\n\x0ehistoryKLQuota\x18\x0f \x01(\x05\x12\x18\n\x10usFutureQotRight\x18\x10 \x01(\x05\x12\x18\n\x10usOptionQotRight\x18\x11 \x01(\x05\x12\x17\n\x0fuserAttribution\x18\x13 \x01(\x05\x12\x16\n\x0eupdateWhatsNew\x18\x14 \x01(\t\x12\x17\n\x0fusIndexQotRight\x18\x15 \x01(\x05\x12\x15\n\rusOtcQotRight\x18\x16 \x01(\x05\x12\x1b\n\x13usCMEFutureQotRight\x18\x17 \x01(\x05\x12\x1c\n\x14usCBOTFutureQotRight\x18\x18 \x01(\x05\x12\x1d\n\x15usNYMEXFutureQotRight\x18\x19 \x01(\x05\x12\x1d\n\x15usCOMEXFutureQotRight\x18\x1a \x01(\x05\x12\x1c\n\x14usCBOEFutureQotRight\x18\x1b \x01(\x05\x12\x18\n\x10sgFutureQotRight\x18\x1c \x01(\x05\x12\x18\n\x10jpFutureQotRight\x18\x1d \x01(\x05\"(\n\x07Request\x12\x1d\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x10.GetUserInfo.C2S\"a\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1d\n\x03s2c\x18\x04 \x01(\x0b\x32\x10.GetUserInfo.S2C*N\n\nUpdateType\x12\x13\n\x0fUpdateType_None\x10\x00\x12\x15\n\x11UpdateType_Advice\x10\x01\x12\x14\n\x10UpdateType_Force\x10\x02*\xae\x01\n\rUserInfoField\x12\x17\n\x13UserInfoField_Basic\x10\x01\x12\x15\n\x11UserInfoField_API\x10\x02\x12\x1a\n\x16UserInfoField_QotRight\x10\x04\x12\x1c\n\x18UserInfoField_Disclaimer\x10\x08\x12\x18\n\x14UserInfoField_Update\x10\x10\x12\x19\n\x14UserInfoField_WebKey\x10\x80\x10\x42\x42\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/getuserinfo')
+  serialized_pb=_b('\n\x11GetUserInfo.proto\x12\x0bGetUserInfo\x1a\x0c\x43ommon.proto\"\x13\n\x03\x43\x32S\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\"\xfb\x05\n\x03S2C\x12\x10\n\x08nickName\x18\x01 \x01(\t\x12\x11\n\tavatarUrl\x18\x02 \x01(\t\x12\x10\n\x08\x61piLevel\x18\x03 \x01(\t\x12\x12\n\nhkQotRight\x18\x04 \x01(\x05\x12\x12\n\nusQotRight\x18\x05 \x01(\x05\x12\x12\n\ncnQotRight\x18\x06 \x01(\x05\x12\x1d\n\x15isNeedAgreeDisclaimer\x18\x07 \x01(\x08\x12\x0e\n\x06userID\x18\x08 \x01(\x03\x12\x12\n\nupdateType\x18\t \x01(\x05\x12\x0e\n\x06webKey\x18\n \x01(\t\x12\x16\n\x0ewebJumpUrlHead\x18\x12 \x01(\t\x12\x18\n\x10hkOptionQotRight\x18\x0b \x01(\x05\x12\x1b\n\x13hasUSOptionQotRight\x18\x0c \x01(\x08\x12\x18\n\x10hkFutureQotRight\x18\r \x01(\x05\x12\x10\n\x08subQuota\x18\x0e \x01(\x05\x12\x16\n\x0ehistoryKLQuota\x18\x0f \x01(\x05\x12\x18\n\x10usFutureQotRight\x18\x10 \x01(\x05\x12\x18\n\x10usOptionQotRight\x18\x11 \x01(\x05\x12\x17\n\x0fuserAttribution\x18\x13 \x01(\x05\x12\x16\n\x0eupdateWhatsNew\x18\x14 \x01(\t\x12\x17\n\x0fusIndexQotRight\x18\x15 \x01(\x05\x12\x15\n\rusOtcQotRight\x18\x16 \x01(\x05\x12\x1b\n\x13usCMEFutureQotRight\x18\x17 \x01(\x05\x12\x1c\n\x14usCBOTFutureQotRight\x18\x18 \x01(\x05\x12\x1d\n\x15usNYMEXFutureQotRight\x18\x19 \x01(\x05\x12\x1d\n\x15usCOMEXFutureQotRight\x18\x1a \x01(\x05\x12\x1c\n\x14usCBOEFutureQotRight\x18\x1b \x01(\x05\x12\x18\n\x10sgFutureQotRight\x18\x1c \x01(\x05\x12\x18\n\x10jpFutureQotRight\x18\x1d \x01(\x05\x12\x13\n\x0bisAppNNOrMM\x18\x1e \x01(\x08\x12\x12\n\nshQotRight\x18\x1f \x01(\x05\x12\x12\n\nszQotRight\x18  \x01(\x05\"(\n\x07Request\x12\x1d\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x10.GetUserInfo.C2S\"a\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1d\n\x03s2c\x18\x04 \x01(\x0b\x32\x10.GetUserInfo.S2C*N\n\nUpdateType\x12\x13\n\x0fUpdateType_None\x10\x00\x12\x15\n\x11UpdateType_Advice\x10\x01\x12\x14\n\x10UpdateType_Force\x10\x02*\xae\x01\n\rUserInfoField\x12\x17\n\x13UserInfoField_Basic\x10\x01\x12\x15\n\x11UserInfoField_API\x10\x02\x12\x1a\n\x16UserInfoField_QotRight\x10\x04\x12\x1c\n\x18UserInfoField_Disclaimer\x10\x08\x12\x18\n\x14UserInfoField_Update\x10\x10\x12\x19\n\x14UserInfoField_WebKey\x10\x80\x10\x42\x42\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/getuserinfo')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,])
 
 _UPDATETYPE = _descriptor.EnumDescriptor(
   name='UpdateType',
   full_name='GetUserInfo.UpdateType',
   filename=None,
@@ -42,16 +42,16 @@
     _descriptor.EnumValueDescriptor(
       name='UpdateType_Force', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=915,
-  serialized_end=993,
+  serialized_start=976,
+  serialized_end=1054,
 )
 _sym_db.RegisterEnumDescriptor(_UPDATETYPE)
 
 UpdateType = enum_type_wrapper.EnumTypeWrapper(_UPDATETYPE)
 _USERINFOFIELD = _descriptor.EnumDescriptor(
   name='UserInfoField',
   full_name='GetUserInfo.UserInfoField',
@@ -81,16 +81,16 @@
     _descriptor.EnumValueDescriptor(
       name='UserInfoField_WebKey', index=5, number=2048,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=996,
-  serialized_end=1170,
+  serialized_start=1057,
+  serialized_end=1231,
 )
 _sym_db.RegisterEnumDescriptor(_USERINFOFIELD)
 
 UserInfoField = enum_type_wrapper.EnumTypeWrapper(_USERINFOFIELD)
 UpdateType_None = 0
 UpdateType_Advice = 1
 UpdateType_Force = 2
@@ -340,28 +340,49 @@
     _descriptor.FieldDescriptor(
       name='jpFutureQotRight', full_name='GetUserInfo.S2C.jpFutureQotRight', index=28,
       number=29, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='isAppNNOrMM', full_name='GetUserInfo.S2C.isAppNNOrMM', index=29,
+      number=30, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='shQotRight', full_name='GetUserInfo.S2C.shQotRight', index=30,
+      number=31, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='szQotRight', full_name='GetUserInfo.S2C.szQotRight', index=31,
+      number=32, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=70,
-  serialized_end=772,
+  serialized_end=833,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='GetUserInfo.Request',
   filename=None,
@@ -383,16 +404,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=774,
-  serialized_end=814,
+  serialized_start=835,
+  serialized_end=875,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='GetUserInfo.Response',
   filename=None,
@@ -435,16 +456,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=816,
-  serialized_end=913,
+  serialized_start=877,
+  serialized_end=974,
 )
 
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['C2S'] = _C2S
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Request'] = _REQUEST
```

### Comparing `futu-api-7.1.3308/futu/common/pb/InitConnect_pb2.py` & `futu-api-7.2.3408/futu/common/pb/InitConnect_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/KeepAlive_pb2.py` & `futu-api-7.2.3408/futu/common/pb/KeepAlive_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Notify_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Notify_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Common_pb2 as Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Notify.proto',
   package='Notify',
   syntax='proto2',
-  serialized_pb=_b('\n\x0cNotify.proto\x12\x06Notify\x1a\x0c\x43ommon.proto\"+\n\x08GtwEvent\x12\x11\n\teventType\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x02(\t\"=\n\rProgramStatus\x12,\n\rprogramStatus\x18\x01 \x02(\x0b\x32\x15.Common.ProgramStatus\"7\n\rConnectStatus\x12\x12\n\nqotLogined\x18\x01 \x02(\x08\x12\x12\n\ntrdLogined\x18\x02 \x02(\x08\"\xc6\x03\n\x08QotRight\x12\x12\n\nhkQotRight\x18\x04 \x02(\x05\x12\x12\n\nusQotRight\x18\x05 \x02(\x05\x12\x12\n\ncnQotRight\x18\x06 \x02(\x05\x12\x18\n\x10hkOptionQotRight\x18\x07 \x01(\x05\x12\x1b\n\x13hasUSOptionQotRight\x18\x08 \x01(\x08\x12\x18\n\x10hkFutureQotRight\x18\t \x01(\x05\x12\x18\n\x10usFutureQotRight\x18\n \x01(\x05\x12\x18\n\x10usOptionQotRight\x18\x0b \x01(\x05\x12\x17\n\x0fusIndexQotRight\x18\x0c \x01(\x05\x12\x15\n\rusOtcQotRight\x18\r \x01(\x05\x12\x18\n\x10sgFutureQotRight\x18\x0e \x01(\x05\x12\x18\n\x10jpFutureQotRight\x18\x0f \x01(\x05\x12\x1b\n\x13usCMEFutureQotRight\x18\x10 \x01(\x05\x12\x1c\n\x14usCBOTFutureQotRight\x18\x11 \x01(\x05\x12\x1d\n\x15usNYMEXFutureQotRight\x18\x12 \x01(\x05\x12\x1d\n\x15usCOMEXFutureQotRight\x18\x13 \x01(\x05\x12\x1c\n\x14usCBOEFutureQotRight\x18\x14 \x01(\x05\"\x1c\n\x08\x41PILevel\x12\x10\n\x08\x61piLevel\x18\x03 \x02(\t\"4\n\x08\x41PIQuota\x12\x10\n\x08subQuota\x18\x01 \x02(\x05\x12\x16\n\x0ehistoryKLQuota\x18\x02 \x02(\x05\"\xfc\x01\n\x03S2C\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12\x1f\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x10.Notify.GtwEvent\x12,\n\rprogramStatus\x18\x03 \x01(\x0b\x32\x15.Notify.ProgramStatus\x12,\n\rconnectStatus\x18\x04 \x01(\x0b\x32\x15.Notify.ConnectStatus\x12\"\n\x08qotRight\x18\x05 \x01(\x0b\x32\x10.Notify.QotRight\x12\"\n\x08\x61piLevel\x18\x06 \x01(\x0b\x32\x10.Notify.APILevel\x12\"\n\x08\x61piQuota\x18\x07 \x01(\x0b\x32\x10.Notify.APIQuota\"\\\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x18\n\x03s2c\x18\x04 \x01(\x0b\x32\x0b.Notify.S2C*\xbe\x01\n\nNotifyType\x12\x13\n\x0fNotifyType_None\x10\x00\x12\x17\n\x13NotifyType_GtwEvent\x10\x01\x12\x1c\n\x18NotifyType_ProgramStatus\x10\x02\x12\x19\n\x15NotifyType_ConnStatus\x10\x03\x12\x17\n\x13NotifyType_QotRight\x10\x04\x12\x17\n\x13NotifyType_APILevel\x10\x05\x12\x17\n\x13NotifyType_APIQuota\x10\x06*\x9b\x04\n\x0cGtwEventType\x12\x15\n\x11GtwEventType_None\x10\x00\x12#\n\x1fGtwEventType_LocalCfgLoadFailed\x10\x01\x12 \n\x1cGtwEventType_APISvrRunFailed\x10\x02\x12\x1c\n\x18GtwEventType_ForceUpdate\x10\x03\x12\x1c\n\x18GtwEventType_LoginFailed\x10\x04\x12\"\n\x1eGtwEventType_UnAgreeDisclaimer\x10\x05\x12\x1e\n\x1aGtwEventType_NetCfgMissing\x10\x06\x12\x1a\n\x16GtwEventType_KickedOut\x10\x07\x12 \n\x1cGtwEventType_LoginPwdChanged\x10\x08\x12\x19\n\x15GtwEventType_BanLogin\x10\t\x12\"\n\x1eGtwEventType_NeedPicVerifyCode\x10\n\x12$\n GtwEventType_NeedPhoneVerifyCode\x10\x0b\x12 \n\x1cGtwEventType_AppDataNotExist\x10\x0c\x12#\n\x1fGtwEventType_NessaryDataMissing\x10\r\x12 \n\x1cGtwEventType_TradePwdChanged\x10\x0e\x12!\n\x1dGtwEventType_EnableDeviceLock\x10\x0f\x42=\n\x13\x63om.futu.openapi.pbZ&github.com/futuopen/ftapi4go/pb/notify')
+  serialized_pb=_b('\n\x0cNotify.proto\x12\x06Notify\x1a\x0c\x43ommon.proto\"+\n\x08GtwEvent\x12\x11\n\teventType\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x65sc\x18\x02 \x02(\t\"=\n\rProgramStatus\x12,\n\rprogramStatus\x18\x01 \x02(\x0b\x32\x15.Common.ProgramStatus\"7\n\rConnectStatus\x12\x12\n\nqotLogined\x18\x01 \x02(\x08\x12\x12\n\ntrdLogined\x18\x02 \x02(\x08\"\xee\x03\n\x08QotRight\x12\x12\n\nhkQotRight\x18\x04 \x02(\x05\x12\x12\n\nusQotRight\x18\x05 \x02(\x05\x12\x12\n\ncnQotRight\x18\x06 \x02(\x05\x12\x18\n\x10hkOptionQotRight\x18\x07 \x01(\x05\x12\x1b\n\x13hasUSOptionQotRight\x18\x08 \x01(\x08\x12\x18\n\x10hkFutureQotRight\x18\t \x01(\x05\x12\x18\n\x10usFutureQotRight\x18\n \x01(\x05\x12\x18\n\x10usOptionQotRight\x18\x0b \x01(\x05\x12\x17\n\x0fusIndexQotRight\x18\x0c \x01(\x05\x12\x15\n\rusOtcQotRight\x18\r \x01(\x05\x12\x18\n\x10sgFutureQotRight\x18\x0e \x01(\x05\x12\x18\n\x10jpFutureQotRight\x18\x0f \x01(\x05\x12\x1b\n\x13usCMEFutureQotRight\x18\x10 \x01(\x05\x12\x1c\n\x14usCBOTFutureQotRight\x18\x11 \x01(\x05\x12\x1d\n\x15usNYMEXFutureQotRight\x18\x12 \x01(\x05\x12\x1d\n\x15usCOMEXFutureQotRight\x18\x13 \x01(\x05\x12\x1c\n\x14usCBOEFutureQotRight\x18\x14 \x01(\x05\x12\x12\n\nshQotRight\x18\x15 \x01(\x05\x12\x12\n\nszQotRight\x18\x16 \x01(\x05\"\x1c\n\x08\x41PILevel\x12\x10\n\x08\x61piLevel\x18\x03 \x02(\t\"4\n\x08\x41PIQuota\x12\x10\n\x08subQuota\x18\x01 \x02(\x05\x12\x16\n\x0ehistoryKLQuota\x18\x02 \x02(\x05\"9\n\tUsedQuota\x12\x14\n\x0cusedSubQuota\x18\x01 \x01(\x05\x12\x16\n\x0eusedKLineQuota\x18\x02 \x01(\x05\"\xa2\x02\n\x03S2C\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12\x1f\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x10.Notify.GtwEvent\x12,\n\rprogramStatus\x18\x03 \x01(\x0b\x32\x15.Notify.ProgramStatus\x12,\n\rconnectStatus\x18\x04 \x01(\x0b\x32\x15.Notify.ConnectStatus\x12\"\n\x08qotRight\x18\x05 \x01(\x0b\x32\x10.Notify.QotRight\x12\"\n\x08\x61piLevel\x18\x06 \x01(\x0b\x32\x10.Notify.APILevel\x12\"\n\x08\x61piQuota\x18\x07 \x01(\x0b\x32\x10.Notify.APIQuota\x12$\n\tusedQuota\x18\x08 \x01(\x0b\x32\x11.Notify.UsedQuota\"\\\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x18\n\x03s2c\x18\x04 \x01(\x0b\x32\x0b.Notify.S2C*\xd8\x01\n\nNotifyType\x12\x13\n\x0fNotifyType_None\x10\x00\x12\x17\n\x13NotifyType_GtwEvent\x10\x01\x12\x1c\n\x18NotifyType_ProgramStatus\x10\x02\x12\x19\n\x15NotifyType_ConnStatus\x10\x03\x12\x17\n\x13NotifyType_QotRight\x10\x04\x12\x17\n\x13NotifyType_APILevel\x10\x05\x12\x17\n\x13NotifyType_APIQuota\x10\x06\x12\x18\n\x14NotifyType_UsedQuota\x10\x07*\x9b\x04\n\x0cGtwEventType\x12\x15\n\x11GtwEventType_None\x10\x00\x12#\n\x1fGtwEventType_LocalCfgLoadFailed\x10\x01\x12 \n\x1cGtwEventType_APISvrRunFailed\x10\x02\x12\x1c\n\x18GtwEventType_ForceUpdate\x10\x03\x12\x1c\n\x18GtwEventType_LoginFailed\x10\x04\x12\"\n\x1eGtwEventType_UnAgreeDisclaimer\x10\x05\x12\x1e\n\x1aGtwEventType_NetCfgMissing\x10\x06\x12\x1a\n\x16GtwEventType_KickedOut\x10\x07\x12 \n\x1cGtwEventType_LoginPwdChanged\x10\x08\x12\x19\n\x15GtwEventType_BanLogin\x10\t\x12\"\n\x1eGtwEventType_NeedPicVerifyCode\x10\n\x12$\n GtwEventType_NeedPhoneVerifyCode\x10\x0b\x12 \n\x1cGtwEventType_AppDataNotExist\x10\x0c\x12#\n\x1fGtwEventType_NessaryDataMissing\x10\r\x12 \n\x1cGtwEventType_TradePwdChanged\x10\x0e\x12!\n\x1dGtwEventType_EnableDeviceLock\x10\x0f\x42=\n\x13\x63om.futu.openapi.pbZ&github.com/futuopen/ftapi4go/pb/notify')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,])
 
 _NOTIFYTYPE = _descriptor.EnumDescriptor(
   name='NotifyType',
   full_name='Notify.NotifyType',
   filename=None,
@@ -55,19 +55,23 @@
       name='NotifyType_APILevel', index=5, number=5,
       options=None,
       type=None),
     _descriptor.EnumValueDescriptor(
       name='NotifyType_APIQuota', index=6, number=6,
       options=None,
       type=None),
+    _descriptor.EnumValueDescriptor(
+      name='NotifyType_UsedQuota', index=7, number=7,
+      options=None,
+      type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=1094,
-  serialized_end=1284,
+  serialized_start=1231,
+  serialized_end=1447,
 )
 _sym_db.RegisterEnumDescriptor(_NOTIFYTYPE)
 
 NotifyType = enum_type_wrapper.EnumTypeWrapper(_NOTIFYTYPE)
 _GTWEVENTTYPE = _descriptor.EnumDescriptor(
   name='GtwEventType',
   full_name='Notify.GtwEventType',
@@ -137,27 +141,28 @@
     _descriptor.EnumValueDescriptor(
       name='GtwEventType_EnableDeviceLock', index=15, number=15,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=1287,
-  serialized_end=1826,
+  serialized_start=1450,
+  serialized_end=1989,
 )
 _sym_db.RegisterEnumDescriptor(_GTWEVENTTYPE)
 
 GtwEventType = enum_type_wrapper.EnumTypeWrapper(_GTWEVENTTYPE)
 NotifyType_None = 0
 NotifyType_GtwEvent = 1
 NotifyType_ProgramStatus = 2
 NotifyType_ConnStatus = 3
 NotifyType_QotRight = 4
 NotifyType_APILevel = 5
 NotifyType_APIQuota = 6
+NotifyType_UsedQuota = 7
 GtwEventType_None = 0
 GtwEventType_LocalCfgLoadFailed = 1
 GtwEventType_APISvrRunFailed = 2
 GtwEventType_ForceUpdate = 3
 GtwEventType_LoginFailed = 4
 GtwEventType_UnAgreeDisclaimer = 5
 GtwEventType_NetCfgMissing = 6
@@ -402,28 +407,42 @@
     _descriptor.FieldDescriptor(
       name='usCBOEFutureQotRight', full_name='Notify.QotRight.usCBOEFutureQotRight', index=16,
       number=20, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='shQotRight', full_name='Notify.QotRight.shQotRight', index=17,
+      number=21, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='szQotRight', full_name='Notify.QotRight.szQotRight', index=18,
+      number=22, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=204,
-  serialized_end=658,
+  serialized_end=698,
 )
 
 
 _APILEVEL = _descriptor.Descriptor(
   name='APILevel',
   full_name='Notify.APILevel',
   filename=None,
@@ -445,16 +464,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=660,
-  serialized_end=688,
+  serialized_start=700,
+  serialized_end=728,
 )
 
 
 _APIQUOTA = _descriptor.Descriptor(
   name='APIQuota',
   full_name='Notify.APIQuota',
   filename=None,
@@ -483,16 +502,54 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=690,
-  serialized_end=742,
+  serialized_start=730,
+  serialized_end=782,
+)
+
+
+_USEDQUOTA = _descriptor.Descriptor(
+  name='UsedQuota',
+  full_name='Notify.UsedQuota',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='usedSubQuota', full_name='Notify.UsedQuota.usedSubQuota', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='usedKLineQuota', full_name='Notify.UsedQuota.usedKLineQuota', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=784,
+  serialized_end=841,
 )
 
 
 _S2C = _descriptor.Descriptor(
   name='S2C',
   full_name='Notify.S2C',
   filename=None,
@@ -544,28 +601,35 @@
     _descriptor.FieldDescriptor(
       name='apiQuota', full_name='Notify.S2C.apiQuota', index=6,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='usedQuota', full_name='Notify.S2C.usedQuota', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=745,
-  serialized_end=997,
+  serialized_start=844,
+  serialized_end=1134,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Notify.Response',
   filename=None,
@@ -608,32 +672,34 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=999,
-  serialized_end=1091,
+  serialized_start=1136,
+  serialized_end=1228,
 )
 
 _PROGRAMSTATUS.fields_by_name['programStatus'].message_type = Common__pb2._PROGRAMSTATUS
 _S2C.fields_by_name['event'].message_type = _GTWEVENT
 _S2C.fields_by_name['programStatus'].message_type = _PROGRAMSTATUS
 _S2C.fields_by_name['connectStatus'].message_type = _CONNECTSTATUS
 _S2C.fields_by_name['qotRight'].message_type = _QOTRIGHT
 _S2C.fields_by_name['apiLevel'].message_type = _APILEVEL
 _S2C.fields_by_name['apiQuota'].message_type = _APIQUOTA
+_S2C.fields_by_name['usedQuota'].message_type = _USEDQUOTA
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['GtwEvent'] = _GTWEVENT
 DESCRIPTOR.message_types_by_name['ProgramStatus'] = _PROGRAMSTATUS
 DESCRIPTOR.message_types_by_name['ConnectStatus'] = _CONNECTSTATUS
 DESCRIPTOR.message_types_by_name['QotRight'] = _QOTRIGHT
 DESCRIPTOR.message_types_by_name['APILevel'] = _APILEVEL
 DESCRIPTOR.message_types_by_name['APIQuota'] = _APIQUOTA
+DESCRIPTOR.message_types_by_name['UsedQuota'] = _USEDQUOTA
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
 DESCRIPTOR.enum_types_by_name['NotifyType'] = _NOTIFYTYPE
 DESCRIPTOR.enum_types_by_name['GtwEventType'] = _GTWEVENTTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 GtwEvent = _reflection.GeneratedProtocolMessageType('GtwEvent', (_message.Message,), dict(
@@ -674,14 +740,21 @@
 APIQuota = _reflection.GeneratedProtocolMessageType('APIQuota', (_message.Message,), dict(
   DESCRIPTOR = _APIQUOTA,
   __module__ = 'Notify_pb2'
   # @@protoc_insertion_point(class_scope:Notify.APIQuota)
   ))
 _sym_db.RegisterMessage(APIQuota)
 
+UsedQuota = _reflection.GeneratedProtocolMessageType('UsedQuota', (_message.Message,), dict(
+  DESCRIPTOR = _USEDQUOTA,
+  __module__ = 'Notify_pb2'
+  # @@protoc_insertion_point(class_scope:Notify.UsedQuota)
+  ))
+_sym_db.RegisterMessage(UsedQuota)
+
 S2C = _reflection.GeneratedProtocolMessageType('S2C', (_message.Message,), dict(
   DESCRIPTOR = _S2C,
   __module__ = 'Notify_pb2'
   # @@protoc_insertion_point(class_scope:Notify.S2C)
   ))
 _sym_db.RegisterMessage(S2C)
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_Common_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_Common_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Common_pb2 as Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_Common.proto',
   package='Qot_Common',
   syntax='proto2',
-  serialized_pb=_b('\n\x10Qot_Common.proto\x12\nQot_Common\x1a\x0c\x43ommon.proto\"(\n\x08Security\x12\x0e\n\x06market\x18\x01 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x02 \x02(\t\"\xf5\x01\n\x05KLine\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x0f\n\x07isBlank\x18\x02 \x02(\x08\x12\x11\n\thighPrice\x18\x03 \x01(\x01\x12\x11\n\topenPrice\x18\x04 \x01(\x01\x12\x10\n\x08lowPrice\x18\x05 \x01(\x01\x12\x12\n\nclosePrice\x18\x06 \x01(\x01\x12\x16\n\x0elastClosePrice\x18\x07 \x01(\x01\x12\x0e\n\x06volume\x18\x08 \x01(\x03\x12\x10\n\x08turnover\x18\t \x01(\x01\x12\x14\n\x0cturnoverRate\x18\n \x01(\x01\x12\n\n\x02pe\x18\x0b \x01(\x01\x12\x12\n\nchangeRate\x18\x0c \x01(\x01\x12\x11\n\ttimestamp\x18\r \x01(\x01\"\xa2\x03\n\x14OptionBasicQotExData\x12\x13\n\x0bstrikePrice\x18\x01 \x02(\x01\x12\x14\n\x0c\x63ontractSize\x18\x02 \x02(\x05\x12\x19\n\x11\x63ontractSizeFloat\x18\x11 \x01(\x01\x12\x14\n\x0copenInterest\x18\x03 \x02(\x05\x12\x19\n\x11impliedVolatility\x18\x04 \x02(\x01\x12\x0f\n\x07premium\x18\x05 \x02(\x01\x12\r\n\x05\x64\x65lta\x18\x06 \x02(\x01\x12\r\n\x05gamma\x18\x07 \x02(\x01\x12\x0c\n\x04vega\x18\x08 \x02(\x01\x12\r\n\x05theta\x18\t \x02(\x01\x12\x0b\n\x03rho\x18\n \x02(\x01\x12\x17\n\x0fnetOpenInterest\x18\x0b \x01(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x0c \x01(\x05\x12\x1c\n\x14\x63ontractNominalValue\x18\r \x01(\x01\x12\x1a\n\x12ownerLotMultiplier\x18\x0e \x01(\x01\x12\x16\n\x0eoptionAreaType\x18\x0f \x01(\x05\x12\x1a\n\x12\x63ontractMultiplier\x18\x10 \x01(\x01\x12\x17\n\x0findexOptionType\x18\x12 \x01(\x05\"\xa4\x01\n\x12PreAfterMarketData\x12\r\n\x05price\x18\x01 \x01(\x01\x12\x11\n\thighPrice\x18\x02 \x01(\x01\x12\x10\n\x08lowPrice\x18\x03 \x01(\x01\x12\x0e\n\x06volume\x18\x04 \x01(\x03\x12\x10\n\x08turnover\x18\x05 \x01(\x01\x12\x11\n\tchangeVal\x18\x06 \x01(\x01\x12\x12\n\nchangeRate\x18\x07 \x01(\x01\x12\x11\n\tamplitude\x18\x08 \x01(\x01\"u\n\x14\x46utureBasicQotExData\x12\x17\n\x0flastSettlePrice\x18\x01 \x02(\x01\x12\x10\n\x08position\x18\x02 \x02(\x05\x12\x16\n\x0epositionChange\x18\x03 \x02(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x04 \x01(\x05\"R\n\x15WarrantBasicQotExData\x12\r\n\x05\x64\x65lta\x18\x01 \x01(\x01\x12\x19\n\x11impliedVolatility\x18\x02 \x01(\x01\x12\x0f\n\x07premium\x18\x03 \x02(\x01\"\x98\x05\n\x08\x42\x61sicQot\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x13\n\x0bisSuspended\x18\x02 \x02(\x08\x12\x10\n\x08listTime\x18\x03 \x02(\t\x12\x13\n\x0bpriceSpread\x18\x04 \x02(\x01\x12\x12\n\nupdateTime\x18\x05 \x02(\t\x12\x11\n\thighPrice\x18\x06 \x02(\x01\x12\x11\n\topenPrice\x18\x07 \x02(\x01\x12\x10\n\x08lowPrice\x18\x08 \x02(\x01\x12\x10\n\x08\x63urPrice\x18\t \x02(\x01\x12\x16\n\x0elastClosePrice\x18\n \x02(\x01\x12\x0e\n\x06volume\x18\x0b \x02(\x03\x12\x10\n\x08turnover\x18\x0c \x02(\x01\x12\x14\n\x0cturnoverRate\x18\r \x02(\x01\x12\x11\n\tamplitude\x18\x0e \x02(\x01\x12\x12\n\ndarkStatus\x18\x0f \x01(\x05\x12\x36\n\x0coptionExData\x18\x10 \x01(\x0b\x32 .Qot_Common.OptionBasicQotExData\x12\x15\n\rlistTimestamp\x18\x11 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x12 \x01(\x01\x12\x31\n\tpreMarket\x18\x13 \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x33\n\x0b\x61\x66terMarket\x18\x14 \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x11\n\tsecStatus\x18\x15 \x01(\x05\x12\x36\n\x0c\x66utureExData\x18\x16 \x01(\x0b\x32 .Qot_Common.FutureBasicQotExData\x12\x38\n\rwarrantExData\x18\x17 \x01(\x0b\x32!.Qot_Common.WarrantBasicQotExData\"\xa8\x01\n\tTimeShare\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x0e\n\x06minute\x18\x02 \x02(\x05\x12\x0f\n\x07isBlank\x18\x03 \x02(\x08\x12\r\n\x05price\x18\x04 \x01(\x01\x12\x16\n\x0elastClosePrice\x18\x05 \x01(\x01\x12\x10\n\x08\x61vgPrice\x18\x06 \x01(\x01\x12\x0e\n\x06volume\x18\x07 \x01(\x03\x12\x10\n\x08turnover\x18\x08 \x01(\x01\x12\x11\n\ttimestamp\x18\t \x01(\x01\"\xc7\x01\n\x13SecurityStaticBasic\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\n\n\x02id\x18\x02 \x02(\x03\x12\x0f\n\x07lotSize\x18\x03 \x02(\x05\x12\x0f\n\x07secType\x18\x04 \x02(\x05\x12\x0c\n\x04name\x18\x05 \x02(\t\x12\x10\n\x08listTime\x18\x06 \x02(\t\x12\x11\n\tdelisting\x18\x07 \x01(\x08\x12\x15\n\rlistTimestamp\x18\x08 \x01(\x01\x12\x10\n\x08\x65xchType\x18\t \x01(\x05\"H\n\x13WarrantStaticExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\"\xc3\x01\n\x12OptionStaticExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x12\n\nstrikeTime\x18\x03 \x02(\t\x12\x13\n\x0bstrikePrice\x18\x04 \x02(\x01\x12\x0f\n\x07suspend\x18\x05 \x02(\x08\x12\x0e\n\x06market\x18\x06 \x02(\t\x12\x17\n\x0fstrikeTimestamp\x18\x07 \x01(\x01\x12\x17\n\x0findexOptionType\x18\x08 \x01(\x05\"_\n\x12\x46utureStaticExData\x12\x15\n\rlastTradeTime\x18\x01 \x02(\t\x12\x1a\n\x12lastTradeTimestamp\x18\x02 \x01(\x01\x12\x16\n\x0eisMainContract\x18\x03 \x02(\x08\"\xe8\x01\n\x12SecurityStaticInfo\x12.\n\x05\x62\x61sic\x18\x01 \x02(\x0b\x32\x1f.Qot_Common.SecurityStaticBasic\x12\x36\n\rwarrantExData\x18\x02 \x01(\x0b\x32\x1f.Qot_Common.WarrantStaticExData\x12\x34\n\x0coptionExData\x18\x03 \x01(\x0b\x32\x1e.Qot_Common.OptionStaticExData\x12\x34\n\x0c\x66utureExData\x18\x04 \x01(\x0b\x32\x1e.Qot_Common.FutureStaticExData\"P\n\x06\x42roker\x12\n\n\x02id\x18\x01 \x02(\x03\x12\x0c\n\x04name\x18\x02 \x02(\t\x12\x0b\n\x03pos\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x01(\x03\x12\x0e\n\x06volume\x18\x05 \x01(\x03\"\xc1\x01\n\x06Ticker\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x10\n\x08sequence\x18\x02 \x02(\x03\x12\x0b\n\x03\x64ir\x18\x03 \x02(\x05\x12\r\n\x05price\x18\x04 \x02(\x01\x12\x0e\n\x06volume\x18\x05 \x02(\x03\x12\x10\n\x08turnover\x18\x06 \x02(\x01\x12\x10\n\x08recvTime\x18\x07 \x01(\x01\x12\x0c\n\x04type\x18\x08 \x01(\x05\x12\x10\n\x08typeSign\x18\t \x01(\x05\x12\x14\n\x0cpushDataType\x18\n \x01(\x05\x12\x11\n\ttimestamp\x18\x0b \x01(\x01\"2\n\x0fOrderBookDetail\x12\x0f\n\x07orderID\x18\x01 \x02(\x03\x12\x0e\n\x06volume\x18\x02 \x02(\x03\"p\n\tOrderBook\x12\r\n\x05price\x18\x01 \x02(\x01\x12\x0e\n\x06volume\x18\x02 \x02(\x03\x12\x13\n\x0borederCount\x18\x03 \x02(\x05\x12/\n\ndetailList\x18\x04 \x03(\x0b\x32\x1b.Qot_Common.OrderBookDetail\"\x9b\x01\n\x12ShareHoldingChange\x12\x12\n\nholderName\x18\x01 \x02(\t\x12\x12\n\nholdingQty\x18\x02 \x02(\x01\x12\x14\n\x0choldingRatio\x18\x03 \x02(\x01\x12\x11\n\tchangeQty\x18\x04 \x02(\x01\x12\x13\n\x0b\x63hangeRatio\x18\x05 \x02(\x01\x12\x0c\n\x04time\x18\x06 \x02(\t\x12\x11\n\ttimestamp\x18\x07 \x01(\x01\"F\n\x07SubInfo\x12\x0f\n\x07subType\x18\x01 \x02(\x05\x12*\n\x0csecurityList\x18\x02 \x03(\x0b\x32\x14.Qot_Common.Security\"a\n\x0b\x43onnSubInfo\x12(\n\x0bsubInfoList\x18\x01 \x03(\x0b\x32\x13.Qot_Common.SubInfo\x12\x11\n\tusedQuota\x18\x02 \x02(\x05\x12\x15\n\risOwnConnData\x18\x03 \x02(\x08\"Q\n\tPlateInfo\x12#\n\x05plate\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x02 \x02(\t\x12\x11\n\tplateType\x18\x03 \x01(\x05\"\xba\x03\n\x05Rehab\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x16\n\x0e\x63ompanyActFlag\x18\x02 \x02(\x03\x12\x12\n\nfwdFactorA\x18\x03 \x02(\x01\x12\x12\n\nfwdFactorB\x18\x04 \x02(\x01\x12\x12\n\nbwdFactorA\x18\x05 \x02(\x01\x12\x12\n\nbwdFactorB\x18\x06 \x02(\x01\x12\x11\n\tsplitBase\x18\x07 \x01(\x05\x12\x10\n\x08splitErt\x18\x08 \x01(\x05\x12\x10\n\x08joinBase\x18\t \x01(\x05\x12\x0f\n\x07joinErt\x18\n \x01(\x05\x12\x11\n\tbonusBase\x18\x0b \x01(\x05\x12\x10\n\x08\x62onusErt\x18\x0c \x01(\x05\x12\x14\n\x0ctransferBase\x18\r \x01(\x05\x12\x13\n\x0btransferErt\x18\x0e \x01(\x05\x12\x11\n\tallotBase\x18\x0f \x01(\x05\x12\x10\n\x08\x61llotErt\x18\x10 \x01(\x05\x12\x12\n\nallotPrice\x18\x11 \x01(\x01\x12\x0f\n\x07\x61\x64\x64\x42\x61se\x18\x12 \x01(\x05\x12\x0e\n\x06\x61\x64\x64\x45rt\x18\x13 \x01(\x05\x12\x10\n\x08\x61\x64\x64Price\x18\x14 \x01(\x01\x12\x10\n\x08\x64ividend\x18\x15 \x01(\x01\x12\x12\n\nspDividend\x18\x16 \x01(\x01\x12\x11\n\ttimestamp\x18\x17 \x01(\x01*\xe1\x01\n\tQotMarket\x12\x15\n\x11QotMarket_Unknown\x10\x00\x12\x19\n\x15QotMarket_HK_Security\x10\x01\x12\x17\n\x13QotMarket_HK_Future\x10\x02\x12\x19\n\x15QotMarket_US_Security\x10\x0b\x12\x1b\n\x17QotMarket_CNSH_Security\x10\x15\x12\x1b\n\x17QotMarket_CNSZ_Security\x10\x16\x12\x19\n\x15QotMarket_SG_Security\x10\x1f\x12\x19\n\x15QotMarket_JP_Security\x10)*\x9a\x02\n\x0cSecurityType\x12\x18\n\x14SecurityType_Unknown\x10\x00\x12\x15\n\x11SecurityType_Bond\x10\x01\x12\x15\n\x11SecurityType_Bwrt\x10\x02\x12\x15\n\x11SecurityType_Eqty\x10\x03\x12\x16\n\x12SecurityType_Trust\x10\x04\x12\x18\n\x14SecurityType_Warrant\x10\x05\x12\x16\n\x12SecurityType_Index\x10\x06\x12\x16\n\x12SecurityType_Plate\x10\x07\x12\x15\n\x11SecurityType_Drvt\x10\x08\x12\x19\n\x15SecurityType_PlateSet\x10\t\x12\x17\n\x13SecurityType_Future\x10\n*\x8a\x01\n\x0cPlateSetType\x12\x14\n\x10PlateSetType_All\x10\x00\x12\x19\n\x15PlateSetType_Industry\x10\x01\x12\x17\n\x13PlateSetType_Region\x10\x02\x12\x18\n\x14PlateSetType_Concept\x10\x03\x12\x16\n\x12PlateSetType_Other\x10\x04*\x95\x01\n\x0bWarrantType\x12\x17\n\x13WarrantType_Unknown\x10\x00\x12\x13\n\x0fWarrantType_Buy\x10\x01\x12\x14\n\x10WarrantType_Sell\x10\x02\x12\x14\n\x10WarrantType_Bull\x10\x03\x12\x14\n\x10WarrantType_Bear\x10\x04\x12\x16\n\x12WarrantType_InLine\x10\x05*M\n\nOptionType\x12\x16\n\x12OptionType_Unknown\x10\x00\x12\x13\n\x0fOptionType_Call\x10\x01\x12\x12\n\x0eOptionType_Put\x10\x02*e\n\x0fIndexOptionType\x12\x1b\n\x17IndexOptionType_Unknown\x10\x00\x12\x1a\n\x16IndexOptionType_Normal\x10\x01\x12\x19\n\x15IndexOptionType_Small\x10\x02*\x82\x01\n\x0eOptionAreaType\x12\x1a\n\x16OptionAreaType_Unknown\x10\x00\x12\x1b\n\x17OptionAreaType_American\x10\x01\x12\x1b\n\x17OptionAreaType_European\x10\x02\x12\x1a\n\x16OptionAreaType_Bermuda\x10\x03*\xa8\x07\n\x0eQotMarketState\x12\x17\n\x13QotMarketState_None\x10\x00\x12\x1a\n\x16QotMarketState_Auction\x10\x01\x12\x1e\n\x1aQotMarketState_WaitingOpen\x10\x02\x12\x1a\n\x16QotMarketState_Morning\x10\x03\x12\x17\n\x13QotMarketState_Rest\x10\x04\x12\x1c\n\x18QotMarketState_Afternoon\x10\x05\x12\x19\n\x15QotMarketState_Closed\x10\x06\x12!\n\x1dQotMarketState_PreMarketBegin\x10\x08\x12\x1f\n\x1bQotMarketState_PreMarketEnd\x10\t\x12\"\n\x1eQotMarketState_AfterHoursBegin\x10\n\x12 \n\x1cQotMarketState_AfterHoursEnd\x10\x0b\x12\x1c\n\x18QotMarketState_NightOpen\x10\r\x12\x1b\n\x17QotMarketState_NightEnd\x10\x0e\x12 \n\x1cQotMarketState_FutureDayOpen\x10\x0f\x12!\n\x1dQotMarketState_FutureDayBreak\x10\x10\x12!\n\x1dQotMarketState_FutureDayClose\x10\x11\x12\'\n#QotMarketState_FutureDayWaitForOpen\x10\x12\x12\x18\n\x14QotMarketState_HkCas\x10\x13\x12\"\n\x1eQotMarketState_FutureNightWait\x10\x14\x12\"\n\x1eQotMarketState_FutureAfternoon\x10\x15\x12#\n\x1fQotMarketState_FutureSwitchDate\x10\x16\x12\x1d\n\x19QotMarketState_FutureOpen\x10\x17\x12\x1e\n\x1aQotMarketState_FutureBreak\x10\x18\x12\"\n\x1eQotMarketState_FutureBreakOver\x10\x19\x12\x1e\n\x1aQotMarketState_FutureClose\x10\x1a\x12%\n!QotMarketState_StibAfterHoursWait\x10\x1b\x12&\n\"QotMarketState_StibAfterHoursBegin\x10\x1c\x12$\n QotMarketState_StibAfterHoursEnd\x10\x1d*\xe4\x01\n\x0fTradeDateMarket\x12\x1b\n\x17TradeDateMarket_Unknown\x10\x00\x12\x16\n\x12TradeDateMarket_HK\x10\x01\x12\x16\n\x12TradeDateMarket_US\x10\x02\x12\x16\n\x12TradeDateMarket_CN\x10\x03\x12\x16\n\x12TradeDateMarket_NT\x10\x04\x12\x16\n\x12TradeDateMarket_ST\x10\x05\x12\x1d\n\x19TradeDateMarket_JP_Future\x10\x06\x12\x1d\n\x19TradeDateMarket_SG_Future\x10\x07*`\n\rTradeDateType\x12\x17\n\x13TradeDateType_Whole\x10\x00\x12\x19\n\x15TradeDateType_Morning\x10\x01\x12\x1b\n\x17TradeDateType_Afternoon\x10\x02*N\n\tRehabType\x12\x12\n\x0eRehabType_None\x10\x00\x12\x15\n\x11RehabType_Forward\x10\x01\x12\x16\n\x12RehabType_Backward\x10\x02*\xdd\x01\n\x06KLType\x12\x12\n\x0eKLType_Unknown\x10\x00\x12\x0f\n\x0bKLType_1Min\x10\x01\x12\x0e\n\nKLType_Day\x10\x02\x12\x0f\n\x0bKLType_Week\x10\x03\x12\x10\n\x0cKLType_Month\x10\x04\x12\x0f\n\x0bKLType_Year\x10\x05\x12\x0f\n\x0bKLType_5Min\x10\x06\x12\x10\n\x0cKLType_15Min\x10\x07\x12\x10\n\x0cKLType_30Min\x10\x08\x12\x10\n\x0cKLType_60Min\x10\t\x12\x0f\n\x0bKLType_3Min\x10\n\x12\x12\n\x0eKLType_Quarter\x10\x0b*\xf5\x01\n\x08KLFields\x12\x11\n\rKLFields_None\x10\x00\x12\x11\n\rKLFields_High\x10\x01\x12\x11\n\rKLFields_Open\x10\x02\x12\x10\n\x0cKLFields_Low\x10\x04\x12\x12\n\x0eKLFields_Close\x10\x08\x12\x16\n\x12KLFields_LastClose\x10\x10\x12\x13\n\x0fKLFields_Volume\x10 \x12\x15\n\x11KLFields_Turnover\x10@\x12\x1a\n\x15KLFields_TurnoverRate\x10\x80\x01\x12\x10\n\x0bKLFields_PE\x10\x80\x02\x12\x18\n\x13KLFields_ChangeRate\x10\x80\x04*\xea\x02\n\x07SubType\x12\x10\n\x0cSubType_None\x10\x00\x12\x11\n\rSubType_Basic\x10\x01\x12\x15\n\x11SubType_OrderBook\x10\x02\x12\x12\n\x0eSubType_Ticker\x10\x04\x12\x0e\n\nSubType_RT\x10\x05\x12\x12\n\x0eSubType_KL_Day\x10\x06\x12\x13\n\x0fSubType_KL_5Min\x10\x07\x12\x14\n\x10SubType_KL_15Min\x10\x08\x12\x14\n\x10SubType_KL_30Min\x10\t\x12\x14\n\x10SubType_KL_60Min\x10\n\x12\x13\n\x0fSubType_KL_1Min\x10\x0b\x12\x13\n\x0fSubType_KL_Week\x10\x0c\x12\x14\n\x10SubType_KL_Month\x10\r\x12\x12\n\x0eSubType_Broker\x10\x0e\x12\x16\n\x12SubType_KL_Qurater\x10\x0f\x12\x13\n\x0fSubType_KL_Year\x10\x10\x12\x13\n\x0fSubType_KL_3Min\x10\x11*}\n\x0fTickerDirection\x12\x1b\n\x17TickerDirection_Unknown\x10\x00\x12\x17\n\x13TickerDirection_Bid\x10\x01\x12\x17\n\x13TickerDirection_Ask\x10\x02\x12\x1b\n\x17TickerDirection_Neutral\x10\x03*\x9c\x07\n\nTickerType\x12\x16\n\x12TickerType_Unknown\x10\x00\x12\x18\n\x14TickerType_Automatch\x10\x01\x12\x13\n\x0fTickerType_Late\x10\x02\x12\x1c\n\x18TickerType_NoneAutomatch\x10\x03\x12\x1d\n\x19TickerType_InterAutomatch\x10\x04\x12!\n\x1dTickerType_InterNoneAutomatch\x10\x05\x12\x15\n\x11TickerType_OddLot\x10\x06\x12\x16\n\x12TickerType_Auction\x10\x07\x12\x13\n\x0fTickerType_Bulk\x10\x08\x12\x14\n\x10TickerType_Crash\x10\t\x12\x1a\n\x16TickerType_CrossMarket\x10\n\x12\x17\n\x13TickerType_BulkSold\x10\x0b\x12\x1a\n\x16TickerType_FreeOnBoard\x10\x0c\x12\x1b\n\x17TickerType_Rule127Or155\x10\r\x12\x14\n\x10TickerType_Delay\x10\x0e\x12%\n!TickerType_MarketCenterClosePrice\x10\x0f\x12\x16\n\x12TickerType_NextDay\x10\x10\x12\"\n\x1eTickerType_MarketCenterOpening\x10\x11\x12\"\n\x1eTickerType_PriorReferencePrice\x10\x12\x12$\n TickerType_MarketCenterOpenPrice\x10\x13\x12\x15\n\x11TickerType_Seller\x10\x14\x12\x10\n\x0cTickerType_T\x10\x15\x12#\n\x1fTickerType_ExtendedTradingHours\x10\x16\x12\x19\n\x15TickerType_Contingent\x10\x17\x12\x17\n\x13TickerType_AvgPrice\x10\x18\x12\x16\n\x12TickerType_OTCSold\x10\x19\x12 \n\x1cTickerType_OddLotCrossMarket\x10\x1a\x12!\n\x1dTickerType_DerivativelyPriced\x10\x1b\x12\x1e\n\x1aTickerType_ReOpeningPriced\x10\x1c\x12\x1c\n\x18TickerType_ClosingPriced\x10\x1d\x12&\n\"TickerType_ComprehensiveDelayPrice\x10\x1e\x12\x17\n\x13TickerType_Overseas\x10\x1f*M\n\nDarkStatus\x12\x13\n\x0f\x44\x61rkStatus_None\x10\x00\x12\x16\n\x12\x44\x61rkStatus_Trading\x10\x01\x12\x12\n\x0e\x44\x61rkStatus_End\x10\x02*\x94\x06\n\x0eSecurityStatus\x12\x1a\n\x16SecurityStatus_Unknown\x10\x00\x12\x19\n\x15SecurityStatus_Normal\x10\x01\x12\x1a\n\x16SecurityStatus_Listing\x10\x02\x12\x1d\n\x19SecurityStatus_Purchasing\x10\x03\x12\x1e\n\x1aSecurityStatus_Subscribing\x10\x04\x12)\n%SecurityStatus_BeforeDrakTradeOpening\x10\x05\x12\x1e\n\x1aSecurityStatus_DrakTrading\x10\x06\x12\x1f\n\x1bSecurityStatus_DrakTradeEnd\x10\x07\x12\x1b\n\x17SecurityStatus_ToBeOpen\x10\x08\x12\x1c\n\x18SecurityStatus_Suspended\x10\t\x12\x19\n\x15SecurityStatus_Called\x10\n\x12)\n%SecurityStatus_ExpiredLastTradingDate\x10\x0b\x12\x1a\n\x16SecurityStatus_Expired\x10\x0c\x12\x1b\n\x17SecurityStatus_Delisted\x10\r\x12(\n$SecurityStatus_ChangeToTemporaryCode\x10\x0e\x12(\n$SecurityStatus_TemporaryCodeTradeEnd\x10\x0f\x12\'\n#SecurityStatus_ChangedPlateTradeEnd\x10\x10\x12&\n\"SecurityStatus_ChangedCodeTradeEnd\x10\x11\x12,\n(SecurityStatus_RecoverableCircuitBreaker\x10\x12\x12.\n*SecurityStatus_UnRecoverableCircuitBreaker\x10\x13\x12#\n\x1fSecurityStatus_AfterCombination\x10\x14\x12\"\n\x1eSecurityStatus_AfterTransation\x10\x15*\x81\x01\n\x0eHolderCategory\x12\x19\n\x15HolderCategory_Unknow\x10\x00\x12\x19\n\x15HolderCategory_Agency\x10\x01\x12\x17\n\x13HolderCategory_Fund\x10\x02\x12 \n\x1cHolderCategory_SeniorManager\x10\x03*v\n\x0cPushDataType\x12\x17\n\x13PushDataType_Unknow\x10\x00\x12\x19\n\x15PushDataType_Realtime\x10\x01\x12\x1a\n\x16PushDataType_ByDisConn\x10\x02\x12\x16\n\x12PushDataType_Cache\x10\x03*\xd3\n\n\tSortField\x12\x14\n\x10SortField_Unknow\x10\x00\x12\x12\n\x0eSortField_Code\x10\x01\x12\x16\n\x12SortField_CurPrice\x10\x02\x12\x1c\n\x18SortField_PriceChangeVal\x10\x03\x12\x18\n\x14SortField_ChangeRate\x10\x04\x12\x14\n\x10SortField_Status\x10\x05\x12\x16\n\x12SortField_BidPrice\x10\x06\x12\x16\n\x12SortField_AskPrice\x10\x07\x12\x14\n\x10SortField_BidVol\x10\x08\x12\x14\n\x10SortField_AskVol\x10\t\x12\x14\n\x10SortField_Volume\x10\n\x12\x16\n\x12SortField_Turnover\x10\x0b\x12\x17\n\x13SortField_Amplitude\x10\x1e\x12\x13\n\x0fSortField_Score\x10\x0c\x12\x15\n\x11SortField_Premium\x10\r\x12\x1f\n\x1bSortField_EffectiveLeverage\x10\x0e\x12\x13\n\x0fSortField_Delta\x10\x0f\x12\x1f\n\x1bSortField_ImpliedVolatility\x10\x10\x12\x12\n\x0eSortField_Type\x10\x11\x12\x19\n\x15SortField_StrikePrice\x10\x12\x12\x1c\n\x18SortField_BreakEvenPoint\x10\x13\x12\x1a\n\x16SortField_MaturityTime\x10\x14\x12\x16\n\x12SortField_ListTime\x10\x15\x12\x1b\n\x17SortField_LastTradeTime\x10\x16\x12\x16\n\x12SortField_Leverage\x10\x17\x12\x18\n\x14SortField_InOutMoney\x10\x18\x12\x1b\n\x17SortField_RecoveryPrice\x10\x19\x12\x19\n\x15SortField_ChangePrice\x10\x1a\x12\x14\n\x10SortField_Change\x10\x1b\x12\x18\n\x14SortField_StreetRate\x10\x1c\x12\x17\n\x13SortField_StreetVol\x10\x1d\x12\x19\n\x15SortField_WarrantName\x10\x1f\x12\x14\n\x10SortField_Issuer\x10 \x12\x15\n\x11SortField_LotSize\x10!\x12\x17\n\x13SortField_IssueSize\x10\"\x12\x1e\n\x1aSortField_UpperStrikePrice\x10-\x12\x1e\n\x1aSortField_LowerStrikePrice\x10.\x12\x1f\n\x1bSortField_InLinePriceStatus\x10/\x12\x19\n\x15SortField_PreCurPrice\x10#\x12\x1b\n\x17SortField_AfterCurPrice\x10$\x12\x1f\n\x1bSortField_PrePriceChangeVal\x10%\x12!\n\x1dSortField_AfterPriceChangeVal\x10&\x12\x1b\n\x17SortField_PreChangeRate\x10\'\x12\x1d\n\x19SortField_AfterChangeRate\x10(\x12\x1a\n\x16SortField_PreAmplitude\x10)\x12\x1c\n\x18SortField_AfterAmplitude\x10*\x12\x19\n\x15SortField_PreTurnover\x10+\x12\x1b\n\x17SortField_AfterTurnover\x10,\x12\x1d\n\x19SortField_LastSettlePrice\x10\x30\x12\x16\n\x12SortField_Position\x10\x31\x12\x1c\n\x18SortField_PositionChange\x10\x32*\x92\x03\n\x06Issuer\x12\x11\n\rIssuer_Unknow\x10\x00\x12\r\n\tIssuer_SG\x10\x01\x12\r\n\tIssuer_BP\x10\x02\x12\r\n\tIssuer_CS\x10\x03\x12\r\n\tIssuer_CT\x10\x04\x12\r\n\tIssuer_EA\x10\x05\x12\r\n\tIssuer_GS\x10\x06\x12\r\n\tIssuer_HS\x10\x07\x12\r\n\tIssuer_JP\x10\x08\x12\r\n\tIssuer_MB\x10\t\x12\r\n\tIssuer_SC\x10\n\x12\r\n\tIssuer_UB\x10\x0b\x12\r\n\tIssuer_BI\x10\x0c\x12\r\n\tIssuer_DB\x10\r\x12\r\n\tIssuer_DC\x10\x0e\x12\r\n\tIssuer_ML\x10\x0f\x12\r\n\tIssuer_NM\x10\x10\x12\r\n\tIssuer_RB\x10\x11\x12\r\n\tIssuer_RS\x10\x12\x12\r\n\tIssuer_BC\x10\x13\x12\r\n\tIssuer_HT\x10\x14\x12\r\n\tIssuer_VT\x10\x15\x12\r\n\tIssuer_KC\x10\x16\x12\r\n\tIssuer_MS\x10\x17\x12\r\n\tIssuer_GJ\x10\x18\x12\r\n\tIssuer_XZ\x10\x19*\x97\x01\n\tIpoPeriod\x12\x14\n\x10IpoPeriod_Unknow\x10\x00\x12\x13\n\x0fIpoPeriod_Today\x10\x01\x12\x16\n\x12IpoPeriod_Tomorrow\x10\x02\x12\x16\n\x12IpoPeriod_Nextweek\x10\x03\x12\x16\n\x12IpoPeriod_Lastweek\x10\x04\x12\x17\n\x13IpoPeriod_Lastmonth\x10\x05*N\n\tPriceType\x12\x14\n\x10PriceType_Unknow\x10\x00\x12\x15\n\x11PriceType_Outside\x10\x01\x12\x14\n\x10PriceType_WithIn\x10\x02*\x9d\x01\n\rWarrantStatus\x12\x18\n\x14WarrantStatus_Unknow\x10\x00\x12\x18\n\x14WarrantStatus_Normal\x10\x01\x12\x19\n\x15WarrantStatus_Suspend\x10\x02\x12\x1b\n\x17WarrantStatus_StopTrade\x10\x03\x12 \n\x1cWarrantStatus_PendingListing\x10\x04*\xda\x01\n\nCompanyAct\x12\x13\n\x0f\x43ompanyAct_None\x10\x00\x12\x14\n\x10\x43ompanyAct_Split\x10\x01\x12\x13\n\x0f\x43ompanyAct_Join\x10\x02\x12\x14\n\x10\x43ompanyAct_Bonus\x10\x04\x12\x17\n\x13\x43ompanyAct_Transfer\x10\x08\x12\x14\n\x10\x43ompanyAct_Allot\x10\x10\x12\x12\n\x0e\x43ompanyAct_Add\x10 \x12\x17\n\x13\x43ompanyAct_Dividend\x10@\x12\x1a\n\x15\x43ompanyAct_SPDividend\x10\x80\x01*}\n\x08QotRight\x12\x13\n\x0fQotRight_Unknow\x10\x00\x12\x10\n\x0cQotRight_Bmp\x10\x01\x12\x13\n\x0fQotRight_Level1\x10\x02\x12\x13\n\x0fQotRight_Level2\x10\x03\x12\x0f\n\x0bQotRight_SF\x10\x04\x12\x0f\n\x0bQotRight_No\x10\x05*\xce\x04\n\x11PriceReminderType\x12\x1d\n\x19PriceReminderType_Unknown\x10\x00\x12\x1d\n\x19PriceReminderType_PriceUp\x10\x01\x12\x1f\n\x1bPriceReminderType_PriceDown\x10\x02\x12\"\n\x1ePriceReminderType_ChangeRateUp\x10\x03\x12$\n PriceReminderType_ChangeRateDown\x10\x04\x12&\n\"PriceReminderType_5MinChangeRateUp\x10\x05\x12(\n$PriceReminderType_5MinChangeRateDown\x10\x06\x12\x1e\n\x1aPriceReminderType_VolumeUp\x10\x07\x12 \n\x1cPriceReminderType_TurnoverUp\x10\x08\x12$\n PriceReminderType_TurnoverRateUp\x10\t\x12 \n\x1cPriceReminderType_BidPriceUp\x10\n\x12\"\n\x1ePriceReminderType_AskPriceDown\x10\x0b\x12\x1e\n\x1aPriceReminderType_BidVolUp\x10\x0c\x12\x1e\n\x1aPriceReminderType_AskVolUp\x10\r\x12&\n\"PriceReminderType_3MinChangeRateUp\x10\x0e\x12(\n$PriceReminderType_3MinChangeRateDown\x10\x0f*\x90\x01\n\x11PriceReminderFreq\x12\x1d\n\x19PriceReminderFreq_Unknown\x10\x00\x12\x1c\n\x18PriceReminderFreq_Always\x10\x01\x12\x1e\n\x1aPriceReminderFreq_OnceADay\x10\x02\x12\x1e\n\x1aPriceReminderFreq_OnlyOnce\x10\x03*\xb3\x01\n\nAssetClass\x12\x15\n\x11\x41ssetClass_Unknow\x10\x00\x12\x14\n\x10\x41ssetClass_Stock\x10\x01\x12\x13\n\x0f\x41ssetClass_Bond\x10\x02\x12\x18\n\x14\x41ssetClass_Commodity\x10\x03\x12\x1d\n\x19\x41ssetClass_CurrencyMarket\x10\x04\x12\x15\n\x11\x41ssetClass_Future\x10\x05\x12\x13\n\x0f\x41ssetClass_Swap\x10\x06*c\n\x0f\x45xpirationCycle\x12\x1b\n\x17\x45xpirationCycle_Unknown\x10\x00\x12\x18\n\x14\x45xpirationCycle_Week\x10\x01\x12\x19\n\x15\x45xpirationCycle_Month\x10\x02*\xb4\x03\n\x08\x45xchType\x12\x14\n\x10\x45xchType_Unknown\x10\x00\x12\x19\n\x15\x45xchType_HK_MainBoard\x10\x01\x12\x18\n\x14\x45xchType_HK_GEMBoard\x10\x02\x12\x14\n\x10\x45xchType_HK_HKEX\x10\x03\x12\x14\n\x10\x45xchType_US_NYSE\x10\x04\x12\x16\n\x12\x45xchType_US_Nasdaq\x10\x05\x12\x14\n\x10\x45xchType_US_Pink\x10\x06\x12\x14\n\x10\x45xchType_US_AMEX\x10\x07\x12\x16\n\x12\x45xchType_US_Option\x10\x08\x12\x15\n\x11\x45xchType_US_NYMEX\x10\t\x12\x15\n\x11\x45xchType_US_COMEX\x10\n\x12\x14\n\x10\x45xchType_US_CBOT\x10\x0b\x12\x13\n\x0f\x45xchType_US_CME\x10\x0c\x12\x14\n\x10\x45xchType_US_CBOE\x10\r\x12\x12\n\x0e\x45xchType_CN_SH\x10\x0e\x12\x12\n\x0e\x45xchType_CN_SZ\x10\x0f\x12\x14\n\x10\x45xchType_CN_STIB\x10\x10\x12\x13\n\x0f\x45xchType_SG_SGX\x10\x11\x12\x13\n\x0f\x45xchType_JP_OSE\x10\x12*|\n\nPeriodType\x12\x16\n\x12PeriodType_Unknown\x10\x00\x12\x17\n\x13PeriodType_INTRADAY\x10\x01\x12\x12\n\x0ePeriodType_DAY\x10\x02\x12\x13\n\x0fPeriodType_WEEK\x10\x03\x12\x14\n\x10PeriodType_MONTH\x10\x04\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/qotcommon')
+  serialized_pb=_b('\n\x10Qot_Common.proto\x12\nQot_Common\x1a\x0c\x43ommon.proto\"(\n\x08Security\x12\x0e\n\x06market\x18\x01 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x02 \x02(\t\"\xf5\x01\n\x05KLine\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x0f\n\x07isBlank\x18\x02 \x02(\x08\x12\x11\n\thighPrice\x18\x03 \x01(\x01\x12\x11\n\topenPrice\x18\x04 \x01(\x01\x12\x10\n\x08lowPrice\x18\x05 \x01(\x01\x12\x12\n\nclosePrice\x18\x06 \x01(\x01\x12\x16\n\x0elastClosePrice\x18\x07 \x01(\x01\x12\x0e\n\x06volume\x18\x08 \x01(\x03\x12\x10\n\x08turnover\x18\t \x01(\x01\x12\x14\n\x0cturnoverRate\x18\n \x01(\x01\x12\n\n\x02pe\x18\x0b \x01(\x01\x12\x12\n\nchangeRate\x18\x0c \x01(\x01\x12\x11\n\ttimestamp\x18\r \x01(\x01\"\xa2\x03\n\x14OptionBasicQotExData\x12\x13\n\x0bstrikePrice\x18\x01 \x02(\x01\x12\x14\n\x0c\x63ontractSize\x18\x02 \x02(\x05\x12\x19\n\x11\x63ontractSizeFloat\x18\x11 \x01(\x01\x12\x14\n\x0copenInterest\x18\x03 \x02(\x05\x12\x19\n\x11impliedVolatility\x18\x04 \x02(\x01\x12\x0f\n\x07premium\x18\x05 \x02(\x01\x12\r\n\x05\x64\x65lta\x18\x06 \x02(\x01\x12\r\n\x05gamma\x18\x07 \x02(\x01\x12\x0c\n\x04vega\x18\x08 \x02(\x01\x12\r\n\x05theta\x18\t \x02(\x01\x12\x0b\n\x03rho\x18\n \x02(\x01\x12\x17\n\x0fnetOpenInterest\x18\x0b \x01(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x0c \x01(\x05\x12\x1c\n\x14\x63ontractNominalValue\x18\r \x01(\x01\x12\x1a\n\x12ownerLotMultiplier\x18\x0e \x01(\x01\x12\x16\n\x0eoptionAreaType\x18\x0f \x01(\x05\x12\x1a\n\x12\x63ontractMultiplier\x18\x10 \x01(\x01\x12\x17\n\x0findexOptionType\x18\x12 \x01(\x05\"\xa4\x01\n\x12PreAfterMarketData\x12\r\n\x05price\x18\x01 \x01(\x01\x12\x11\n\thighPrice\x18\x02 \x01(\x01\x12\x10\n\x08lowPrice\x18\x03 \x01(\x01\x12\x0e\n\x06volume\x18\x04 \x01(\x03\x12\x10\n\x08turnover\x18\x05 \x01(\x01\x12\x11\n\tchangeVal\x18\x06 \x01(\x01\x12\x12\n\nchangeRate\x18\x07 \x01(\x01\x12\x11\n\tamplitude\x18\x08 \x01(\x01\"u\n\x14\x46utureBasicQotExData\x12\x17\n\x0flastSettlePrice\x18\x01 \x02(\x01\x12\x10\n\x08position\x18\x02 \x02(\x05\x12\x16\n\x0epositionChange\x18\x03 \x02(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x04 \x01(\x05\"R\n\x15WarrantBasicQotExData\x12\r\n\x05\x64\x65lta\x18\x01 \x01(\x01\x12\x19\n\x11impliedVolatility\x18\x02 \x01(\x01\x12\x0f\n\x07premium\x18\x03 \x02(\x01\"\xa6\x05\n\x08\x42\x61sicQot\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x18 \x01(\t\x12\x13\n\x0bisSuspended\x18\x02 \x02(\x08\x12\x10\n\x08listTime\x18\x03 \x02(\t\x12\x13\n\x0bpriceSpread\x18\x04 \x02(\x01\x12\x12\n\nupdateTime\x18\x05 \x02(\t\x12\x11\n\thighPrice\x18\x06 \x02(\x01\x12\x11\n\topenPrice\x18\x07 \x02(\x01\x12\x10\n\x08lowPrice\x18\x08 \x02(\x01\x12\x10\n\x08\x63urPrice\x18\t \x02(\x01\x12\x16\n\x0elastClosePrice\x18\n \x02(\x01\x12\x0e\n\x06volume\x18\x0b \x02(\x03\x12\x10\n\x08turnover\x18\x0c \x02(\x01\x12\x14\n\x0cturnoverRate\x18\r \x02(\x01\x12\x11\n\tamplitude\x18\x0e \x02(\x01\x12\x12\n\ndarkStatus\x18\x0f \x01(\x05\x12\x36\n\x0coptionExData\x18\x10 \x01(\x0b\x32 .Qot_Common.OptionBasicQotExData\x12\x15\n\rlistTimestamp\x18\x11 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x12 \x01(\x01\x12\x31\n\tpreMarket\x18\x13 \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x33\n\x0b\x61\x66terMarket\x18\x14 \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x11\n\tsecStatus\x18\x15 \x01(\x05\x12\x36\n\x0c\x66utureExData\x18\x16 \x01(\x0b\x32 .Qot_Common.FutureBasicQotExData\x12\x38\n\rwarrantExData\x18\x17 \x01(\x0b\x32!.Qot_Common.WarrantBasicQotExData\"\xa8\x01\n\tTimeShare\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x0e\n\x06minute\x18\x02 \x02(\x05\x12\x0f\n\x07isBlank\x18\x03 \x02(\x08\x12\r\n\x05price\x18\x04 \x01(\x01\x12\x16\n\x0elastClosePrice\x18\x05 \x01(\x01\x12\x10\n\x08\x61vgPrice\x18\x06 \x01(\x01\x12\x0e\n\x06volume\x18\x07 \x01(\x03\x12\x10\n\x08turnover\x18\x08 \x01(\x01\x12\x11\n\ttimestamp\x18\t \x01(\x01\"\xc7\x01\n\x13SecurityStaticBasic\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\n\n\x02id\x18\x02 \x02(\x03\x12\x0f\n\x07lotSize\x18\x03 \x02(\x05\x12\x0f\n\x07secType\x18\x04 \x02(\x05\x12\x0c\n\x04name\x18\x05 \x02(\t\x12\x10\n\x08listTime\x18\x06 \x02(\t\x12\x11\n\tdelisting\x18\x07 \x01(\x08\x12\x15\n\rlistTimestamp\x18\x08 \x01(\x01\x12\x10\n\x08\x65xchType\x18\t \x01(\x05\"H\n\x13WarrantStaticExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\"\xc3\x01\n\x12OptionStaticExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x12\n\nstrikeTime\x18\x03 \x02(\t\x12\x13\n\x0bstrikePrice\x18\x04 \x02(\x01\x12\x0f\n\x07suspend\x18\x05 \x02(\x08\x12\x0e\n\x06market\x18\x06 \x02(\t\x12\x17\n\x0fstrikeTimestamp\x18\x07 \x01(\x01\x12\x17\n\x0findexOptionType\x18\x08 \x01(\x05\"_\n\x12\x46utureStaticExData\x12\x15\n\rlastTradeTime\x18\x01 \x02(\t\x12\x1a\n\x12lastTradeTimestamp\x18\x02 \x01(\x01\x12\x16\n\x0eisMainContract\x18\x03 \x02(\x08\"\xe8\x01\n\x12SecurityStaticInfo\x12.\n\x05\x62\x61sic\x18\x01 \x02(\x0b\x32\x1f.Qot_Common.SecurityStaticBasic\x12\x36\n\rwarrantExData\x18\x02 \x01(\x0b\x32\x1f.Qot_Common.WarrantStaticExData\x12\x34\n\x0coptionExData\x18\x03 \x01(\x0b\x32\x1e.Qot_Common.OptionStaticExData\x12\x34\n\x0c\x66utureExData\x18\x04 \x01(\x0b\x32\x1e.Qot_Common.FutureStaticExData\"P\n\x06\x42roker\x12\n\n\x02id\x18\x01 \x02(\x03\x12\x0c\n\x04name\x18\x02 \x02(\t\x12\x0b\n\x03pos\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x01(\x03\x12\x0e\n\x06volume\x18\x05 \x01(\x03\"\xc1\x01\n\x06Ticker\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x10\n\x08sequence\x18\x02 \x02(\x03\x12\x0b\n\x03\x64ir\x18\x03 \x02(\x05\x12\r\n\x05price\x18\x04 \x02(\x01\x12\x0e\n\x06volume\x18\x05 \x02(\x03\x12\x10\n\x08turnover\x18\x06 \x02(\x01\x12\x10\n\x08recvTime\x18\x07 \x01(\x01\x12\x0c\n\x04type\x18\x08 \x01(\x05\x12\x10\n\x08typeSign\x18\t \x01(\x05\x12\x14\n\x0cpushDataType\x18\n \x01(\x05\x12\x11\n\ttimestamp\x18\x0b \x01(\x01\"2\n\x0fOrderBookDetail\x12\x0f\n\x07orderID\x18\x01 \x02(\x03\x12\x0e\n\x06volume\x18\x02 \x02(\x03\"p\n\tOrderBook\x12\r\n\x05price\x18\x01 \x02(\x01\x12\x0e\n\x06volume\x18\x02 \x02(\x03\x12\x13\n\x0borederCount\x18\x03 \x02(\x05\x12/\n\ndetailList\x18\x04 \x03(\x0b\x32\x1b.Qot_Common.OrderBookDetail\"\x9b\x01\n\x12ShareHoldingChange\x12\x12\n\nholderName\x18\x01 \x02(\t\x12\x12\n\nholdingQty\x18\x02 \x02(\x01\x12\x14\n\x0choldingRatio\x18\x03 \x02(\x01\x12\x11\n\tchangeQty\x18\x04 \x02(\x01\x12\x13\n\x0b\x63hangeRatio\x18\x05 \x02(\x01\x12\x0c\n\x04time\x18\x06 \x02(\t\x12\x11\n\ttimestamp\x18\x07 \x01(\x01\"F\n\x07SubInfo\x12\x0f\n\x07subType\x18\x01 \x02(\x05\x12*\n\x0csecurityList\x18\x02 \x03(\x0b\x32\x14.Qot_Common.Security\"a\n\x0b\x43onnSubInfo\x12(\n\x0bsubInfoList\x18\x01 \x03(\x0b\x32\x13.Qot_Common.SubInfo\x12\x11\n\tusedQuota\x18\x02 \x02(\x05\x12\x15\n\risOwnConnData\x18\x03 \x02(\x08\"Q\n\tPlateInfo\x12#\n\x05plate\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x02 \x02(\t\x12\x11\n\tplateType\x18\x03 \x01(\x05\"\xba\x03\n\x05Rehab\x12\x0c\n\x04time\x18\x01 \x02(\t\x12\x16\n\x0e\x63ompanyActFlag\x18\x02 \x02(\x03\x12\x12\n\nfwdFactorA\x18\x03 \x02(\x01\x12\x12\n\nfwdFactorB\x18\x04 \x02(\x01\x12\x12\n\nbwdFactorA\x18\x05 \x02(\x01\x12\x12\n\nbwdFactorB\x18\x06 \x02(\x01\x12\x11\n\tsplitBase\x18\x07 \x01(\x05\x12\x10\n\x08splitErt\x18\x08 \x01(\x05\x12\x10\n\x08joinBase\x18\t \x01(\x05\x12\x0f\n\x07joinErt\x18\n \x01(\x05\x12\x11\n\tbonusBase\x18\x0b \x01(\x05\x12\x10\n\x08\x62onusErt\x18\x0c \x01(\x05\x12\x14\n\x0ctransferBase\x18\r \x01(\x05\x12\x13\n\x0btransferErt\x18\x0e \x01(\x05\x12\x11\n\tallotBase\x18\x0f \x01(\x05\x12\x10\n\x08\x61llotErt\x18\x10 \x01(\x05\x12\x12\n\nallotPrice\x18\x11 \x01(\x01\x12\x0f\n\x07\x61\x64\x64\x42\x61se\x18\x12 \x01(\x05\x12\x0e\n\x06\x61\x64\x64\x45rt\x18\x13 \x01(\x05\x12\x10\n\x08\x61\x64\x64Price\x18\x14 \x01(\x01\x12\x10\n\x08\x64ividend\x18\x15 \x01(\x01\x12\x12\n\nspDividend\x18\x16 \x01(\x01\x12\x11\n\ttimestamp\x18\x17 \x01(\x01*\xe1\x01\n\tQotMarket\x12\x15\n\x11QotMarket_Unknown\x10\x00\x12\x19\n\x15QotMarket_HK_Security\x10\x01\x12\x17\n\x13QotMarket_HK_Future\x10\x02\x12\x19\n\x15QotMarket_US_Security\x10\x0b\x12\x1b\n\x17QotMarket_CNSH_Security\x10\x15\x12\x1b\n\x17QotMarket_CNSZ_Security\x10\x16\x12\x19\n\x15QotMarket_SG_Security\x10\x1f\x12\x19\n\x15QotMarket_JP_Security\x10)*\x9a\x02\n\x0cSecurityType\x12\x18\n\x14SecurityType_Unknown\x10\x00\x12\x15\n\x11SecurityType_Bond\x10\x01\x12\x15\n\x11SecurityType_Bwrt\x10\x02\x12\x15\n\x11SecurityType_Eqty\x10\x03\x12\x16\n\x12SecurityType_Trust\x10\x04\x12\x18\n\x14SecurityType_Warrant\x10\x05\x12\x16\n\x12SecurityType_Index\x10\x06\x12\x16\n\x12SecurityType_Plate\x10\x07\x12\x15\n\x11SecurityType_Drvt\x10\x08\x12\x19\n\x15SecurityType_PlateSet\x10\t\x12\x17\n\x13SecurityType_Future\x10\n*\x8a\x01\n\x0cPlateSetType\x12\x14\n\x10PlateSetType_All\x10\x00\x12\x19\n\x15PlateSetType_Industry\x10\x01\x12\x17\n\x13PlateSetType_Region\x10\x02\x12\x18\n\x14PlateSetType_Concept\x10\x03\x12\x16\n\x12PlateSetType_Other\x10\x04*\x95\x01\n\x0bWarrantType\x12\x17\n\x13WarrantType_Unknown\x10\x00\x12\x13\n\x0fWarrantType_Buy\x10\x01\x12\x14\n\x10WarrantType_Sell\x10\x02\x12\x14\n\x10WarrantType_Bull\x10\x03\x12\x14\n\x10WarrantType_Bear\x10\x04\x12\x16\n\x12WarrantType_InLine\x10\x05*M\n\nOptionType\x12\x16\n\x12OptionType_Unknown\x10\x00\x12\x13\n\x0fOptionType_Call\x10\x01\x12\x12\n\x0eOptionType_Put\x10\x02*e\n\x0fIndexOptionType\x12\x1b\n\x17IndexOptionType_Unknown\x10\x00\x12\x1a\n\x16IndexOptionType_Normal\x10\x01\x12\x19\n\x15IndexOptionType_Small\x10\x02*\x82\x01\n\x0eOptionAreaType\x12\x1a\n\x16OptionAreaType_Unknown\x10\x00\x12\x1b\n\x17OptionAreaType_American\x10\x01\x12\x1b\n\x17OptionAreaType_European\x10\x02\x12\x1a\n\x16OptionAreaType_Bermuda\x10\x03*\xa8\x07\n\x0eQotMarketState\x12\x17\n\x13QotMarketState_None\x10\x00\x12\x1a\n\x16QotMarketState_Auction\x10\x01\x12\x1e\n\x1aQotMarketState_WaitingOpen\x10\x02\x12\x1a\n\x16QotMarketState_Morning\x10\x03\x12\x17\n\x13QotMarketState_Rest\x10\x04\x12\x1c\n\x18QotMarketState_Afternoon\x10\x05\x12\x19\n\x15QotMarketState_Closed\x10\x06\x12!\n\x1dQotMarketState_PreMarketBegin\x10\x08\x12\x1f\n\x1bQotMarketState_PreMarketEnd\x10\t\x12\"\n\x1eQotMarketState_AfterHoursBegin\x10\n\x12 \n\x1cQotMarketState_AfterHoursEnd\x10\x0b\x12\x1c\n\x18QotMarketState_NightOpen\x10\r\x12\x1b\n\x17QotMarketState_NightEnd\x10\x0e\x12 \n\x1cQotMarketState_FutureDayOpen\x10\x0f\x12!\n\x1dQotMarketState_FutureDayBreak\x10\x10\x12!\n\x1dQotMarketState_FutureDayClose\x10\x11\x12\'\n#QotMarketState_FutureDayWaitForOpen\x10\x12\x12\x18\n\x14QotMarketState_HkCas\x10\x13\x12\"\n\x1eQotMarketState_FutureNightWait\x10\x14\x12\"\n\x1eQotMarketState_FutureAfternoon\x10\x15\x12#\n\x1fQotMarketState_FutureSwitchDate\x10\x16\x12\x1d\n\x19QotMarketState_FutureOpen\x10\x17\x12\x1e\n\x1aQotMarketState_FutureBreak\x10\x18\x12\"\n\x1eQotMarketState_FutureBreakOver\x10\x19\x12\x1e\n\x1aQotMarketState_FutureClose\x10\x1a\x12%\n!QotMarketState_StibAfterHoursWait\x10\x1b\x12&\n\"QotMarketState_StibAfterHoursBegin\x10\x1c\x12$\n QotMarketState_StibAfterHoursEnd\x10\x1d*\xe4\x01\n\x0fTradeDateMarket\x12\x1b\n\x17TradeDateMarket_Unknown\x10\x00\x12\x16\n\x12TradeDateMarket_HK\x10\x01\x12\x16\n\x12TradeDateMarket_US\x10\x02\x12\x16\n\x12TradeDateMarket_CN\x10\x03\x12\x16\n\x12TradeDateMarket_NT\x10\x04\x12\x16\n\x12TradeDateMarket_ST\x10\x05\x12\x1d\n\x19TradeDateMarket_JP_Future\x10\x06\x12\x1d\n\x19TradeDateMarket_SG_Future\x10\x07*`\n\rTradeDateType\x12\x17\n\x13TradeDateType_Whole\x10\x00\x12\x19\n\x15TradeDateType_Morning\x10\x01\x12\x1b\n\x17TradeDateType_Afternoon\x10\x02*N\n\tRehabType\x12\x12\n\x0eRehabType_None\x10\x00\x12\x15\n\x11RehabType_Forward\x10\x01\x12\x16\n\x12RehabType_Backward\x10\x02*\xdd\x01\n\x06KLType\x12\x12\n\x0eKLType_Unknown\x10\x00\x12\x0f\n\x0bKLType_1Min\x10\x01\x12\x0e\n\nKLType_Day\x10\x02\x12\x0f\n\x0bKLType_Week\x10\x03\x12\x10\n\x0cKLType_Month\x10\x04\x12\x0f\n\x0bKLType_Year\x10\x05\x12\x0f\n\x0bKLType_5Min\x10\x06\x12\x10\n\x0cKLType_15Min\x10\x07\x12\x10\n\x0cKLType_30Min\x10\x08\x12\x10\n\x0cKLType_60Min\x10\t\x12\x0f\n\x0bKLType_3Min\x10\n\x12\x12\n\x0eKLType_Quarter\x10\x0b*\xf5\x01\n\x08KLFields\x12\x11\n\rKLFields_None\x10\x00\x12\x11\n\rKLFields_High\x10\x01\x12\x11\n\rKLFields_Open\x10\x02\x12\x10\n\x0cKLFields_Low\x10\x04\x12\x12\n\x0eKLFields_Close\x10\x08\x12\x16\n\x12KLFields_LastClose\x10\x10\x12\x13\n\x0fKLFields_Volume\x10 \x12\x15\n\x11KLFields_Turnover\x10@\x12\x1a\n\x15KLFields_TurnoverRate\x10\x80\x01\x12\x10\n\x0bKLFields_PE\x10\x80\x02\x12\x18\n\x13KLFields_ChangeRate\x10\x80\x04*\xea\x02\n\x07SubType\x12\x10\n\x0cSubType_None\x10\x00\x12\x11\n\rSubType_Basic\x10\x01\x12\x15\n\x11SubType_OrderBook\x10\x02\x12\x12\n\x0eSubType_Ticker\x10\x04\x12\x0e\n\nSubType_RT\x10\x05\x12\x12\n\x0eSubType_KL_Day\x10\x06\x12\x13\n\x0fSubType_KL_5Min\x10\x07\x12\x14\n\x10SubType_KL_15Min\x10\x08\x12\x14\n\x10SubType_KL_30Min\x10\t\x12\x14\n\x10SubType_KL_60Min\x10\n\x12\x13\n\x0fSubType_KL_1Min\x10\x0b\x12\x13\n\x0fSubType_KL_Week\x10\x0c\x12\x14\n\x10SubType_KL_Month\x10\r\x12\x12\n\x0eSubType_Broker\x10\x0e\x12\x16\n\x12SubType_KL_Qurater\x10\x0f\x12\x13\n\x0fSubType_KL_Year\x10\x10\x12\x13\n\x0fSubType_KL_3Min\x10\x11*}\n\x0fTickerDirection\x12\x1b\n\x17TickerDirection_Unknown\x10\x00\x12\x17\n\x13TickerDirection_Bid\x10\x01\x12\x17\n\x13TickerDirection_Ask\x10\x02\x12\x1b\n\x17TickerDirection_Neutral\x10\x03*\x9c\x07\n\nTickerType\x12\x16\n\x12TickerType_Unknown\x10\x00\x12\x18\n\x14TickerType_Automatch\x10\x01\x12\x13\n\x0fTickerType_Late\x10\x02\x12\x1c\n\x18TickerType_NoneAutomatch\x10\x03\x12\x1d\n\x19TickerType_InterAutomatch\x10\x04\x12!\n\x1dTickerType_InterNoneAutomatch\x10\x05\x12\x15\n\x11TickerType_OddLot\x10\x06\x12\x16\n\x12TickerType_Auction\x10\x07\x12\x13\n\x0fTickerType_Bulk\x10\x08\x12\x14\n\x10TickerType_Crash\x10\t\x12\x1a\n\x16TickerType_CrossMarket\x10\n\x12\x17\n\x13TickerType_BulkSold\x10\x0b\x12\x1a\n\x16TickerType_FreeOnBoard\x10\x0c\x12\x1b\n\x17TickerType_Rule127Or155\x10\r\x12\x14\n\x10TickerType_Delay\x10\x0e\x12%\n!TickerType_MarketCenterClosePrice\x10\x0f\x12\x16\n\x12TickerType_NextDay\x10\x10\x12\"\n\x1eTickerType_MarketCenterOpening\x10\x11\x12\"\n\x1eTickerType_PriorReferencePrice\x10\x12\x12$\n TickerType_MarketCenterOpenPrice\x10\x13\x12\x15\n\x11TickerType_Seller\x10\x14\x12\x10\n\x0cTickerType_T\x10\x15\x12#\n\x1fTickerType_ExtendedTradingHours\x10\x16\x12\x19\n\x15TickerType_Contingent\x10\x17\x12\x17\n\x13TickerType_AvgPrice\x10\x18\x12\x16\n\x12TickerType_OTCSold\x10\x19\x12 \n\x1cTickerType_OddLotCrossMarket\x10\x1a\x12!\n\x1dTickerType_DerivativelyPriced\x10\x1b\x12\x1e\n\x1aTickerType_ReOpeningPriced\x10\x1c\x12\x1c\n\x18TickerType_ClosingPriced\x10\x1d\x12&\n\"TickerType_ComprehensiveDelayPrice\x10\x1e\x12\x17\n\x13TickerType_Overseas\x10\x1f*M\n\nDarkStatus\x12\x13\n\x0f\x44\x61rkStatus_None\x10\x00\x12\x16\n\x12\x44\x61rkStatus_Trading\x10\x01\x12\x12\n\x0e\x44\x61rkStatus_End\x10\x02*\x94\x06\n\x0eSecurityStatus\x12\x1a\n\x16SecurityStatus_Unknown\x10\x00\x12\x19\n\x15SecurityStatus_Normal\x10\x01\x12\x1a\n\x16SecurityStatus_Listing\x10\x02\x12\x1d\n\x19SecurityStatus_Purchasing\x10\x03\x12\x1e\n\x1aSecurityStatus_Subscribing\x10\x04\x12)\n%SecurityStatus_BeforeDrakTradeOpening\x10\x05\x12\x1e\n\x1aSecurityStatus_DrakTrading\x10\x06\x12\x1f\n\x1bSecurityStatus_DrakTradeEnd\x10\x07\x12\x1b\n\x17SecurityStatus_ToBeOpen\x10\x08\x12\x1c\n\x18SecurityStatus_Suspended\x10\t\x12\x19\n\x15SecurityStatus_Called\x10\n\x12)\n%SecurityStatus_ExpiredLastTradingDate\x10\x0b\x12\x1a\n\x16SecurityStatus_Expired\x10\x0c\x12\x1b\n\x17SecurityStatus_Delisted\x10\r\x12(\n$SecurityStatus_ChangeToTemporaryCode\x10\x0e\x12(\n$SecurityStatus_TemporaryCodeTradeEnd\x10\x0f\x12\'\n#SecurityStatus_ChangedPlateTradeEnd\x10\x10\x12&\n\"SecurityStatus_ChangedCodeTradeEnd\x10\x11\x12,\n(SecurityStatus_RecoverableCircuitBreaker\x10\x12\x12.\n*SecurityStatus_UnRecoverableCircuitBreaker\x10\x13\x12#\n\x1fSecurityStatus_AfterCombination\x10\x14\x12\"\n\x1eSecurityStatus_AfterTransation\x10\x15*\x81\x01\n\x0eHolderCategory\x12\x19\n\x15HolderCategory_Unknow\x10\x00\x12\x19\n\x15HolderCategory_Agency\x10\x01\x12\x17\n\x13HolderCategory_Fund\x10\x02\x12 \n\x1cHolderCategory_SeniorManager\x10\x03*v\n\x0cPushDataType\x12\x17\n\x13PushDataType_Unknow\x10\x00\x12\x19\n\x15PushDataType_Realtime\x10\x01\x12\x1a\n\x16PushDataType_ByDisConn\x10\x02\x12\x16\n\x12PushDataType_Cache\x10\x03*\xd3\n\n\tSortField\x12\x14\n\x10SortField_Unknow\x10\x00\x12\x12\n\x0eSortField_Code\x10\x01\x12\x16\n\x12SortField_CurPrice\x10\x02\x12\x1c\n\x18SortField_PriceChangeVal\x10\x03\x12\x18\n\x14SortField_ChangeRate\x10\x04\x12\x14\n\x10SortField_Status\x10\x05\x12\x16\n\x12SortField_BidPrice\x10\x06\x12\x16\n\x12SortField_AskPrice\x10\x07\x12\x14\n\x10SortField_BidVol\x10\x08\x12\x14\n\x10SortField_AskVol\x10\t\x12\x14\n\x10SortField_Volume\x10\n\x12\x16\n\x12SortField_Turnover\x10\x0b\x12\x17\n\x13SortField_Amplitude\x10\x1e\x12\x13\n\x0fSortField_Score\x10\x0c\x12\x15\n\x11SortField_Premium\x10\r\x12\x1f\n\x1bSortField_EffectiveLeverage\x10\x0e\x12\x13\n\x0fSortField_Delta\x10\x0f\x12\x1f\n\x1bSortField_ImpliedVolatility\x10\x10\x12\x12\n\x0eSortField_Type\x10\x11\x12\x19\n\x15SortField_StrikePrice\x10\x12\x12\x1c\n\x18SortField_BreakEvenPoint\x10\x13\x12\x1a\n\x16SortField_MaturityTime\x10\x14\x12\x16\n\x12SortField_ListTime\x10\x15\x12\x1b\n\x17SortField_LastTradeTime\x10\x16\x12\x16\n\x12SortField_Leverage\x10\x17\x12\x18\n\x14SortField_InOutMoney\x10\x18\x12\x1b\n\x17SortField_RecoveryPrice\x10\x19\x12\x19\n\x15SortField_ChangePrice\x10\x1a\x12\x14\n\x10SortField_Change\x10\x1b\x12\x18\n\x14SortField_StreetRate\x10\x1c\x12\x17\n\x13SortField_StreetVol\x10\x1d\x12\x19\n\x15SortField_WarrantName\x10\x1f\x12\x14\n\x10SortField_Issuer\x10 \x12\x15\n\x11SortField_LotSize\x10!\x12\x17\n\x13SortField_IssueSize\x10\"\x12\x1e\n\x1aSortField_UpperStrikePrice\x10-\x12\x1e\n\x1aSortField_LowerStrikePrice\x10.\x12\x1f\n\x1bSortField_InLinePriceStatus\x10/\x12\x19\n\x15SortField_PreCurPrice\x10#\x12\x1b\n\x17SortField_AfterCurPrice\x10$\x12\x1f\n\x1bSortField_PrePriceChangeVal\x10%\x12!\n\x1dSortField_AfterPriceChangeVal\x10&\x12\x1b\n\x17SortField_PreChangeRate\x10\'\x12\x1d\n\x19SortField_AfterChangeRate\x10(\x12\x1a\n\x16SortField_PreAmplitude\x10)\x12\x1c\n\x18SortField_AfterAmplitude\x10*\x12\x19\n\x15SortField_PreTurnover\x10+\x12\x1b\n\x17SortField_AfterTurnover\x10,\x12\x1d\n\x19SortField_LastSettlePrice\x10\x30\x12\x16\n\x12SortField_Position\x10\x31\x12\x1c\n\x18SortField_PositionChange\x10\x32*\x92\x03\n\x06Issuer\x12\x11\n\rIssuer_Unknow\x10\x00\x12\r\n\tIssuer_SG\x10\x01\x12\r\n\tIssuer_BP\x10\x02\x12\r\n\tIssuer_CS\x10\x03\x12\r\n\tIssuer_CT\x10\x04\x12\r\n\tIssuer_EA\x10\x05\x12\r\n\tIssuer_GS\x10\x06\x12\r\n\tIssuer_HS\x10\x07\x12\r\n\tIssuer_JP\x10\x08\x12\r\n\tIssuer_MB\x10\t\x12\r\n\tIssuer_SC\x10\n\x12\r\n\tIssuer_UB\x10\x0b\x12\r\n\tIssuer_BI\x10\x0c\x12\r\n\tIssuer_DB\x10\r\x12\r\n\tIssuer_DC\x10\x0e\x12\r\n\tIssuer_ML\x10\x0f\x12\r\n\tIssuer_NM\x10\x10\x12\r\n\tIssuer_RB\x10\x11\x12\r\n\tIssuer_RS\x10\x12\x12\r\n\tIssuer_BC\x10\x13\x12\r\n\tIssuer_HT\x10\x14\x12\r\n\tIssuer_VT\x10\x15\x12\r\n\tIssuer_KC\x10\x16\x12\r\n\tIssuer_MS\x10\x17\x12\r\n\tIssuer_GJ\x10\x18\x12\r\n\tIssuer_XZ\x10\x19*\x97\x01\n\tIpoPeriod\x12\x14\n\x10IpoPeriod_Unknow\x10\x00\x12\x13\n\x0fIpoPeriod_Today\x10\x01\x12\x16\n\x12IpoPeriod_Tomorrow\x10\x02\x12\x16\n\x12IpoPeriod_Nextweek\x10\x03\x12\x16\n\x12IpoPeriod_Lastweek\x10\x04\x12\x17\n\x13IpoPeriod_Lastmonth\x10\x05*N\n\tPriceType\x12\x14\n\x10PriceType_Unknow\x10\x00\x12\x15\n\x11PriceType_Outside\x10\x01\x12\x14\n\x10PriceType_WithIn\x10\x02*\x9d\x01\n\rWarrantStatus\x12\x18\n\x14WarrantStatus_Unknow\x10\x00\x12\x18\n\x14WarrantStatus_Normal\x10\x01\x12\x19\n\x15WarrantStatus_Suspend\x10\x02\x12\x1b\n\x17WarrantStatus_StopTrade\x10\x03\x12 \n\x1cWarrantStatus_PendingListing\x10\x04*\xda\x01\n\nCompanyAct\x12\x13\n\x0f\x43ompanyAct_None\x10\x00\x12\x14\n\x10\x43ompanyAct_Split\x10\x01\x12\x13\n\x0f\x43ompanyAct_Join\x10\x02\x12\x14\n\x10\x43ompanyAct_Bonus\x10\x04\x12\x17\n\x13\x43ompanyAct_Transfer\x10\x08\x12\x14\n\x10\x43ompanyAct_Allot\x10\x10\x12\x12\n\x0e\x43ompanyAct_Add\x10 \x12\x17\n\x13\x43ompanyAct_Dividend\x10@\x12\x1a\n\x15\x43ompanyAct_SPDividend\x10\x80\x01*}\n\x08QotRight\x12\x13\n\x0fQotRight_Unknow\x10\x00\x12\x10\n\x0cQotRight_Bmp\x10\x01\x12\x13\n\x0fQotRight_Level1\x10\x02\x12\x13\n\x0fQotRight_Level2\x10\x03\x12\x0f\n\x0bQotRight_SF\x10\x04\x12\x0f\n\x0bQotRight_No\x10\x05*\xce\x04\n\x11PriceReminderType\x12\x1d\n\x19PriceReminderType_Unknown\x10\x00\x12\x1d\n\x19PriceReminderType_PriceUp\x10\x01\x12\x1f\n\x1bPriceReminderType_PriceDown\x10\x02\x12\"\n\x1ePriceReminderType_ChangeRateUp\x10\x03\x12$\n PriceReminderType_ChangeRateDown\x10\x04\x12&\n\"PriceReminderType_5MinChangeRateUp\x10\x05\x12(\n$PriceReminderType_5MinChangeRateDown\x10\x06\x12\x1e\n\x1aPriceReminderType_VolumeUp\x10\x07\x12 \n\x1cPriceReminderType_TurnoverUp\x10\x08\x12$\n PriceReminderType_TurnoverRateUp\x10\t\x12 \n\x1cPriceReminderType_BidPriceUp\x10\n\x12\"\n\x1ePriceReminderType_AskPriceDown\x10\x0b\x12\x1e\n\x1aPriceReminderType_BidVolUp\x10\x0c\x12\x1e\n\x1aPriceReminderType_AskVolUp\x10\r\x12&\n\"PriceReminderType_3MinChangeRateUp\x10\x0e\x12(\n$PriceReminderType_3MinChangeRateDown\x10\x0f*\x90\x01\n\x11PriceReminderFreq\x12\x1d\n\x19PriceReminderFreq_Unknown\x10\x00\x12\x1c\n\x18PriceReminderFreq_Always\x10\x01\x12\x1e\n\x1aPriceReminderFreq_OnceADay\x10\x02\x12\x1e\n\x1aPriceReminderFreq_OnlyOnce\x10\x03*\xb3\x01\n\nAssetClass\x12\x15\n\x11\x41ssetClass_Unknow\x10\x00\x12\x14\n\x10\x41ssetClass_Stock\x10\x01\x12\x13\n\x0f\x41ssetClass_Bond\x10\x02\x12\x18\n\x14\x41ssetClass_Commodity\x10\x03\x12\x1d\n\x19\x41ssetClass_CurrencyMarket\x10\x04\x12\x15\n\x11\x41ssetClass_Future\x10\x05\x12\x13\n\x0f\x41ssetClass_Swap\x10\x06*c\n\x0f\x45xpirationCycle\x12\x1b\n\x17\x45xpirationCycle_Unknown\x10\x00\x12\x18\n\x14\x45xpirationCycle_Week\x10\x01\x12\x19\n\x15\x45xpirationCycle_Month\x10\x02*\xb4\x03\n\x08\x45xchType\x12\x14\n\x10\x45xchType_Unknown\x10\x00\x12\x19\n\x15\x45xchType_HK_MainBoard\x10\x01\x12\x18\n\x14\x45xchType_HK_GEMBoard\x10\x02\x12\x14\n\x10\x45xchType_HK_HKEX\x10\x03\x12\x14\n\x10\x45xchType_US_NYSE\x10\x04\x12\x16\n\x12\x45xchType_US_Nasdaq\x10\x05\x12\x14\n\x10\x45xchType_US_Pink\x10\x06\x12\x14\n\x10\x45xchType_US_AMEX\x10\x07\x12\x16\n\x12\x45xchType_US_Option\x10\x08\x12\x15\n\x11\x45xchType_US_NYMEX\x10\t\x12\x15\n\x11\x45xchType_US_COMEX\x10\n\x12\x14\n\x10\x45xchType_US_CBOT\x10\x0b\x12\x13\n\x0f\x45xchType_US_CME\x10\x0c\x12\x14\n\x10\x45xchType_US_CBOE\x10\r\x12\x12\n\x0e\x45xchType_CN_SH\x10\x0e\x12\x12\n\x0e\x45xchType_CN_SZ\x10\x0f\x12\x14\n\x10\x45xchType_CN_STIB\x10\x10\x12\x13\n\x0f\x45xchType_SG_SGX\x10\x11\x12\x13\n\x0f\x45xchType_JP_OSE\x10\x12*|\n\nPeriodType\x12\x16\n\x12PeriodType_Unknown\x10\x00\x12\x17\n\x13PeriodType_INTRADAY\x10\x01\x12\x12\n\x0ePeriodType_DAY\x10\x02\x12\x13\n\x0fPeriodType_WEEK\x10\x03\x12\x14\n\x10PeriodType_MONTH\x10\x04\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/qotcommon')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,])
 
 _QOTMARKET = _descriptor.EnumDescriptor(
   name='QotMarket',
   full_name='Qot_Common.QotMarket',
   filename=None,
@@ -62,16 +62,16 @@
     _descriptor.EnumValueDescriptor(
       name='QotMarket_JP_Security', index=7, number=41,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4073,
-  serialized_end=4298,
+  serialized_start=4087,
+  serialized_end=4312,
 )
 _sym_db.RegisterEnumDescriptor(_QOTMARKET)
 
 QotMarket = enum_type_wrapper.EnumTypeWrapper(_QOTMARKET)
 _SECURITYTYPE = _descriptor.EnumDescriptor(
   name='SecurityType',
   full_name='Qot_Common.SecurityType',
@@ -121,16 +121,16 @@
     _descriptor.EnumValueDescriptor(
       name='SecurityType_Future', index=10, number=10,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4301,
-  serialized_end=4583,
+  serialized_start=4315,
+  serialized_end=4597,
 )
 _sym_db.RegisterEnumDescriptor(_SECURITYTYPE)
 
 SecurityType = enum_type_wrapper.EnumTypeWrapper(_SECURITYTYPE)
 _PLATESETTYPE = _descriptor.EnumDescriptor(
   name='PlateSetType',
   full_name='Qot_Common.PlateSetType',
@@ -156,16 +156,16 @@
     _descriptor.EnumValueDescriptor(
       name='PlateSetType_Other', index=4, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4586,
-  serialized_end=4724,
+  serialized_start=4600,
+  serialized_end=4738,
 )
 _sym_db.RegisterEnumDescriptor(_PLATESETTYPE)
 
 PlateSetType = enum_type_wrapper.EnumTypeWrapper(_PLATESETTYPE)
 _WARRANTTYPE = _descriptor.EnumDescriptor(
   name='WarrantType',
   full_name='Qot_Common.WarrantType',
@@ -195,16 +195,16 @@
     _descriptor.EnumValueDescriptor(
       name='WarrantType_InLine', index=5, number=5,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4727,
-  serialized_end=4876,
+  serialized_start=4741,
+  serialized_end=4890,
 )
 _sym_db.RegisterEnumDescriptor(_WARRANTTYPE)
 
 WarrantType = enum_type_wrapper.EnumTypeWrapper(_WARRANTTYPE)
 _OPTIONTYPE = _descriptor.EnumDescriptor(
   name='OptionType',
   full_name='Qot_Common.OptionType',
@@ -222,16 +222,16 @@
     _descriptor.EnumValueDescriptor(
       name='OptionType_Put', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4878,
-  serialized_end=4955,
+  serialized_start=4892,
+  serialized_end=4969,
 )
 _sym_db.RegisterEnumDescriptor(_OPTIONTYPE)
 
 OptionType = enum_type_wrapper.EnumTypeWrapper(_OPTIONTYPE)
 _INDEXOPTIONTYPE = _descriptor.EnumDescriptor(
   name='IndexOptionType',
   full_name='Qot_Common.IndexOptionType',
@@ -249,16 +249,16 @@
     _descriptor.EnumValueDescriptor(
       name='IndexOptionType_Small', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4957,
-  serialized_end=5058,
+  serialized_start=4971,
+  serialized_end=5072,
 )
 _sym_db.RegisterEnumDescriptor(_INDEXOPTIONTYPE)
 
 IndexOptionType = enum_type_wrapper.EnumTypeWrapper(_INDEXOPTIONTYPE)
 _OPTIONAREATYPE = _descriptor.EnumDescriptor(
   name='OptionAreaType',
   full_name='Qot_Common.OptionAreaType',
@@ -280,16 +280,16 @@
     _descriptor.EnumValueDescriptor(
       name='OptionAreaType_Bermuda', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5061,
-  serialized_end=5191,
+  serialized_start=5075,
+  serialized_end=5205,
 )
 _sym_db.RegisterEnumDescriptor(_OPTIONAREATYPE)
 
 OptionAreaType = enum_type_wrapper.EnumTypeWrapper(_OPTIONAREATYPE)
 _QOTMARKETSTATE = _descriptor.EnumDescriptor(
   name='QotMarketState',
   full_name='Qot_Common.QotMarketState',
@@ -407,16 +407,16 @@
     _descriptor.EnumValueDescriptor(
       name='QotMarketState_StibAfterHoursEnd', index=27, number=29,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5194,
-  serialized_end=6130,
+  serialized_start=5208,
+  serialized_end=6144,
 )
 _sym_db.RegisterEnumDescriptor(_QOTMARKETSTATE)
 
 QotMarketState = enum_type_wrapper.EnumTypeWrapper(_QOTMARKETSTATE)
 _TRADEDATEMARKET = _descriptor.EnumDescriptor(
   name='TradeDateMarket',
   full_name='Qot_Common.TradeDateMarket',
@@ -454,16 +454,16 @@
     _descriptor.EnumValueDescriptor(
       name='TradeDateMarket_SG_Future', index=7, number=7,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=6133,
-  serialized_end=6361,
+  serialized_start=6147,
+  serialized_end=6375,
 )
 _sym_db.RegisterEnumDescriptor(_TRADEDATEMARKET)
 
 TradeDateMarket = enum_type_wrapper.EnumTypeWrapper(_TRADEDATEMARKET)
 _TRADEDATETYPE = _descriptor.EnumDescriptor(
   name='TradeDateType',
   full_name='Qot_Common.TradeDateType',
@@ -481,16 +481,16 @@
     _descriptor.EnumValueDescriptor(
       name='TradeDateType_Afternoon', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=6363,
-  serialized_end=6459,
+  serialized_start=6377,
+  serialized_end=6473,
 )
 _sym_db.RegisterEnumDescriptor(_TRADEDATETYPE)
 
 TradeDateType = enum_type_wrapper.EnumTypeWrapper(_TRADEDATETYPE)
 _REHABTYPE = _descriptor.EnumDescriptor(
   name='RehabType',
   full_name='Qot_Common.RehabType',
@@ -508,16 +508,16 @@
     _descriptor.EnumValueDescriptor(
       name='RehabType_Backward', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=6461,
-  serialized_end=6539,
+  serialized_start=6475,
+  serialized_end=6553,
 )
 _sym_db.RegisterEnumDescriptor(_REHABTYPE)
 
 RehabType = enum_type_wrapper.EnumTypeWrapper(_REHABTYPE)
 _KLTYPE = _descriptor.EnumDescriptor(
   name='KLType',
   full_name='Qot_Common.KLType',
@@ -571,16 +571,16 @@
     _descriptor.EnumValueDescriptor(
       name='KLType_Quarter', index=11, number=11,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=6542,
-  serialized_end=6763,
+  serialized_start=6556,
+  serialized_end=6777,
 )
 _sym_db.RegisterEnumDescriptor(_KLTYPE)
 
 KLType = enum_type_wrapper.EnumTypeWrapper(_KLTYPE)
 _KLFIELDS = _descriptor.EnumDescriptor(
   name='KLFields',
   full_name='Qot_Common.KLFields',
@@ -630,16 +630,16 @@
     _descriptor.EnumValueDescriptor(
       name='KLFields_ChangeRate', index=10, number=512,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=6766,
-  serialized_end=7011,
+  serialized_start=6780,
+  serialized_end=7025,
 )
 _sym_db.RegisterEnumDescriptor(_KLFIELDS)
 
 KLFields = enum_type_wrapper.EnumTypeWrapper(_KLFIELDS)
 _SUBTYPE = _descriptor.EnumDescriptor(
   name='SubType',
   full_name='Qot_Common.SubType',
@@ -713,16 +713,16 @@
     _descriptor.EnumValueDescriptor(
       name='SubType_KL_3Min', index=16, number=17,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=7014,
-  serialized_end=7376,
+  serialized_start=7028,
+  serialized_end=7390,
 )
 _sym_db.RegisterEnumDescriptor(_SUBTYPE)
 
 SubType = enum_type_wrapper.EnumTypeWrapper(_SUBTYPE)
 _TICKERDIRECTION = _descriptor.EnumDescriptor(
   name='TickerDirection',
   full_name='Qot_Common.TickerDirection',
@@ -744,16 +744,16 @@
     _descriptor.EnumValueDescriptor(
       name='TickerDirection_Neutral', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=7378,
-  serialized_end=7503,
+  serialized_start=7392,
+  serialized_end=7517,
 )
 _sym_db.RegisterEnumDescriptor(_TICKERDIRECTION)
 
 TickerDirection = enum_type_wrapper.EnumTypeWrapper(_TICKERDIRECTION)
 _TICKERTYPE = _descriptor.EnumDescriptor(
   name='TickerType',
   full_name='Qot_Common.TickerType',
@@ -887,16 +887,16 @@
     _descriptor.EnumValueDescriptor(
       name='TickerType_Overseas', index=31, number=31,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=7506,
-  serialized_end=8430,
+  serialized_start=7520,
+  serialized_end=8444,
 )
 _sym_db.RegisterEnumDescriptor(_TICKERTYPE)
 
 TickerType = enum_type_wrapper.EnumTypeWrapper(_TICKERTYPE)
 _DARKSTATUS = _descriptor.EnumDescriptor(
   name='DarkStatus',
   full_name='Qot_Common.DarkStatus',
@@ -914,16 +914,16 @@
     _descriptor.EnumValueDescriptor(
       name='DarkStatus_End', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=8432,
-  serialized_end=8509,
+  serialized_start=8446,
+  serialized_end=8523,
 )
 _sym_db.RegisterEnumDescriptor(_DARKSTATUS)
 
 DarkStatus = enum_type_wrapper.EnumTypeWrapper(_DARKSTATUS)
 _SECURITYSTATUS = _descriptor.EnumDescriptor(
   name='SecurityStatus',
   full_name='Qot_Common.SecurityStatus',
@@ -1017,16 +1017,16 @@
     _descriptor.EnumValueDescriptor(
       name='SecurityStatus_AfterTransation', index=21, number=21,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=8512,
-  serialized_end=9300,
+  serialized_start=8526,
+  serialized_end=9314,
 )
 _sym_db.RegisterEnumDescriptor(_SECURITYSTATUS)
 
 SecurityStatus = enum_type_wrapper.EnumTypeWrapper(_SECURITYSTATUS)
 _HOLDERCATEGORY = _descriptor.EnumDescriptor(
   name='HolderCategory',
   full_name='Qot_Common.HolderCategory',
@@ -1048,16 +1048,16 @@
     _descriptor.EnumValueDescriptor(
       name='HolderCategory_SeniorManager', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=9303,
-  serialized_end=9432,
+  serialized_start=9317,
+  serialized_end=9446,
 )
 _sym_db.RegisterEnumDescriptor(_HOLDERCATEGORY)
 
 HolderCategory = enum_type_wrapper.EnumTypeWrapper(_HOLDERCATEGORY)
 _PUSHDATATYPE = _descriptor.EnumDescriptor(
   name='PushDataType',
   full_name='Qot_Common.PushDataType',
@@ -1079,16 +1079,16 @@
     _descriptor.EnumValueDescriptor(
       name='PushDataType_Cache', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=9434,
-  serialized_end=9552,
+  serialized_start=9448,
+  serialized_end=9566,
 )
 _sym_db.RegisterEnumDescriptor(_PUSHDATATYPE)
 
 PushDataType = enum_type_wrapper.EnumTypeWrapper(_PUSHDATATYPE)
 _SORTFIELD = _descriptor.EnumDescriptor(
   name='SortField',
   full_name='Qot_Common.SortField',
@@ -1298,16 +1298,16 @@
     _descriptor.EnumValueDescriptor(
       name='SortField_PositionChange', index=50, number=50,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=9555,
-  serialized_end=10918,
+  serialized_start=9569,
+  serialized_end=10932,
 )
 _sym_db.RegisterEnumDescriptor(_SORTFIELD)
 
 SortField = enum_type_wrapper.EnumTypeWrapper(_SORTFIELD)
 _ISSUER = _descriptor.EnumDescriptor(
   name='Issuer',
   full_name='Qot_Common.Issuer',
@@ -1417,16 +1417,16 @@
     _descriptor.EnumValueDescriptor(
       name='Issuer_XZ', index=25, number=25,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=10921,
-  serialized_end=11323,
+  serialized_start=10935,
+  serialized_end=11337,
 )
 _sym_db.RegisterEnumDescriptor(_ISSUER)
 
 Issuer = enum_type_wrapper.EnumTypeWrapper(_ISSUER)
 _IPOPERIOD = _descriptor.EnumDescriptor(
   name='IpoPeriod',
   full_name='Qot_Common.IpoPeriod',
@@ -1456,16 +1456,16 @@
     _descriptor.EnumValueDescriptor(
       name='IpoPeriod_Lastmonth', index=5, number=5,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=11326,
-  serialized_end=11477,
+  serialized_start=11340,
+  serialized_end=11491,
 )
 _sym_db.RegisterEnumDescriptor(_IPOPERIOD)
 
 IpoPeriod = enum_type_wrapper.EnumTypeWrapper(_IPOPERIOD)
 _PRICETYPE = _descriptor.EnumDescriptor(
   name='PriceType',
   full_name='Qot_Common.PriceType',
@@ -1483,16 +1483,16 @@
     _descriptor.EnumValueDescriptor(
       name='PriceType_WithIn', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=11479,
-  serialized_end=11557,
+  serialized_start=11493,
+  serialized_end=11571,
 )
 _sym_db.RegisterEnumDescriptor(_PRICETYPE)
 
 PriceType = enum_type_wrapper.EnumTypeWrapper(_PRICETYPE)
 _WARRANTSTATUS = _descriptor.EnumDescriptor(
   name='WarrantStatus',
   full_name='Qot_Common.WarrantStatus',
@@ -1518,16 +1518,16 @@
     _descriptor.EnumValueDescriptor(
       name='WarrantStatus_PendingListing', index=4, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=11560,
-  serialized_end=11717,
+  serialized_start=11574,
+  serialized_end=11731,
 )
 _sym_db.RegisterEnumDescriptor(_WARRANTSTATUS)
 
 WarrantStatus = enum_type_wrapper.EnumTypeWrapper(_WARRANTSTATUS)
 _COMPANYACT = _descriptor.EnumDescriptor(
   name='CompanyAct',
   full_name='Qot_Common.CompanyAct',
@@ -1569,16 +1569,16 @@
     _descriptor.EnumValueDescriptor(
       name='CompanyAct_SPDividend', index=8, number=128,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=11720,
-  serialized_end=11938,
+  serialized_start=11734,
+  serialized_end=11952,
 )
 _sym_db.RegisterEnumDescriptor(_COMPANYACT)
 
 CompanyAct = enum_type_wrapper.EnumTypeWrapper(_COMPANYACT)
 _QOTRIGHT = _descriptor.EnumDescriptor(
   name='QotRight',
   full_name='Qot_Common.QotRight',
@@ -1608,16 +1608,16 @@
     _descriptor.EnumValueDescriptor(
       name='QotRight_No', index=5, number=5,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=11940,
-  serialized_end=12065,
+  serialized_start=11954,
+  serialized_end=12079,
 )
 _sym_db.RegisterEnumDescriptor(_QOTRIGHT)
 
 QotRight = enum_type_wrapper.EnumTypeWrapper(_QOTRIGHT)
 _PRICEREMINDERTYPE = _descriptor.EnumDescriptor(
   name='PriceReminderType',
   full_name='Qot_Common.PriceReminderType',
@@ -1687,16 +1687,16 @@
     _descriptor.EnumValueDescriptor(
       name='PriceReminderType_3MinChangeRateDown', index=15, number=15,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=12068,
-  serialized_end=12658,
+  serialized_start=12082,
+  serialized_end=12672,
 )
 _sym_db.RegisterEnumDescriptor(_PRICEREMINDERTYPE)
 
 PriceReminderType = enum_type_wrapper.EnumTypeWrapper(_PRICEREMINDERTYPE)
 _PRICEREMINDERFREQ = _descriptor.EnumDescriptor(
   name='PriceReminderFreq',
   full_name='Qot_Common.PriceReminderFreq',
@@ -1718,16 +1718,16 @@
     _descriptor.EnumValueDescriptor(
       name='PriceReminderFreq_OnlyOnce', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=12661,
-  serialized_end=12805,
+  serialized_start=12675,
+  serialized_end=12819,
 )
 _sym_db.RegisterEnumDescriptor(_PRICEREMINDERFREQ)
 
 PriceReminderFreq = enum_type_wrapper.EnumTypeWrapper(_PRICEREMINDERFREQ)
 _ASSETCLASS = _descriptor.EnumDescriptor(
   name='AssetClass',
   full_name='Qot_Common.AssetClass',
@@ -1761,16 +1761,16 @@
     _descriptor.EnumValueDescriptor(
       name='AssetClass_Swap', index=6, number=6,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=12808,
-  serialized_end=12987,
+  serialized_start=12822,
+  serialized_end=13001,
 )
 _sym_db.RegisterEnumDescriptor(_ASSETCLASS)
 
 AssetClass = enum_type_wrapper.EnumTypeWrapper(_ASSETCLASS)
 _EXPIRATIONCYCLE = _descriptor.EnumDescriptor(
   name='ExpirationCycle',
   full_name='Qot_Common.ExpirationCycle',
@@ -1788,16 +1788,16 @@
     _descriptor.EnumValueDescriptor(
       name='ExpirationCycle_Month', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=12989,
-  serialized_end=13088,
+  serialized_start=13003,
+  serialized_end=13102,
 )
 _sym_db.RegisterEnumDescriptor(_EXPIRATIONCYCLE)
 
 ExpirationCycle = enum_type_wrapper.EnumTypeWrapper(_EXPIRATIONCYCLE)
 _EXCHTYPE = _descriptor.EnumDescriptor(
   name='ExchType',
   full_name='Qot_Common.ExchType',
@@ -1879,16 +1879,16 @@
     _descriptor.EnumValueDescriptor(
       name='ExchType_JP_OSE', index=18, number=18,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=13091,
-  serialized_end=13527,
+  serialized_start=13105,
+  serialized_end=13541,
 )
 _sym_db.RegisterEnumDescriptor(_EXCHTYPE)
 
 ExchType = enum_type_wrapper.EnumTypeWrapper(_EXCHTYPE)
 _PERIODTYPE = _descriptor.EnumDescriptor(
   name='PeriodType',
   full_name='Qot_Common.PeriodType',
@@ -1914,16 +1914,16 @@
     _descriptor.EnumValueDescriptor(
       name='PeriodType_MONTH', index=4, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=13529,
-  serialized_end=13653,
+  serialized_start=13543,
+  serialized_end=13667,
 )
 _sym_db.RegisterEnumDescriptor(_PERIODTYPE)
 
 PeriodType = enum_type_wrapper.EnumTypeWrapper(_PERIODTYPE)
 QotMarket_Unknown = 0
 QotMarket_HK_Security = 1
 QotMarket_HK_Future = 2
@@ -2769,162 +2769,169 @@
       name='security', full_name='Qot_Common.BasicQot.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='isSuspended', full_name='Qot_Common.BasicQot.isSuspended', index=1,
+      name='name', full_name='Qot_Common.BasicQot.name', index=1,
+      number=24, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='isSuspended', full_name='Qot_Common.BasicQot.isSuspended', index=2,
       number=2, type=8, cpp_type=7, label=2,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='listTime', full_name='Qot_Common.BasicQot.listTime', index=2,
+      name='listTime', full_name='Qot_Common.BasicQot.listTime', index=3,
       number=3, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='priceSpread', full_name='Qot_Common.BasicQot.priceSpread', index=3,
+      name='priceSpread', full_name='Qot_Common.BasicQot.priceSpread', index=4,
       number=4, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='updateTime', full_name='Qot_Common.BasicQot.updateTime', index=4,
+      name='updateTime', full_name='Qot_Common.BasicQot.updateTime', index=5,
       number=5, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='highPrice', full_name='Qot_Common.BasicQot.highPrice', index=5,
+      name='highPrice', full_name='Qot_Common.BasicQot.highPrice', index=6,
       number=6, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='openPrice', full_name='Qot_Common.BasicQot.openPrice', index=6,
+      name='openPrice', full_name='Qot_Common.BasicQot.openPrice', index=7,
       number=7, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lowPrice', full_name='Qot_Common.BasicQot.lowPrice', index=7,
+      name='lowPrice', full_name='Qot_Common.BasicQot.lowPrice', index=8,
       number=8, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='curPrice', full_name='Qot_Common.BasicQot.curPrice', index=8,
+      name='curPrice', full_name='Qot_Common.BasicQot.curPrice', index=9,
       number=9, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lastClosePrice', full_name='Qot_Common.BasicQot.lastClosePrice', index=9,
+      name='lastClosePrice', full_name='Qot_Common.BasicQot.lastClosePrice', index=10,
       number=10, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='volume', full_name='Qot_Common.BasicQot.volume', index=10,
+      name='volume', full_name='Qot_Common.BasicQot.volume', index=11,
       number=11, type=3, cpp_type=2, label=2,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='turnover', full_name='Qot_Common.BasicQot.turnover', index=11,
+      name='turnover', full_name='Qot_Common.BasicQot.turnover', index=12,
       number=12, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='turnoverRate', full_name='Qot_Common.BasicQot.turnoverRate', index=12,
+      name='turnoverRate', full_name='Qot_Common.BasicQot.turnoverRate', index=13,
       number=13, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='amplitude', full_name='Qot_Common.BasicQot.amplitude', index=13,
+      name='amplitude', full_name='Qot_Common.BasicQot.amplitude', index=14,
       number=14, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='darkStatus', full_name='Qot_Common.BasicQot.darkStatus', index=14,
+      name='darkStatus', full_name='Qot_Common.BasicQot.darkStatus', index=15,
       number=15, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='optionExData', full_name='Qot_Common.BasicQot.optionExData', index=15,
+      name='optionExData', full_name='Qot_Common.BasicQot.optionExData', index=16,
       number=16, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='listTimestamp', full_name='Qot_Common.BasicQot.listTimestamp', index=16,
+      name='listTimestamp', full_name='Qot_Common.BasicQot.listTimestamp', index=17,
       number=17, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='updateTimestamp', full_name='Qot_Common.BasicQot.updateTimestamp', index=17,
+      name='updateTimestamp', full_name='Qot_Common.BasicQot.updateTimestamp', index=18,
       number=18, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='preMarket', full_name='Qot_Common.BasicQot.preMarket', index=18,
+      name='preMarket', full_name='Qot_Common.BasicQot.preMarket', index=19,
       number=19, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='afterMarket', full_name='Qot_Common.BasicQot.afterMarket', index=19,
+      name='afterMarket', full_name='Qot_Common.BasicQot.afterMarket', index=20,
       number=20, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='secStatus', full_name='Qot_Common.BasicQot.secStatus', index=20,
+      name='secStatus', full_name='Qot_Common.BasicQot.secStatus', index=21,
       number=21, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='futureExData', full_name='Qot_Common.BasicQot.futureExData', index=21,
+      name='futureExData', full_name='Qot_Common.BasicQot.futureExData', index=22,
       number=22, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='warrantExData', full_name='Qot_Common.BasicQot.warrantExData', index=22,
+      name='warrantExData', full_name='Qot_Common.BasicQot.warrantExData', index=23,
       number=23, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -2935,15 +2942,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1128,
-  serialized_end=1792,
+  serialized_end=1806,
 )
 
 
 _TIMESHARE = _descriptor.Descriptor(
   name='TimeShare',
   full_name='Qot_Common.TimeShare',
   filename=None,
@@ -3021,16 +3028,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1795,
-  serialized_end=1963,
+  serialized_start=1809,
+  serialized_end=1977,
 )
 
 
 _SECURITYSTATICBASIC = _descriptor.Descriptor(
   name='SecurityStaticBasic',
   full_name='Qot_Common.SecurityStaticBasic',
   filename=None,
@@ -3108,16 +3115,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1966,
-  serialized_end=2165,
+  serialized_start=1980,
+  serialized_end=2179,
 )
 
 
 _WARRANTSTATICEXDATA = _descriptor.Descriptor(
   name='WarrantStaticExData',
   full_name='Qot_Common.WarrantStaticExData',
   filename=None,
@@ -3146,16 +3153,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2167,
-  serialized_end=2239,
+  serialized_start=2181,
+  serialized_end=2253,
 )
 
 
 _OPTIONSTATICEXDATA = _descriptor.Descriptor(
   name='OptionStaticExData',
   full_name='Qot_Common.OptionStaticExData',
   filename=None,
@@ -3226,16 +3233,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2242,
-  serialized_end=2437,
+  serialized_start=2256,
+  serialized_end=2451,
 )
 
 
 _FUTURESTATICEXDATA = _descriptor.Descriptor(
   name='FutureStaticExData',
   full_name='Qot_Common.FutureStaticExData',
   filename=None,
@@ -3271,16 +3278,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2439,
-  serialized_end=2534,
+  serialized_start=2453,
+  serialized_end=2548,
 )
 
 
 _SECURITYSTATICINFO = _descriptor.Descriptor(
   name='SecurityStaticInfo',
   full_name='Qot_Common.SecurityStaticInfo',
   filename=None,
@@ -3323,16 +3330,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2537,
-  serialized_end=2769,
+  serialized_start=2551,
+  serialized_end=2783,
 )
 
 
 _BROKER = _descriptor.Descriptor(
   name='Broker',
   full_name='Qot_Common.Broker',
   filename=None,
@@ -3382,16 +3389,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2771,
-  serialized_end=2851,
+  serialized_start=2785,
+  serialized_end=2865,
 )
 
 
 _TICKER = _descriptor.Descriptor(
   name='Ticker',
   full_name='Qot_Common.Ticker',
   filename=None,
@@ -3483,16 +3490,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2854,
-  serialized_end=3047,
+  serialized_start=2868,
+  serialized_end=3061,
 )
 
 
 _ORDERBOOKDETAIL = _descriptor.Descriptor(
   name='OrderBookDetail',
   full_name='Qot_Common.OrderBookDetail',
   filename=None,
@@ -3521,16 +3528,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3049,
-  serialized_end=3099,
+  serialized_start=3063,
+  serialized_end=3113,
 )
 
 
 _ORDERBOOK = _descriptor.Descriptor(
   name='OrderBook',
   full_name='Qot_Common.OrderBook',
   filename=None,
@@ -3573,16 +3580,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3101,
-  serialized_end=3213,
+  serialized_start=3115,
+  serialized_end=3227,
 )
 
 
 _SHAREHOLDINGCHANGE = _descriptor.Descriptor(
   name='ShareHoldingChange',
   full_name='Qot_Common.ShareHoldingChange',
   filename=None,
@@ -3646,16 +3653,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3216,
-  serialized_end=3371,
+  serialized_start=3230,
+  serialized_end=3385,
 )
 
 
 _SUBINFO = _descriptor.Descriptor(
   name='SubInfo',
   full_name='Qot_Common.SubInfo',
   filename=None,
@@ -3684,16 +3691,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3373,
-  serialized_end=3443,
+  serialized_start=3387,
+  serialized_end=3457,
 )
 
 
 _CONNSUBINFO = _descriptor.Descriptor(
   name='ConnSubInfo',
   full_name='Qot_Common.ConnSubInfo',
   filename=None,
@@ -3729,16 +3736,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3445,
-  serialized_end=3542,
+  serialized_start=3459,
+  serialized_end=3556,
 )
 
 
 _PLATEINFO = _descriptor.Descriptor(
   name='PlateInfo',
   full_name='Qot_Common.PlateInfo',
   filename=None,
@@ -3774,16 +3781,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3544,
-  serialized_end=3625,
+  serialized_start=3558,
+  serialized_end=3639,
 )
 
 
 _REHAB = _descriptor.Descriptor(
   name='Rehab',
   full_name='Qot_Common.Rehab',
   filename=None,
@@ -3959,16 +3966,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3628,
-  serialized_end=4070,
+  serialized_start=3642,
+  serialized_end=4084,
 )
 
 _BASICQOT.fields_by_name['security'].message_type = _SECURITY
 _BASICQOT.fields_by_name['optionExData'].message_type = _OPTIONBASICQOTEXDATA
 _BASICQOT.fields_by_name['preMarket'].message_type = _PREAFTERMARKETDATA
 _BASICQOT.fields_by_name['afterMarket'].message_type = _PREAFTERMARKETDATA
 _BASICQOT.fields_by_name['futureExData'].message_type = _FUTUREBASICQOTEXDATA
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetBasicQot_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetBasicQot_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetBroker_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetBroker_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetBroker.proto',
   package='Qot_GetBroker',
   syntax='proto2',
-  serialized_pb=_b('\n\x13Qot_GetBroker.proto\x12\rQot_GetBroker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"-\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\"\x83\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12)\n\rbrokerAskList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Broker\x12)\n\rbrokerBidList\x18\x03 \x03(\x0b\x32\x12.Qot_Common.Broker\"*\n\x07Request\x12\x1f\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x12.Qot_GetBroker.C2S\"c\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1f\n\x03s2c\x18\x04 \x01(\x0b\x32\x12.Qot_GetBroker.S2CBC\n\x13\x63om.futu.openapi.pbZ,github.com/futuopen/ftapi4go/pb/qotgetbroker')
+  serialized_pb=_b('\n\x13Qot_GetBroker.proto\x12\rQot_GetBroker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"-\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\"\x91\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\rbrokerAskList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Broker\x12)\n\rbrokerBidList\x18\x03 \x03(\x0b\x32\x12.Qot_Common.Broker\"*\n\x07Request\x12\x1f\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x12.Qot_GetBroker.C2S\"c\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1f\n\x03s2c\x18\x04 \x01(\x0b\x32\x12.Qot_GetBroker.S2CBC\n\x13\x63om.futu.openapi.pbZ,github.com/futuopen/ftapi4go/pb/qotgetbroker')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -70,22 +70,29 @@
       name='security', full_name='Qot_GetBroker.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='brokerAskList', full_name='Qot_GetBroker.S2C.brokerAskList', index=1,
+      name='name', full_name='Qot_GetBroker.S2C.name', index=1,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='brokerAskList', full_name='Qot_GetBroker.S2C.brokerAskList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='brokerBidList', full_name='Qot_GetBroker.S2C.brokerBidList', index=2,
+      name='brokerBidList', full_name='Qot_GetBroker.S2C.brokerBidList', index=3,
       number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -96,15 +103,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=118,
-  serialized_end=249,
+  serialized_end=263,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetBroker.Request',
   filename=None,
@@ -126,16 +133,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=251,
-  serialized_end=293,
+  serialized_start=265,
+  serialized_end=307,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetBroker.Response',
   filename=None,
@@ -178,16 +185,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=295,
-  serialized_end=394,
+  serialized_start=309,
+  serialized_end=408,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['brokerAskList'].message_type = Qot__Common__pb2._BROKER
 _S2C.fields_by_name['brokerBidList'].message_type = Qot__Common__pb2._BROKER
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetCapitalDistribution_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetCapitalDistribution_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetCapitalFlow_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetCapitalFlow_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetCodeChange_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetCodeChange_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetFutureInfo_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetFutureInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetHistoryKLPoints_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetHistoryKL_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetHistoryKL_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetHoldingChangeList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetHoldingChangeList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetIpoList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetIpoList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetKL_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetKL_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetKL.proto',
   package='Qot_GetKL',
   syntax='proto2',
-  serialized_pb=_b('\n\x0fQot_GetKL.proto\x12\tQot_GetKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"`\n\x03\x43\x32S\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0e\n\x06reqNum\x18\x04 \x02(\x05\"P\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12!\n\x06klList\x18\x02 \x03(\x0b\x32\x11.Qot_Common.KLine\"&\n\x07Request\x12\x1b\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x0e.Qot_GetKL.C2S\"_\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1b\n\x03s2c\x18\x04 \x01(\x0b\x32\x0e.Qot_GetKL.S2CB?\n\x13\x63om.futu.openapi.pbZ(github.com/futuopen/ftapi4go/pb/qotgetkl')
+  serialized_pb=_b('\n\x0fQot_GetKL.proto\x12\tQot_GetKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"`\n\x03\x43\x32S\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0e\n\x06reqNum\x18\x04 \x02(\x05\"^\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12!\n\x06klList\x18\x02 \x03(\x0b\x32\x11.Qot_Common.KLine\"&\n\x07Request\x12\x1b\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x0e.Qot_GetKL.C2S\"_\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1b\n\x03s2c\x18\x04 \x01(\x0b\x32\x0e.Qot_GetKL.S2CB?\n\x13\x63om.futu.openapi.pbZ(github.com/futuopen/ftapi4go/pb/qotgetkl')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -91,15 +91,22 @@
       name='security', full_name='Qot_GetKL.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='klList', full_name='Qot_GetKL.S2C.klList', index=1,
+      name='name', full_name='Qot_GetKL.S2C.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='klList', full_name='Qot_GetKL.S2C.klList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -110,15 +117,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=160,
-  serialized_end=240,
+  serialized_end=254,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetKL.Request',
   filename=None,
@@ -140,16 +147,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=242,
-  serialized_end=280,
+  serialized_start=256,
+  serialized_end=294,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetKL.Response',
   filename=None,
@@ -192,16 +199,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=282,
-  serialized_end=377,
+  serialized_start=296,
+  serialized_end=391,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['klList'].message_type = Qot__Common__pb2._KLINE
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetMarketState_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetMarketState_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetOptionChain_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetOptionChain_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetOptionExpirationDate_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetOrderBook_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetOrderBook_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetOrderBook.proto',
   package='Qot_GetOrderBook',
   syntax='proto2',
-  serialized_pb=_b('\n\x16Qot_GetOrderBook.proto\x12\x10Qot_GetOrderBook\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\":\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0b\n\x03num\x18\x02 \x02(\x05\"\x81\x02\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12/\n\x10orderBookAskList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12/\n\x10orderBookBidList\x18\x03 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12\x16\n\x0esvrRecvTimeBid\x18\x04 \x01(\t\x12\x1f\n\x17svrRecvTimeBidTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0esvrRecvTimeAsk\x18\x06 \x01(\t\x12\x1f\n\x17svrRecvTimeAskTimestamp\x18\x07 \x01(\x01\"-\n\x07Request\x12\"\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x15.Qot_GetOrderBook.C2S\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_GetOrderBook.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotgetorderbook')
+  serialized_pb=_b('\n\x16Qot_GetOrderBook.proto\x12\x10Qot_GetOrderBook\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\":\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0b\n\x03num\x18\x02 \x02(\x05\"\x8f\x02\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x08 \x01(\t\x12/\n\x10orderBookAskList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12/\n\x10orderBookBidList\x18\x03 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12\x16\n\x0esvrRecvTimeBid\x18\x04 \x01(\t\x12\x1f\n\x17svrRecvTimeBidTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0esvrRecvTimeAsk\x18\x06 \x01(\t\x12\x1f\n\x17svrRecvTimeAskTimestamp\x18\x07 \x01(\x01\"-\n\x07Request\x12\"\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x15.Qot_GetOrderBook.C2S\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_GetOrderBook.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotgetorderbook')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -77,50 +77,57 @@
       name='security', full_name='Qot_GetOrderBook.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='orderBookAskList', full_name='Qot_GetOrderBook.S2C.orderBookAskList', index=1,
+      name='name', full_name='Qot_GetOrderBook.S2C.name', index=1,
+      number=8, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderBookAskList', full_name='Qot_GetOrderBook.S2C.orderBookAskList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='orderBookBidList', full_name='Qot_GetOrderBook.S2C.orderBookBidList', index=2,
+      name='orderBookBidList', full_name='Qot_GetOrderBook.S2C.orderBookBidList', index=3,
       number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeBid', full_name='Qot_GetOrderBook.S2C.svrRecvTimeBid', index=3,
+      name='svrRecvTimeBid', full_name='Qot_GetOrderBook.S2C.svrRecvTimeBid', index=4,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeBidTimestamp', full_name='Qot_GetOrderBook.S2C.svrRecvTimeBidTimestamp', index=4,
+      name='svrRecvTimeBidTimestamp', full_name='Qot_GetOrderBook.S2C.svrRecvTimeBidTimestamp', index=5,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeAsk', full_name='Qot_GetOrderBook.S2C.svrRecvTimeAsk', index=5,
+      name='svrRecvTimeAsk', full_name='Qot_GetOrderBook.S2C.svrRecvTimeAsk', index=6,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeAskTimestamp', full_name='Qot_GetOrderBook.S2C.svrRecvTimeAskTimestamp', index=6,
+      name='svrRecvTimeAskTimestamp', full_name='Qot_GetOrderBook.S2C.svrRecvTimeAskTimestamp', index=7,
       number=7, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -131,15 +138,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=137,
-  serialized_end=394,
+  serialized_end=408,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetOrderBook.Request',
   filename=None,
@@ -161,16 +168,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=396,
-  serialized_end=441,
+  serialized_start=410,
+  serialized_end=455,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetOrderBook.Response',
   filename=None,
@@ -213,16 +220,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=443,
-  serialized_end=545,
+  serialized_start=457,
+  serialized_end=559,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['orderBookAskList'].message_type = Qot__Common__pb2._ORDERBOOK
 _S2C.fields_by_name['orderBookBidList'].message_type = Qot__Common__pb2._ORDERBOOK
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetOwnerPlate_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetOwnerPlate_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetOwnerPlate.proto',
   package='Qot_GetOwnerPlate',
   syntax='proto2',
-  serialized_pb=_b('\n\x17Qot_GetOwnerPlate.proto\x12\x11Qot_GetOwnerPlate\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"1\n\x03\x43\x32S\x12*\n\x0csecurityList\x18\x01 \x03(\x0b\x32\x14.Qot_Common.Security\"j\n\x12SecurityOwnerPlate\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12,\n\rplateInfoList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.PlateInfo\"D\n\x03S2C\x12=\n\x0eownerPlateList\x18\x01 \x03(\x0b\x32%.Qot_GetOwnerPlate.SecurityOwnerPlate\".\n\x07Request\x12#\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x16.Qot_GetOwnerPlate.C2S\"g\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12#\n\x03s2c\x18\x04 \x01(\x0b\x32\x16.Qot_GetOwnerPlate.S2CBG\n\x13\x63om.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/qotgetownerplate')
+  serialized_pb=_b('\n\x17Qot_GetOwnerPlate.proto\x12\x11Qot_GetOwnerPlate\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"1\n\x03\x43\x32S\x12*\n\x0csecurityList\x18\x01 \x03(\x0b\x32\x14.Qot_Common.Security\"x\n\x12SecurityOwnerPlate\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12,\n\rplateInfoList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.PlateInfo\"D\n\x03S2C\x12=\n\x0eownerPlateList\x18\x01 \x03(\x0b\x32%.Qot_GetOwnerPlate.SecurityOwnerPlate\".\n\x07Request\x12#\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x16.Qot_GetOwnerPlate.C2S\"g\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12#\n\x03s2c\x18\x04 \x01(\x0b\x32\x16.Qot_GetOwnerPlate.S2CBG\n\x13\x63om.futu.openapi.pbZ0github.com/futuopen/ftapi4go/pb/qotgetownerplate')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -70,15 +70,22 @@
       name='security', full_name='Qot_GetOwnerPlate.SecurityOwnerPlate.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='plateInfoList', full_name='Qot_GetOwnerPlate.SecurityOwnerPlate.plateInfoList', index=1,
+      name='name', full_name='Qot_GetOwnerPlate.SecurityOwnerPlate.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='plateInfoList', full_name='Qot_GetOwnerPlate.SecurityOwnerPlate.plateInfoList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -89,15 +96,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=129,
-  serialized_end=235,
+  serialized_end=249,
 )
 
 
 _S2C = _descriptor.Descriptor(
   name='S2C',
   full_name='Qot_GetOwnerPlate.S2C',
   filename=None,
@@ -119,16 +126,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=237,
-  serialized_end=305,
+  serialized_start=251,
+  serialized_end=319,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetOwnerPlate.Request',
   filename=None,
@@ -150,16 +157,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=307,
-  serialized_end=353,
+  serialized_start=321,
+  serialized_end=367,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetOwnerPlate.Response',
   filename=None,
@@ -202,16 +209,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=355,
-  serialized_end=458,
+  serialized_start=369,
+  serialized_end=472,
 )
 
 _C2S.fields_by_name['securityList'].message_type = Qot__Common__pb2._SECURITY
 _SECURITYOWNERPLATE.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _SECURITYOWNERPLATE.fields_by_name['plateInfoList'].message_type = Qot__Common__pb2._PLATEINFO
 _S2C.fields_by_name['ownerPlateList'].message_type = _SECURITYOWNERPLATE
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetPlateSecurity_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetPlateSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetPlateSet_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetPlateSet_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetPriceReminder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetPriceReminder_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetPriceReminder.proto',
   package='Qot_GetPriceReminder',
   syntax='proto2',
-  serialized_pb=_b('\n\x1aQot_GetPriceReminder.proto\x12\x14Qot_GetPriceReminder\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"k\n\x11PriceReminderItem\x12\x0b\n\x03key\x18\x01 \x02(\x03\x12\x0c\n\x04type\x18\x02 \x02(\x05\x12\r\n\x05value\x18\x03 \x02(\x01\x12\x0c\n\x04note\x18\x04 \x02(\t\x12\x0c\n\x04\x66req\x18\x05 \x02(\x05\x12\x10\n\x08isEnable\x18\x06 \x02(\x08\"r\n\rPriceReminder\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x39\n\x08itemList\x18\x02 \x03(\x0b\x32\'.Qot_GetPriceReminder.PriceReminderItem\"=\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x01(\x0b\x32\x14.Qot_Common.Security\x12\x0e\n\x06market\x18\x02 \x01(\x05\"E\n\x03S2C\x12>\n\x11priceReminderList\x18\x01 \x03(\x0b\x32#.Qot_GetPriceReminder.PriceReminder\"1\n\x07Request\x12&\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x19.Qot_GetPriceReminder.C2S\"j\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12&\n\x03s2c\x18\x04 \x01(\x0b\x32\x19.Qot_GetPriceReminder.S2CBJ\n\x13\x63om.futu.openapi.pbZ3github.com/futuopen/ftapi4go/pb/qotgetpricereminder')
+  serialized_pb=_b('\n\x1aQot_GetPriceReminder.proto\x12\x14Qot_GetPriceReminder\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"k\n\x11PriceReminderItem\x12\x0b\n\x03key\x18\x01 \x02(\x03\x12\x0c\n\x04type\x18\x02 \x02(\x05\x12\r\n\x05value\x18\x03 \x02(\x01\x12\x0c\n\x04note\x18\x04 \x02(\t\x12\x0c\n\x04\x66req\x18\x05 \x02(\x05\x12\x10\n\x08isEnable\x18\x06 \x02(\x08\"\x80\x01\n\rPriceReminder\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x39\n\x08itemList\x18\x02 \x03(\x0b\x32\'.Qot_GetPriceReminder.PriceReminderItem\"=\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x01(\x0b\x32\x14.Qot_Common.Security\x12\x0e\n\x06market\x18\x02 \x01(\x05\"E\n\x03S2C\x12>\n\x11priceReminderList\x18\x01 \x03(\x0b\x32#.Qot_GetPriceReminder.PriceReminder\"1\n\x07Request\x12&\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x19.Qot_GetPriceReminder.C2S\"j\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12&\n\x03s2c\x18\x04 \x01(\x0b\x32\x19.Qot_GetPriceReminder.S2CBJ\n\x13\x63om.futu.openapi.pbZ3github.com/futuopen/ftapi4go/pb/qotgetpricereminder')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _PRICEREMINDERITEM = _descriptor.Descriptor(
@@ -105,15 +105,22 @@
       name='security', full_name='Qot_GetPriceReminder.PriceReminder.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='itemList', full_name='Qot_GetPriceReminder.PriceReminder.itemList', index=1,
+      name='name', full_name='Qot_GetPriceReminder.PriceReminder.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='itemList', full_name='Qot_GetPriceReminder.PriceReminder.itemList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -123,16 +130,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=193,
-  serialized_end=307,
+  serialized_start=194,
+  serialized_end=322,
 )
 
 
 _C2S = _descriptor.Descriptor(
   name='C2S',
   full_name='Qot_GetPriceReminder.C2S',
   filename=None,
@@ -161,16 +168,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=309,
-  serialized_end=370,
+  serialized_start=324,
+  serialized_end=385,
 )
 
 
 _S2C = _descriptor.Descriptor(
   name='S2C',
   full_name='Qot_GetPriceReminder.S2C',
   filename=None,
@@ -192,16 +199,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=372,
-  serialized_end=441,
+  serialized_start=387,
+  serialized_end=456,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetPriceReminder.Request',
   filename=None,
@@ -223,16 +230,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=443,
-  serialized_end=492,
+  serialized_start=458,
+  serialized_end=507,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetPriceReminder.Response',
   filename=None,
@@ -275,16 +282,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=494,
-  serialized_end=600,
+  serialized_start=509,
+  serialized_end=615,
 )
 
 _PRICEREMINDER.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _PRICEREMINDER.fields_by_name['itemList'].message_type = _PRICEREMINDERITEM
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['priceReminderList'].message_type = _PRICEREMINDER
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetRT_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetRT_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetRT.proto',
   package='Qot_GetRT',
   syntax='proto2',
-  serialized_pb=_b('\n\x0fQot_GetRT.proto\x12\tQot_GetRT\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"-\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\"T\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12%\n\x06rtList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.TimeShare\"&\n\x07Request\x12\x1b\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x0e.Qot_GetRT.C2S\"_\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1b\n\x03s2c\x18\x04 \x01(\x0b\x32\x0e.Qot_GetRT.S2CB?\n\x13\x63om.futu.openapi.pbZ(github.com/futuopen/ftapi4go/pb/qotgetrt')
+  serialized_pb=_b('\n\x0fQot_GetRT.proto\x12\tQot_GetRT\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"-\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\"b\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12%\n\x06rtList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.TimeShare\"&\n\x07Request\x12\x1b\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x0e.Qot_GetRT.C2S\"_\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1b\n\x03s2c\x18\x04 \x01(\x0b\x32\x0e.Qot_GetRT.S2CB?\n\x13\x63om.futu.openapi.pbZ(github.com/futuopen/ftapi4go/pb/qotgetrt')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -70,15 +70,22 @@
       name='security', full_name='Qot_GetRT.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='rtList', full_name='Qot_GetRT.S2C.rtList', index=1,
+      name='name', full_name='Qot_GetRT.S2C.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='rtList', full_name='Qot_GetRT.S2C.rtList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -89,15 +96,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=109,
-  serialized_end=193,
+  serialized_end=207,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetRT.Request',
   filename=None,
@@ -119,16 +126,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=195,
-  serialized_end=233,
+  serialized_start=209,
+  serialized_end=247,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetRT.Response',
   filename=None,
@@ -171,16 +178,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=235,
-  serialized_end=330,
+  serialized_start=249,
+  serialized_end=344,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['rtList'].message_type = Qot__Common__pb2._TIMESHARE
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetReference_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetReference_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetRehab_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetRehab_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetSecuritySnapshot_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetSecuritySnapshot.proto',
   package='Qot_GetSecuritySnapshot',
   syntax='proto2',
-  serialized_pb=_b('\n\x1dQot_GetSecuritySnapshot.proto\x12\x17Qot_GetSecuritySnapshot\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"1\n\x03\x43\x32S\x12*\n\x0csecurityList\x18\x01 \x03(\x0b\x32\x14.Qot_Common.Security\"\xf8\x02\n\x14\x45quitySnapshotExData\x12\x14\n\x0cissuedShares\x18\x01 \x02(\x03\x12\x17\n\x0fissuedMarketVal\x18\x02 \x02(\x01\x12\x10\n\x08netAsset\x18\x03 \x02(\x01\x12\x11\n\tnetProfit\x18\x04 \x02(\x01\x12\x18\n\x10\x65\x61rningsPershare\x18\x05 \x02(\x01\x12\x19\n\x11outstandingShares\x18\x06 \x02(\x03\x12\x1c\n\x14outstandingMarketVal\x18\x07 \x02(\x01\x12\x18\n\x10netAssetPershare\x18\x08 \x02(\x01\x12\x0e\n\x06\x65yRate\x18\t \x02(\x01\x12\x0e\n\x06peRate\x18\n \x02(\x01\x12\x0e\n\x06pbRate\x18\x0b \x02(\x01\x12\x11\n\tpeTTMRate\x18\x0c \x02(\x01\x12\x13\n\x0b\x64ividendTTM\x18\r \x01(\x01\x12\x18\n\x10\x64ividendRatioTTM\x18\x0e \x01(\x01\x12\x13\n\x0b\x64ividendLFY\x18\x0f \x01(\x01\x12\x18\n\x10\x64ividendLFYRatio\x18\x10 \x01(\x01\"\xd0\x04\n\x15WarrantSnapshotExData\x12\x16\n\x0e\x63onversionRate\x18\x01 \x02(\x01\x12\x13\n\x0bwarrantType\x18\x02 \x02(\x05\x12\x13\n\x0bstrikePrice\x18\x03 \x02(\x01\x12\x14\n\x0cmaturityTime\x18\x04 \x02(\t\x12\x14\n\x0c\x65ndTradeTime\x18\x05 \x02(\t\x12#\n\x05owner\x18\x06 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x15\n\rrecoveryPrice\x18\x07 \x02(\x01\x12\x14\n\x0cstreetVolumn\x18\x08 \x02(\x03\x12\x13\n\x0bissueVolumn\x18\t \x02(\x03\x12\x12\n\nstreetRate\x18\n \x02(\x01\x12\r\n\x05\x64\x65lta\x18\x0b \x02(\x01\x12\x19\n\x11impliedVolatility\x18\x0c \x02(\x01\x12\x0f\n\x07premium\x18\r \x02(\x01\x12\x19\n\x11maturityTimestamp\x18\x0e \x01(\x01\x12\x19\n\x11\x65ndTradeTimestamp\x18\x0f \x01(\x01\x12\x10\n\x08leverage\x18\x10 \x01(\x01\x12\x0c\n\x04ipop\x18\x11 \x01(\x01\x12\x16\n\x0e\x62reakEvenPoint\x18\x12 \x01(\x01\x12\x17\n\x0f\x63onversionPrice\x18\x13 \x01(\x01\x12\x1a\n\x12priceRecoveryRatio\x18\x14 \x01(\x01\x12\r\n\x05score\x18\x15 \x01(\x01\x12\x18\n\x10upperStrikePrice\x18\x16 \x01(\x01\x12\x18\n\x10lowerStrikePrice\x18\x17 \x01(\x01\x12\x19\n\x11inLinePriceStatus\x18\x18 \x01(\x05\x12\x12\n\nissuerCode\x18\x19 \x01(\t\"\x82\x04\n\x14OptionSnapshotExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x12\n\nstrikeTime\x18\x03 \x02(\t\x12\x13\n\x0bstrikePrice\x18\x04 \x02(\x01\x12\x14\n\x0c\x63ontractSize\x18\x05 \x02(\x05\x12\x19\n\x11\x63ontractSizeFloat\x18\x16 \x01(\x01\x12\x14\n\x0copenInterest\x18\x06 \x02(\x05\x12\x19\n\x11impliedVolatility\x18\x07 \x02(\x01\x12\x0f\n\x07premium\x18\x08 \x02(\x01\x12\r\n\x05\x64\x65lta\x18\t \x02(\x01\x12\r\n\x05gamma\x18\n \x02(\x01\x12\x0c\n\x04vega\x18\x0b \x02(\x01\x12\r\n\x05theta\x18\x0c \x02(\x01\x12\x0b\n\x03rho\x18\r \x02(\x01\x12\x17\n\x0fstrikeTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0findexOptionType\x18\x0f \x01(\x05\x12\x17\n\x0fnetOpenInterest\x18\x10 \x01(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x11 \x01(\x05\x12\x1c\n\x14\x63ontractNominalValue\x18\x12 \x01(\x01\x12\x1a\n\x12ownerLotMultiplier\x18\x13 \x01(\x01\x12\x16\n\x0eoptionAreaType\x18\x14 \x01(\x05\x12\x1a\n\x12\x63ontractMultiplier\x18\x15 \x01(\x01\"P\n\x13IndexSnapshotExData\x12\x12\n\nraiseCount\x18\x01 \x02(\x05\x12\x11\n\tfallCount\x18\x02 \x02(\x05\x12\x12\n\nequalCount\x18\x03 \x02(\x05\"P\n\x13PlateSnapshotExData\x12\x12\n\nraiseCount\x18\x01 \x02(\x05\x12\x11\n\tfallCount\x18\x02 \x02(\x05\x12\x12\n\nequalCount\x18\x03 \x02(\x05\"\xa4\x01\n\x14\x46utureSnapshotExData\x12\x17\n\x0flastSettlePrice\x18\x01 \x02(\x01\x12\x10\n\x08position\x18\x02 \x02(\x05\x12\x16\n\x0epositionChange\x18\x03 \x02(\x05\x12\x15\n\rlastTradeTime\x18\x04 \x02(\t\x12\x1a\n\x12lastTradeTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0eisMainContract\x18\x06 \x02(\x08\"\x8f\x01\n\x13TrustSnapshotExData\x12\x15\n\rdividendYield\x18\x01 \x02(\x01\x12\x0b\n\x03\x61um\x18\x02 \x02(\x01\x12\x18\n\x10outstandingUnits\x18\x03 \x02(\x03\x12\x15\n\rnetAssetValue\x18\x04 \x02(\x01\x12\x0f\n\x07premium\x18\x05 \x02(\x01\x12\x12\n\nassetClass\x18\x06 \x02(\x05\"\xc9\x07\n\x11SnapshotBasicData\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04type\x18\x02 \x02(\x05\x12\x11\n\tisSuspend\x18\x03 \x02(\x08\x12\x10\n\x08listTime\x18\x04 \x02(\t\x12\x0f\n\x07lotSize\x18\x05 \x02(\x05\x12\x13\n\x0bpriceSpread\x18\x06 \x02(\x01\x12\x12\n\nupdateTime\x18\x07 \x02(\t\x12\x11\n\thighPrice\x18\x08 \x02(\x01\x12\x11\n\topenPrice\x18\t \x02(\x01\x12\x10\n\x08lowPrice\x18\n \x02(\x01\x12\x16\n\x0elastClosePrice\x18\x0b \x02(\x01\x12\x10\n\x08\x63urPrice\x18\x0c \x02(\x01\x12\x0e\n\x06volume\x18\r \x02(\x03\x12\x10\n\x08turnover\x18\x0e \x02(\x01\x12\x14\n\x0cturnoverRate\x18\x0f \x02(\x01\x12\x15\n\rlistTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x10\n\x08\x61skPrice\x18\x12 \x01(\x01\x12\x10\n\x08\x62idPrice\x18\x13 \x01(\x01\x12\x0e\n\x06\x61skVol\x18\x14 \x01(\x03\x12\x0e\n\x06\x62idVol\x18\x15 \x01(\x03\x12\x14\n\x0c\x65nableMargin\x18\x16 \x01(\x08\x12\x15\n\rmortgageRatio\x18\x17 \x01(\x01\x12\x1e\n\x16longMarginInitialRatio\x18\x18 \x01(\x01\x12\x17\n\x0f\x65nableShortSell\x18\x19 \x01(\x08\x12\x15\n\rshortSellRate\x18\x1a \x01(\x01\x12\x1c\n\x14shortAvailableVolume\x18\x1b \x01(\x03\x12\x1f\n\x17shortMarginInitialRatio\x18\x1c \x01(\x01\x12\x11\n\tamplitude\x18\x1d \x01(\x01\x12\x10\n\x08\x61vgPrice\x18\x1e \x01(\x01\x12\x13\n\x0b\x62idAskRatio\x18\x1f \x01(\x01\x12\x13\n\x0bvolumeRatio\x18  \x01(\x01\x12\x1b\n\x13highest52WeeksPrice\x18! \x01(\x01\x12\x1a\n\x12lowest52WeeksPrice\x18\" \x01(\x01\x12\x1b\n\x13highestHistoryPrice\x18# \x01(\x01\x12\x1a\n\x12lowestHistoryPrice\x18$ \x01(\x01\x12\x31\n\tpreMarket\x18% \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x33\n\x0b\x61\x66terMarket\x18& \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x11\n\tsecStatus\x18\' \x01(\x05\x12\x19\n\x11\x63losePrice5Minute\x18( \x01(\x01\"\xa4\x04\n\x08Snapshot\x12\x39\n\x05\x62\x61sic\x18\x01 \x02(\x0b\x32*.Qot_GetSecuritySnapshot.SnapshotBasicData\x12\x43\n\x0c\x65quityExData\x18\x02 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.EquitySnapshotExData\x12\x45\n\rwarrantExData\x18\x03 \x01(\x0b\x32..Qot_GetSecuritySnapshot.WarrantSnapshotExData\x12\x43\n\x0coptionExData\x18\x04 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.OptionSnapshotExData\x12\x41\n\x0bindexExData\x18\x05 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.IndexSnapshotExData\x12\x41\n\x0bplateExData\x18\x06 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.PlateSnapshotExData\x12\x43\n\x0c\x66utureExData\x18\x07 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.FutureSnapshotExData\x12\x41\n\x0btrustExData\x18\x08 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.TrustSnapshotExData\">\n\x03S2C\x12\x37\n\x0csnapshotList\x18\x01 \x03(\x0b\x32!.Qot_GetSecuritySnapshot.Snapshot\"4\n\x07Request\x12)\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x1c.Qot_GetSecuritySnapshot.C2S\"m\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12)\n\x03s2c\x18\x04 \x01(\x0b\x32\x1c.Qot_GetSecuritySnapshot.S2CBM\n\x13\x63om.futu.openapi.pbZ6github.com/futuopen/ftapi4go/pb/qotgetsecuritysnapshot')
+  serialized_pb=_b('\n\x1dQot_GetSecuritySnapshot.proto\x12\x17Qot_GetSecuritySnapshot\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"1\n\x03\x43\x32S\x12*\n\x0csecurityList\x18\x01 \x03(\x0b\x32\x14.Qot_Common.Security\"\xf8\x02\n\x14\x45quitySnapshotExData\x12\x14\n\x0cissuedShares\x18\x01 \x02(\x03\x12\x17\n\x0fissuedMarketVal\x18\x02 \x02(\x01\x12\x10\n\x08netAsset\x18\x03 \x02(\x01\x12\x11\n\tnetProfit\x18\x04 \x02(\x01\x12\x18\n\x10\x65\x61rningsPershare\x18\x05 \x02(\x01\x12\x19\n\x11outstandingShares\x18\x06 \x02(\x03\x12\x1c\n\x14outstandingMarketVal\x18\x07 \x02(\x01\x12\x18\n\x10netAssetPershare\x18\x08 \x02(\x01\x12\x0e\n\x06\x65yRate\x18\t \x02(\x01\x12\x0e\n\x06peRate\x18\n \x02(\x01\x12\x0e\n\x06pbRate\x18\x0b \x02(\x01\x12\x11\n\tpeTTMRate\x18\x0c \x02(\x01\x12\x13\n\x0b\x64ividendTTM\x18\r \x01(\x01\x12\x18\n\x10\x64ividendRatioTTM\x18\x0e \x01(\x01\x12\x13\n\x0b\x64ividendLFY\x18\x0f \x01(\x01\x12\x18\n\x10\x64ividendLFYRatio\x18\x10 \x01(\x01\"\xd0\x04\n\x15WarrantSnapshotExData\x12\x16\n\x0e\x63onversionRate\x18\x01 \x02(\x01\x12\x13\n\x0bwarrantType\x18\x02 \x02(\x05\x12\x13\n\x0bstrikePrice\x18\x03 \x02(\x01\x12\x14\n\x0cmaturityTime\x18\x04 \x02(\t\x12\x14\n\x0c\x65ndTradeTime\x18\x05 \x02(\t\x12#\n\x05owner\x18\x06 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x15\n\rrecoveryPrice\x18\x07 \x02(\x01\x12\x14\n\x0cstreetVolumn\x18\x08 \x02(\x03\x12\x13\n\x0bissueVolumn\x18\t \x02(\x03\x12\x12\n\nstreetRate\x18\n \x02(\x01\x12\r\n\x05\x64\x65lta\x18\x0b \x02(\x01\x12\x19\n\x11impliedVolatility\x18\x0c \x02(\x01\x12\x0f\n\x07premium\x18\r \x02(\x01\x12\x19\n\x11maturityTimestamp\x18\x0e \x01(\x01\x12\x19\n\x11\x65ndTradeTimestamp\x18\x0f \x01(\x01\x12\x10\n\x08leverage\x18\x10 \x01(\x01\x12\x0c\n\x04ipop\x18\x11 \x01(\x01\x12\x16\n\x0e\x62reakEvenPoint\x18\x12 \x01(\x01\x12\x17\n\x0f\x63onversionPrice\x18\x13 \x01(\x01\x12\x1a\n\x12priceRecoveryRatio\x18\x14 \x01(\x01\x12\r\n\x05score\x18\x15 \x01(\x01\x12\x18\n\x10upperStrikePrice\x18\x16 \x01(\x01\x12\x18\n\x10lowerStrikePrice\x18\x17 \x01(\x01\x12\x19\n\x11inLinePriceStatus\x18\x18 \x01(\x05\x12\x12\n\nissuerCode\x18\x19 \x01(\t\"\x82\x04\n\x14OptionSnapshotExData\x12\x0c\n\x04type\x18\x01 \x02(\x05\x12#\n\x05owner\x18\x02 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x12\n\nstrikeTime\x18\x03 \x02(\t\x12\x13\n\x0bstrikePrice\x18\x04 \x02(\x01\x12\x14\n\x0c\x63ontractSize\x18\x05 \x02(\x05\x12\x19\n\x11\x63ontractSizeFloat\x18\x16 \x01(\x01\x12\x14\n\x0copenInterest\x18\x06 \x02(\x05\x12\x19\n\x11impliedVolatility\x18\x07 \x02(\x01\x12\x0f\n\x07premium\x18\x08 \x02(\x01\x12\r\n\x05\x64\x65lta\x18\t \x02(\x01\x12\r\n\x05gamma\x18\n \x02(\x01\x12\x0c\n\x04vega\x18\x0b \x02(\x01\x12\r\n\x05theta\x18\x0c \x02(\x01\x12\x0b\n\x03rho\x18\r \x02(\x01\x12\x17\n\x0fstrikeTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0findexOptionType\x18\x0f \x01(\x05\x12\x17\n\x0fnetOpenInterest\x18\x10 \x01(\x05\x12\x1a\n\x12\x65xpiryDateDistance\x18\x11 \x01(\x05\x12\x1c\n\x14\x63ontractNominalValue\x18\x12 \x01(\x01\x12\x1a\n\x12ownerLotMultiplier\x18\x13 \x01(\x01\x12\x16\n\x0eoptionAreaType\x18\x14 \x01(\x05\x12\x1a\n\x12\x63ontractMultiplier\x18\x15 \x01(\x01\"P\n\x13IndexSnapshotExData\x12\x12\n\nraiseCount\x18\x01 \x02(\x05\x12\x11\n\tfallCount\x18\x02 \x02(\x05\x12\x12\n\nequalCount\x18\x03 \x02(\x05\"P\n\x13PlateSnapshotExData\x12\x12\n\nraiseCount\x18\x01 \x02(\x05\x12\x11\n\tfallCount\x18\x02 \x02(\x05\x12\x12\n\nequalCount\x18\x03 \x02(\x05\"\xa4\x01\n\x14\x46utureSnapshotExData\x12\x17\n\x0flastSettlePrice\x18\x01 \x02(\x01\x12\x10\n\x08position\x18\x02 \x02(\x05\x12\x16\n\x0epositionChange\x18\x03 \x02(\x05\x12\x15\n\rlastTradeTime\x18\x04 \x02(\t\x12\x1a\n\x12lastTradeTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0eisMainContract\x18\x06 \x02(\x08\"\x8f\x01\n\x13TrustSnapshotExData\x12\x15\n\rdividendYield\x18\x01 \x02(\x01\x12\x0b\n\x03\x61um\x18\x02 \x02(\x01\x12\x18\n\x10outstandingUnits\x18\x03 \x02(\x03\x12\x15\n\rnetAssetValue\x18\x04 \x02(\x01\x12\x0f\n\x07premium\x18\x05 \x02(\x01\x12\x12\n\nassetClass\x18\x06 \x02(\x05\"\xd7\x07\n\x11SnapshotBasicData\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18) \x01(\t\x12\x0c\n\x04type\x18\x02 \x02(\x05\x12\x11\n\tisSuspend\x18\x03 \x02(\x08\x12\x10\n\x08listTime\x18\x04 \x02(\t\x12\x0f\n\x07lotSize\x18\x05 \x02(\x05\x12\x13\n\x0bpriceSpread\x18\x06 \x02(\x01\x12\x12\n\nupdateTime\x18\x07 \x02(\t\x12\x11\n\thighPrice\x18\x08 \x02(\x01\x12\x11\n\topenPrice\x18\t \x02(\x01\x12\x10\n\x08lowPrice\x18\n \x02(\x01\x12\x16\n\x0elastClosePrice\x18\x0b \x02(\x01\x12\x10\n\x08\x63urPrice\x18\x0c \x02(\x01\x12\x0e\n\x06volume\x18\r \x02(\x03\x12\x10\n\x08turnover\x18\x0e \x02(\x01\x12\x14\n\x0cturnoverRate\x18\x0f \x02(\x01\x12\x15\n\rlistTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x10\n\x08\x61skPrice\x18\x12 \x01(\x01\x12\x10\n\x08\x62idPrice\x18\x13 \x01(\x01\x12\x0e\n\x06\x61skVol\x18\x14 \x01(\x03\x12\x0e\n\x06\x62idVol\x18\x15 \x01(\x03\x12\x14\n\x0c\x65nableMargin\x18\x16 \x01(\x08\x12\x15\n\rmortgageRatio\x18\x17 \x01(\x01\x12\x1e\n\x16longMarginInitialRatio\x18\x18 \x01(\x01\x12\x17\n\x0f\x65nableShortSell\x18\x19 \x01(\x08\x12\x15\n\rshortSellRate\x18\x1a \x01(\x01\x12\x1c\n\x14shortAvailableVolume\x18\x1b \x01(\x03\x12\x1f\n\x17shortMarginInitialRatio\x18\x1c \x01(\x01\x12\x11\n\tamplitude\x18\x1d \x01(\x01\x12\x10\n\x08\x61vgPrice\x18\x1e \x01(\x01\x12\x13\n\x0b\x62idAskRatio\x18\x1f \x01(\x01\x12\x13\n\x0bvolumeRatio\x18  \x01(\x01\x12\x1b\n\x13highest52WeeksPrice\x18! \x01(\x01\x12\x1a\n\x12lowest52WeeksPrice\x18\" \x01(\x01\x12\x1b\n\x13highestHistoryPrice\x18# \x01(\x01\x12\x1a\n\x12lowestHistoryPrice\x18$ \x01(\x01\x12\x31\n\tpreMarket\x18% \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x33\n\x0b\x61\x66terMarket\x18& \x01(\x0b\x32\x1e.Qot_Common.PreAfterMarketData\x12\x11\n\tsecStatus\x18\' \x01(\x05\x12\x19\n\x11\x63losePrice5Minute\x18( \x01(\x01\"\xa4\x04\n\x08Snapshot\x12\x39\n\x05\x62\x61sic\x18\x01 \x02(\x0b\x32*.Qot_GetSecuritySnapshot.SnapshotBasicData\x12\x43\n\x0c\x65quityExData\x18\x02 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.EquitySnapshotExData\x12\x45\n\rwarrantExData\x18\x03 \x01(\x0b\x32..Qot_GetSecuritySnapshot.WarrantSnapshotExData\x12\x43\n\x0coptionExData\x18\x04 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.OptionSnapshotExData\x12\x41\n\x0bindexExData\x18\x05 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.IndexSnapshotExData\x12\x41\n\x0bplateExData\x18\x06 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.PlateSnapshotExData\x12\x43\n\x0c\x66utureExData\x18\x07 \x01(\x0b\x32-.Qot_GetSecuritySnapshot.FutureSnapshotExData\x12\x41\n\x0btrustExData\x18\x08 \x01(\x0b\x32,.Qot_GetSecuritySnapshot.TrustSnapshotExData\">\n\x03S2C\x12\x37\n\x0csnapshotList\x18\x01 \x03(\x0b\x32!.Qot_GetSecuritySnapshot.Snapshot\"4\n\x07Request\x12)\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x1c.Qot_GetSecuritySnapshot.C2S\"m\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12)\n\x03s2c\x18\x04 \x01(\x0b\x32\x1c.Qot_GetSecuritySnapshot.S2CBM\n\x13\x63om.futu.openapi.pbZ6github.com/futuopen/ftapi4go/pb/qotgetsecuritysnapshot')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -805,281 +805,288 @@
       name='security', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='type', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.type', index=1,
+      name='name', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.name', index=1,
+      number=41, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='type', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.type', index=2,
       number=2, type=5, cpp_type=1, label=2,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='isSuspend', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.isSuspend', index=2,
+      name='isSuspend', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.isSuspend', index=3,
       number=3, type=8, cpp_type=7, label=2,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='listTime', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.listTime', index=3,
+      name='listTime', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.listTime', index=4,
       number=4, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lotSize', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lotSize', index=4,
+      name='lotSize', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lotSize', index=5,
       number=5, type=5, cpp_type=1, label=2,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='priceSpread', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.priceSpread', index=5,
+      name='priceSpread', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.priceSpread', index=6,
       number=6, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='updateTime', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.updateTime', index=6,
+      name='updateTime', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.updateTime', index=7,
       number=7, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='highPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highPrice', index=7,
+      name='highPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highPrice', index=8,
       number=8, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='openPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.openPrice', index=8,
+      name='openPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.openPrice', index=9,
       number=9, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lowPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowPrice', index=9,
+      name='lowPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowPrice', index=10,
       number=10, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lastClosePrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lastClosePrice', index=10,
+      name='lastClosePrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lastClosePrice', index=11,
       number=11, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='curPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.curPrice', index=11,
+      name='curPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.curPrice', index=12,
       number=12, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='volume', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.volume', index=12,
+      name='volume', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.volume', index=13,
       number=13, type=3, cpp_type=2, label=2,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='turnover', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.turnover', index=13,
+      name='turnover', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.turnover', index=14,
       number=14, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='turnoverRate', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.turnoverRate', index=14,
+      name='turnoverRate', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.turnoverRate', index=15,
       number=15, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='listTimestamp', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.listTimestamp', index=15,
+      name='listTimestamp', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.listTimestamp', index=16,
       number=16, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='updateTimestamp', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.updateTimestamp', index=16,
+      name='updateTimestamp', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.updateTimestamp', index=17,
       number=17, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='askPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.askPrice', index=17,
+      name='askPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.askPrice', index=18,
       number=18, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='bidPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidPrice', index=18,
+      name='bidPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidPrice', index=19,
       number=19, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='askVol', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.askVol', index=19,
+      name='askVol', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.askVol', index=20,
       number=20, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='bidVol', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidVol', index=20,
+      name='bidVol', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidVol', index=21,
       number=21, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='enableMargin', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.enableMargin', index=21,
+      name='enableMargin', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.enableMargin', index=22,
       number=22, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='mortgageRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.mortgageRatio', index=22,
+      name='mortgageRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.mortgageRatio', index=23,
       number=23, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='longMarginInitialRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.longMarginInitialRatio', index=23,
+      name='longMarginInitialRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.longMarginInitialRatio', index=24,
       number=24, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='enableShortSell', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.enableShortSell', index=24,
+      name='enableShortSell', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.enableShortSell', index=25,
       number=25, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='shortSellRate', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortSellRate', index=25,
+      name='shortSellRate', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortSellRate', index=26,
       number=26, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='shortAvailableVolume', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortAvailableVolume', index=26,
+      name='shortAvailableVolume', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortAvailableVolume', index=27,
       number=27, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='shortMarginInitialRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortMarginInitialRatio', index=27,
+      name='shortMarginInitialRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.shortMarginInitialRatio', index=28,
       number=28, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='amplitude', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.amplitude', index=28,
+      name='amplitude', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.amplitude', index=29,
       number=29, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='avgPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.avgPrice', index=29,
+      name='avgPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.avgPrice', index=30,
       number=30, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='bidAskRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidAskRatio', index=30,
+      name='bidAskRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.bidAskRatio', index=31,
       number=31, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='volumeRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.volumeRatio', index=31,
+      name='volumeRatio', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.volumeRatio', index=32,
       number=32, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='highest52WeeksPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highest52WeeksPrice', index=32,
+      name='highest52WeeksPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highest52WeeksPrice', index=33,
       number=33, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lowest52WeeksPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowest52WeeksPrice', index=33,
+      name='lowest52WeeksPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowest52WeeksPrice', index=34,
       number=34, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='highestHistoryPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highestHistoryPrice', index=34,
+      name='highestHistoryPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.highestHistoryPrice', index=35,
       number=35, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='lowestHistoryPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowestHistoryPrice', index=35,
+      name='lowestHistoryPrice', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.lowestHistoryPrice', index=36,
       number=36, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='preMarket', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.preMarket', index=36,
+      name='preMarket', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.preMarket', index=37,
       number=37, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='afterMarket', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.afterMarket', index=37,
+      name='afterMarket', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.afterMarket', index=38,
       number=38, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='secStatus', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.secStatus', index=38,
+      name='secStatus', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.secStatus', index=39,
       number=39, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='closePrice5Minute', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.closePrice5Minute', index=39,
+      name='closePrice5Minute', full_name='Qot_GetSecuritySnapshot.SnapshotBasicData.closePrice5Minute', index=40,
       number=40, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -1090,15 +1097,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=2110,
-  serialized_end=3079,
+  serialized_end=3093,
 )
 
 
 _SNAPSHOT = _descriptor.Descriptor(
   name='Snapshot',
   full_name='Qot_GetSecuritySnapshot.Snapshot',
   filename=None,
@@ -1169,16 +1176,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3082,
-  serialized_end=3630,
+  serialized_start=3096,
+  serialized_end=3644,
 )
 
 
 _S2C = _descriptor.Descriptor(
   name='S2C',
   full_name='Qot_GetSecuritySnapshot.S2C',
   filename=None,
@@ -1200,16 +1207,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3632,
-  serialized_end=3694,
+  serialized_start=3646,
+  serialized_end=3708,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetSecuritySnapshot.Request',
   filename=None,
@@ -1231,16 +1238,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3696,
-  serialized_end=3748,
+  serialized_start=3710,
+  serialized_end=3762,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetSecuritySnapshot.Response',
   filename=None,
@@ -1283,16 +1290,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3750,
-  serialized_end=3859,
+  serialized_start=3764,
+  serialized_end=3873,
 )
 
 _C2S.fields_by_name['securityList'].message_type = Qot__Common__pb2._SECURITY
 _WARRANTSNAPSHOTEXDATA.fields_by_name['owner'].message_type = Qot__Common__pb2._SECURITY
 _OPTIONSNAPSHOTEXDATA.fields_by_name['owner'].message_type = Qot__Common__pb2._SECURITY
 _SNAPSHOTBASICDATA.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _SNAPSHOTBASICDATA.fields_by_name['preMarket'].message_type = Qot__Common__pb2._PREAFTERMARKETDATA
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetStaticInfo_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetStaticInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetSubInfo_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetSubInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetSuspend_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetSuspend_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetTicker_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetTicker_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_GetTicker.proto',
   package='Qot_GetTicker',
   syntax='proto2',
-  serialized_pb=_b('\n\x13Qot_GetTicker.proto\x12\rQot_GetTicker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"@\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x11\n\tmaxRetNum\x18\x02 \x02(\x05\"U\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12&\n\ntickerList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Ticker\"*\n\x07Request\x12\x1f\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x12.Qot_GetTicker.C2S\"c\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1f\n\x03s2c\x18\x04 \x01(\x0b\x32\x12.Qot_GetTicker.S2CBC\n\x13\x63om.futu.openapi.pbZ,github.com/futuopen/ftapi4go/pb/qotgetticker')
+  serialized_pb=_b('\n\x13Qot_GetTicker.proto\x12\rQot_GetTicker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"@\n\x03\x43\x32S\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x11\n\tmaxRetNum\x18\x02 \x02(\x05\"c\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\ntickerList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Ticker\"*\n\x07Request\x12\x1f\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x12.Qot_GetTicker.C2S\"c\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1f\n\x03s2c\x18\x04 \x01(\x0b\x32\x12.Qot_GetTicker.S2CBC\n\x13\x63om.futu.openapi.pbZ,github.com/futuopen/ftapi4go/pb/qotgetticker')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -77,15 +77,22 @@
       name='security', full_name='Qot_GetTicker.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='tickerList', full_name='Qot_GetTicker.S2C.tickerList', index=1,
+      name='name', full_name='Qot_GetTicker.S2C.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tickerList', full_name='Qot_GetTicker.S2C.tickerList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -96,15 +103,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=136,
-  serialized_end=221,
+  serialized_end=235,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_GetTicker.Request',
   filename=None,
@@ -126,16 +133,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=223,
-  serialized_end=265,
+  serialized_start=237,
+  serialized_end=279,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_GetTicker.Response',
   filename=None,
@@ -178,16 +185,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=267,
-  serialized_end=366,
+  serialized_start=281,
+  serialized_end=380,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['tickerList'].message_type = Qot__Common__pb2._TICKER
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetUserSecurityGroup_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetUserSecurity_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetUserSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_GetWarrant_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_GetWarrant_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_ModifyUserSecurity_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_ModifyUserSecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_RegQotPush_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_RegQotPush_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_RequestHistoryKLQuota_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_RequestHistoryKLQuota.proto',
   package='Qot_RequestHistoryKLQuota',
   syntax='proto2',
-  serialized_pb=_b('\n\x1fQot_RequestHistoryKLQuota.proto\x12\x19Qot_RequestHistoryKLQuota\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"c\n\nDetailItem\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x13\n\x0brequestTime\x18\x02 \x02(\t\x12\x18\n\x10requestTimeStamp\x18\x03 \x01(\x03\"\x19\n\x03\x43\x32S\x12\x12\n\nbGetDetail\x18\x02 \x01(\x08\"h\n\x03S2C\x12\x11\n\tusedQuota\x18\x01 \x02(\x05\x12\x13\n\x0bremainQuota\x18\x02 \x02(\x05\x12\x39\n\ndetailList\x18\x03 \x03(\x0b\x32%.Qot_RequestHistoryKLQuota.DetailItem\"6\n\x07Request\x12+\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x1e.Qot_RequestHistoryKLQuota.C2S\"o\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12+\n\x03s2c\x18\x04 \x01(\x0b\x32\x1e.Qot_RequestHistoryKLQuota.S2CBO\n\x13\x63om.futu.openapi.pbZ8github.com/futuopen/ftapi4go/pb/qotrequesthistoryklquota')
+  serialized_pb=_b('\n\x1fQot_RequestHistoryKLQuota.proto\x12\x19Qot_RequestHistoryKLQuota\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"q\n\nDetailItem\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0brequestTime\x18\x02 \x02(\t\x12\x18\n\x10requestTimeStamp\x18\x03 \x01(\x03\"\x19\n\x03\x43\x32S\x12\x12\n\nbGetDetail\x18\x02 \x01(\x08\"h\n\x03S2C\x12\x11\n\tusedQuota\x18\x01 \x02(\x05\x12\x13\n\x0bremainQuota\x18\x02 \x02(\x05\x12\x39\n\ndetailList\x18\x03 \x03(\x0b\x32%.Qot_RequestHistoryKLQuota.DetailItem\"6\n\x07Request\x12+\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x1e.Qot_RequestHistoryKLQuota.C2S\"o\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12+\n\x03s2c\x18\x04 \x01(\x0b\x32\x1e.Qot_RequestHistoryKLQuota.S2CBO\n\x13\x63om.futu.openapi.pbZ8github.com/futuopen/ftapi4go/pb/qotrequesthistoryklquota')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _DETAILITEM = _descriptor.Descriptor(
@@ -39,22 +39,29 @@
       name='security', full_name='Qot_RequestHistoryKLQuota.DetailItem.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='requestTime', full_name='Qot_RequestHistoryKLQuota.DetailItem.requestTime', index=1,
+      name='name', full_name='Qot_RequestHistoryKLQuota.DetailItem.name', index=1,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='requestTime', full_name='Qot_RequestHistoryKLQuota.DetailItem.requestTime', index=2,
       number=2, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='requestTimeStamp', full_name='Qot_RequestHistoryKLQuota.DetailItem.requestTimeStamp', index=2,
+      name='requestTimeStamp', full_name='Qot_RequestHistoryKLQuota.DetailItem.requestTimeStamp', index=3,
       number=3, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -65,15 +72,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=94,
-  serialized_end=193,
+  serialized_end=207,
 )
 
 
 _C2S = _descriptor.Descriptor(
   name='C2S',
   full_name='Qot_RequestHistoryKLQuota.C2S',
   filename=None,
@@ -95,16 +102,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=195,
-  serialized_end=220,
+  serialized_start=209,
+  serialized_end=234,
 )
 
 
 _S2C = _descriptor.Descriptor(
   name='S2C',
   full_name='Qot_RequestHistoryKLQuota.S2C',
   filename=None,
@@ -140,16 +147,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=222,
-  serialized_end=326,
+  serialized_start=236,
+  serialized_end=340,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_RequestHistoryKLQuota.Request',
   filename=None,
@@ -171,16 +178,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=328,
-  serialized_end=382,
+  serialized_start=342,
+  serialized_end=396,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_RequestHistoryKLQuota.Response',
   filename=None,
@@ -223,16 +230,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=384,
-  serialized_end=495,
+  serialized_start=398,
+  serialized_end=509,
 )
 
 _DETAILITEM.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['detailList'].message_type = _DETAILITEM
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['DetailItem'] = _DETAILITEM
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_RequestHistoryKL_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_RequestHistoryKL_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_RequestHistoryKL.proto',
   package='Qot_RequestHistoryKL',
   syntax='proto2',
-  serialized_pb=_b('\n\x1aQot_RequestHistoryKL.proto\x12\x14Qot_RequestHistoryKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\xcd\x01\n\x03\x43\x32S\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x11\n\tbeginTime\x18\x04 \x02(\t\x12\x0f\n\x07\x65ndTime\x18\x05 \x02(\t\x12\x13\n\x0bmaxAckKLNum\x18\x06 \x01(\x05\x12\x18\n\x10needKLFieldsFlag\x18\x07 \x01(\x03\x12\x12\n\nnextReqKey\x18\x08 \x01(\x0c\x12\x14\n\x0c\x65xtendedTime\x18\t \x01(\x08\"d\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12!\n\x06klList\x18\x02 \x03(\x0b\x32\x11.Qot_Common.KLine\x12\x12\n\nnextReqKey\x18\x03 \x01(\x0c\"1\n\x07Request\x12&\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x19.Qot_RequestHistoryKL.C2S\"j\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12&\n\x03s2c\x18\x04 \x01(\x0b\x32\x19.Qot_RequestHistoryKL.S2CBJ\n\x13\x63om.futu.openapi.pbZ3github.com/futuopen/ftapi4go/pb/qotrequesthistorykl')
+  serialized_pb=_b('\n\x1aQot_RequestHistoryKL.proto\x12\x14Qot_RequestHistoryKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\xcd\x01\n\x03\x43\x32S\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x11\n\tbeginTime\x18\x04 \x02(\t\x12\x0f\n\x07\x65ndTime\x18\x05 \x02(\t\x12\x13\n\x0bmaxAckKLNum\x18\x06 \x01(\x05\x12\x18\n\x10needKLFieldsFlag\x18\x07 \x01(\x03\x12\x12\n\nnextReqKey\x18\x08 \x01(\x0c\x12\x14\n\x0c\x65xtendedTime\x18\t \x01(\x08\"r\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x04 \x01(\t\x12!\n\x06klList\x18\x02 \x03(\x0b\x32\x11.Qot_Common.KLine\x12\x12\n\nnextReqKey\x18\x03 \x01(\x0c\"1\n\x07Request\x12&\n\x03\x63\x32s\x18\x01 \x02(\x0b\x32\x19.Qot_RequestHistoryKL.C2S\"j\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12&\n\x03s2c\x18\x04 \x01(\x0b\x32\x19.Qot_RequestHistoryKL.S2CBJ\n\x13\x63om.futu.openapi.pbZ3github.com/futuopen/ftapi4go/pb/qotrequesthistorykl')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _C2S = _descriptor.Descriptor(
@@ -126,22 +126,29 @@
       name='security', full_name='Qot_RequestHistoryKL.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='klList', full_name='Qot_RequestHistoryKL.S2C.klList', index=1,
+      name='name', full_name='Qot_RequestHistoryKL.S2C.name', index=1,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='klList', full_name='Qot_RequestHistoryKL.S2C.klList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='nextReqKey', full_name='Qot_RequestHistoryKL.S2C.nextReqKey', index=2,
+      name='nextReqKey', full_name='Qot_RequestHistoryKL.S2C.nextReqKey', index=3,
       number=3, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=_b(""),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -152,15 +159,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=292,
-  serialized_end=392,
+  serialized_end=406,
 )
 
 
 _REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='Qot_RequestHistoryKL.Request',
   filename=None,
@@ -182,16 +189,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=394,
-  serialized_end=443,
+  serialized_start=408,
+  serialized_end=457,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_RequestHistoryKL.Response',
   filename=None,
@@ -234,16 +241,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=445,
-  serialized_end=551,
+  serialized_start=459,
+  serialized_end=565,
 )
 
 _C2S.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['klList'].message_type = Qot__Common__pb2._KLINE
 _REQUEST.fields_by_name['c2s'].message_type = _C2S
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_RequestRehab_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_RequestRehab_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_RequestTradeDate_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_RequestTradeDate_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_SetPriceReminder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_SetPriceReminder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_StockFilter_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_StockFilter_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_Sub_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_Sub_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateBasicQot_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateBasicQot_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateBroker_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateBroker_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdateBroker.proto',
   package='Qot_UpdateBroker',
   syntax='proto2',
-  serialized_pb=_b('\n\x16Qot_UpdateBroker.proto\x12\x10Qot_UpdateBroker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\x83\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12)\n\rbrokerAskList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Broker\x12)\n\rbrokerBidList\x18\x03 \x03(\x0b\x32\x12.Qot_Common.Broker\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_UpdateBroker.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotupdatebroker')
+  serialized_pb=_b('\n\x16Qot_UpdateBroker.proto\x12\x10Qot_UpdateBroker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\x91\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x04 \x01(\t\x12)\n\rbrokerAskList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Broker\x12)\n\rbrokerBidList\x18\x03 \x03(\x0b\x32\x12.Qot_Common.Broker\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_UpdateBroker.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotupdatebroker')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _S2C = _descriptor.Descriptor(
@@ -39,22 +39,29 @@
       name='security', full_name='Qot_UpdateBroker.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='brokerAskList', full_name='Qot_UpdateBroker.S2C.brokerAskList', index=1,
+      name='name', full_name='Qot_UpdateBroker.S2C.name', index=1,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='brokerAskList', full_name='Qot_UpdateBroker.S2C.brokerAskList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='brokerBidList', full_name='Qot_UpdateBroker.S2C.brokerBidList', index=2,
+      name='brokerBidList', full_name='Qot_UpdateBroker.S2C.brokerBidList', index=3,
       number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -65,15 +72,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=77,
-  serialized_end=208,
+  serialized_end=222,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdateBroker.Response',
   filename=None,
@@ -116,16 +123,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=210,
-  serialized_end=312,
+  serialized_start=224,
+  serialized_end=326,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['brokerAskList'].message_type = Qot__Common__pb2._BROKER
 _S2C.fields_by_name['brokerBidList'].message_type = Qot__Common__pb2._BROKER
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateKL_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateKL_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdateKL.proto',
   package='Qot_UpdateKL',
   syntax='proto2',
-  serialized_pb=_b('\n\x12Qot_UpdateKL.proto\x12\x0cQot_UpdateKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"s\n\x03S2C\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12!\n\x06klList\x18\x04 \x03(\x0b\x32\x11.Qot_Common.KLine\"b\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1e\n\x03s2c\x18\x04 \x01(\x0b\x32\x11.Qot_UpdateKL.S2CBB\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/qotupdatekl')
+  serialized_pb=_b('\n\x12Qot_UpdateKL.proto\x12\x0cQot_UpdateKL\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\x81\x01\n\x03S2C\x12\x11\n\trehabType\x18\x01 \x02(\x05\x12\x0e\n\x06klType\x18\x02 \x02(\x05\x12&\n\x08security\x18\x03 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x05 \x01(\t\x12!\n\x06klList\x18\x04 \x03(\x0b\x32\x11.Qot_Common.KLine\"b\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1e\n\x03s2c\x18\x04 \x01(\x0b\x32\x11.Qot_UpdateKL.S2CBB\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/qotupdatekl')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _S2C = _descriptor.Descriptor(
@@ -53,15 +53,22 @@
       name='security', full_name='Qot_UpdateKL.S2C.security', index=2,
       number=3, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='klList', full_name='Qot_UpdateKL.S2C.klList', index=3,
+      name='name', full_name='Qot_UpdateKL.S2C.name', index=3,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='klList', full_name='Qot_UpdateKL.S2C.klList', index=4,
       number=4, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -71,16 +78,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=68,
-  serialized_end=183,
+  serialized_start=69,
+  serialized_end=198,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdateKL.Response',
   filename=None,
@@ -123,16 +130,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=185,
-  serialized_end=283,
+  serialized_start=200,
+  serialized_end=298,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['klList'].message_type = Qot__Common__pb2._KLINE
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateOrderBook_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateOrderBook_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdateOrderBook.proto',
   package='Qot_UpdateOrderBook',
   syntax='proto2',
-  serialized_pb=_b('\n\x19Qot_UpdateOrderBook.proto\x12\x13Qot_UpdateOrderBook\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\x81\x02\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12/\n\x10orderBookAskList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12/\n\x10orderBookBidList\x18\x03 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12\x16\n\x0esvrRecvTimeBid\x18\x04 \x01(\t\x12\x1f\n\x17svrRecvTimeBidTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0esvrRecvTimeAsk\x18\x06 \x01(\t\x12\x1f\n\x17svrRecvTimeAskTimestamp\x18\x07 \x01(\x01\"i\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12%\n\x03s2c\x18\x04 \x01(\x0b\x32\x18.Qot_UpdateOrderBook.S2CBI\n\x13\x63om.futu.openapi.pbZ2github.com/futuopen/ftapi4go/pb/qotupdateorderbook')
+  serialized_pb=_b('\n\x19Qot_UpdateOrderBook.proto\x12\x13Qot_UpdateOrderBook\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\x8f\x02\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x08 \x01(\t\x12/\n\x10orderBookAskList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12/\n\x10orderBookBidList\x18\x03 \x03(\x0b\x32\x15.Qot_Common.OrderBook\x12\x16\n\x0esvrRecvTimeBid\x18\x04 \x01(\t\x12\x1f\n\x17svrRecvTimeBidTimestamp\x18\x05 \x01(\x01\x12\x16\n\x0esvrRecvTimeAsk\x18\x06 \x01(\t\x12\x1f\n\x17svrRecvTimeAskTimestamp\x18\x07 \x01(\x01\"i\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12%\n\x03s2c\x18\x04 \x01(\x0b\x32\x18.Qot_UpdateOrderBook.S2CBI\n\x13\x63om.futu.openapi.pbZ2github.com/futuopen/ftapi4go/pb/qotupdateorderbook')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _S2C = _descriptor.Descriptor(
@@ -39,50 +39,57 @@
       name='security', full_name='Qot_UpdateOrderBook.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='orderBookAskList', full_name='Qot_UpdateOrderBook.S2C.orderBookAskList', index=1,
+      name='name', full_name='Qot_UpdateOrderBook.S2C.name', index=1,
+      number=8, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='orderBookAskList', full_name='Qot_UpdateOrderBook.S2C.orderBookAskList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='orderBookBidList', full_name='Qot_UpdateOrderBook.S2C.orderBookBidList', index=2,
+      name='orderBookBidList', full_name='Qot_UpdateOrderBook.S2C.orderBookBidList', index=3,
       number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeBid', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeBid', index=3,
+      name='svrRecvTimeBid', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeBid', index=4,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeBidTimestamp', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeBidTimestamp', index=4,
+      name='svrRecvTimeBidTimestamp', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeBidTimestamp', index=5,
       number=5, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeAsk', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeAsk', index=5,
+      name='svrRecvTimeAsk', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeAsk', index=6,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='svrRecvTimeAskTimestamp', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeAskTimestamp', index=6,
+      name='svrRecvTimeAskTimestamp', full_name='Qot_UpdateOrderBook.S2C.svrRecvTimeAskTimestamp', index=7,
       number=7, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -93,15 +100,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=83,
-  serialized_end=340,
+  serialized_end=354,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdateOrderBook.Response',
   filename=None,
@@ -144,16 +151,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=342,
-  serialized_end=447,
+  serialized_start=356,
+  serialized_end=461,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['orderBookAskList'].message_type = Qot__Common__pb2._ORDERBOOK
 _S2C.fields_by_name['orderBookBidList'].message_type = Qot__Common__pb2._ORDERBOOK
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdatePriceReminder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdatePriceReminder_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdatePriceReminder.proto',
   package='Qot_UpdatePriceReminder',
   syntax='proto2',
-  serialized_pb=_b('\n\x1dQot_UpdatePriceReminder.proto\x12\x17Qot_UpdatePriceReminder\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\xc4\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\r\n\x05price\x18\x02 \x02(\x01\x12\x12\n\nchangeRate\x18\x03 \x02(\x01\x12\x14\n\x0cmarketStatus\x18\x04 \x02(\x05\x12\x0f\n\x07\x63ontent\x18\x05 \x02(\t\x12\x0c\n\x04note\x18\x06 \x02(\t\x12\x0b\n\x03key\x18\x07 \x01(\x03\x12\x0c\n\x04type\x18\x08 \x01(\x05\x12\x10\n\x08setValue\x18\t \x01(\x01\x12\x10\n\x08\x63urValue\x18\n \x01(\x01\"m\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12)\n\x03s2c\x18\x04 \x01(\x0b\x32\x1c.Qot_UpdatePriceReminder.S2C*p\n\x0cMarketStatus\x12\x17\n\x13MarketStatus_Unknow\x10\x00\x12\x15\n\x11MarketStatus_Open\x10\x01\x12\x16\n\x12MarketStatus_USPre\x10\x02\x12\x18\n\x14MarketStatus_USAfter\x10\x03\x42M\n\x13\x63om.futu.openapi.pbZ6github.com/futuopen/ftapi4go/pb/qotupdatepricereminder')
+  serialized_pb=_b('\n\x1dQot_UpdatePriceReminder.proto\x12\x17Qot_UpdatePriceReminder\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"\xd2\x01\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x0b \x01(\t\x12\r\n\x05price\x18\x02 \x02(\x01\x12\x12\n\nchangeRate\x18\x03 \x02(\x01\x12\x14\n\x0cmarketStatus\x18\x04 \x02(\x05\x12\x0f\n\x07\x63ontent\x18\x05 \x02(\t\x12\x0c\n\x04note\x18\x06 \x02(\t\x12\x0b\n\x03key\x18\x07 \x01(\x03\x12\x0c\n\x04type\x18\x08 \x01(\x05\x12\x10\n\x08setValue\x18\t \x01(\x01\x12\x10\n\x08\x63urValue\x18\n \x01(\x01\"m\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12)\n\x03s2c\x18\x04 \x01(\x0b\x32\x1c.Qot_UpdatePriceReminder.S2C*p\n\x0cMarketStatus\x12\x17\n\x13MarketStatus_Unknow\x10\x00\x12\x15\n\x11MarketStatus_Open\x10\x01\x12\x16\n\x12MarketStatus_USPre\x10\x02\x12\x18\n\x14MarketStatus_USAfter\x10\x03\x42M\n\x13\x63om.futu.openapi.pbZ6github.com/futuopen/ftapi4go/pb/qotupdatepricereminder')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 _MARKETSTATUS = _descriptor.EnumDescriptor(
   name='MarketStatus',
   full_name='Qot_UpdatePriceReminder.MarketStatus',
   filename=None,
@@ -47,16 +47,16 @@
     _descriptor.EnumValueDescriptor(
       name='MarketStatus_USAfter', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=400,
-  serialized_end=512,
+  serialized_start=414,
+  serialized_end=526,
 )
 _sym_db.RegisterEnumDescriptor(_MARKETSTATUS)
 
 MarketStatus = enum_type_wrapper.EnumTypeWrapper(_MARKETSTATUS)
 MarketStatus_Unknow = 0
 MarketStatus_Open = 1
 MarketStatus_USPre = 2
@@ -75,71 +75,78 @@
       name='security', full_name='Qot_UpdatePriceReminder.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='price', full_name='Qot_UpdatePriceReminder.S2C.price', index=1,
+      name='name', full_name='Qot_UpdatePriceReminder.S2C.name', index=1,
+      number=11, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='price', full_name='Qot_UpdatePriceReminder.S2C.price', index=2,
       number=2, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='changeRate', full_name='Qot_UpdatePriceReminder.S2C.changeRate', index=2,
+      name='changeRate', full_name='Qot_UpdatePriceReminder.S2C.changeRate', index=3,
       number=3, type=1, cpp_type=5, label=2,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='marketStatus', full_name='Qot_UpdatePriceReminder.S2C.marketStatus', index=3,
+      name='marketStatus', full_name='Qot_UpdatePriceReminder.S2C.marketStatus', index=4,
       number=4, type=5, cpp_type=1, label=2,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='content', full_name='Qot_UpdatePriceReminder.S2C.content', index=4,
+      name='content', full_name='Qot_UpdatePriceReminder.S2C.content', index=5,
       number=5, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='note', full_name='Qot_UpdatePriceReminder.S2C.note', index=5,
+      name='note', full_name='Qot_UpdatePriceReminder.S2C.note', index=6,
       number=6, type=9, cpp_type=9, label=2,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='key', full_name='Qot_UpdatePriceReminder.S2C.key', index=6,
+      name='key', full_name='Qot_UpdatePriceReminder.S2C.key', index=7,
       number=7, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='type', full_name='Qot_UpdatePriceReminder.S2C.type', index=7,
+      name='type', full_name='Qot_UpdatePriceReminder.S2C.type', index=8,
       number=8, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='setValue', full_name='Qot_UpdatePriceReminder.S2C.setValue', index=8,
+      name='setValue', full_name='Qot_UpdatePriceReminder.S2C.setValue', index=9,
       number=9, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='curValue', full_name='Qot_UpdatePriceReminder.S2C.curValue', index=9,
+      name='curValue', full_name='Qot_UpdatePriceReminder.S2C.curValue', index=10,
       number=10, type=1, cpp_type=5, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -150,15 +157,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=91,
-  serialized_end=287,
+  serialized_end=301,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdatePriceReminder.Response',
   filename=None,
@@ -201,16 +208,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=289,
-  serialized_end=398,
+  serialized_start=303,
+  serialized_end=412,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
 DESCRIPTOR.enum_types_by_name['MarketStatus'] = _MARKETSTATUS
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateRT_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateRT_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdateRT.proto',
   package='Qot_UpdateRT',
   syntax='proto2',
-  serialized_pb=_b('\n\x12Qot_UpdateRT.proto\x12\x0cQot_UpdateRT\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"T\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12%\n\x06rtList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.TimeShare\"b\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1e\n\x03s2c\x18\x04 \x01(\x0b\x32\x11.Qot_UpdateRT.S2CBB\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/qotupdatert')
+  serialized_pb=_b('\n\x12Qot_UpdateRT.proto\x12\x0cQot_UpdateRT\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"b\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12%\n\x06rtList\x18\x02 \x03(\x0b\x32\x15.Qot_Common.TimeShare\"b\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\x1e\n\x03s2c\x18\x04 \x01(\x0b\x32\x11.Qot_UpdateRT.S2CBB\n\x13\x63om.futu.openapi.pbZ+github.com/futuopen/ftapi4go/pb/qotupdatert')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _S2C = _descriptor.Descriptor(
@@ -39,15 +39,22 @@
       name='security', full_name='Qot_UpdateRT.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='rtList', full_name='Qot_UpdateRT.S2C.rtList', index=1,
+      name='name', full_name='Qot_UpdateRT.S2C.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='rtList', full_name='Qot_UpdateRT.S2C.rtList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -58,15 +65,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=68,
-  serialized_end=152,
+  serialized_end=166,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdateRT.Response',
   filename=None,
@@ -109,16 +116,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=154,
-  serialized_end=252,
+  serialized_start=168,
+  serialized_end=266,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['rtList'].message_type = Qot__Common__pb2._TIMESHARE
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Qot_UpdateTicker_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Qot_UpdateTicker_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Qot_Common_pb2 as Qot__Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Qot_UpdateTicker.proto',
   package='Qot_UpdateTicker',
   syntax='proto2',
-  serialized_pb=_b('\n\x16Qot_UpdateTicker.proto\x12\x10Qot_UpdateTicker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"U\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12&\n\ntickerList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Ticker\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_UpdateTicker.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotupdateticker')
+  serialized_pb=_b('\n\x16Qot_UpdateTicker.proto\x12\x10Qot_UpdateTicker\x1a\x0c\x43ommon.proto\x1a\x10Qot_Common.proto\"c\n\x03S2C\x12&\n\x08security\x18\x01 \x02(\x0b\x32\x14.Qot_Common.Security\x12\x0c\n\x04name\x18\x03 \x01(\t\x12&\n\ntickerList\x18\x02 \x03(\x0b\x32\x12.Qot_Common.Ticker\"f\n\x08Response\x12\x15\n\x07retType\x18\x01 \x02(\x05:\x04-400\x12\x0e\n\x06retMsg\x18\x02 \x01(\t\x12\x0f\n\x07\x65rrCode\x18\x03 \x01(\x05\x12\"\n\x03s2c\x18\x04 \x01(\x0b\x32\x15.Qot_UpdateTicker.S2CBF\n\x13\x63om.futu.openapi.pbZ/github.com/futuopen/ftapi4go/pb/qotupdateticker')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,Qot__Common__pb2.DESCRIPTOR,])
 
 
 
 
 _S2C = _descriptor.Descriptor(
@@ -39,15 +39,22 @@
       name='security', full_name='Qot_UpdateTicker.S2C.security', index=0,
       number=1, type=11, cpp_type=10, label=2,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='tickerList', full_name='Qot_UpdateTicker.S2C.tickerList', index=1,
+      name='name', full_name='Qot_UpdateTicker.S2C.name', index=1,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='tickerList', full_name='Qot_UpdateTicker.S2C.tickerList', index=2,
       number=2, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -58,15 +65,15 @@
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=76,
-  serialized_end=161,
+  serialized_end=175,
 )
 
 
 _RESPONSE = _descriptor.Descriptor(
   name='Response',
   full_name='Qot_UpdateTicker.Response',
   filename=None,
@@ -109,16 +116,16 @@
   ],
   options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=163,
-  serialized_end=265,
+  serialized_start=177,
+  serialized_end=279,
 )
 
 _S2C.fields_by_name['security'].message_type = Qot__Common__pb2._SECURITY
 _S2C.fields_by_name['tickerList'].message_type = Qot__Common__pb2._TICKER
 _RESPONSE.fields_by_name['s2c'].message_type = _S2C
 DESCRIPTOR.message_types_by_name['S2C'] = _S2C
 DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
```

### Comparing `futu-api-7.1.3308/futu/common/pb/TestCmd_pb2.py` & `futu-api-7.2.3408/futu/common/pb/TestCmd_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_Common_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_Common_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import Common_pb2 as Common__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='Trd_Common.proto',
   package='Trd_Common',
   syntax='proto2',
-  serialized_pb=_b('\n\x10Trd_Common.proto\x12\nTrd_Common\x1a\x0c\x43ommon.proto\"G\n\x0b\x41\x63\x63\x43\x61shInfo\x12\x10\n\x08\x63urrency\x18\x01 \x01(\x05\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x18\n\x10\x61vailableBalance\x18\x03 \x01(\x01\"=\n\tTrdHeader\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x11\n\ttrdMarket\x18\x03 \x02(\x05\"\x8e\x01\n\x06TrdAcc\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x19\n\x11trdMarketAuthList\x18\x03 \x03(\x05\x12\x0f\n\x07\x61\x63\x63Type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63\x61rdNum\x18\x05 \x01(\t\x12\x14\n\x0csecurityFirm\x18\x06 \x01(\x05\x12\x12\n\nsimAccType\x18\x07 \x01(\x05\"\xf3\x04\n\x05\x46unds\x12\r\n\x05power\x18\x01 \x02(\x01\x12\x13\n\x0btotalAssets\x18\x02 \x02(\x01\x12\x0c\n\x04\x63\x61sh\x18\x03 \x02(\x01\x12\x11\n\tmarketVal\x18\x04 \x02(\x01\x12\x12\n\nfrozenCash\x18\x05 \x02(\x01\x12\x10\n\x08\x64\x65\x62tCash\x18\x06 \x02(\x01\x12\x19\n\x11\x61vlWithdrawalCash\x18\x07 \x02(\x01\x12\x10\n\x08\x63urrency\x18\x08 \x01(\x05\x12\x16\n\x0e\x61vailableFunds\x18\t \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\n \x01(\x01\x12\x12\n\nrealizedPL\x18\x0b \x01(\x01\x12\x11\n\triskLevel\x18\x0c \x01(\x05\x12\x15\n\rinitialMargin\x18\r \x01(\x01\x12\x19\n\x11maintenanceMargin\x18\x0e \x01(\x01\x12-\n\x0c\x63\x61shInfoList\x18\x0f \x03(\x0b\x32\x17.Trd_Common.AccCashInfo\x12\x15\n\rmaxPowerShort\x18\x10 \x01(\x01\x12\x14\n\x0cnetCashPower\x18\x11 \x01(\x01\x12\x0e\n\x06longMv\x18\x12 \x01(\x01\x12\x0f\n\x07shortMv\x18\x13 \x01(\x01\x12\x14\n\x0cpendingAsset\x18\x14 \x01(\x01\x12\x15\n\rmaxWithdrawal\x18\x15 \x01(\x01\x12\x12\n\nriskStatus\x18\x16 \x01(\x05\x12\x18\n\x10marginCallMargin\x18\x17 \x01(\x01\x12\r\n\x05isPdt\x18\x18 \x01(\x08\x12\x0e\n\x06pdtSeq\x18\x19 \x01(\t\x12\x15\n\rbeginningDTBP\x18\x1a \x01(\x01\x12\x15\n\rremainingDTBP\x18\x1b \x01(\x01\x12\x14\n\x0c\x64tCallAmount\x18\x1c \x01(\x01\x12\x10\n\x08\x64tStatus\x18\x1d \x01(\x05\"\x95\x03\n\x08Position\x12\x12\n\npositionID\x18\x01 \x02(\x04\x12\x14\n\x0cpositionSide\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\x0c\n\x04name\x18\x04 \x02(\t\x12\x0b\n\x03qty\x18\x05 \x02(\x01\x12\x12\n\ncanSellQty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x02(\x01\x12\x11\n\tcostPrice\x18\x08 \x01(\x01\x12\x0b\n\x03val\x18\t \x02(\x01\x12\r\n\x05plVal\x18\n \x02(\x01\x12\x0f\n\x07plRatio\x18\x0b \x01(\x01\x12\x11\n\tsecMarket\x18\x0c \x01(\x05\x12\x10\n\x08td_plVal\x18\x15 \x01(\x01\x12\x11\n\ttd_trdVal\x18\x16 \x01(\x01\x12\x11\n\ttd_buyVal\x18\x17 \x01(\x01\x12\x11\n\ttd_buyQty\x18\x18 \x01(\x01\x12\x12\n\ntd_sellVal\x18\x19 \x01(\x01\x12\x12\n\ntd_sellQty\x18\x1a \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\x1c \x01(\x01\x12\x12\n\nrealizedPL\x18\x1d \x01(\x01\x12\x10\n\x08\x63urrency\x18\x1e \x01(\x05\x12\x11\n\ttrdMarket\x18\x1f \x01(\x05\"\xf4\x03\n\x05Order\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x13\n\x0borderStatus\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x02(\x04\x12\x11\n\torderIDEx\x18\x05 \x02(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x12\n\nupdateTime\x18\x0b \x02(\t\x12\x0f\n\x07\x66illQty\x18\x0c \x01(\x01\x12\x14\n\x0c\x66illAvgPrice\x18\r \x01(\x01\x12\x12\n\nlastErrMsg\x18\x0e \x01(\t\x12\x11\n\tsecMarket\x18\x0f \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x0e\n\x06remark\x18\x12 \x01(\t\x12\x13\n\x0btimeInForce\x18\x13 \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\x14 \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x15 \x01(\x01\x12\x11\n\ttrailType\x18\x16 \x01(\x05\x12\x12\n\ntrailValue\x18\x17 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x18 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x19 \x01(\x05\x12\x11\n\ttrdMarket\x18\x1a \x01(\x05\"\xb7\x02\n\tOrderFill\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x0e\n\x06\x66illID\x18\x02 \x02(\x04\x12\x10\n\x08\x66illIDEx\x18\x03 \x02(\t\x12\x0f\n\x07orderID\x18\x04 \x01(\x04\x12\x11\n\torderIDEx\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x02(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x17\n\x0f\x63ounterBrokerID\x18\x0b \x01(\x05\x12\x19\n\x11\x63ounterBrokerName\x18\x0c \x01(\t\x12\x11\n\tsecMarket\x18\r \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x0f \x01(\x01\x12\x0e\n\x06status\x18\x10 \x01(\x05\"\xb1\x01\n\nMaxTrdQtys\x12\x12\n\nmaxCashBuy\x18\x01 \x02(\x01\x12\x1b\n\x13maxCashAndMarginBuy\x18\x02 \x01(\x01\x12\x17\n\x0fmaxPositionSell\x18\x03 \x02(\x01\x12\x14\n\x0cmaxSellShort\x18\x04 \x01(\x01\x12\x12\n\nmaxBuyBack\x18\x05 \x01(\x01\x12\x16\n\x0elongRequiredIM\x18\x06 \x01(\x01\x12\x17\n\x0fshortRequiredIM\x18\x07 \x01(\x01\"[\n\x13TrdFilterConditions\x12\x10\n\x08\x63odeList\x18\x01 \x03(\t\x12\x0e\n\x06idList\x18\x02 \x03(\x04\x12\x11\n\tbeginTime\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndTime\x18\x04 \x01(\t*.\n\x06TrdEnv\x12\x13\n\x0fTrdEnv_Simulate\x10\x00\x12\x0f\n\x0bTrdEnv_Real\x10\x01*X\n\x0bTrdCategory\x12\x17\n\x13TrdCategory_Unknown\x10\x00\x12\x18\n\x14TrdCategory_Security\x10\x01\x12\x16\n\x12TrdCategory_Future\x10\x02*\x95\x01\n\tTrdMarket\x12\x15\n\x11TrdMarket_Unknown\x10\x00\x12\x10\n\x0cTrdMarket_HK\x10\x01\x12\x10\n\x0cTrdMarket_US\x10\x02\x12\x10\n\x0cTrdMarket_CN\x10\x03\x12\x12\n\x0eTrdMarket_HKCC\x10\x04\x12\x15\n\x11TrdMarket_Futures\x10\x05\x12\x10\n\x0cTrdMarket_SG\x10\x06*\xac\x01\n\x0cTrdSecMarket\x12\x18\n\x14TrdSecMarket_Unknown\x10\x00\x12\x13\n\x0fTrdSecMarket_HK\x10\x01\x12\x13\n\x0fTrdSecMarket_US\x10\x02\x12\x16\n\x12TrdSecMarket_CN_SH\x10\x1f\x12\x16\n\x12TrdSecMarket_CN_SZ\x10 \x12\x13\n\x0fTrdSecMarket_SG\x10)\x12\x13\n\x0fTrdSecMarket_JP\x10\x33*m\n\x07TrdSide\x12\x13\n\x0fTrdSide_Unknown\x10\x00\x12\x0f\n\x0bTrdSide_Buy\x10\x01\x12\x10\n\x0cTrdSide_Sell\x10\x02\x12\x15\n\x11TrdSide_SellShort\x10\x03\x12\x13\n\x0fTrdSide_BuyBack\x10\x04*\x81\x03\n\tOrderType\x12\x15\n\x11OrderType_Unknown\x10\x00\x12\x14\n\x10OrderType_Normal\x10\x01\x12\x14\n\x10OrderType_Market\x10\x02\x12\x1b\n\x17OrderType_AbsoluteLimit\x10\x05\x12\x15\n\x11OrderType_Auction\x10\x06\x12\x1a\n\x16OrderType_AuctionLimit\x10\x07\x12\x1a\n\x16OrderType_SpecialLimit\x10\x08\x12\x1e\n\x1aOrderType_SpecialLimit_All\x10\t\x12\x12\n\x0eOrderType_Stop\x10\n\x12\x17\n\x13OrderType_StopLimit\x10\x0b\x12\x1d\n\x19OrderType_MarketifTouched\x10\x0c\x12\x1c\n\x18OrderType_LimitifTouched\x10\r\x12\x1a\n\x16OrderType_TrailingStop\x10\x0e\x12\x1f\n\x1bOrderType_TrailingStopLimit\x10\x0f*M\n\tTrailType\x12\x15\n\x11TrailType_Unknown\x10\x00\x12\x13\n\x0fTrailType_Ratio\x10\x01\x12\x14\n\x10TrailType_Amount\x10\x02*\xfc\x03\n\x0bOrderStatus\x12\x1b\n\x17OrderStatus_Unsubmitted\x10\x00\x12 \n\x13OrderStatus_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x1d\n\x19OrderStatus_WaitingSubmit\x10\x01\x12\x1a\n\x16OrderStatus_Submitting\x10\x02\x12\x1c\n\x18OrderStatus_SubmitFailed\x10\x03\x12\x17\n\x13OrderStatus_TimeOut\x10\x04\x12\x19\n\x15OrderStatus_Submitted\x10\x05\x12\x1b\n\x17OrderStatus_Filled_Part\x10\n\x12\x1a\n\x16OrderStatus_Filled_All\x10\x0b\x12\x1f\n\x1bOrderStatus_Cancelling_Part\x10\x0c\x12\x1e\n\x1aOrderStatus_Cancelling_All\x10\r\x12\x1e\n\x1aOrderStatus_Cancelled_Part\x10\x0e\x12\x1d\n\x19OrderStatus_Cancelled_All\x10\x0f\x12\x16\n\x12OrderStatus_Failed\x10\x15\x12\x18\n\x14OrderStatus_Disabled\x10\x16\x12\x17\n\x13OrderStatus_Deleted\x10\x17\x12\x1d\n\x19OrderStatus_FillCancelled\x10\x18*e\n\x0fOrderFillStatus\x12\x16\n\x12OrderFillStatus_OK\x10\x00\x12\x1d\n\x19OrderFillStatus_Cancelled\x10\x01\x12\x1b\n\x17OrderFillStatus_Changed\x10\x02*`\n\x0cPositionSide\x12\x15\n\x11PositionSide_Long\x10\x00\x12!\n\x14PositionSide_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x16\n\x12PositionSide_Short\x10\x01*\xad\x01\n\rModifyOrderOp\x12\x19\n\x15ModifyOrderOp_Unknown\x10\x00\x12\x18\n\x14ModifyOrderOp_Normal\x10\x01\x12\x18\n\x14ModifyOrderOp_Cancel\x10\x02\x12\x19\n\x15ModifyOrderOp_Disable\x10\x03\x12\x18\n\x14ModifyOrderOp_Enable\x10\x04\x12\x18\n\x14ModifyOrderOp_Delete\x10\x05*P\n\nTrdAccType\x12\x16\n\x12TrdAccType_Unknown\x10\x00\x12\x13\n\x0fTrdAccType_Cash\x10\x01\x12\x15\n\x11TrdAccType_Margin\x10\x02*z\n\x08\x43urrency\x12\x14\n\x10\x43urrency_Unknown\x10\x00\x12\x10\n\x0c\x43urrency_HKD\x10\x01\x12\x10\n\x0c\x43urrency_USD\x10\x02\x12\x10\n\x0c\x43urrency_CNH\x10\x03\x12\x10\n\x0c\x43urrency_JPY\x10\x04\x12\x10\n\x0c\x43urrency_SGD\x10\x05*\xb6\x01\n\x0c\x43ltRiskLevel\x12!\n\x14\x43ltRiskLevel_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x43ltRiskLevel_Safe\x10\x00\x12\x18\n\x14\x43ltRiskLevel_Warning\x10\x01\x12\x17\n\x13\x43ltRiskLevel_Danger\x10\x02\x12\x1d\n\x19\x43ltRiskLevel_AbsoluteSafe\x10\x03\x12\x1a\n\x16\x43ltRiskLevel_OptDanger\x10\x04*7\n\x0bTimeInForce\x12\x13\n\x0fTimeInForce_DAY\x10\x00\x12\x13\n\x0fTimeInForce_GTC\x10\x01*|\n\x0cSecurityFirm\x12\x18\n\x14SecurityFirm_Unknown\x10\x00\x12\x1f\n\x1bSecurityFirm_FutuSecurities\x10\x01\x12\x18\n\x14SecurityFirm_FutuInc\x10\x02\x12\x17\n\x13SecurityFirm_FutuSG\x10\x03*Q\n\nSimAccType\x12\x16\n\x12SimAccType_Unknown\x10\x00\x12\x14\n\x10SimAccType_Stock\x10\x01\x12\x15\n\x11SimAccType_Option\x10\x02*\x94\x02\n\rCltRiskStatus\x12\x19\n\x15\x43ltRiskStatus_Unknown\x10\x00\x12\x18\n\x14\x43ltRiskStatus_Level1\x10\x01\x12\x18\n\x14\x43ltRiskStatus_Level2\x10\x02\x12\x18\n\x14\x43ltRiskStatus_Level3\x10\x03\x12\x18\n\x14\x43ltRiskStatus_Level4\x10\x04\x12\x18\n\x14\x43ltRiskStatus_Level5\x10\x05\x12\x18\n\x14\x43ltRiskStatus_Level6\x10\x06\x12\x18\n\x14\x43ltRiskStatus_Level7\x10\x07\x12\x18\n\x14\x43ltRiskStatus_Level8\x10\x08\x12\x18\n\x14\x43ltRiskStatus_Level9\x10\t*b\n\x08\x44TStatus\x12\x14\n\x10\x44TStatus_Unknown\x10\x00\x12\x16\n\x12\x44TStatus_Unlimited\x10\x01\x12\x13\n\x0f\x44TStatus_EMCall\x10\x02\x12\x13\n\x0f\x44TStatus_DTCall\x10\x03\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/trdcommon')
+  serialized_pb=_b('\n\x10Trd_Common.proto\x12\nTrd_Common\x1a\x0c\x43ommon.proto\"G\n\x0b\x41\x63\x63\x43\x61shInfo\x12\x10\n\x08\x63urrency\x18\x01 \x01(\x05\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x18\n\x10\x61vailableBalance\x18\x03 \x01(\x01\"=\n\tTrdHeader\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x11\n\ttrdMarket\x18\x03 \x02(\x05\"\x8e\x01\n\x06TrdAcc\x12\x0e\n\x06trdEnv\x18\x01 \x02(\x05\x12\r\n\x05\x61\x63\x63ID\x18\x02 \x02(\x04\x12\x19\n\x11trdMarketAuthList\x18\x03 \x03(\x05\x12\x0f\n\x07\x61\x63\x63Type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63\x61rdNum\x18\x05 \x01(\t\x12\x14\n\x0csecurityFirm\x18\x06 \x01(\x05\x12\x12\n\nsimAccType\x18\x07 \x01(\x05\"\xf3\x04\n\x05\x46unds\x12\r\n\x05power\x18\x01 \x02(\x01\x12\x13\n\x0btotalAssets\x18\x02 \x02(\x01\x12\x0c\n\x04\x63\x61sh\x18\x03 \x02(\x01\x12\x11\n\tmarketVal\x18\x04 \x02(\x01\x12\x12\n\nfrozenCash\x18\x05 \x02(\x01\x12\x10\n\x08\x64\x65\x62tCash\x18\x06 \x02(\x01\x12\x19\n\x11\x61vlWithdrawalCash\x18\x07 \x02(\x01\x12\x10\n\x08\x63urrency\x18\x08 \x01(\x05\x12\x16\n\x0e\x61vailableFunds\x18\t \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\n \x01(\x01\x12\x12\n\nrealizedPL\x18\x0b \x01(\x01\x12\x11\n\triskLevel\x18\x0c \x01(\x05\x12\x15\n\rinitialMargin\x18\r \x01(\x01\x12\x19\n\x11maintenanceMargin\x18\x0e \x01(\x01\x12-\n\x0c\x63\x61shInfoList\x18\x0f \x03(\x0b\x32\x17.Trd_Common.AccCashInfo\x12\x15\n\rmaxPowerShort\x18\x10 \x01(\x01\x12\x14\n\x0cnetCashPower\x18\x11 \x01(\x01\x12\x0e\n\x06longMv\x18\x12 \x01(\x01\x12\x0f\n\x07shortMv\x18\x13 \x01(\x01\x12\x14\n\x0cpendingAsset\x18\x14 \x01(\x01\x12\x15\n\rmaxWithdrawal\x18\x15 \x01(\x01\x12\x12\n\nriskStatus\x18\x16 \x01(\x05\x12\x18\n\x10marginCallMargin\x18\x17 \x01(\x01\x12\r\n\x05isPdt\x18\x18 \x01(\x08\x12\x0e\n\x06pdtSeq\x18\x19 \x01(\t\x12\x15\n\rbeginningDTBP\x18\x1a \x01(\x01\x12\x15\n\rremainingDTBP\x18\x1b \x01(\x01\x12\x14\n\x0c\x64tCallAmount\x18\x1c \x01(\x01\x12\x10\n\x08\x64tStatus\x18\x1d \x01(\x05\"\x95\x03\n\x08Position\x12\x12\n\npositionID\x18\x01 \x02(\x04\x12\x14\n\x0cpositionSide\x18\x02 \x02(\x05\x12\x0c\n\x04\x63ode\x18\x03 \x02(\t\x12\x0c\n\x04name\x18\x04 \x02(\t\x12\x0b\n\x03qty\x18\x05 \x02(\x01\x12\x12\n\ncanSellQty\x18\x06 \x02(\x01\x12\r\n\x05price\x18\x07 \x02(\x01\x12\x11\n\tcostPrice\x18\x08 \x01(\x01\x12\x0b\n\x03val\x18\t \x02(\x01\x12\r\n\x05plVal\x18\n \x02(\x01\x12\x0f\n\x07plRatio\x18\x0b \x01(\x01\x12\x11\n\tsecMarket\x18\x0c \x01(\x05\x12\x10\n\x08td_plVal\x18\x15 \x01(\x01\x12\x11\n\ttd_trdVal\x18\x16 \x01(\x01\x12\x11\n\ttd_buyVal\x18\x17 \x01(\x01\x12\x11\n\ttd_buyQty\x18\x18 \x01(\x01\x12\x12\n\ntd_sellVal\x18\x19 \x01(\x01\x12\x12\n\ntd_sellQty\x18\x1a \x01(\x01\x12\x14\n\x0cunrealizedPL\x18\x1c \x01(\x01\x12\x12\n\nrealizedPL\x18\x1d \x01(\x01\x12\x10\n\x08\x63urrency\x18\x1e \x01(\x05\x12\x11\n\ttrdMarket\x18\x1f \x01(\x05\"\xf4\x03\n\x05Order\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x11\n\torderType\x18\x02 \x02(\x05\x12\x13\n\x0borderStatus\x18\x03 \x02(\x05\x12\x0f\n\x07orderID\x18\x04 \x02(\x04\x12\x11\n\torderIDEx\x18\x05 \x02(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x01(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x12\n\nupdateTime\x18\x0b \x02(\t\x12\x0f\n\x07\x66illQty\x18\x0c \x01(\x01\x12\x14\n\x0c\x66illAvgPrice\x18\r \x01(\x01\x12\x12\n\nlastErrMsg\x18\x0e \x01(\t\x12\x11\n\tsecMarket\x18\x0f \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x10 \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x11 \x01(\x01\x12\x0e\n\x06remark\x18\x12 \x01(\t\x12\x13\n\x0btimeInForce\x18\x13 \x01(\x05\x12\x16\n\x0e\x66illOutsideRTH\x18\x14 \x01(\x08\x12\x10\n\x08\x61uxPrice\x18\x15 \x01(\x01\x12\x11\n\ttrailType\x18\x16 \x01(\x05\x12\x12\n\ntrailValue\x18\x17 \x01(\x01\x12\x13\n\x0btrailSpread\x18\x18 \x01(\x01\x12\x10\n\x08\x63urrency\x18\x19 \x01(\x05\x12\x11\n\ttrdMarket\x18\x1a \x01(\x05\"\xb7\x02\n\tOrderFill\x12\x0f\n\x07trdSide\x18\x01 \x02(\x05\x12\x0e\n\x06\x66illID\x18\x02 \x02(\x04\x12\x10\n\x08\x66illIDEx\x18\x03 \x02(\t\x12\x0f\n\x07orderID\x18\x04 \x01(\x04\x12\x11\n\torderIDEx\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x02(\t\x12\x0c\n\x04name\x18\x07 \x02(\t\x12\x0b\n\x03qty\x18\x08 \x02(\x01\x12\r\n\x05price\x18\t \x02(\x01\x12\x12\n\ncreateTime\x18\n \x02(\t\x12\x17\n\x0f\x63ounterBrokerID\x18\x0b \x01(\x05\x12\x19\n\x11\x63ounterBrokerName\x18\x0c \x01(\t\x12\x11\n\tsecMarket\x18\r \x01(\x05\x12\x17\n\x0f\x63reateTimestamp\x18\x0e \x01(\x01\x12\x17\n\x0fupdateTimestamp\x18\x0f \x01(\x01\x12\x0e\n\x06status\x18\x10 \x01(\x05\"\xb1\x01\n\nMaxTrdQtys\x12\x12\n\nmaxCashBuy\x18\x01 \x02(\x01\x12\x1b\n\x13maxCashAndMarginBuy\x18\x02 \x01(\x01\x12\x17\n\x0fmaxPositionSell\x18\x03 \x02(\x01\x12\x14\n\x0cmaxSellShort\x18\x04 \x01(\x01\x12\x12\n\nmaxBuyBack\x18\x05 \x01(\x01\x12\x16\n\x0elongRequiredIM\x18\x06 \x01(\x01\x12\x17\n\x0fshortRequiredIM\x18\x07 \x01(\x01\"[\n\x13TrdFilterConditions\x12\x10\n\x08\x63odeList\x18\x01 \x03(\t\x12\x0e\n\x06idList\x18\x02 \x03(\x04\x12\x11\n\tbeginTime\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndTime\x18\x04 \x01(\t*.\n\x06TrdEnv\x12\x13\n\x0fTrdEnv_Simulate\x10\x00\x12\x0f\n\x0bTrdEnv_Real\x10\x01*X\n\x0bTrdCategory\x12\x17\n\x13TrdCategory_Unknown\x10\x00\x12\x18\n\x14TrdCategory_Security\x10\x01\x12\x16\n\x12TrdCategory_Future\x10\x02*\x95\x01\n\tTrdMarket\x12\x15\n\x11TrdMarket_Unknown\x10\x00\x12\x10\n\x0cTrdMarket_HK\x10\x01\x12\x10\n\x0cTrdMarket_US\x10\x02\x12\x10\n\x0cTrdMarket_CN\x10\x03\x12\x12\n\x0eTrdMarket_HKCC\x10\x04\x12\x15\n\x11TrdMarket_Futures\x10\x05\x12\x10\n\x0cTrdMarket_SG\x10\x06*\xac\x01\n\x0cTrdSecMarket\x12\x18\n\x14TrdSecMarket_Unknown\x10\x00\x12\x13\n\x0fTrdSecMarket_HK\x10\x01\x12\x13\n\x0fTrdSecMarket_US\x10\x02\x12\x16\n\x12TrdSecMarket_CN_SH\x10\x1f\x12\x16\n\x12TrdSecMarket_CN_SZ\x10 \x12\x13\n\x0fTrdSecMarket_SG\x10)\x12\x13\n\x0fTrdSecMarket_JP\x10\x33*m\n\x07TrdSide\x12\x13\n\x0fTrdSide_Unknown\x10\x00\x12\x0f\n\x0bTrdSide_Buy\x10\x01\x12\x10\n\x0cTrdSide_Sell\x10\x02\x12\x15\n\x11TrdSide_SellShort\x10\x03\x12\x13\n\x0fTrdSide_BuyBack\x10\x04*\x81\x03\n\tOrderType\x12\x15\n\x11OrderType_Unknown\x10\x00\x12\x14\n\x10OrderType_Normal\x10\x01\x12\x14\n\x10OrderType_Market\x10\x02\x12\x1b\n\x17OrderType_AbsoluteLimit\x10\x05\x12\x15\n\x11OrderType_Auction\x10\x06\x12\x1a\n\x16OrderType_AuctionLimit\x10\x07\x12\x1a\n\x16OrderType_SpecialLimit\x10\x08\x12\x1e\n\x1aOrderType_SpecialLimit_All\x10\t\x12\x12\n\x0eOrderType_Stop\x10\n\x12\x17\n\x13OrderType_StopLimit\x10\x0b\x12\x1d\n\x19OrderType_MarketifTouched\x10\x0c\x12\x1c\n\x18OrderType_LimitifTouched\x10\r\x12\x1a\n\x16OrderType_TrailingStop\x10\x0e\x12\x1f\n\x1bOrderType_TrailingStopLimit\x10\x0f*M\n\tTrailType\x12\x15\n\x11TrailType_Unknown\x10\x00\x12\x13\n\x0fTrailType_Ratio\x10\x01\x12\x14\n\x10TrailType_Amount\x10\x02*\xfc\x03\n\x0bOrderStatus\x12\x1b\n\x17OrderStatus_Unsubmitted\x10\x00\x12 \n\x13OrderStatus_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x1d\n\x19OrderStatus_WaitingSubmit\x10\x01\x12\x1a\n\x16OrderStatus_Submitting\x10\x02\x12\x1c\n\x18OrderStatus_SubmitFailed\x10\x03\x12\x17\n\x13OrderStatus_TimeOut\x10\x04\x12\x19\n\x15OrderStatus_Submitted\x10\x05\x12\x1b\n\x17OrderStatus_Filled_Part\x10\n\x12\x1a\n\x16OrderStatus_Filled_All\x10\x0b\x12\x1f\n\x1bOrderStatus_Cancelling_Part\x10\x0c\x12\x1e\n\x1aOrderStatus_Cancelling_All\x10\r\x12\x1e\n\x1aOrderStatus_Cancelled_Part\x10\x0e\x12\x1d\n\x19OrderStatus_Cancelled_All\x10\x0f\x12\x16\n\x12OrderStatus_Failed\x10\x15\x12\x18\n\x14OrderStatus_Disabled\x10\x16\x12\x17\n\x13OrderStatus_Deleted\x10\x17\x12\x1d\n\x19OrderStatus_FillCancelled\x10\x18*e\n\x0fOrderFillStatus\x12\x16\n\x12OrderFillStatus_OK\x10\x00\x12\x1d\n\x19OrderFillStatus_Cancelled\x10\x01\x12\x1b\n\x17OrderFillStatus_Changed\x10\x02*`\n\x0cPositionSide\x12\x15\n\x11PositionSide_Long\x10\x00\x12!\n\x14PositionSide_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x16\n\x12PositionSide_Short\x10\x01*\xad\x01\n\rModifyOrderOp\x12\x19\n\x15ModifyOrderOp_Unknown\x10\x00\x12\x18\n\x14ModifyOrderOp_Normal\x10\x01\x12\x18\n\x14ModifyOrderOp_Cancel\x10\x02\x12\x19\n\x15ModifyOrderOp_Disable\x10\x03\x12\x18\n\x14ModifyOrderOp_Enable\x10\x04\x12\x18\n\x14ModifyOrderOp_Delete\x10\x05*P\n\nTrdAccType\x12\x16\n\x12TrdAccType_Unknown\x10\x00\x12\x13\n\x0fTrdAccType_Cash\x10\x01\x12\x15\n\x11TrdAccType_Margin\x10\x02*\x8c\x01\n\x08\x43urrency\x12\x14\n\x10\x43urrency_Unknown\x10\x00\x12\x10\n\x0c\x43urrency_HKD\x10\x01\x12\x10\n\x0c\x43urrency_USD\x10\x02\x12\x10\n\x0c\x43urrency_CNH\x10\x03\x12\x10\n\x0c\x43urrency_JPY\x10\x04\x12\x10\n\x0c\x43urrency_SGD\x10\x05\x12\x10\n\x0c\x43urrency_AUD\x10\x06*\xb6\x01\n\x0c\x43ltRiskLevel\x12!\n\x14\x43ltRiskLevel_Unknown\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\x12\x15\n\x11\x43ltRiskLevel_Safe\x10\x00\x12\x18\n\x14\x43ltRiskLevel_Warning\x10\x01\x12\x17\n\x13\x43ltRiskLevel_Danger\x10\x02\x12\x1d\n\x19\x43ltRiskLevel_AbsoluteSafe\x10\x03\x12\x1a\n\x16\x43ltRiskLevel_OptDanger\x10\x04*7\n\x0bTimeInForce\x12\x13\n\x0fTimeInForce_DAY\x10\x00\x12\x13\n\x0fTimeInForce_GTC\x10\x01*\x95\x01\n\x0cSecurityFirm\x12\x18\n\x14SecurityFirm_Unknown\x10\x00\x12\x1f\n\x1bSecurityFirm_FutuSecurities\x10\x01\x12\x18\n\x14SecurityFirm_FutuInc\x10\x02\x12\x17\n\x13SecurityFirm_FutuSG\x10\x03\x12\x17\n\x13SecurityFirm_FutuAU\x10\x04*Q\n\nSimAccType\x12\x16\n\x12SimAccType_Unknown\x10\x00\x12\x14\n\x10SimAccType_Stock\x10\x01\x12\x15\n\x11SimAccType_Option\x10\x02*\x94\x02\n\rCltRiskStatus\x12\x19\n\x15\x43ltRiskStatus_Unknown\x10\x00\x12\x18\n\x14\x43ltRiskStatus_Level1\x10\x01\x12\x18\n\x14\x43ltRiskStatus_Level2\x10\x02\x12\x18\n\x14\x43ltRiskStatus_Level3\x10\x03\x12\x18\n\x14\x43ltRiskStatus_Level4\x10\x04\x12\x18\n\x14\x43ltRiskStatus_Level5\x10\x05\x12\x18\n\x14\x43ltRiskStatus_Level6\x10\x06\x12\x18\n\x14\x43ltRiskStatus_Level7\x10\x07\x12\x18\n\x14\x43ltRiskStatus_Level8\x10\x08\x12\x18\n\x14\x43ltRiskStatus_Level9\x10\t*b\n\x08\x44TStatus\x12\x14\n\x10\x44TStatus_Unknown\x10\x00\x12\x16\n\x12\x44TStatus_Unlimited\x10\x01\x12\x13\n\x0f\x44TStatus_EMCall\x10\x02\x12\x13\n\x0f\x44TStatus_DTCall\x10\x03\x42@\n\x13\x63om.futu.openapi.pbZ)github.com/futuopen/ftapi4go/pb/trdcommon')
   ,
   dependencies=[Common__pb2.DESCRIPTOR,])
 
 _TRDENV = _descriptor.EnumDescriptor(
   name='TrdEnv',
   full_name='Trd_Common.TrdEnv',
   filename=None,
@@ -523,19 +523,23 @@
       name='Currency_JPY', index=4, number=4,
       options=None,
       type=None),
     _descriptor.EnumValueDescriptor(
       name='Currency_SGD', index=5, number=5,
       options=None,
       type=None),
+    _descriptor.EnumValueDescriptor(
+      name='Currency_AUD', index=6, number=6,
+      options=None,
+      type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4468,
-  serialized_end=4590,
+  serialized_start=4469,
+  serialized_end=4609,
 )
 _sym_db.RegisterEnumDescriptor(_CURRENCY)
 
 Currency = enum_type_wrapper.EnumTypeWrapper(_CURRENCY)
 _CLTRISKLEVEL = _descriptor.EnumDescriptor(
   name='CltRiskLevel',
   full_name='Trd_Common.CltRiskLevel',
@@ -565,16 +569,16 @@
     _descriptor.EnumValueDescriptor(
       name='CltRiskLevel_OptDanger', index=5, number=4,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4593,
-  serialized_end=4775,
+  serialized_start=4612,
+  serialized_end=4794,
 )
 _sym_db.RegisterEnumDescriptor(_CLTRISKLEVEL)
 
 CltRiskLevel = enum_type_wrapper.EnumTypeWrapper(_CLTRISKLEVEL)
 _TIMEINFORCE = _descriptor.EnumDescriptor(
   name='TimeInForce',
   full_name='Trd_Common.TimeInForce',
@@ -588,16 +592,16 @@
     _descriptor.EnumValueDescriptor(
       name='TimeInForce_GTC', index=1, number=1,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4777,
-  serialized_end=4832,
+  serialized_start=4796,
+  serialized_end=4851,
 )
 _sym_db.RegisterEnumDescriptor(_TIMEINFORCE)
 
 TimeInForce = enum_type_wrapper.EnumTypeWrapper(_TIMEINFORCE)
 _SECURITYFIRM = _descriptor.EnumDescriptor(
   name='SecurityFirm',
   full_name='Trd_Common.SecurityFirm',
@@ -616,19 +620,23 @@
       name='SecurityFirm_FutuInc', index=2, number=2,
       options=None,
       type=None),
     _descriptor.EnumValueDescriptor(
       name='SecurityFirm_FutuSG', index=3, number=3,
       options=None,
       type=None),
+    _descriptor.EnumValueDescriptor(
+      name='SecurityFirm_FutuAU', index=4, number=4,
+      options=None,
+      type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4834,
-  serialized_end=4958,
+  serialized_start=4854,
+  serialized_end=5003,
 )
 _sym_db.RegisterEnumDescriptor(_SECURITYFIRM)
 
 SecurityFirm = enum_type_wrapper.EnumTypeWrapper(_SECURITYFIRM)
 _SIMACCTYPE = _descriptor.EnumDescriptor(
   name='SimAccType',
   full_name='Trd_Common.SimAccType',
@@ -646,16 +654,16 @@
     _descriptor.EnumValueDescriptor(
       name='SimAccType_Option', index=2, number=2,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=4960,
-  serialized_end=5041,
+  serialized_start=5005,
+  serialized_end=5086,
 )
 _sym_db.RegisterEnumDescriptor(_SIMACCTYPE)
 
 SimAccType = enum_type_wrapper.EnumTypeWrapper(_SIMACCTYPE)
 _CLTRISKSTATUS = _descriptor.EnumDescriptor(
   name='CltRiskStatus',
   full_name='Trd_Common.CltRiskStatus',
@@ -701,16 +709,16 @@
     _descriptor.EnumValueDescriptor(
       name='CltRiskStatus_Level9', index=9, number=9,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5044,
-  serialized_end=5320,
+  serialized_start=5089,
+  serialized_end=5365,
 )
 _sym_db.RegisterEnumDescriptor(_CLTRISKSTATUS)
 
 CltRiskStatus = enum_type_wrapper.EnumTypeWrapper(_CLTRISKSTATUS)
 _DTSTATUS = _descriptor.EnumDescriptor(
   name='DTStatus',
   full_name='Trd_Common.DTStatus',
@@ -732,16 +740,16 @@
     _descriptor.EnumValueDescriptor(
       name='DTStatus_DTCall', index=3, number=3,
       options=None,
       type=None),
   ],
   containing_type=None,
   options=None,
-  serialized_start=5322,
-  serialized_end=5420,
+  serialized_start=5367,
+  serialized_end=5465,
 )
 _sym_db.RegisterEnumDescriptor(_DTSTATUS)
 
 DTStatus = enum_type_wrapper.EnumTypeWrapper(_DTSTATUS)
 TrdEnv_Simulate = 0
 TrdEnv_Real = 1
 TrdCategory_Unknown = 0
@@ -817,26 +825,28 @@
 TrdAccType_Margin = 2
 Currency_Unknown = 0
 Currency_HKD = 1
 Currency_USD = 2
 Currency_CNH = 3
 Currency_JPY = 4
 Currency_SGD = 5
+Currency_AUD = 6
 CltRiskLevel_Unknown = -1
 CltRiskLevel_Safe = 0
 CltRiskLevel_Warning = 1
 CltRiskLevel_Danger = 2
 CltRiskLevel_AbsoluteSafe = 3
 CltRiskLevel_OptDanger = 4
 TimeInForce_DAY = 0
 TimeInForce_GTC = 1
 SecurityFirm_Unknown = 0
 SecurityFirm_FutuSecurities = 1
 SecurityFirm_FutuInc = 2
 SecurityFirm_FutuSG = 3
+SecurityFirm_FutuAU = 4
 SimAccType_Unknown = 0
 SimAccType_Stock = 1
 SimAccType_Option = 2
 CltRiskStatus_Unknown = 0
 CltRiskStatus_Level1 = 1
 CltRiskStatus_Level2 = 2
 CltRiskStatus_Level3 = 3
```

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetAccList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetAccList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetFunds_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetFunds_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetHistoryOrderFillList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetHistoryOrderList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetHistoryOrderList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetMarginRatio_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetMarginRatio_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetMaxTrdQtys_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetOrderFillList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetOrderFillList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetOrderList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetOrderList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_GetPositionList_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_GetPositionList_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_ModifyOrder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_ModifyOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_Notify_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_Notify_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_PlaceOrder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_PlaceOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_ReconfirmOrder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_ReconfirmOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_SubAccPush_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_SubAccPush_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_UnlockTrade_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_UnlockTrade_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_UpdateOrderFill_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_UpdateOrderFill_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Trd_UpdateOrder_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Trd_UpdateOrder_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pb/Verification_pb2.py` & `futu-api-7.2.3408/futu/common/pb/Verification_pb2.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/pbjson.py` & `futu-api-7.2.3408/futu/common/pbjson.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/sys_config.py` & `futu-api-7.2.3408/futu/common/sys_config.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/common/utils.py` & `futu-api-7.2.3408/futu/common/utils.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/get_mkt_snapshot_demo.py` & `futu-api-7.2.3408/futu/examples/get_mkt_snapshot_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/macd_strategy.py` & `futu-api-7.2.3408/futu/examples/macd_strategy.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/quote_and_trade_demo.py` & `futu-api-7.2.3408/futu/examples/quote_and_trade_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/quote_push.py` & `futu-api-7.2.3408/futu/examples/quote_push.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/simple_filter_demo.py` & `futu-api-7.2.3408/futu/examples/simple_filter_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/examples/stocksell_demo.py` & `futu-api-7.2.3408/futu/examples/stocksell_demo.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/quote/open_quote_context.py` & `futu-api-7.2.3408/futu/quote/open_quote_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
                     max_kl_num = min(max_count - len(list_ret), 1000)
                 else:
                     data_finish = True
             else:
                 data_finish = not has_next
 
         # 表头列
-        col_list = ['code']
+        col_list = ['code', 'name']
         for field in req_fields:
             str_field = KL_FIELD.DICT_KL_FIELD_STR[field]
             if str_field not in col_list:
                 col_list.append(str_field)
 
         kline_frame_table = pd.DataFrame(list_ret, columns=col_list)
 
@@ -658,14 +658,15 @@
                           'trust_netAssetValue',
                           'trust_premium',
                           'trust_assetClass',
                         ]
 
         col_list = [
             'code',
+            'name',
             'update_time',
             'last_price',
             'open_price',
             'high_price',
             'low_price',
             'prev_close_price',
             'volume',
@@ -765,15 +766,15 @@
         if ret_code == RET_ERROR:
             return ret_code, msg
 
         for x in rt_data_list:
             x['code'] = code
 
         col_list = [
-            'code', 'time', 'is_blank', 'opened_mins', 'cur_price',
+            'code', 'name', 'time', 'is_blank', 'opened_mins', 'cur_price',
             'last_close', 'avg_price', 'volume', 'turnover'
         ]
 
         rt_data_table = pd.DataFrame(rt_data_list, columns=col_list)
 
         return RET_OK, rt_data_table
 
@@ -937,18 +938,18 @@
 
         ret_code, ret_msg, content = query_processor(**kargs)
         if ret_code != RET_OK:
             return ret_code, ret_msg, ret_msg
 
         (_, bid_list, ask_list) = content
         col_bid_list = [
-            'code', 'bid_broker_id', 'bid_broker_name', 'bid_broker_pos', 'order_id', 'order_volume'
+            'code', 'name', 'bid_broker_id', 'bid_broker_name', 'bid_broker_pos', 'order_id', 'order_volume'
         ]
         col_ask_list = [
-            'code', 'ask_broker_id', 'ask_broker_name', 'ask_broker_pos', 'order_id', 'order_volume'
+            'code', 'name', 'ask_broker_id', 'ask_broker_name', 'ask_broker_pos', 'order_id', 'order_volume'
         ]
 
         bid_frame_table = pd.DataFrame(bid_list, columns=col_bid_list)
         ask_frame_table = pd.DataFrame(ask_list, columns=col_ask_list)
         return RET_OK, bid_frame_table, ask_frame_table
 
     def _check_subscribe_param(self, code_list, subtype_list):
@@ -1287,15 +1288,15 @@
         }
 
         ret_code, msg, quote_list = query_processor(**kargs)
         if ret_code == RET_ERROR:
             return ret_code, msg
 
         col_list = [
-            'code', 'data_date', 'data_time', 'last_price', 'open_price',
+            'code', 'name', 'data_date', 'data_time', 'last_price', 'open_price',
             'high_price', 'low_price', 'prev_close_price', 'volume',
             'turnover', 'turnover_rate', 'amplitude', 'suspension',
             'listing_date', 'price_spread', 'dark_status', 'sec_status', 'strike_price',
             'contract_size', 'open_interest', 'implied_volatility',
             'premium', 'delta', 'gamma', 'vega', 'theta', 'rho',
             'net_open_interest', 'expiry_date_distance', 'contract_nominal_value',
             'owner_lot_multiplier', 'option_area_type', 'contract_multiplier',
@@ -1353,15 +1354,15 @@
             "conn_id": self.get_sync_conn_id()
         }
         ret_code, msg, ticker_list = query_processor(**kargs)
         if ret_code == RET_ERROR:
             return ret_code, msg
 
         col_list = [
-            'code', 'time', 'price', 'volume', 'turnover', "ticker_direction",
+            'code', 'name', 'time', 'price', 'volume', 'turnover', "ticker_direction",
             'sequence', 'type'
         ]
         ticker_frame_table = pd.DataFrame(ticker_list, columns=col_list)
 
         return RET_OK, ticker_frame_table
 
     def get_cur_kline(self, code, num, ktype=SubType.K_DAY, autype=AuType.QFQ):
@@ -1421,15 +1422,15 @@
             "conn_id": self.get_sync_conn_id()
         }
         ret_code, msg, kline_list = query_processor(**kargs)
         if ret_code == RET_ERROR:
             return ret_code, msg
 
         col_list = [
-            'code', 'time_key', 'open', 'close', 'high', 'low', 'volume',
+            'code', 'name', 'time_key', 'open', 'close', 'high', 'low', 'volume',
             'turnover', 'pe_ratio', 'turnover_rate', 'last_close'
         ]
         kline_frame_table = pd.DataFrame(kline_list, columns=col_list)
 
         return RET_OK, kline_frame_table
 
     def get_order_book(self, code, num = 10):
@@ -1574,15 +1575,15 @@
         }
 
         ret_code, msg, owner_plate_list = query_processor(**kargs)
         if ret_code == RET_ERROR:
             return ret_code, msg
 
         col_list = [
-            'code', 'plate_code', 'plate_name', 'plate_type'
+            'code', 'name', 'plate_code', 'plate_name', 'plate_type'
         ]
 
         owner_plate_table = pd.DataFrame(owner_plate_list, columns=col_list)
 
         return RET_OK, owner_plate_table
 
     def get_holding_change_list(self, code, holder_type, start=None, end=None):
@@ -2472,14 +2473,15 @@
         }
         ret_code, msg, ret = query_processor(**kargs)
         if ret_code == RET_ERROR:
             return ret_code, msg
         if isinstance(ret, list):
             col_list = [
                 'code',
+                'name',
                 'key',
                 'reminder_type',
                 'reminder_freq',
                 'value',
                 'enable',
                 'note',
             ]
```

### Comparing `futu-api-7.1.3308/futu/quote/quote_get_warrant.py` & `futu-api-7.2.3408/futu/quote/quote_get_warrant.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/quote/quote_query.py` & `futu-api-7.2.3408/futu/quote/quote_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,14 +406,15 @@
         raw_snapshot_list = rsp_pb.s2c.snapshotList
 
         snapshot_list = []
         for record in raw_snapshot_list:
             snapshot_tmp = {}
             snapshot_tmp['code'] = merge_qot_mkt_stock_str(
                 int(record.basic.security.market), record.basic.security.code)
+            snapshot_tmp['name'] = record.basic.name if record.basic.HasField('name') else 'N/A'
             snapshot_tmp['update_time'] = record.basic.updateTime
             snapshot_tmp['last_price'] = record.basic.curPrice
             snapshot_tmp['open_price'] = record.basic.openPrice
             snapshot_tmp['high_price'] = record.basic.highPrice
             snapshot_tmp['low_price'] = record.basic.lowPrice
             snapshot_tmp['prev_close_price'] = record.basic.lastClosePrice
             snapshot_tmp['volume'] = record.basic.volume
@@ -656,14 +657,15 @@
         if ret_type != RET_OK:
             return RET_ERROR, ret_msg, None
 
         raw_rt_data_list = rsp_pb.s2c.rtList
         rt_list = [
             {
                 "code": merge_qot_mkt_stock_str(rsp_pb.s2c.security.market, rsp_pb.s2c.security.code),
+                "name": rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else 'N/A',
                 "time": record.time,
                 "is_blank":  True if record.isBlank else False,
                 "opened_mins": record.minute,
                 "cur_price": record.price,
                 "last_close": record.lastClosePrice,
                 # 期权没有计算这个均价，应该是N/A
                 # 期权是正股的衍生品，其价格完全依赖正股的波动，而不是期权自身的博弈。
@@ -801,26 +803,28 @@
         bid_list = []
         if raw_broker_bid is not None:
             bid_list = [{
                 "bid_broker_id": record.id,
                 "bid_broker_name": record.name,
                 "bid_broker_pos": record.pos,
                 "code": merge_qot_mkt_stock_str(rsp_pb.s2c.security.market, rsp_pb.s2c.security.code),
+                "name": rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else 'N/A',
                 "order_id": record.orderID if record.HasField('orderID') else 'N/A',
                 "order_volume": record.volume if record.HasField('volume') else 'N/A'
             } for record in raw_broker_bid]
 
         raw_broker_ask = rsp_pb.s2c.brokerAskList
         ask_list = []
         if raw_broker_ask is not None:
             ask_list = [{
                 "ask_broker_id": record.id,
                 "ask_broker_name": record.name,
                 "ask_broker_pos": record.pos,
                 "code": merge_qot_mkt_stock_str(rsp_pb.s2c.security.market, rsp_pb.s2c.security.code),
+                "name": rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else 'N/A',
                 "order_id": record.orderID if record.HasField('orderID') else 'N/A',
                 "order_volume": record.volume if record.HasField('volume') else 'N/A'
             } for record in raw_broker_ask]
 
         return RET_OK, "", (stock_code, bid_list, ask_list)
 
 
@@ -879,20 +883,22 @@
         next_req_key = None
         if rsp_pb.s2c.HasField('nextReqKey'):
             has_next = True
             next_req_key = bytes(rsp_pb.s2c.nextReqKey)
 
         stock_code = merge_qot_mkt_stock_str(rsp_pb.s2c.security.market,
                                              rsp_pb.s2c.security.code)
+        stock_name = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else "N/A"
 
         list_ret = []
         dict_data = {}
         raw_kline_list = rsp_pb.s2c.klList
         for record in raw_kline_list:
             dict_data['code'] = stock_code
+            dict_data['name'] = stock_name
             dict_data['time_key'] = record.time
             if record.isBlank:
                 continue
             if record.HasField('openPrice'):
                 dict_data['open'] = record.openPrice
             if record.HasField('highPrice'):
                 dict_data['high'] = record.highPrice
@@ -1087,14 +1093,15 @@
 
         return SubscriptionQuery.pack_push_or_unpush_req(code_list, subtype_list, False, conn_id, is_first_push)
 
 
 def parse_pb_BasicQot(pb):
     item = {
         'code': merge_qot_mkt_stock_str(int(pb.security.market), pb.security.code),
+        'name': "N/A" if not pb.HasField('name') else pb.name,
         'data_date':pb.updateTime.split()[0] if len(pb.updateTime) > 0 else '',
         'data_time': pb.updateTime.split()[1] if len(pb.updateTime) > 0 else '',
         'last_price': pb.curPrice,
         'open_price': pb.openPrice,
         'high_price': pb.highPrice,
         'low_price': pb.lowPrice,
         'prev_close_price': pb.lastClosePrice,
@@ -1219,17 +1226,19 @@
     def unpack_rsp(cls, rsp_pb):
 
         if rsp_pb.retType != RET_OK:
             return RET_ERROR, rsp_pb.retMsg, None
 
         stock_code = merge_qot_mkt_stock_str(rsp_pb.s2c.security.market,
                                              rsp_pb.s2c.security.code)
+        stock_name = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else "N/A"
         raw_ticker_list = rsp_pb.s2c.tickerList
         ticker_list = [{
             "code": stock_code,
+            "name": stock_name,
             "time": record.time,
             "price": record.price,
             "volume": record.volume,
             "turnover": record.turnover,
             "ticker_direction": TickerDirect.to_string2(record.dir) if record.HasField('dir') else 'N/A',# 初始化枚举类型
             "sequence": record.sequence,
             "recv_timestamp":record.recvTime,
@@ -1287,17 +1296,19 @@
     def unpack_rsp(cls, rsp_pb):
 
         if rsp_pb.retType != RET_OK:
             return RET_ERROR, rsp_pb.retMsg, []
 
         stock_code = merge_qot_mkt_stock_str(rsp_pb.s2c.security.market,
                                              rsp_pb.s2c.security.code)
+        stock_name = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else "N/A"
         raw_kline_list = rsp_pb.s2c.klList
         kline_list = [{
             "code": stock_code,
+            "name": stock_name,
             "time_key": record.time,
             "open": record.openPrice,
             "high": record.highPrice,
             "low": record.lowPrice,
             "close": record.closePrice,
             "volume": record.volume,
             "turnover": record.turnover,
@@ -1323,18 +1334,20 @@
 
         r, kl_type = KLType.to_string(rsp_pb.s2c.klType);
         if not r:
             return RET_ERROR, "kline push error kltype", None
 
         stock_code = merge_qot_mkt_stock_str(rsp_pb.s2c.security.market,
                                              rsp_pb.s2c.security.code)
+        stock_name = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else "N/A"
         raw_kline_list = rsp_pb.s2c.klList
         kline_list = [{
             "k_type": kl_type,
             "code": stock_code,
+            "name": stock_name,
             "time_key": record.time,
             "open": record.openPrice,
             "high": record.highPrice,
             "low": record.lowPrice,
             "close": record.closePrice,
             "volume": record.volume,
             "turnover": record.turnover,
@@ -1379,14 +1392,15 @@
 
         raw_order_book_ask = rsp_pb.s2c.orderBookAskList
         raw_order_book_bid = rsp_pb.s2c.orderBookBidList
 
         order_book = {}
         order_book['code'] = merge_qot_mkt_stock_str(
             rsp_pb.s2c.security.market, rsp_pb.s2c.security.code)
+        order_book['name'] = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else 'N/A'
         order_book['svr_recv_time_bid'] = rsp_pb.s2c.svrRecvTimeBid
         order_book['svr_recv_time_ask'] = rsp_pb.s2c.svrRecvTimeAsk
         order_book['Bid'] = []
         order_book['Ask'] = []
 
         for record in raw_order_book_bid:
             detail = {}
@@ -1584,18 +1598,14 @@
                     'us_future_qot_right_comex': QotRight.to_string2(qot_right.usCOMEXFutureQotRight) if qot_right.HasField('usCOMEXFutureQotRight') else 'N/A',
                     'us_future_qot_right_cboe': QotRight.to_string2(qot_right.usCBOEFutureQotRight) if qot_right.HasField('usCBOEFutureQotRight') else 'N/A',
                 }
         elif notify_type == SysNotifyType.API_LEVEL:
             if rsp_pb.s2c.HasField('apiLevel'):
                 data = {'api_level': rsp_pb.s2c.apiLevel.apiLevel}
 
-        if data is None:
-            logger.warning(
-                "SysNotifyPush data is None: notify_type={}".format(notify_type))
-
         return RET_OK, (notify_type, sub_type, data)
 
 
 
 class StockReferenceList:
     def __init__(self):
         pass
@@ -1696,14 +1706,15 @@
 
         data_list = []
         for record in raw_quote_list:
             plate_info_list = record.plateInfoList
             for plate_info in plate_info_list:
                 quote_list = {
                     'code': merge_qot_mkt_stock_str(record.security.market, record.security.code),
+                    'name': record.name if record.HasField('name') else 'N/A',
                     'plate_code': merge_qot_mkt_stock_str(plate_info.plate.market, plate_info.plate.code),
                     'plate_name': str(plate_info.name),
                     'plate_type': Plate.to_string2(plate_info.plateType) if plate_info.HasField('plateType') else 'N/A' # 初始化枚举类型
                 }
                 data_list.append(quote_list)
 
         return RET_OK, "", data_list
@@ -1988,16 +1999,17 @@
         remain_quota = rsp_pb.s2c.remainQuota
         detail_list = []
 
         details = rsp_pb.s2c.detailList
         for item in details:
             code = merge_qot_mkt_stock_str(
                 int(item.security.market), item.security.code)
+            name = item.name if item.HasField('name') else "N/A"
             request_time = str(item.requestTime)
-            detail_list.append({"code": code, "request_time": request_time})
+            detail_list.append({"code": code, "name": name, "request_time": request_time})
 
         data = {
             "used_quota": used_quota,
             "remain_quota": remain_quota,
             "detail_list": detail_list
         }
         return RET_OK, "", data
@@ -2867,14 +2879,15 @@
         if ret_type != RET_OK:
             return RET_ERROR, ret_msg, None
 
         res = {}
         if rsp_pb.HasField('s2c'):
             res['code'] = merge_qot_mkt_stock_str(rsp_pb.s2c.security.market,
                                                   rsp_pb.s2c.security.code)
+            res['name'] = rsp_pb.s2c.name if rsp_pb.s2c.HasField('name') else 'N/A'
             res['price'] = rsp_pb.s2c.price
             res['change_rate'] = rsp_pb.s2c.changeRate
             res['market_status'] = PriceReminderMarketStatus.to_string2(rsp_pb.s2c.marketStatus) if rsp_pb.s2c.HasField('marketStatus') else 'N/A' # 初始化枚举类型
             res['content'] = rsp_pb.s2c.content
             res['note'] = rsp_pb.s2c.note
             if rsp_pb.s2c.key is not None:
                 res['key'] = rsp_pb.s2c.key
@@ -2970,18 +2983,20 @@
         if rsp_pb.retType != RET_OK:
             return RET_ERROR, rsp_pb.retMsg, None
 
         ret_list = list()
         #  到价提醒 type = Qot_GetPriceReminder.PriceReminder
         for item in rsp_pb.s2c.priceReminderList:
             stock_code = merge_qot_mkt_stock_str(item.security.market, item.security.code)
+            stock_name = item.name if item.HasField('name') else 'N/A'
             #  提醒信息列表 type = Qot_GetPriceReminder.PriceReminderItem
             for sub_item in item.itemList:
                 data = {}
                 data["code"] = stock_code
+                data["name"] = stock_name
                 #  每个提醒的唯一标识 type = int64
                 data["key"] = sub_item.key
                 #  Qot_Common::PriceReminderType 提醒类型 type = int32
                 data["reminder_type"] = PriceReminderType.to_string2(sub_item.type) if sub_item.HasField('type') else 'N/A' # 初始化枚举类型
                 #  Qot_Common::PriceReminderFreq 提醒频率类型 type = int32
                 data["reminder_freq"] = PriceReminderFreq.to_string2(sub_item.freq) if sub_item.HasField('freq') else 'N/A' # 初始化枚举类型
                 #  提醒参数值 type = double
```

### Comparing `futu-api-7.1.3308/futu/quote/quote_response_handler.py` & `futu-api-7.2.3408/futu/quote/quote_response_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         :return: 参见get_stock_quote的返回值
         """
         ret_code, content = self.parse_rsp_pb(rsp_pb)
         if ret_code != RET_OK:
             return ret_code, content
         else:
             col_list = [
-                'code', 'data_date', 'data_time', 'last_price', 'open_price',
+                'code', 'name', 'data_date', 'data_time', 'last_price', 'open_price',
                 'high_price', 'low_price', 'prev_close_price', 'volume',
                 'turnover', 'turnover_rate', 'amplitude', 'suspension',
                 'listing_date', 'price_spread', 'dark_status', 'sec_status', 'strike_price',
                 'contract_size', 'open_interest', 'implied_volatility',
                 'premium', 'delta', 'gamma', 'vega', 'theta', 'rho',
                 'net_open_interest', 'expiry_date_distance', 'contract_nominal_value', 
                 'owner_lot_multiplier', 'option_area_type', 'contract_multiplier',
@@ -138,15 +138,15 @@
         :return: 参见get_cur_kline的返回值
         """
         ret_code, content = self.parse_rsp_pb(rsp_pb)
         if ret_code != RET_OK:
             return ret_code, content
         else:
             col_list = [
-                'code', 'time_key', 'open', 'close', 'high', 'low', 'volume',
+                'code', 'name', 'time_key', 'open', 'close', 'high', 'low', 'volume',
                 'turnover', 'k_type', 'last_close'
             ]
             kline_frame_table = pd.DataFrame(content, columns=col_list)
 
             return RET_OK, kline_frame_table
 
 
@@ -186,16 +186,16 @@
         """
         ret_code, content = self.parse_rsp_pb(rsp_pb)
         if ret_code != RET_OK:
             return ret_code, content
         else:
             self.on_recv_log(content)
             col_list = [
-                'code', 'time', 'price', 'volume', 'turnover',
-                "ticker_direction", 'sequence', 'type', 'push_data_type',
+                'code', 'name', 'time', 'price', 'volume', 'turnover',
+                "ticker_direction", 'sequence', 'type', 'push_data_type'
             ]
             ticker_frame_table = pd.DataFrame(content, columns=col_list)
 
             return RET_OK, ticker_frame_table
 
 
 class RTDataHandlerBase(RspHandlerBase):
@@ -234,15 +234,15 @@
         """
         ret_code, content = self.parse_rsp_pb(rsp_pb)
         if ret_code != RET_OK:
             return ret_code, content
         else:
 
             col_list = [
-                'code', 'time', 'is_blank', 'opened_mins', 'cur_price',
+                'code', 'name', 'time', 'is_blank', 'opened_mins', 'cur_price',
                 "last_close", 'avg_price', 'turnover', 'volume'
             ]
             rt_data_table = pd.DataFrame(content, columns=col_list)
 
             return RET_OK, rt_data_table
 
 
@@ -286,18 +286,18 @@
         ret_code, content = self.parse_rsp_pb(rsp_pb)
         if ret_code != RET_OK:
             return ret_code, content, None
         else:
             self.on_recv_log(content)
             stock_code, bid_content, ask_content = content
             bid_list = [
-                'code', 'bid_broker_id', 'bid_broker_name', 'bid_broker_pos', 'order_id', 'order_volume'
+                'code', 'name', 'bid_broker_id', 'bid_broker_name', 'bid_broker_pos', 'order_id', 'order_volume'
             ]
             ask_list = [
-                'code', 'ask_broker_id', 'ask_broker_name', 'ask_broker_pos', 'order_id', 'order_volume'
+                'code', 'name', 'ask_broker_id', 'ask_broker_name', 'ask_broker_pos', 'order_id', 'order_volume'
             ]
             bid_frame_table = pd.DataFrame(bid_content, columns=bid_list)
             ask_frame_table = pd.DataFrame(ask_content, columns=ask_list)
             return ret_code, stock_code, [bid_frame_table, ask_frame_table]
 
 
 class KeepAliveHandlerBase(RspHandlerBase):
```

### Comparing `futu-api-7.1.3308/futu/quote/quote_stockfilter_info.py` & `futu-api-7.2.3408/futu/quote/quote_stockfilter_info.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/quote/quote_tool.py` & `futu-api-7.2.3408/futu/quote/quote_tool.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/tools/Common.proto.json` & `futu-api-7.2.3408/futu/tools/Common.proto.json`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/tools/generate_code.py` & `futu-api-7.2.3408/futu/tools/generate_code.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/tools/load_template.py` & `futu-api-7.2.3408/futu/tools/load_template.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu/trade/open_trade_context.py` & `futu-api-7.2.3408/futu/trade/open_trade_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 
         col_list = [
             'power', 'max_power_short', 'net_cash_power', 'total_assets', 'cash', 'market_val', 'long_mv', 'short_mv',
             'pending_asset', 'interest_charged_amount', 'frozen_cash', 'avl_withdrawal_cash', 'max_withdrawal', 'currency',
             'available_funds', 'unrealized_pl', 'realized_pl', 'risk_level', 'risk_status', 'initial_margin',
             'margin_call_margin', 'maintenance_margin', 'hk_cash', 'hk_avl_withdrawal_cash', 'us_cash',
             'us_avl_withdrawal_cash', 'cn_cash', 'cn_avl_withdrawal_cash', 'jp_cash', 'jp_avl_withdrawal_cash',
-            'sg_cash', 'sg_avl_withdrawal_cash', 'is_pdt', 'pdt_seq', 'beginning_dtbp', 'remaining_dtbp',
+            'sg_cash', 'sg_avl_withdrawal_cash', 'au_cash', 'au_avl_withdrawal_cash', 'is_pdt', 'pdt_seq', 'beginning_dtbp', 'remaining_dtbp',
             'dt_call_amount', 'dt_status'
         ]
         accinfo_frame_table = pd.DataFrame(accinfo_list, columns=col_list)
 
         return RET_OK, accinfo_frame_table
 
     def _get_trd_market_from_market(self, qot_market, trd_env, trd_category):
```

### Comparing `futu-api-7.1.3308/futu/trade/trade_query.py` & `futu-api-7.2.3408/futu/trade/trade_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,16 @@
             'us_avl_withdrawal_cash': NoneDataValue,
             'cn_cash': NoneDataValue,
             'cn_avl_withdrawal_cash': NoneDataValue,
             'jp_cash': NoneDataValue,
             'jp_avl_withdrawal_cash': NoneDataValue,
             'sg_cash': NoneDataValue,
             'sg_avl_withdrawal_cash': NoneDataValue,
+            'au_cash': NoneDataValue,
+            'au_avl_withdrawal_cash': NoneDataValue,
             'is_pdt':  get_pb_value(raw_funds, 'isPdt'),
             'pdt_seq': get_pb_value(raw_funds, 'pdtSeq'),
             'beginning_dtbp': get_pb_value(raw_funds, 'beginningDTBP'),
             'remaining_dtbp': get_pb_value(raw_funds, 'remainingDTBP'),
             'dt_call_amount': get_pb_value(raw_funds, 'dtCallAmount'),
             'dt_status': get_pb_enum(raw_funds, 'dtStatus', DTStatus, DTStatus.NONE)
         }]
@@ -186,14 +188,17 @@
                 accinfo_list[0]['cn_avl_withdrawal_cash'] = cashInfo.availableBalance
             elif cashInfo.currency == Trd_Common_pb2.Currency_JPY:
                 accinfo_list[0]['jp_cash'] = cashInfo.cash
                 accinfo_list[0]['jp_avl_withdrawal_cash'] = cashInfo.availableBalance
             elif cashInfo.currency == Trd_Common_pb2.Currency_SGD:
                 accinfo_list[0]['sg_cash'] = cashInfo.cash
                 accinfo_list[0]['sg_avl_withdrawal_cash'] = cashInfo.availableBalance
+            elif cashInfo.currency == Trd_Common_pb2.Currency_AUD:
+                accinfo_list[0]['au_cash'] = cashInfo.cash
+                accinfo_list[0]['au_avl_withdrawal_cash'] = cashInfo.availableBalance
         return RET_OK, "", accinfo_list
 
 
 class PositionListQuery:
     """Class for querying position list"""
 
     def __init__(self):
@@ -239,15 +244,15 @@
                              "pl_ratio": 100 * position.plRatio if position.HasField('plRatio') else NoneDataValue,
                              "pl_ratio_valid": position.HasField('plRatio'),
                              "pl_val": position.plVal,
                              "pl_val_valid": position.HasField('plVal'),
                              "today_buy_qty": position.td_buyQty if position.HasField('td_buyQty') else NoneDataValue,
                              "today_buy_val": position.td_buyVal if position.HasField('td_buyVal') else NoneDataValue,
                              "today_pl_val": position.td_plVal if position.HasField('td_plVal') else NoneDataValue,
-                             "today_trd_val": position.td_plVal if position.HasField('td_trdVal') else NoneDataValue,
+                             "today_trd_val": position.td_trdVal if position.HasField('td_trdVal') else NoneDataValue,
                              "today_sell_qty": position.td_sellQty if position.HasField('td_sellQty') else NoneDataValue,
                              "today_sell_val": position.td_sellVal if position.HasField('td_sellVal') else NoneDataValue,
                              "position_side": PositionSide.to_string2(position.positionSide) if position.HasField('positionSide') else 'N/A',# 初始化枚举类型
                              "unrealized_pl": position.unrealizedPL if position.HasField('unrealizedPL') else NoneDataValue,
                              "realized_pl": position.realizedPL if position.HasField('realizedPL') else NoneDataValue,
                              "currency": Currency.to_string2(position.currency) if position.HasField('currency') else NoneDataValue,
                          } for position in raw_position_list]
```

### Comparing `futu-api-7.1.3308/futu/trade/trade_response_handler.py` & `futu-api-7.2.3408/futu/trade/trade_response_handler.py`

 * *Files identical despite different names*

### Comparing `futu-api-7.1.3308/futu_api.egg-info/PKG-INFO` & `futu-api-7.2.3408/futu_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: futu-api
-Version: 7.1.3308
+Version: 7.2.3408
 Summary: Futu Quantitative Trading API
 Home-page: https://github.com/FutunnOpen/py-futu-api
 Author: Futu, Inc.
 Author-email: ftdev@futunn.com
 License: Apache License 2.0
 Keywords: Futu HK/US Stock Quant Trading API
 Platform: UNKNOWN
```

### Comparing `futu-api-7.1.3308/futu_api.egg-info/SOURCES.txt` & `futu-api-7.2.3408/futu_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 futu/common/pb/Trd_Notify_pb2.py
 futu/common/pb/Trd_PlaceOrder_pb2.py
 futu/common/pb/Trd_ReconfirmOrder_pb2.py
 futu/common/pb/Trd_SubAccPush_pb2.py
 futu/common/pb/Trd_UnlockTrade_pb2.py
 futu/common/pb/Trd_UpdateOrderFill_pb2.py
 futu/common/pb/Trd_UpdateOrder_pb2.py
+futu/common/pb/UsedQuota_pb2.py
 futu/common/pb/Verification_pb2.py
 futu/common/pb/__init__.py
 futu/common/pb/build.bat
 futu/common/pb/generate_python.bat
 futu/examples/__init__.py
 futu/examples/get_mkt_snapshot_demo.py
 futu/examples/macd_strategy.py
```

### Comparing `futu-api-7.1.3308/setup.py` & `futu-api-7.2.3408/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     version = f.read().decode('ascii').strip()
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_desc = fh.read()
 
 install_requires = ["pandas",
                     "simplejson",
-                    "protobuf>=3.5.1,==3.*",
+                    "protobuf>=3.8.0,==3.*",
                     "PyCryptodome",
                     ]
 
 if is_py2:
     install_requires.append("selectors2")
 
 setup(
```

