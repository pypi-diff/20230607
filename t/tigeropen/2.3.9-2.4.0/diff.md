# Comparing `tmp/tigeropen-2.3.9.tar.gz` & `tmp/tigeropen-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.3.9.tar", last modified: Thu Jun  1 07:01:44 2023, max compression
+gzip compressed data, was "tigeropen-2.4.0.tar", last modified: Wed Jun  7 11:40:27 2023, max compression
```

## Comparing `tigeropen-2.3.9.tar` & `tigeropen-2.4.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.388480 tigeropen-2.3.9/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.9/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-01 07:01:44.388336 tigeropen-2.3.9/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.9/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.9/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-01 07:01:44.388530 tigeropen-2.3.9/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.9/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.339447 tigeropen-2.3.9/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.341277 tigeropen-2.3.9/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.343178 tigeropen-2.3.9/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.9/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.9/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.9/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.345017 tigeropen-2.3.9/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.3.9/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.9/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.9/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.9/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346112 tigeropen-2.3.9/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346444 tigeropen-2.3.9/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346608 tigeropen-2.3.9/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346765 tigeropen-2.3.9/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.347072 tigeropen-2.3.9/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.348243 tigeropen-2.3.9/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.348906 tigeropen-2.3.9/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.350367 tigeropen-2.3.9/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-2.3.9/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.357590 tigeropen-2.3.9/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.9/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.358068 tigeropen-2.3.9/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.360364 tigeropen-2.3.9/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    76884 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.360653 tigeropen-2.3.9/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.370380 tigeropen-2.3.9/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.9/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.9/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.9/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.9/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.9/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-06-01 02:40:59.000000 tigeropen-2.3.9/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-2.3.9/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.370871 tigeropen-2.3.9/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.380371 tigeropen-2.3.9/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     4529 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.380855 tigeropen-2.3.9/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.387954 tigeropen-2.3.9/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.340288 tigeropen-2.3.9/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.870142 tigeropen-2.4.0/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.4.0/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-07 11:40:27.869956 tigeropen-2.4.0/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.4.0/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.4.0/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-07 11:40:27.870186 tigeropen-2.4.0/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.4.0/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.837015 tigeropen-2.4.0/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.839369 tigeropen-2.4.0/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.842044 tigeropen-2.4.0/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4706 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.4.0/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.844159 tigeropen-2.4.0/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.4.0/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.4.0/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.4.0/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.845626 tigeropen-2.4.0/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.845926 tigeropen-2.4.0/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846105 tigeropen-2.4.0/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846287 tigeropen-2.4.0/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846666 tigeropen-2.4.0/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.848520 tigeropen-2.4.0/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.849638 tigeropen-2.4.0/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.851287 tigeropen-2.4.0/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-2.4.0/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.858275 tigeropen-2.4.0/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.4.0/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.858605 tigeropen-2.4.0/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.860314 tigeropen-2.4.0/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    77148 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.860585 tigeropen-2.4.0/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.865913 tigeropen-2.4.0/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.4.0/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.4.0/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.4.0/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.4.0/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.4.0/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-2.4.0/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.866190 tigeropen-2.4.0/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.867453 tigeropen-2.4.0/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.4.0/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.867832 tigeropen-2.4.0/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.869669 tigeropen-2.4.0/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7277 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4759 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.838100 tigeropen-2.4.0/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.3.9/PKG-INFO` & `tigeropen-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.9
+Version: 2.4.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.9/README.md` & `tigeropen-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/setup.py` & `tigeropen-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/__init__.py` & `tigeropen-2.4.0/tigeropen/common/consts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     STK = 'STK'  # 股票
     OPT = 'OPT'  # 期权
     WAR = 'WAR'  # 窝轮
     IOPT = 'IOPT'  # 权证(牛熊证)
     FUT = 'FUT'  # 期货
     FOP = 'FOP'  # 期货期权
     CASH = 'CASH'  # 外汇
-
+    MLEG = 'MLEG'
 
 @unique
 class SegmentType(Enum):
     ALL = 'ALL'
     SEC = 'SEC'
     FUT = 'FUT'
 
@@ -185,21 +185,33 @@
     MKT = 'MKT'  # 市价单
     LMT = 'LMT'  # 限价单
     STP = 'STP'  # 止损单
     STP_LMT = 'STP_LMT'  # 止损限价单
     TRAIL = 'TRAIL'  # 跟踪止损单
     AM = 'AM'  # Auction Market ，竞价市价单
     AL = 'AL'  # Auction Limit ，竞价限价单
-
+    TWAP = 'TWAP'  # 'Time Weighted Average Price' 时间加权平均价格算法
+    VWAP = 'VWAP'  # 'Volume Weighted Average Price'  成交量加权平均价格算法
 
 @unique
 class License(Enum):
     TBNZ = 'TBNZ'
     TBSG = 'TBSG'
 
 
 @unique
 class ServiceType(Enum):
     COMMON = 'COMMON'
     TRADE = 'TRADE'
     QUOTE = 'QUOTE'
 
+@unique
+class ComboType(Enum):
+    COVERED = 'COVERED'
+    PROTECTIVE = 'PROTECTIVE'
+    VERTICAL = 'VERTICAL'
+    STRADDLE = 'STRADDLE'
+    STRANGLE = 'STRANGLE'
+    CALENDAR = 'CALENDAR'
+    DIAGONAL = 'DIAGONAL'
+    SYNTHETIC = 'SYNTHETIC'
+    CUSTOM = 'CUSTOM'
```

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/filter_fields.py` & `tigeropen-2.4.0/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-2.4.0/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/params.py` & `tigeropen-2.4.0/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/push_types.py` & `tigeropen-2.4.0/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/quote_keys.py` & `tigeropen-2.4.0/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/service_types.py` & `tigeropen-2.4.0/tigeropen/common/consts/service_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/consts/tick_constants.py` & `tigeropen-2.4.0/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/model.py` & `tigeropen-2.4.0/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/request.py` & `tigeropen-2.4.0/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/response.py` & `tigeropen-2.4.0/tigeropen/common/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/9/20
 
 @author: gaoan
 """
+import json
 
 
 class TigerResponse:
     def __init__(self):
         self.code = None
         self.message = None
         self.data = None
@@ -18,8 +19,10 @@
     def parse_response_content(self, response):
         if 'code' in response:
             self.code = response['code']
         if 'message' in response:
             self.message = response['message']
         if 'data' in response:
             self.data = response['data']
+            if isinstance(self.data, str):
+                self.data = json.loads(self.data)
         return response
```

### Comparing `tigeropen-2.3.9/tigeropen/common/util/common_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/contract_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/order_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/order_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/11/1
 
 @author: gaoan
 """
+from tigeropen.trade.domain.contract import ContractLeg
 from tigeropen.trade.domain.order import Order, OrderLeg, AlgoParams
-from tigeropen.common.consts import OrderStatus
+from tigeropen.common.consts import OrderStatus, OrderType
 
 
 def market_order(account, contract, action, quantity):
     """
     市价单
     :param account:
     :param contract:
@@ -160,14 +161,25 @@
     :param limit_price:
     :return:
     """
     return Order(account, contract, action, order_type=strategy, quantity=quantity, algo_params=algo_params,
                  limit_price=limit_price, outside_rth=False)
 
 
+def contract_leg(symbol=None, sec_type=None, expiry=None, strike=None, put_call=None, action=None,
+                 ratio=1):
+    return ContractLeg(symbol=symbol, sec_type=sec_type, expiry=expiry, strike=strike, put_call=put_call,
+                        action=action, ratio=ratio)
+
+
+def combo_order(account, contract_legs, combo_type, action, quantity, order_type=OrderType.LMT.value, limit_price=None,
+                aux_price=None, trailing_percent=None):
+    return Order(account, None, action=action, order_type=order_type, quantity=quantity, limit_price=limit_price,
+                 aux_price=aux_price, trailing_percent=trailing_percent, combo_type=combo_type,
+                 contract_legs=contract_legs)
 def get_order_status(value):
     """
     Invalid(-2), Initial(-1), PendingCancel(3), Cancelled(4), Submitted(5), Filled(6), Inactive(7), PendingSubmit(8)
     :param value:
     :return:
     """
     if value == -1 or value == 'Initial':
```

### Comparing `tigeropen-2.3.9/tigeropen/common/util/price_util.py` & `tigeropen-2.4.0/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/signature_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/string_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/tick_util.py` & `tigeropen-2.4.0/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/common/util/web_utils.py` & `tigeropen-2.4.0/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/client_config.py` & `tigeropen-2.4.0/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/nasdaq100.py` & `tigeropen-2.4.0/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-2.4.0/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/push_client_demo.py` & `tigeropen-2.4.0/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-2.4.0/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/quote_client_demo.py` & `tigeropen-2.4.0/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/examples/trade_client_demo.py` & `tigeropen-2.4.0/tigeropen/examples/trade_client_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 
 
 def algo_order_demo():
     account = client_config.account
     openapi_client = TradeClient(client_config, logger=logger)
     contract = stock_contract(symbol='AAPL', currency='USD')
-    params = algo_order_params(start_time='2020-11-19 23:00:00', end_time='2020-11-19 23:50:00', no_take_liq=True,
+    params = algo_order_params(start_time=1686147201000, end_time=1686150801000, no_take_liq=True,
                                allow_past_end_time=True, participation_rate=0.1)
     order = algo_order(account, contract, 'BUY', 1000, 'VWAP', algo_params=params, limit_price=100.0)
     openapi_client.place_order(order)
     print(order)
 
 
 def get_account_info():
```

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/request/model.py` & `tigeropen-2.4.0/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/fundamental/response/industry_response.py` & `tigeropen-2.4.0/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/__init__.py` & `tigeropen-2.4.0/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/connect.py` & `tigeropen-2.4.0/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/exception.py` & `tigeropen-2.4.0/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/listener.py` & `tigeropen-2.4.0/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/protocal.py` & `tigeropen-2.4.0/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/transport.py` & `tigeropen-2.4.0/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/network/utils.py` & `tigeropen-2.4.0/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/AssetData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PositionData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PushData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteData.proto`

 * *Files 7% similar despite different names*

```diff
@@ -44,12 +44,12 @@
   optional Minute mi = 28;
 
   message Minute {
     double p = 1; // last price of the minute bar
     double a = 2; // average price of the minute bar
     uint64 t = 3; // timestamp of the minute bar
     sint64 v = 4; // trading volume of the minute bar
-    double o = 5; // open price of the minute bar (only futures support)
-    double h = 6; // highest price of the minute bar (only futures support)
-    double l = 7; // lowest price of the minute bar (only futures support)
+    double o = 5; // open price of the minute bar
+    double h = 6; // highest price of the minute bar
+    double l = 7; // lowest price of the minute bar
   }
 }
```

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/Request.proto` & `tigeropen-2.4.0/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/trade_tick.py` & `tigeropen-2.4.0/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/pb/util.py` & `tigeropen-2.4.0/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/protobuf_push_client.py` & `tigeropen-2.4.0/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/push_client.py` & `tigeropen-2.4.0/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/push/stomp_push_client.py` & `tigeropen-2.4.0/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/domain/filter.py` & `tigeropen-2.4.0/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/domain/quote_brief.py` & `tigeropen-2.4.0/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/domain/stock_broker.py` & `tigeropen-2.4.0/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/quote_client.py` & `tigeropen-2.4.0/tigeropen/quote/quote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,26 +476,30 @@
         if begin_time == -1 and end_time == -1:
             raise ApiException(400, 'One of the begin_time or end_time must be specified')
         if isinstance(symbol, list) and len(symbol) != 1:
             raise ApiException(400, 'Paging queries support only one symbol at each request')
         current = 0
         next_page_token = None
         result = list()
+        result_df = None
         while current < total:
             if current + page_size >= total:
                 page_size = total - current
             current += page_size
             bars = self.get_bars(symbols=symbol, period=period, begin_time=begin_time, end_time=end_time, right=right,
                                  limit=page_size, lang=lang, page_token=next_page_token)
+            if bars.empty:
+                result_df = bars
+                break
             next_page_token = bars['next_page_token'].iloc[0]
             result.append(bars)
             if not next_page_token:
                 break
             time.sleep(time_interval)
-        return pd.concat(result).sort_values('time').reset_index(drop=True)
+        return pd.concat(result).sort_values('time').reset_index(drop=True) if result else result_df
 
     def get_trade_ticks(self, symbols, trade_session=None, begin_index=None, end_index=None, limit=None, lang=None,
                         **kwargs):
         """
         获取逐笔成交
         :param symbols: 股票代号列表
         :param trade_session: tigeropen.common.consts.TradingSession, like TradingSession.PreMarket
@@ -1041,26 +1045,30 @@
         if begin_time == -1 and end_time == -1:
             raise ApiException(400, 'One of the begin_time or end_time must be specified')
         if isinstance(identifier, list) and len(identifier) != 1:
             raise ApiException(400, 'Paging queries support only one identifier at each request')
         current = 0
         next_page_token = None
         result = list()
+        result_df = None
         while current < total:
             if current + page_size >= total:
                 page_size = total - current
             current += page_size
             bars = self.get_future_bars(identifiers=identifier, period=period, begin_time=begin_time, end_time=end_time,
                                         limit=page_size, page_token=next_page_token)
+            if bars.empty:
+                result_df = bars
+                break
             next_page_token = bars['next_page_token'].iloc[0]
             result.append(bars)
             if not next_page_token:
                 break
             time.sleep(time_interval)
-        return pd.concat(result).sort_values('time').reset_index(drop=True)
+        return pd.concat(result).sort_values('time').reset_index(drop=True) if result else result_df
 
     def get_future_trade_ticks(self, identifier, begin_index=0, end_index=30, limit=1000):
         """
         获取期货逐笔成交
         :param identifier: future identifier. Only supports one identifier
         :param begin_index: 开始索引
         :param end_index: 结束索引
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/request/model.py` & `tigeropen-2.4.0/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_contract_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
            'open_interest', 'next_page_token']
 BAR_FIELD_MAPPINGS = {'avgPrice': 'avg_price', 'openInterest': 'open_interest', 'lastTime': 'latest_time'}
 
 
 class FutureQuoteBarResponse(TigerResponse):
     def __init__(self):
         super(FutureQuoteBarResponse, self).__init__()
-        self.bars = []
+        self.bars = pd.DataFrame(columns=COLUMNS)
         self._is_success = None
 
     def parse_response_content(self, response_content):
         response = super(FutureQuoteBarResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/market_status_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/option_chains_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_bar_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 COLUMNS = ['symbol', 'time', 'open', 'high', 'low', 'close', 'volume', 'amount', 'next_page_token']
 BAR_FIELD_MAPPINGS = {'avgPrice': 'avg_price'}
 
 
 class QuoteBarResponse(TigerResponse):
     def __init__(self):
         super(QuoteBarResponse, self).__init__()
-        self.bars = None
+        self.bars = pd.DataFrame(columns=COLUMNS)
         self._is_success = None
 
     def parse_response_content(self, response_content):
         response = super(QuoteBarResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_brief_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
 
-import json
-
 from tigeropen.common.consts import TradingSession
 from tigeropen.common.response import TigerResponse
 from tigeropen.quote.domain.quote_brief import QuoteBrief, HourTrading
 
 BRIEF_FIELD_MAPPINGS = {'latestPrice': 'latest_price', 'preClose': 'prev_close', 'secType': 'sec_type',
                         'timestamp': 'latest_time', 'askPrice': 'ask_price', 'askSize': 'ask_size',
                         'bidPrice': 'bid_price', 'bidSize': 'bid_size'}
@@ -24,17 +22,16 @@
 
     def parse_response_content(self, response_content):
         response = super(QuoteBriefResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            if 'items' in data_json:
-                for item in data_json['items']:
+            if 'items' in self.data:
+                for item in self.data['items']:
                     brief = QuoteBrief()
                     for key, value in item.items():
                         if value is None:
                             continue
                         if key == 'hourTrading':
                             hour_trading = HourTrading()
                             for sub_key, sub_value in value.items():
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def parse_response_content(self, response_content):
         response = super(QuoteHourTradingTimelineResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
+            data_json = self.data
             pre_close = data_json.get('preClose')
             if 'detail' in data_json:
                 detail = data_json['detail']
                 hour_trading = HourTrading()
                 if 'timestamp' in response:
                     hour_trading.latest_time = response['timestamp']
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_ticks_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 import pandas as pd
 
 from tigeropen.common.response import TigerResponse
 
 COLUMNS = ['symbol', 'index', 'time', 'price', 'volume', 'direction']
 
 
@@ -34,16 +32,15 @@
         # {"time":1663963192142,"volume":100,"price":150.61,"type":"+"}
 
         if self.data:
             # v2
             if isinstance(self.data, list):
                 symbol_items = self.data
             else:
-                data = json.loads(self.data)
-                symbol_items = [data]
+                symbol_items = [self.data]
 
             tick_items = []
             for symbol_item in symbol_items:
                 symbol = symbol_item.get('symbol')
                 if 'items' in symbol_item:
                     index = symbol_item.get('beginIndex')
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/stock_details_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/stock_details_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 import pandas as pd
 
 from tigeropen.common.response import TigerResponse
 
 # 盘前盘后
 HOUR_TRADING_COLUMNS = [
     'hour_trading_tag',
@@ -107,16 +105,15 @@
     def parse_response_content(self, response_content):
         response = super(StockDetailsResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
         if not self.data:
             return
         detail_data = []
-        data_json = json.loads(self.data)
-        for item in data_json.get('items', {}):
+        for item in self.data.get('items', {}):
             item_values = dict()
             for key, value in item.items():
                 if value is None:
                     continue
                 tag = self._key_to_tag(key)
                 if tag in SUB_FIELDS:
                     for sub_k, sub_v in value.items():
```

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/symbols_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-2.4.0/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/tiger_open_client.py` & `tigeropen-2.4.0/tigeropen/tiger_open_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,30 +198,30 @@
             response_content = self.execute(request)
         except Exception as e:
             self.__logger.error(e, exc_info=True)
         if response_content:
             response = TigerResponse()
             response.parse_response_content(response_content)
             if response.is_success():
-                return json.loads(response.data).get('license')
+                return response.data.get('license')
         self.__logger.error(f"failed to query license, response: {response_content}")
 
     def query_token(self):
         request = OpenApiRequest(method=USER_TOKEN_REFRESH)
 
         response_content = None
         try:
             response_content = self.execute(request)
         except Exception as e:
             self.__logger.error(e, exc_info=True)
         if response_content:
             response = TigerResponse()
             response.parse_response_content(response_content)
             if response.is_success():
-                return json.loads(response.data).get('token')
+                return response.data.get('token')
         self.__logger.error(f"failed to refresh token, response: {response_content}")
         return None
 
     def refresh_token(self):
         self.__config.token = self.__config.load_token()
         new_token = self.query_token()
         if new_token:
```

### Comparing `tigeropen-2.3.9/tigeropen/tiger_open_config.py` & `tigeropen-2.4.0/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/domain/account.py` & `tigeropen-2.4.0/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/domain/contract.py` & `tigeropen-2.4.0/tigeropen/trade/domain/contract.py`

 * *Files 25% similar despite different names*

```diff
@@ -105,7 +105,52 @@
 
     def is_cn_stock(self):
         """
         是否是A股
         :return:
         """
         return self.sec_type == 'STK' and (self.currency == 'CNH' or self.currency == 'CNY')
+
+
+class ContractLeg:
+    def __init__(self, symbol=None, sec_type=None, expiry=None, strike=None, put_call=None, action=None,
+                 ratio=1):
+        self.symbol = symbol
+        self.sec_type = sec_type
+        self.expiry = expiry
+        self.strike = strike
+        self.put_call = put_call
+        self.action = action
+        self.ratio = ratio
+
+    def to_openapi_dict(self):
+        d = dict(**self.__dict__)
+        d['right'] = d.pop('put_call', None)
+        return d
+
+    def __repr__(self):
+        return str(self.__dict__)
+
+class OrderContractLeg(ContractLeg):
+    def __init__(self, symbol=None, sec_type=None, expiry=None, strike=None, put_call=None, action=None,
+                 ratio=1, market=None, currency=None, multiplier=None, total_quantity=None, filled_quantity=None,
+                 avg_filled_price=None, created_at=None, updated_at=None, **kwargs):
+        if 'right' in kwargs and not put_call:
+            put_call = kwargs.get('right')
+        super().__init__(symbol=symbol, sec_type=sec_type, expiry=expiry, strike=strike, put_call=put_call, action=action,
+                 ratio=ratio)
+        self.market = market
+        self.currency = currency
+        self.multiplier = multiplier
+        self.total_quantity = total_quantity
+        self.filled_quantity = filled_quantity
+        self.avg_filled_price = avg_filled_price
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    def to_openapi_dict(self):
+        d = super().to_openapi_dict()
+        d.update(self.__dict__)
+        return d
+
+    def __repr__(self):
+        return str(self.__dict__)
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/domain/order.py` & `tigeropen-2.4.0/tigeropen/trade/domain/order.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 class Order:
     __slots__ = ["account", "id", "order_id", "parent_id", "order_time", "reason", "trade_time", "contract", "action",
                  "quantity", "filled", "_remaining", "avg_fill_price", "commission", "realized_pnl", "_status",
                  "trail_stop_price", "limit_price", "aux_price", "trailing_percent", "percent_offset", "action",
                  "order_type", "time_in_force", "outside_rth", "order_legs", "algo_params", "algo_strategy",
                  "secret_key", "liquidation", "discount", "attr_desc", "source", 'adjust_limit', 'sub_ids', "user_mark",
-                 "update_time", "expire_time", "can_modify", "external_id"]
+                 "update_time", "expire_time", "can_modify", "external_id", "combo_type", "combo_type_desc", 'is_open',
+                 "contract_legs"]
 
     def __init__(self, account, contract, action, order_type, quantity, limit_price=None, aux_price=None,
                  trail_stop_price=None, trailing_percent=None, percent_offset=None, time_in_force=None,
                  outside_rth=None, filled=0, avg_fill_price=0, commission=None, realized_pnl=None,
                  id=None, order_id=None, parent_id=None, order_time=None, trade_time=None, order_legs=None,
                  algo_params=None, secret_key=None, **kwargs):
         """
@@ -98,14 +99,18 @@
         self.source = kwargs.get('source')
         self.adjust_limit = kwargs.get('adjust_limit')
         self.sub_ids = kwargs.get('sub_ids')
         self.user_mark = kwargs.get('user_mark')
         self.expire_time = kwargs.get('expire_time')
         self.can_modify = kwargs.get('can_modify')
         self.external_id = kwargs.get('external_id')
+        self.combo_type = kwargs.get('combo_type')
+        self.combo_type_desc = kwargs.get('combo_type_desc')
+        self.is_open = kwargs.get('is_open')
+        self.contract_legs = kwargs.get('contract_legs')
 
     def to_dict(self):
         dct = {name: getattr(self, name) for name in self.__slots__ if name not in ORDER_FIELDS_TO_IGNORE}
 
         dct['contract'] = self.contract
         if self.status:
             dct['status'] = self.status.name
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/domain/position.py` & `tigeropen-2.4.0/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/domain/prime_account.py` & `tigeropen-2.4.0/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/request/model.py` & `tigeropen-2.4.0/tigeropen/trade/request/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -771,14 +771,16 @@
         self.time_in_force = None
         self.outside_rth = None
         self.order_legs = None
         self.algo_params = None
         self.adjust_limit = None
         self.user_mark = None
         self.expire_time = None
+        self.combo_type = None
+        self.contract_legs = None
 
     def to_openapi_dict(self):
         params = super().to_openapi_dict()
 
         if self.contract:
             if self.contract.symbol is not None:
                 params['symbol'] = self.contract.symbol
@@ -794,87 +796,93 @@
                 params['expiry'] = self.contract.expiry
             if self.contract.strike is not None:
                 params['strike'] = self.contract.strike
             if self.contract.put_call is not None:
                 params['right'] = self.contract.put_call
             if self.contract.multiplier is not None:
                 params['multiplier'] = self.contract.multiplier
-
-            if self.account:
-                params['account'] = self.account
-            if self.secret_key:
-                params['secret_key'] = self.secret_key
-
-            if self.order_id:
-                params['order_id'] = self.order_id
-            if self.id:
-                params['id'] = self.id
-            if self.order_type:
-                params['order_type'] = self.order_type
-            if self.action:
-                params['action'] = self.action
-            if self.quantity is not None:
-                params['total_quantity'] = self.quantity
-            if self.limit_price is not None:
-                params['limit_price'] = self.limit_price
-            if self.aux_price is not None:
-                params['aux_price'] = self.aux_price
-            if self.trail_stop_price is not None:
-                params['trail_stop_price'] = self.trail_stop_price
-            if self.trailing_percent is not None:
-                params['trailing_percent'] = self.trailing_percent
-            if self.percent_offset is not None:
-                params['percent_offset'] = self.percent_offset
-            if self.time_in_force is not None:
-                params['time_in_force'] = self.time_in_force
-            if self.outside_rth is not None:
-                params['outside_rth'] = self.outside_rth
-            if self.adjust_limit is not None:
-                params['adjust_limit'] = self.adjust_limit
-            if self.user_mark is not None:
-                params['user_mark'] = self.user_mark
-            if self.expire_time is not None:
-                params['expire_time'] = self.expire_time
-
-            if self.order_legs:
-                if len(self.order_legs) > 2:
-                    raise Exception('2 order legs at most')
-                leg_types = set()
-                for order_leg in self.order_legs:
-                    if order_leg.leg_type == 'PROFIT':
-                        leg_types.add('PROFIT')
-                        params['attach_type'] = 'PROFIT'
-                        if order_leg.price is not None:
-                            params['profit_taker_price'] = order_leg.price
-                        if order_leg.time_in_force is not None:
-                            params['profit_taker_tif'] = order_leg.time_in_force
-                        if order_leg.outside_rth is not None:
-                            params['profit_taker_rth'] = order_leg.outside_rth
-                    if order_leg.leg_type == 'LOSS':
-                        leg_types.add('LOSS')
-                        params['attach_type'] = 'LOSS'
-                        if order_leg.price is not None:
-                            params['stop_loss_price'] = order_leg.price
-                        if order_leg.time_in_force is not None:
-                            params['stop_loss_tif'] = order_leg.time_in_force
-                        if order_leg.outside_rth is not None:
-                            params['stop_loss_rth'] = order_leg.outside_rth
-                        if order_leg.limit_price is not None:
-                            params['stop_loss_limit_price'] = order_leg.limit_price
-                        if order_leg.trailing_percent is not None:
-                            params['stop_loss_trailing_percent'] = order_leg.trailing_percent
-                        if order_leg.trailing_percent is not None:
-                            params['stop_loss_trailing_amount'] = order_leg.trailing_amount
-
-                # 括号订单(止盈和止损)
-                if len(leg_types) == 2:
-                    params['attach_type'] = 'BRACKETS'
-
-            if self.algo_params:
-                params['algo_params'] = [{'tag': item[0], 'value': item[1]} for item in self.algo_params.to_dict().items()]
+        if self.contract_legs:
+            params['contract_legs'] = list()
+            for item in self.contract_legs:
+                params['contract_legs'].append(item.to_openapi_dict())
+            params['sec_type'] = 'MLEG'
+        if self.account:
+            params['account'] = self.account
+        if self.secret_key:
+            params['secret_key'] = self.secret_key
+
+        if self.order_id:
+            params['order_id'] = self.order_id
+        if self.id:
+            params['id'] = self.id
+        if self.order_type:
+            params['order_type'] = self.order_type
+        if self.action:
+            params['action'] = self.action
+        if self.quantity is not None:
+            params['total_quantity'] = self.quantity
+        if self.limit_price is not None:
+            params['limit_price'] = self.limit_price
+        if self.aux_price is not None:
+            params['aux_price'] = self.aux_price
+        if self.trail_stop_price is not None:
+            params['trail_stop_price'] = self.trail_stop_price
+        if self.trailing_percent is not None:
+            params['trailing_percent'] = self.trailing_percent
+        if self.percent_offset is not None:
+            params['percent_offset'] = self.percent_offset
+        if self.time_in_force is not None:
+            params['time_in_force'] = self.time_in_force
+        if self.outside_rth is not None:
+            params['outside_rth'] = self.outside_rth
+        if self.adjust_limit is not None:
+            params['adjust_limit'] = self.adjust_limit
+        if self.user_mark is not None:
+            params['user_mark'] = self.user_mark
+        if self.expire_time is not None:
+            params['expire_time'] = self.expire_time
+
+        if self.order_legs:
+            if len(self.order_legs) > 2:
+                raise Exception('2 order legs at most')
+            leg_types = set()
+            for order_leg in self.order_legs:
+                if order_leg.leg_type == 'PROFIT':
+                    leg_types.add('PROFIT')
+                    params['attach_type'] = 'PROFIT'
+                    if order_leg.price is not None:
+                        params['profit_taker_price'] = order_leg.price
+                    if order_leg.time_in_force is not None:
+                        params['profit_taker_tif'] = order_leg.time_in_force
+                    if order_leg.outside_rth is not None:
+                        params['profit_taker_rth'] = order_leg.outside_rth
+                if order_leg.leg_type == 'LOSS':
+                    leg_types.add('LOSS')
+                    params['attach_type'] = 'LOSS'
+                    if order_leg.price is not None:
+                        params['stop_loss_price'] = order_leg.price
+                    if order_leg.time_in_force is not None:
+                        params['stop_loss_tif'] = order_leg.time_in_force
+                    if order_leg.outside_rth is not None:
+                        params['stop_loss_rth'] = order_leg.outside_rth
+                    if order_leg.limit_price is not None:
+                        params['stop_loss_limit_price'] = order_leg.limit_price
+                    if order_leg.trailing_percent is not None:
+                        params['stop_loss_trailing_percent'] = order_leg.trailing_percent
+                    if order_leg.trailing_percent is not None:
+                        params['stop_loss_trailing_amount'] = order_leg.trailing_amount
+
+            # 括号订单(止盈和止损)
+            if len(leg_types) == 2:
+                params['attach_type'] = 'BRACKETS'
+
+        if self.algo_params:
+            params['algo_params'] = [{'tag': item[0], 'value': item[1]} for item in self.algo_params.to_dict().items()]
+        if self.combo_type:
+            params['combo_type'] = self.combo_type
         return params
 
 
 class CancelOrderParams(BaseParams):
     def __init__(self):
         super(CancelOrderParams, self).__init__()
         self._account = None
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/__init__.py` & `tigeropen-2.4.0/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/account_profile_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/account_profile_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util.string_utils import camel_to_underline_obj
 from tigeropen.trade.domain.profile import AccountProfile
 
 
 class ProfilesResponse(TigerResponse):
     def __init__(self):
@@ -19,14 +17,13 @@
 
     def parse_response_content(self, response_content):
         response = super(ProfilesResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            if 'items' in data_json:
-                for item in data_json['items']:
+            if 'items' in self.data:
+                for item in self.data['items']:
                     data_dict = camel_to_underline_obj(item)
                     profile = AccountProfile(account=data_dict.get('account'), capability=data_dict.get('capability'),
                                              status=data_dict.get('status'), account_type=data_dict.get('account_type'))
                     self.profiles.append(profile)
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/analytics_asset_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 # 
 # @Date    : 2022/7/8
 # @Author  : sukai
-import json
 from datetime import datetime
 
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util.string_utils import camel_to_underline_obj
 
 
 class AnalyticsAssetResponse(TigerResponse):
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/assets_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/assets_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/9/20
 
 @author: gaoan
 """
-import json
 from tigeropen.common.response import TigerResponse
 from tigeropen.trade.domain.account import PortfolioAccount
 from tigeropen.common.util.string_utils import camel_to_underline
 
 ACCOUNT_FIELD_MAPPINGS = {'sMA': 'sma', 'updateTime': 'timestamp', 'realizedPnL': 'realized_pnl',
                           'unrealizedPnL': 'unrealized_pnl', 'regTMargin': 'regt_margin', 'regTEquity': 'regt_equity',
                           'cashValue': 'cash', 'initMarginReq': 'initial_margin_requirement',
@@ -25,17 +24,16 @@
 
     def parse_response_content(self, response_content):
         response = super(AssetsResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            if 'items' in data_json:
-                for item in data_json['items']:
+            if 'items' in self.data:
+                for item in self.data['items']:
                     account = item['account']
                     asset = PortfolioAccount(account)
                     summary = asset.summary
 
                     for key, value in item.items():
                         if value is None:
                             continue
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/contracts_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/contracts_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util.string_utils import camel_to_underline, camel_to_underline_obj
 from tigeropen.trade.domain.contract import Contract
 
 CONTRACT_FIELD_MAPPINGS = {'conid': 'contract_id', 'right': 'put_call', 'tradeable': 'trade'}
 
 
@@ -21,19 +19,18 @@
     
     def parse_response_content(self, response_content):
         response = super(ContractsResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
         
         if self.data:
-            data_json = self.data if isinstance(self.data, dict) else json.loads(self.data)
-            if 'items' in data_json:
-                items = data_json['items']
+            if 'items' in self.data:
+                items = self.data['items']
             else:
-                items = [data_json]
+                items = [self.data]
             for item in items:
                 contract_fields = {}
                 for key, value in item.items():
                     tag = CONTRACT_FIELD_MAPPINGS[key] if key in CONTRACT_FIELD_MAPPINGS else camel_to_underline(key)
                     if isinstance(value, (list, dict)):
                         value = camel_to_underline_obj(value)
                     contract_fields[tag] = value
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/forex_order_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/order_id_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/order_id_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
 from tigeropen.common.response import TigerResponse
 
 
 class OrderIdResponse(TigerResponse):
     def __init__(self):
         super(OrderIdResponse, self).__init__()
         self.order_id = None
         self.id = None
         self.sub_ids = None
+        self.orders = None
         self._is_success = None
     
     def parse_response_content(self, response_content):
         response = super(OrderIdResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
         
         if self.data:
-            data_json = json.loads(self.data)
+            data_json = self.data
             if 'code' in data_json and data_json['code'] != '0':
                 self.code = int(data_json['code'])
                 if 'message' in data_json:
                     self.message = data_json['message']
             
             if 'orderId' in data_json:
                 self.order_id = data_json['orderId']
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/order_preview_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/order_preview_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from tigeropen.common.response import TigerResponse
 
 PREVIEW_ORDER_FIELD_MAPPING = {"initMarginBefore": "init_margin_before", "commissionCurrency": "commission_currency",
                                "maintMargin": "maint_margin", "equityWithLoan": "equity_with_loan",
                                "minCommission": "min_commission", "maintMarginBefore": "maint_margin_before",
                                "initMargin": "init_margin", "equityWithLoanBefore": "equity_with_loan_before",
                                "marginCurrency": "margin_currency", "maxCommission": "max_commission",
@@ -17,12 +16,11 @@
 
     def parse_response_content(self, response_content):
         response = super(PreviewOrderResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            for key, value in data_json.items():
+            for key, value in self.data.items():
                 field = PREVIEW_ORDER_FIELD_MAPPING.get(key, key)
                 self.preview_order[field] = value
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/orders_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/orders_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util.order_utils import get_order_status
-from tigeropen.trade.domain.contract import Contract
+from tigeropen.common.util.string_utils import camel_to_underline_obj
+from tigeropen.trade.domain.contract import Contract, OrderContractLeg
 from tigeropen.trade.domain.order import Order, AlgoParams
 from tigeropen.trade.response import CONTRACT_FIELDS
 
 ORDER_FIELD_MAPPINGS = {'parentId': 'parent_id', 'orderId': 'order_id', 'orderType': 'order_type',
                         'limitPrice': 'limit_price', 'auxPrice': 'aux_price', 'avgFillPrice': 'avg_fill_price',
                         'totalQuantity': 'quantity', 'filledQuantity': 'filled', 'lastFillPrice': 'last_fill_price',
                         'realizedPnl': 'realized_pnl', 'secType': 'sec_type',
                         'remark': 'reason',
                         'localSymbol': 'local_symbol', 'originSymbol': 'origin_symbol', 'outsideRth': 'outside_rth',
                         'timeInForce': 'time_in_force', 'openTime': 'order_time', 'latestTime': 'trade_time',
                         'contractId': 'contract_id', 'algoStrategy': 'algo_strategy',
                         'trailStopPrice': 'trail_stop_price', 'trailingPercent': 'trailing_percent',
                         'percentOffset': 'percent_offset', 'identifier': 'identifier', 'algoParameters': 'algo_params',
                         'userMark': 'user_mark', 'updateTime': 'update_time', 'expireTime': 'expire_time',
-                        'canModify': 'can_modify', 'externalId': 'external_id',
+                        'canModify': 'can_modify', 'externalId': 'external_id', 'isOpen': 'is_open',
+                        'comboType': 'combo_type', 'comboTypeDesc': 'combo_type_desc'
                         }
 
 
 class OrdersResponse(TigerResponse):
     def __init__(self):
         super(OrdersResponse, self).__init__()
         self.orders = []
@@ -35,22 +35,21 @@
 
     def parse_response_content(self, response_content, secret_key=None):
         response = super(OrdersResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            if 'items' in data_json:
-                for item in data_json['items']:
+            if 'items' in self.data:
+                for item in self.data['items']:
                     order = OrdersResponse.parse_order(item, secret_key)
                     if order:
                         self.orders.append(order)
-            elif 'symbol' in data_json:
-                order = OrdersResponse.parse_order(data_json, secret_key)
+            elif 'symbol' in self.data:
+                order = OrdersResponse.parse_order(self.data, secret_key)
                 if order:
                     self.orders.append(order)
 
     @staticmethod
     def parse_order(item, secret_key=None):
         contract_fields = {}
         order_fields = {}
@@ -103,30 +102,35 @@
         algo_strategy = order_fields.get('algo_strategy')
         discount = order_fields.get('discount')
         attr_desc = order_fields.get('attr_desc')
         source = order_fields.get('source')
         user_mark = order_fields.get('user_mark')
         can_modify = order_fields.get('can_modify')
         external_id = order_fields.get('external_id')
+        is_open = order_fields.get('is_open')
+        combo_type = order_fields.get('combo_type')
+        combo_type_desc = order_fields.get('combo_type_desc')
 
         order = Order(account, contract, action, order_type, quantity, limit_price=limit_price, aux_price=aux_price,
                       trail_stop_price=trail_stop_price, trailing_percent=trailing_percent,
                       percent_offset=percent_offset, time_in_force=time_in_force, outside_rth=outside_rth,
                       filled=filled, avg_fill_price=avg_fill_price, commission=commission,
                       realized_pnl=realized_pnl, id=id_, order_id=order_id, parent_id=parent_id,
                       algo_params=algo_params, liquidation=liquidation, algo_strategy=algo_strategy, discount=discount,
                       attr_desc=attr_desc, source=source, user_mark=user_mark, expire_time=expire_time,
-                      can_modify=can_modify, external_id=external_id)
+                      can_modify=can_modify, external_id=external_id, is_open=is_open, combo_type=combo_type,
+                      combo_type_desc=combo_type_desc)
         if 'order_time' in order_fields:
             order.order_time = order_fields.get('order_time')
         if 'trade_time' in order_fields:
             order.trade_time = order_fields.get('trade_time')
         if 'update_time' in order_fields:
             order.update_time = order_fields.get('update_time')
         if 'reason' in order_fields:
             order.reason = order_fields.get('reason')
         if secret_key is not None:
             order.secret_key = secret_key
         order.status = status
-
+        if 'legs' in order_fields:
+            order.contract_legs = [OrderContractLeg(**camel_to_underline_obj(leg)) for leg in order_fields['legs']]
         return order
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/positions_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/positions_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2018/10/31
 
 @author: gaoan
 """
-import json
-
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util import string_utils
 from tigeropen.trade.domain.contract import Contract
 from tigeropen.trade.domain.position import Position, TradableQuantityItem
 from tigeropen.trade.response import CONTRACT_FIELDS
 
 POSITION_FIELD_MAPPINGS = {'averageCost': 'average_cost', 'position': 'quantity', 'latestPrice': 'market_price',
@@ -27,17 +25,16 @@
     
     def parse_response_content(self, response_content):
         response = super(PositionsResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
         
         if self.data:
-            data_json = json.loads(self.data)
-            if 'items' in data_json:
-                for item in data_json['items']:
+            if 'items' in self.data:
+                for item in self.data['items']:
                     contract_fields = {}
                     position_fields = {}
                     for key, value in item.items():
                         if value is None:
                             continue
                         tag = POSITION_FIELD_MAPPINGS[key] if key in POSITION_FIELD_MAPPINGS else key
                         if tag in CONTRACT_FIELDS:
@@ -85,9 +82,8 @@
 
     def parse_response_content(self, response_content):
         response = super(EstimateTradableQuantityResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            self.result = TradableQuantityItem(**string_utils.camel_to_underline_obj(data_json))
+            self.result = TradableQuantityItem(**string_utils.camel_to_underline_obj(self.data))
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.9/tigeropen/trade/response/transactions_response.py` & `tigeropen-2.4.0/tigeropen/trade/response/transactions_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # -*- coding: utf-8 -*-
-import json
-
 from tigeropen.common.response import TigerResponse
 from tigeropen.common.util import string_utils
 from tigeropen.trade.domain.contract import Contract
 from tigeropen.trade.domain.order import Transaction
 from tigeropen.trade.response import CONTRACT_FIELDS
 
 FIELD_MAPPINGS = {'account_id': 'account', 'right': 'put_call'}
@@ -18,16 +16,15 @@
 
     def parse_response_content(self, response_content):
         response = super(TransactionsResponse, self).parse_response_content(response_content)
         if 'is_success' in response:
             self._is_success = response['is_success']
 
         if self.data:
-            data_json = json.loads(self.data)
-            for item in data_json.get('items', list()):
+            for item in self.data.get('items', list()):
                 trans = self._parse_transactions(string_utils.camel_to_underline_obj(item))
                 if trans:
                     self.transactions.append(trans)
 
     def _parse_transactions(self, item_dict):
         trans = Transaction()
         contract = Contract()
```

### Comparing `tigeropen-2.3.9/tigeropen/trade/trade_client.py` & `tigeropen-2.4.0/tigeropen/trade/trade_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,14 +573,16 @@
         params.order_legs = order.order_legs
         params.algo_params = order.algo_params
         params.secret_key = order.secret_key if order.secret_key else self._secret_key
         params.adjust_limit = order.adjust_limit
         params.user_mark = order.user_mark
         params.expire_time = order.expire_time
         params.lang = get_enum_value(self._lang)
+        params.combo_type = get_enum_value(order.combo_type)
+        params.contract_legs = order.contract_legs
 
         request = OpenApiRequest(PLACE_ORDER, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OrderIdResponse()
             response.parse_response_content(response_content)
             if response.is_success():
```

### Comparing `tigeropen-2.3.9/tigeropen.egg-info/PKG-INFO` & `tigeropen-2.4.0/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.9
+Version: 2.4.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.9/tigeropen.egg-info/SOURCES.txt` & `tigeropen-2.4.0/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

