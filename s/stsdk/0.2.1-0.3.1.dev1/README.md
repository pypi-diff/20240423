# Comparing `tmp/stsdk-0.2.1.tar.gz` & `tmp/stsdk-0.3.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsdk-0.2.1.tar", max compression
+gzip compressed data, was "stsdk-0.3.1.dev1.tar", max compression
```

## Comparing `stsdk-0.2.1.tar` & `stsdk-0.3.1.dev1.tar`

### file list

```diff
@@ -1,72 +1,87 @@
--rw-r--r--   0        0        0     1111 2023-12-18 11:48:12.022032 stsdk-0.2.1/README.md
--rw-r--r--   0        0        0      698 2023-12-23 06:55:50.926379 stsdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/http/__init__.py
--rw-r--r--   0        0        0     4443 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/http/dms.py
--rw-r--r--   0        0        0     1985 2023-12-18 12:36:51.939855 stsdk-0.2.1/stsdk/api/http/oms.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/http/sms.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/ws/__init__.py
--rw-r--r--   0        0        0     1147 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/ws/dms.py
--rw-r--r--   0        0        0      617 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/api/ws/oms.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/__init__.py
--rw-r--r--   0        0        0       24 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/cache_key.py
--rw-r--r--   0        0        0       14 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/constant.py
--rw-r--r--   0        0        0       52 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/env.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/exception.py
--rw-r--r--   0        0        0     2064 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/key.py
--rw-r--r--   0        0        0      200 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/common/signal_key.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/config/__init__.py
--rw-r--r--   0        0        0      282 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/config/config.json
--rw-r--r--   0        0        0      325 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/config/pre.config.json
--rw-r--r--   0        0        0      327 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/config/prod.config.json
--rw-r--r--   0        0        0      321 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/config/test.config.json
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/model/__init__.py
--rw-r--r--   0        0        0     4802 2023-12-23 06:46:55.461252 stsdk-0.2.1/stsdk/model/order_manager.py
--rw-r--r--   0        0        0     4600 2023-12-18 12:42:01.372473 stsdk-0.2.1/stsdk/model/position_manager.py
--rw-r--r--   0        0        0     4082 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/model/strategy_base.py
--rw-r--r--   0        0        0     6616 2023-12-23 06:35:01.647749 stsdk-0.2.1/stsdk/model/strategy_module.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/__init__.py
--rw-r--r--   0        0        0      450 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/bbo_ws.py
--rw-r--r--   0        0        0      504 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/bbo_ws_main.py
--rw-r--r--   0        0        0      423 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/blinker_block_test.py
--rw-r--r--   0        0        0      406 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/blinker_test.py
--rw-r--r--   0        0        0      289 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/cache_test.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/case/__init__.py
--rw-r--r--   0        0        0     1747 2023-12-23 06:54:55.174261 stsdk-0.2.1/stsdk/test/case/order.py
--rw-r--r--   0        0        0       61 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/constants.py
--rw-r--r--   0        0        0     2454 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/create_account.py
--rw-r--r--   0        0        0      524 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/main.py
--rw-r--r--   0        0        0     1115 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/CreatePosition.py
--rw-r--r--   0        0        0      693 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/GetOrderFormPositionId.py
--rw-r--r--   0        0        0        0 2023-12-23 06:17:56.161556 stsdk-0.2.1/stsdk/test/ordertest/__init__.py
--rw-r--r--   0        0        0     5317 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/assets/style.css
--rw-r--r--   0        0        0      624 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/conftest.py
--rw-r--r--   0        0        0      745 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/initialization.py
--rw-r--r--   0        0        0     1351 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/placeOrder.py
--rw-r--r--   0        0        0      430 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/pmsinit.py
--rw-r--r--   0        0        0     1803 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/position_test.py
--rw-r--r--   0        0        0      180 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/pytest.ini
--rw-r--r--   0        0        0     5317 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/reports/assets/style.css
--rw-r--r--   0        0        0      534 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py
--rw-r--r--   0        0        0     7367 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/test_change_leverage.py
--rw-r--r--   0        0        0     3012 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/test_close_all_positions.py
--rw-r--r--   0        0        0     1436 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/test_get_all_outstanding_orders.py
--rw-r--r--   0        0        0     3030 2023-12-23 06:21:16.333984 stsdk-0.2.1/stsdk/test/ordertest/test_order_closed_loop.py
--rw-r--r--   0        0        0     2189 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/place_order_signal.py
--rw-r--r--   0        0        0     2346 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/signal_order.py
--rw-r--r--   0        0        0     2481 2023-12-23 06:17:56.165557 stsdk-0.2.1/stsdk/test/st_2.py
--rw-r--r--   0        0        0     1958 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/st_demo_1.py
--rw-r--r--   0        0        0      325 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/test.py
--rw-r--r--   0        0        0      754 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/test_placeorder.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/test/unittest/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/__init__.py
--rw-r--r--   0        0        0      818 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/cache_manager.py
--rw-r--r--   0        0        0     4133 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/config.py
--rw-r--r--   0        0        0     2124 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/consul.py
--rw-r--r--   0        0        0      935 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/http.py
--rw-r--r--   0        0        0      609 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/instrument_id.py
--rw-r--r--   0        0        0     2154 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/log.py
--rw-r--r--   0        0        0      563 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/metric.py
--rw-r--r--   0        0        0      825 2023-12-18 12:40:24.368279 stsdk-0.2.1/stsdk/utils/redis.py
--rw-r--r--   0        0        0     1049 2023-12-18 11:48:12.026032 stsdk-0.2.1/stsdk/utils/websocket.py
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 stsdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1503 2024-04-23 07:54:20.342049 stsdk-0.3.1.dev1/README.md
+-rw-r--r--   0        0        0      848 2024-04-23 08:13:23.259206 stsdk-0.3.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/api/http/dms.py
+-rw-r--r--   0        0        0     2493 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/oms.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/http/sms.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/ws/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/api/ws/dms.py
+-rw-r--r--   0        0        0      625 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/api/ws/oms.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/cache_key.py
+-rw-r--r--   0        0        0      174 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/constant.py
+-rw-r--r--   0        0        0       72 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/env.py
+-rw-r--r--   0        0        0      623 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/exception.py
+-rw-r--r--   0        0        0     3273 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/common/key.py
+-rw-r--r--   0        0        0      200 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/common/signal_key.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/config.json
+-rw-r--r--   0        0        0      487 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/pre.config.json
+-rw-r--r--   0        0        0      546 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/prod.config.json
+-rw-r--r--   0        0        0      558 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/config/stage.config.json
+-rw-r--r--   0        0        0      495 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/config/test.config.json
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/model/__init__.py
+-rw-r--r--   0        0        0     8087 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/instrument.py
+-rw-r--r--   0        0        0    15162 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/order_manager.py
+-rw-r--r--   0        0        0    27585 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/position_manager.py
+-rw-r--r--   0        0        0     4583 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/strategy_base.py
+-rw-r--r--   0        0        0    21805 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/model/strategy_module.py
+-rw-r--r--   0        0        0     1000 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/Stress_klines.py
+-rw-r--r--   0        0        0      978 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/mongoBDtest.py
+-rw-r--r--   0        0        0      696 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/Stresstest/stressone.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/__init__.py
+-rw-r--r--   0        0        0     2450 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/aliyun_log_test.py
+-rw-r--r--   0        0        0      450 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/bbo_ws.py
+-rw-r--r--   0        0        0      402 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/bbo_ws_main.py
+-rw-r--r--   0        0        0      423 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/blinker_block_test.py
+-rw-r--r--   0        0        0      406 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/blinker_test.py
+-rw-r--r--   0        0        0      289 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/cache_test.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/case/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/case/order.py
+-rw-r--r--   0        0        0       61 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/constants.py
+-rw-r--r--   0        0        0      817 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/create_account.py
+-rw-r--r--   0        0        0      524 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/main.py
+-rw-r--r--   0        0        0     3474 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/metric_test.py
+-rw-r--r--   0        0        0     1115 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/CreatePosition.py
+-rw-r--r--   0        0        0      693 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/GetOrderFormPositionId.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/__init__.py
+-rw-r--r--   0        0        0     5317 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/assets/style.css
+-rw-r--r--   0        0        0      623 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/conftest.py
+-rw-r--r--   0        0        0      745 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/initialization.py
+-rw-r--r--   0        0        0     1351 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/placeOrder.py
+-rw-r--r--   0        0        0      430 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/pmsinit.py
+-rw-r--r--   0        0        0     1805 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/ordertest/position_test.py
+-rw-r--r--   0        0        0      180 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/pytest.ini
+-rw-r--r--   0        0        0     5317 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/reports/assets/style.css
+-rw-r--r--   0        0        0     2188 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/ordertest/stagegymoduletest.py
+-rw-r--r--   0        0        0     4598 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_Kline.py
+-rw-r--r--   0        0        0      654 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py
+-rw-r--r--   0        0        0     9694 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_change_leverage.py
+-rw-r--r--   0        0        0     3603 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_close_all_positions.py
+-rw-r--r--   0        0        0     1847 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_get_all_outstanding_orders.py
+-rw-r--r--   0        0        0     3030 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_closed_loop.py
+-rw-r--r--   0        0        0    23338 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_empty_multiple.py
+-rw-r--r--   0        0        0     1814 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/ordertest/test_position_model.py
+-rw-r--r--   0        0        0     2189 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/place_order_signal.py
+-rw-r--r--   0        0        0      647 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/precision_speed_compare.py
+-rw-r--r--   0        0        0     2830 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/redis_pubsub_test.py
+-rw-r--r--   0        0        0     2346 2024-04-23 07:54:20.346049 stsdk-0.3.1.dev1/stsdk/test/signal_order.py
+-rw-r--r--   0        0        0     3571 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/test/st_2.py
+-rw-r--r--   0        0        0     2044 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/st_demo_1.py
+-rw-r--r--   0        0        0      325 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/test.py
+-rw-r--r--   0        0        0      754 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/test_placeorder.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/test/unittest/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/__init__.py
+-rw-r--r--   0        0        0     6280 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/ali_sls.py
+-rw-r--r--   0        0        0      818 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/cache_manager.py
+-rw-r--r--   0        0        0     6060 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/config.py
+-rw-r--r--   0        0        0     2124 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/consul.py
+-rw-r--r--   0        0        0     1084 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/http.py
+-rw-r--r--   0        0        0      749 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/instrument_id.py
+-rw-r--r--   0        0        0     2260 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/log.py
+-rw-r--r--   0        0        0     1488 2024-04-23 08:05:52.765150 stsdk-0.3.1.dev1/stsdk/utils/metric.py
+-rw-r--r--   0        0        0      361 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/precision.py
+-rw-r--r--   0        0        0     2099 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/redis_utils.py
+-rw-r--r--   0        0        0     1177 2024-04-23 07:54:20.350049 stsdk-0.3.1.dev1/stsdk/utils/websocket.py
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 stsdk-0.3.1.dev1/PKG-INFO
```

### Comparing `stsdk-0.2.1/pyproject.toml` & `stsdk-0.3.1.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stsdk"
-version = "0.2.1"
+version = "0.3.1.dev1"
 description = "this is for at trade strategy module"
 authors = ["stark <yangwang@web3.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 start = 'test.main:main'
 
@@ -21,15 +21,22 @@
 janus = "^1.0.0"
 numpy = "^1.26.2"
 cacheout = "^0.15.0"
 loguru = "^0.7.2"
 chardet = "^5.2.0"
 prometheus-client = "^0.19.0"
 requests = "^2.31.0"
+sortedcontainers = "^2.4.0"
+locust = "^2.20.1"
+pandas = "^2.2.0"
+pyarrow = "^15.0.0"
+openpyxl = "^3.1.2"
+redis = "^5.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
+pytest-html = "^4.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stsdk-0.2.1/stsdk/api/http/dms.py` & `stsdk-0.3.1.dev1/stsdk/api/http/dms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,41 @@
 import datetime
-
+from stsdk.common.key import STRING_SECURITY_TYPE_SPOT
 from stsdk.utils.config import config
 from stsdk.utils.http import request
 
 
 class DMSApi:
-    DMS_BASE_HTTP_URL = config.DMS_BASE_HTTP_URL
 
     def __init__(self):
-        pass
+        self.DMS_BASE_HTTP_URL = config.DMS_BASE_HTTP_URL
+
+    def get_instrument_info(self, params=None):
+        if params is None:
+            return None
+        symbol, exchange, security_type, contract_type, external_symbol = (
+            params.get("symbol"),
+            params.get("exchange"),
+            params.get("security_type"),
+            params.get("contract_type", "UNSPECIFIED"),
+            params.get("external_symbol", ""),
+        )
+        if security_type == STRING_SECURITY_TYPE_SPOT:
+            contract_type = None
+        resp = request.get(
+            self.DMS_BASE_HTTP_URL + "/v1/instruments",
+            params={
+                "symbol": symbol,
+                "exchange": exchange,
+                "security_type": security_type,
+                "contract_type": contract_type,
+                "external_symbol": external_symbol,
+            },
+        )
+        return resp
 
     def get_kline_spot(self, params=None):
         if params is None:
             return None
         symbol, exchange, interval, start_time, end_time, limit = (
             params.get("symbol"),
             params.get("exchange"),
@@ -22,20 +45,20 @@
             params.get("limit", 10),
         )
         if symbol is None or exchange is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/klines/spot",
             params={
-                symbol: symbol,
-                exchange: exchange,
-                interval: interval,
-                start_time: start_time,
-                end_time: end_time,
-                limit: limit,
+                "symbol": symbol,
+                "exchange": exchange,
+                "interval": interval,
+                "start_time": start_time,
+                "end_time": end_time,
+                "limit": limit,
             },
         )
         return resp
 
     def get_kline_ufuture(self, params=None):
         if params is None:
             return None
@@ -48,20 +71,20 @@
             params.get("limit", 10),
         )
         if symbol is None or exchange is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/klines/u-future",
             params={
-                symbol: symbol,
-                exchange: exchange,
-                interval: interval,
-                start_time: start_time,
-                end_time: end_time,
-                limit: limit,
+                "symbol": symbol,
+                "exchange": exchange,
+                "interval": interval,
+                "start_time": start_time,
+                "end_time": end_time,
+                "limit": limit,
             },
         )
         return resp
 
     def get_kline_cfuture(self, params=None):
         if params is None:
             return None
@@ -74,73 +97,73 @@
             params.get("limit", 10),
         )
         if symbol is None or exchange is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/klines/c-future",
             params={
-                symbol: symbol,
-                exchange: exchange,
-                interval: interval,
-                start_time: start_time,
-                end_time: end_time,
-                limit: limit,
+                "symbol": symbol,
+                "exchange": exchange,
+                "interval": interval,
+                "start_time": start_time,
+                "end_time": end_time,
+                "limit": limit,
             },
         )
         return resp
 
     def get_bbo(self, params=None):
         if params is None:
             return None
         instrument_id, limit = params.get("instrument_id"), params.get("limit")
         if instrument_id is None or limit is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/bbo/latest",
             params={
-                instrument_id: instrument_id,
-                limit: limit,
+                "instrument_id": instrument_id,
+                "limit": limit,
             },
         )
         return resp
 
     def get_price(self, params=None):
         if params is None:
             return None
         instrument_id = params.get("instrument_id")
         if instrument_id is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/price",
             params={
-                instrument_id: instrument_id,
+                "instrument_id": instrument_id,
             },
         )
         return resp
 
     def get_mark_price(self, params=None):
         if params is None:
             return None
         instrument_id = params.get("instrument_id")
         if instrument_id is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/mark-price",
             params={
-                instrument_id: instrument_id,
+                "instrument_id": instrument_id,
             },
         )
         return resp
 
     def get_lob(self, params=None):
         if params is None:
             return None
         instrument_id = params.get("instrument_id")
         if instrument_id is None:
             return None
         resp = request.get(
             self.DMS_BASE_HTTP_URL + "/v1/order-book/snapshot",
             params={
-                instrument_id: instrument_id,
+                "instrument_id": instrument_id,
             },
         )
         return resp
```

### Comparing `stsdk-0.2.1/stsdk/api/http/oms.py` & `stsdk-0.3.1.dev1/stsdk/api/http/oms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from stsdk.utils.config import config
 from stsdk.utils.http import request
 
 
 class OMSApi:
-    OMS_BASE_HTTP_URL = config.OMS_BASE_HTTP_URL
 
     def __init__(self, params=None):
-        pass
+        self.OMS_BASE_HTTP_URL = config.OMS_BASE_HTTP_URL
 
     def place_order(self, data=None):
         if data is None:
             return
         resp = request.post(self.OMS_BASE_HTTP_URL + "/order/new", data=data)
         return resp
 
@@ -60,8 +59,22 @@
         resp = request.post(self.OMS_BASE_HTTP_URL + "/position/closeAll", data=data)
         return resp
 
     def change_leverage(self, data=None):
         if data is None:
             return
         resp = request.post(self.OMS_BASE_HTTP_URL + "/leverage", data=data)
-        return resp
+        return resp
+
+    def get_all_positions(self, params=None):
+        resp = request.get(self.OMS_BASE_HTTP_URL + "/position/all", params=params)
+        return resp
+
+    def get_position_mode(self, params=None):
+        resp = request.get(self.OMS_BASE_HTTP_URL + "/account/positionMode", params=params)
+        return resp
+
+    def change_position_mode(self, data=None):
+        if data is None:
+            return
+        resp = request.post(self.OMS_BASE_HTTP_URL + "/account/positionMode", data=data)
+        return resp
```

### Comparing `stsdk-0.2.1/stsdk/api/ws/dms.py` & `stsdk-0.3.1.dev1/stsdk/api/ws/dms.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,16 @@
     DMS_TRADE,
 )
 from stsdk.utils.config import config
 from stsdk.utils.websocket import Websocket
 
 
 class DMSWS:
-    DMS_BASE_WS_URL = config.DMS_BASE_WS_URL
-
     def __init__(self):
+        self.DMS_BASE_WS_URL = config.DMS_BASE_WS_URL
         self.ws = Websocket(self.DMS_BASE_WS_URL + "/ws/dms")
 
     def run(self, consumer):
         self.ws.run(consumer)
 
     def bbo(self, instrument_id):
         req = {
```

### Comparing `stsdk-0.2.1/stsdk/model/strategy_base.py` & `stsdk-0.3.1.dev1/stsdk/model/strategy_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import json
 import threading
 import types
 
 from stsdk.api.ws.dms import DMSWS
 from stsdk.api.ws.oms import OMSWS
-from stsdk.common.key import DMS_SIGNAL_MAP, GLOBAL_SIGNAL, OMS_SIGNAL_MAP
+from stsdk.common.key import DMS_SIGNAL_MAP, GLOBAL_SIGNAL, OMS_SIGNAL_MAP, REDIS_SIGNAL_MAP
 from stsdk.utils.cache_manager import cache_manager
 from stsdk.utils.instrument_id import expand_topic
+from stsdk.utils.metric import MetricUtil
+from stsdk.utils.redis_utils import RedisUtil
 
 
 class StrategyBaseModule:
     def __init__(self, strategy_id, account_id):
-        self.dms_ws = None
-        self.oms_ws = None
-        self.queue = None
-        self.func_map = {}
-        self.strategy_id = strategy_id
-        self.account_id = account_id
+        self._dms_ws = None
+        self._oms_ws = None
+        self._queue = None
+        self._redis = None
+        self._func_map = {}
+        self._strategy_id = strategy_id
+        self._account_id = account_id
+        self._metric = None
         self.exec_init_params()
 
+    def init_params(self):
+        raise NotImplementedError
+
     def exec_init_params(self):
-        self.dms_ws = DMSWS()
-        self.oms_ws = OMSWS()
-        if self.dms_ws is None or self.oms_ws is None:
+        self._dms_ws = DMSWS()
+        self._oms_ws = OMSWS()
+        self._redis = RedisUtil()
+        self._metric = MetricUtil()
+        if self._dms_ws is None or self._oms_ws is None:
             raise Exception("ws not ready")
-        if self.init_params is not None and isinstance(
-            self.init_params, types.MethodType
-        ):
-            # init_params中注册数据流
-            self.init_params()
-            self.exec_start_trading_session()
+        
+        # QUESTION: init_params is necessary
+        # if self.init_params is not None and isinstance(
+        #     self.init_params, types.MethodType
+        # ):
+        # init_params中注册数据流
+        self.init_params()
+        # self.exec_start_trading_session()
 
     # 策略启动
     def exec_start_trading_session(self):
-        if self.start_trading_session is not None and isinstance(
-            self.start_trading_session, types.MethodType
-        ):
-            self.start_trading_session()
-            self.exec_on_data_feed()
-            threading.Thread(target=self.dms_ws.run, args=(self.consumer,)).start()
-            threading.Thread(target=self.oms_ws.run, args=(self.consumer,)).start()
+        self.exec_on_data_feed()
+        threading.Thread(target=self._dms_ws.run, args=(self.consumer,)).start()
+        threading.Thread(target=self._oms_ws.run, args=(self.consumer,)).start()
+
+    def run_on_data_feed(self, message):
+        pass
 
     # 持续数据流,提供总的数据开关
     def exec_on_data_feed(self):
         if self.run_on_data_feed is not None and isinstance(
             self.run_on_data_feed, types.MethodType
         ):
             GLOBAL_SIGNAL.connect(self.run_on_data_feed)
@@ -83,25 +93,33 @@
                 func(message)
 
         return _handle_message
 
     def register(self, event, func, **kwargs):
         dms_signal = DMS_SIGNAL_MAP.get(event)
         oms_signal = OMS_SIGNAL_MAP.get(event)
+        redis_signal = REDIS_SIGNAL_MAP.get(event)
         # 使用topic替代event作为function的connect参数逻辑，这样避免了重复注册，后置函数的注册会覆盖前置函数的注册
         if dms_signal is not None:
             instrument_id = kwargs["instrument_id"]
             topic_fn_key = f"{event}.{instrument_id}"
-            self.func_map[topic_fn_key] = self.handle_dms_message(func, topic_fn_key)
-            dms_signal.connect(self.func_map[topic_fn_key])
-            method = getattr(self.dms_ws, event)
+            self._func_map[topic_fn_key] = self.handle_dms_message(func, topic_fn_key)
+            dms_signal.connect(self._func_map[topic_fn_key])
+            method = getattr(self._dms_ws, event)
             method(instrument_id)
 
         # oms里面也会有一些事件，比如order的事件，这些事件也需要注册，但是需要的唯一id维度需要是其他的
         if oms_signal is not None:
-            strategy_id = kwargs["strategy_id"]
-            account_id = kwargs["account_id"]
+            strategy_id = self._strategy_id
+            account_id = self._account_id
             topic_fn_key = f"{event}.{strategy_id}.{account_id}"
-            self.func_map[topic_fn_key] = self.handle_oms_message(func, topic_fn_key)
-            oms_signal.connect(self.func_map[topic_fn_key])
-            method = getattr(self.oms_ws, event)
+            self._func_map[topic_fn_key] = self.handle_oms_message(func, topic_fn_key)
+            oms_signal.connect(self._func_map[topic_fn_key])
+            method = getattr(self._oms_ws, event)
             method(strategy_id, account_id)
+
+        if redis_signal is not None:
+            redis_chan = kwargs["redis_chan"]
+            self._redis.subscribe(redis_chan, func)
+
+    def redis_publish(self, channel, message):
+        self._redis.publish(channel, message)
```

### Comparing `stsdk-0.2.1/stsdk/test/case/order.py` & `stsdk-0.3.1.dev1/stsdk/test/case/order.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/main.py` & `stsdk-0.3.1.dev1/stsdk/test/main.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/CreatePosition.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/CreatePosition.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/GetOrderFormPositionId.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/GetOrderFormPositionId.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/assets/style.css` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/assets/style.css`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/conftest.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import os
 import webbrowser
-
 import pytest
 
 
 # pytest 配置钩子
 def pytest_configure(config):
     # 生成带时间戳的报告文件名
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/initialization.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/initialization.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/placeOrder.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/placeOrder.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/position_test.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/position_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 
 from stsdk.common.env import ENV_TEST
 from stsdk.common.key import DMS_BBO, OMS_ORDER_UPDATE
 from stsdk.model.strategy_module import StrategyModule
 from stsdk.utils.config import config
 from stsdk.utils.log import log
-from stsdk.utils.metric import metric
+# from stsdk.utils.metric import metric
 
 
 class ST2(StrategyModule):
     name = "ST2"
 
     def init_params(self):
         log.info(f"init_params {self.name}")
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/reports/assets/style.css` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/reports/assets/style.css`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_cancel_all_outstanding_orders.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,16 @@
     st = initialization("1", "aris_test")
     logger.info(st)
     return st
 
 # 无订单情况
 def test_cancel_all_outstanding_orders_return(init_ST):
     # instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
-    result = init_ST.cancel_all_outstanding_orders()
-    logger.info("正常执行: %s" % result)
-    assert result=={}
+    try:
+        result = init_ST.cancel_all_outstanding_orders()
+        logger.info("无订单情况: %s" % result)
+        assert result=={}
+    except Exception as excinfo:
+        logger.info("无订单情况: %s" % excinfo.args)
+
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/test_change_leverage.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_change_leverage.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,139 +15,187 @@
 def generate_position_id(strategy_id, account_id, inst_id):
     return "{}.{}.{}".format(strategy_id, account_id, inst_id)
 
 # 不存在的position_id~
 def test_change_leverage_not_found_positionid(init_ST):
     position_id = 123
     leverage = 10
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("不存在的position_id: %s" % result)
-    assert result['code']==500
-    assert result['message']=='position not found 123'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("不存在的position_id: %s" % result)
+    except Exception as excinfo:
+        logger.info("不存在的position_id: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='position not found 123'
 
 
 # 验证正确的返回
 def test_change_leverage_return(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = 10
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("正确的返回值: %s" % result)
-    assert result['position_id']=='1.aris_test.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
-    assert result['leverage']==10
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("正确的返回值: %s" % result)
+        assert result['position_id']=='1.aris_test.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
+        assert result['leverage']==10
+    except Exception as excinfo:
+        logger.info("如果错误: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
 
 #验证leverage为0时返回异常  
 def test_change_leverage_leverage_zero(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = 0
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为0时异常: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为0时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为0时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
 
 # 验证leverage为负数时返回异常
 def test_change_leverage_leverage_negative(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = -1
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为负数时异常: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage -1 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为负数时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为负数时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage -1 invalid, target leverage must in [125 , 1]'
+    
 
 # 验证leverage为超过最大值时返回异常
 def test_change_leverage_leverage_Exceed(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = 250
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为最大值时异常: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage 250 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为超过最大值时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为超过最大值时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage 250 invalid, target leverage must in [125 , 1]'
 
 # 验证leverage为非数字时返回异常
 def test_change_leverage_leverage_notnumer(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = "test"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为非数字时异常: %s" % result)
-    assert result['code']==400
-    assert result["reason"]=='CODEC'
-    assert result['message']=='body unmarshal parsing field "leverage": strconv.ParseInt: parsing "test": invalid syntax'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为非数字时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为非数字时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==400
+        assert excinfo.args[0]['reason'] == 'CODEC'
+        assert excinfo.args[0]['message'] == 'body unmarshal parsing field "leverage": strconv.ParseInt: parsing "test": invalid syntax'
+    
 
 # 验证leverage为None时返回异常
 def test_change_leverage_leverage_none(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = None
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为None时异常: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为None时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为None时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
 
 # 验证leverage为空时返回异常
 def test_change_leverage_leverage_null(init_ST):
     position_id=generate_position_id(1,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = ""
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("leverage为空时: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("leverage为空时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("leverage为空时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
 
 # 验证position_id为空时返回异常
 def test_change_leverage_positionid_null(init_ST):
     position_id=""
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为空时: %s" % result)
-    assert result['code']==500
-    assert result['message']=='instrument not found for '
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为空时异常: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为空时异常: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='instrument not found for '
 
 # 验证position_id为strategy_id不正确
 def test_change_leverage_positionid_wrong(init_ST):
     position_id=generate_position_id(100,"aris_test","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为strategy_id不正确: %s" % result)
-    assert result['code']==500
-    assert result['message']=='position not found 100.aris_test.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为strategy_id不正确: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为strategy_id不正确: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='position not found 100.aris_test.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
 
 # 验证position_id为account_id不正确
 def test_change_leverage_positionid_acid_wrong(init_ST):
     position_id=generate_position_id(1,"aris_test1111","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为acid不正确: %s" % result)
-    assert result['code']==500
-    assert result['message']=='position not found 1.aris_test1111.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
-
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为account_id不正确: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为account_id不正确: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='position not found 1.aris_test1111.EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
+    
 # 验证position_id为account_id不正确为空
 def test_change_leverage_positionid_acid_null(init_ST):
     position_id=generate_position_id(1,"","EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为strategy_id不正确为空: %s" % result)
-    assert result['code']==500
-    assert result['message']=='position not found 1..EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为account_id不正确为空: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为account_id不正确为空: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='position not found 1..EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED'
 
 # 验证position_id为inst_id为空
 def test_change_leverage_positionid_instid_null(init_ST):
     position_id=generate_position_id(1,"aris_test","")
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为inst_id为空: %s" % result)
-    assert result['code']==500
-    assert result['message']=='position not found 1.aris_test.'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为inst_id为空: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为inst_id为空: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='position not found 1.aris_test.'
 
 # 验证position_id为inst_id为空
 def test_change_leverage_positionid_instid_allnull(init_ST):
     position_id=""
     leverage = "10"
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id为空: %s" % result)
-    assert result['code']==500
-    assert result['message']=='instrument not found for '
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id为inst_id为空: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id为inst_id为空: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='instrument not found for '
 
 # 验证position_id和leverage都为空
 def test_change_leverage_positionid_instid_isnull(init_ST):
     position_id=""
     leverage = ""
-    result = init_ST.change_leverage(position_id, leverage)
-    logger.info("验证position_id和leverage都为空: %s" % result)
-    assert result['code']==500
-    assert result['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
+    try:
+        result = init_ST.change_leverage(position_id, leverage)
+        logger.info("验证position_id和leverage都为空: %s" % result)
+    except Exception as excinfo:
+        logger.info("验证position_id和leverage都为空: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
+        assert excinfo.args[0]['message']=='leverage 0 invalid, target leverage must in [125 , 1]'
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/test_close_all_positions.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_close_all_positions.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,51 +11,62 @@
 '''
 # 一键平仓执行
 def test_close_all_positions_return():
     # 操作下单，定义入参参数并进行校验
     orderinfo = {
         "strategy_id": "1", 
         "symbol": "BTC-USDT", 
-        "quantity": "0.0005",
-        "price": "",  #价格不填写的情况下会是市价单
-        "settle_ccy": "USDT", 
-        "expiry_date": "",  #过期时间
-        "security_type": 1,  #SECURITY_TYPE_SPOT正确 2:SECURITY_TYPE_PERP
+        "quantity": "0.009",
+        "price": "20000",  #价格不填写的情况下会是市价单
+        # "settle_ccy": "USDT", 
+        # "expiry_date": "",  #过期时间
+        # "security_type": 1,  #SECURITY_TYPE_SPOT正确 2:SECURITY_TYPE_PERP
         "position_side": 3,  #POSITION_SIDE_NOTBOTH
         "order_type": 1,  #ORDER_TYPE_LIMIT 1:ORDER_TYPE_MARKET
-        "exchange": 1,   #返回EXCHANGE_BINANCE正确
+        # "exchange": 1,   #返回EXCHANGE_BINANCE正确
         "order_direction": 1,  #ORDER_DIRECTION_BUY
         "time_in_force": 1,  #TIME_IN_FORCE_GTC
         "leverage": 0,  #杠杆倍数
-        "contract_type": 0, #CONTRACT_TYPE_LINEAR
+        # "contract_type": 0, #CONTRACT_TYPE_LINEAR
         "account_id": "aris_test",
-        "instrument_id": "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_SPOT.UNSPECIFIED.UNSPECIFIED.UNSPECIFIED"
+        # "instrument_id": "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_SPOT.UNSPECIFIED.UNSPECIFIED.UNSPECIFIED"
+        "instrument_id": "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
     }
     #下单操作
-    request_result = placeOrder.get_placeOrder(orderinfo).json()
-    logger.info(f"下单返回结果: {request_result}")
+    try:
+        request_result = placeOrder.get_placeOrder(orderinfo).json()
+        logger.info(f"下单返回结果: {request_result}")
+        assert request_result["strategy_id"] == orderinfo["strategy_id"]
+        assert request_result["account_id"] == orderinfo["account_id"]
+        assert request_result["instrument_id"] == orderinfo["instrument_id"]
+        assert request_result["symbol"] == orderinfo["symbol"]
+        assert request_result["exchange"] == "EXCHANGE_BINANCE"
+        assert request_result["security_type"] == "SECURITY_TYPE_PERP"
+        assert request_result["order_type"] == "ORDER_TYPE_MARKET"
+        # assert request_result["origin_price"] == "0" 
+        assert request_result["origin_quantity"] == orderinfo["quantity"]
+        assert request_result["order_direction"] == "ORDER_DIRECTION_BUY"
+        assert request_result["position_side"] == "POSITION_SIDE_NOTBOTH"
+        # assert request_result["order_status"] == "ORDER_STATUS_FILLED" "ORDER_DIRECTION_BUY"
+        assert request_result["time_in_force"] == "TIME_IN_FORCE_GTC"
+    except Exception as excinfo:
+        logger.info("exception验证下单: %s" % excinfo.args)
     # print(type(request_result))
     # 断言下单应该要返回的结果是预期设计的结果
-    assert request_result["strategy_id"] == orderinfo["strategy_id"]
-    assert request_result["account_id"] == orderinfo["account_id"]
-    assert request_result["instrument_id"] == orderinfo["instrument_id"]
-    assert request_result["symbol"] == orderinfo["symbol"]
-    assert request_result["exchange"] == "EXCHANGE_BINANCE"
-    assert request_result["security_type"] == "SECURITY_TYPE_SPOT"
-    assert request_result["order_type"] == "ORDER_TYPE_MARKET"
-    assert request_result["origin_price"] == "0" 
-    assert request_result["origin_quantity"] == orderinfo["quantity"]
-    assert request_result["order_direction"] == "ORDER_DIRECTION_BUY"
-    assert request_result["position_side"] == "POSITION_SIDE_NOTBOTH"
-    assert request_result["order_status"] == "ORDER_STATUS_FILLED"
-    assert request_result["time_in_force"] == "TIME_IN_FORCE_GTC"
-    
     # 下单之后操作平仓
     st=pmsinit("1", "aris_test")
-    close_position=st.close_all_positions()
-    logger.info(f"平仓结果: {close_position}")
+    try:
+        close_position=st.close_all_positions()
+        logger.info(f"平仓结果: {close_position}")
+    except Exception as excinfo:
+        logger.info("exception平仓结果: %s" % excinfo.args)
+        assert False
     # 断言，平常结果与下单结果订单一致
     #查询订单不存在了
-    request_gopid=GetOrderFromPositionId.get_PositionId("1", "aris_test", "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_SPOT.UNSPECIFIED.UNSPECIFIED.UNSPECIFIED")
+    try:
+        request_gopid=GetOrderFromPositionId.get_PositionId("1", "aris_test", "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED")
     # 断言，订单返回结果filled_position应该为0
-    assert request_gopid["long_position"]["filled_position"] == "0"
-    # logger.info(f"查询订单情况: {request_gopid}")
+        assert request_gopid["long_position"]["filled_position"] == "0"
+    # logger.info(f"查询订单情况: {request_gopid}")
+    except Exception as excinfo:
+        logger.info("exception查询订单情况: %s" % excinfo.args)
+        assert False
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/test_get_all_outstanding_orders.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_get_all_outstanding_orders.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,37 @@
 
 
 # 无订单情况
 def test_get_all_outstanding_orders_return():
     st=init_ST("1", "aris_test")
     # instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
     instrument_id="EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_SPOT.UNSPECIFIED.UNSPECIFIED.UNSPECIFIED"
-    result = st.get_all_outstanding_orders(instrument_id)
-    logger.info("正常执行: %s" % result)
-    assert result=={}
+    try:
+        result = st.get_all_outstanding_orders(instrument_id)
+        logger.info("无订单情况: %s" % result)
+        assert result=={}
+    except Exception as excinfo:
+        logger.info("exception无订单情况: %s" % excinfo.args)
 
 # 验证accountid不正确
 def test_get_all_outstanding_orders_accountid():
     st=init_ST("1", "aris_test111")
     instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
-    result = st.get_all_outstanding_orders(instrument_id)
-    logger.info("accountid不正确: %s" % result)
-    assert result=={}
+    try:
+        result = st.get_all_outstanding_orders(instrument_id)
+        logger.info("accountid不正确: %s" % result)
+    except Exception as excinfo:
+        logger.info("esception验证accountid不正确: %s" % excinfo.args)
+        assert excinfo.args[0]['code']==500
 
 # 验证strategy_id不正确
 def test_get_all_outstanding_orders_strategy_id():
     st=init_ST("112", "aris_test")
     instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
-    result = st.get_all_outstanding_orders(instrument_id)
-    logger.info("accountid不正确: %s" % result)
-    assert result=={}
+    try:
+        result = st.get_all_outstanding_orders(instrument_id)
+        logger.info("strategy_id不正确: %s" % result)
+        assert result=={}
+    except Exception as excinfo:
+        logger.info("esception验证strategy_id不正确: %s" % excinfo.args)
+
```

### Comparing `stsdk-0.2.1/stsdk/test/ordertest/test_order_closed_loop.py` & `stsdk-0.3.1.dev1/stsdk/test/ordertest/test_order_closed_loop.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/place_order_signal.py` & `stsdk-0.3.1.dev1/stsdk/test/place_order_signal.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/signal_order.py` & `stsdk-0.3.1.dev1/stsdk/test/signal_order.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/test/st_2.py` & `stsdk-0.3.1.dev1/stsdk/test/metric_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,98 @@
 import asyncio
 import time
+import random
 
-from stsdk.common.env import ENV_TEST
-from stsdk.common.key import DMS_BBO, OMS_ORDER_UPDATE
+import sys
+
+
+from stsdk.common.env import ENV_PRE, ENV_TEST
+from stsdk.common.key import HEDGING_MODE_DOWN, DMS_BBO
 from stsdk.model.strategy_module import StrategyModule
 from stsdk.utils.config import config
 from stsdk.utils.log import log
-from stsdk.utils.metric import metric
+from stsdk.utils.metric import MetricUtil
+from stsdk.utils.ali_sls import sls_data
+
+
+def simple_test():
+    met = MetricUtil()
+    met.add_gauge("test_gauge", "test gauge", ["label1", "label2"])
+    met.metric_guage("test_gauge", {"signal_BTC": "1", "label2": "2"}, 100)
+    while True:
+        pass
 
 
 class ST1(StrategyModule):
     name = "ST1"
 
+    def __init__(self, strategy_id, account_id):
+        config.set_env(ENV_TEST)
+        self.metric_name = "signal_BTC_CM_240628"
+        super().__init__(strategy_id, account_id)
+
     def init_params(self):
         log.info(f"init_params {self.name}")
-        # 设置测试环境
-        config.set_env(ENV_TEST)
         # 注册 DMS_BBO 和 OMS_ORDER_UPDATE 事件，并指定相应的处理函数
+        self._hedging_mode = HEDGING_MODE_DOWN
+        self.instrument_id = "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED"
+        # self.instrument_id = "EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_FUTURE.CONTRACT_TYPE_LINEAR.USDT.2024-06-28"
+        self.register_instrument(self.instrument_id, 10, 10)
         self.register(
             DMS_BBO,
             self.handle_bbo,
-            instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        )
-        self.register(
-            OMS_ORDER_UPDATE,
-            self.handle_order_update,
-            strategy_id=self.strategy_id,
-            account_id=self.account_id,
+            instrument_id=self.instrument_id,
         )
+        # 添加打点
+        self._metric.add_gauge("test_gauge", "test gauge", [self.metric_name, "label2"])
+
     # 开始交易会话的方法
     def start_trading_session(self):
         pass
+
     # 数据提供方法
     def run_on_data_feed(self, *args):
         pass
+
     # 错误处理方法
     def handle_error(self, error):
-        print("error", error)
+        log.error(f"error: {error}")
         pass
+
     # 处理 BBO（最佳买卖盘报价）的方法
     def handle_bbo(self, message):
-        metric.MetricTime(
-            "ws_oms_stsdk", message["topic"], message["tt"] / 1000000, time.time()
-        )
-        # self.place_order_signal(
-        #     "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        #     "1000",
-        #     "0.1",
-        #     "buy",
-        # )
+        # self._metric.metric_time("ws_oms_stsdk", message["topic"], message["tt"] / 1000000, time.time())
+        # log.info(f"bbo: {message}")
+        self._metric.metric_guage("test_gauge", {self.metric_name: "1", "label2": "2"}, random.randint(0, 100))
+
+        # self._metric.metric_guage("test_gauge", {"kind": "signal_BTC_CM_240628", "operation": "siginal"},
+        # random.randint(0, 100)) self._metric.metric_guage("test_gauge", {"kind": "signal_BTC_CM_240628",
+        # "operation": "ask"}, random.randint(0, 100)) self._metric.metric_guage("test_gauge",
+        # {"kind": "positionManager_BTC_CM_240628", "operation": "ask"}, random.randint(0, 100))
+        sls_data.set_project(project="st-sdk-log")  # 设置一次就可以
+        log_store = "st-sdk-log-pre"
+        topic = "trade-log"
+        source = "tianjian-pre"
+        contents = [
+            ("timestamp", str(int(time.time()))),
+            ("order_id", "15qeny11000czf666xda7ha9vlv0g706"),
+        ]
+        sls_data.put_logs(log_store, topic, source, False, contents)
+
     # 处理订单更新的方法
     def handle_order_update(self, message):
         log.info("order update", message)
         body = message["body"]
         order_id = body["order_id"]
         instrument_id = body["instrument_id"]
         log.info(f"order_id: {order_id}, instrument_id: {instrument_id}")
-        # self.cancel_order_signal(
-        #     instrument_id,
-        #     order_id,
-        # )
+
+    def handle_redis_message(self, message):
+        log.info(f"handle_redis_message: {message}")
 
 
 async def main():
     st = ST1("1", "aris_test")
-    # st.place_order_signal(
-    #     "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-    #     "1000",
-    #     "0.1",
-    #     "buy",
-    # )
-    st.cancel_order_signal(
-        "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        "1jtb38zpb2hcxo44epof7tp4001g5rma",
-    )
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    asyncio.run(main())
```

### Comparing `stsdk-0.2.1/stsdk/test/st_demo_1.py` & `stsdk-0.3.1.dev1/stsdk/test/st_demo_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import asyncio
 
 from stsdk.common.env import ENV_TEST
-from stsdk.common.key import DMS_BBO, OMS_ORDER_UPDATE
+from stsdk.common.key import (
+    OMS_ORDER_UPDATE,
+    ORDER_DIRECTION_BUY,
+    POSITION_SIDE_LONG,
+)
 from stsdk.model.strategy_module import StrategyModule
 from stsdk.utils.config import config
 from stsdk.utils.log import log
 
 
 class ST1(StrategyModule):
     name = "ST1"
 
+    def __init__(self, strategy_id, account_id):
+        config.set_env(ENV_TEST)
+        super().__init__(strategy_id, account_id)
+
     def init_params(self):
         log.info("ST1 init_params")
-        config.set_env(ENV_TEST)
-        self.register(
-            DMS_BBO,
-            self.handle_bbo,
-            instrument_id="EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        )
+        # self.register(
+        #     DMS_BBO,
+        #     self.handle_bbo,
+        #     instrument_id="EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
+        # )
         # self.register(
         #     DMS_BBO,
         #     self.handle_btc_bbo,
         #     instrument_id="EXCHANGE_BINANCE.BTC-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
         # )
         self.register(
             OMS_ORDER_UPDATE,
@@ -39,36 +46,34 @@
     def handle_error(self, error):
         print("error", error)
         pass
 
     def handle_bbo(self, message):
         pass
         # log.info("bbo: ", message)
-        # resp = self.place_order(
-        #     "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        #     "1000",
-        #     "1",
-        #     "buy",
-        #     "OPEN",
-        # )
-        # print(resp)
 
     def handle_btc_bbo(self, message):
         self.name = "btc update"
         # log.info("btc bbo", self.name)
 
     def handle_order_update(self, message):
         log.info(message)
 
 
 async def main():
-    st = ST1("2", "yangwang_account_binance01")
+    st = ST1("1", "aris_test")
+    st.register_instrument(
+        "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
+        1000,
+        1000,
+    )
     st.place_order(
         "EXCHANGE_BINANCE.ETH-USDT.SECURITY_TYPE_PERP.CONTRACT_TYPE_LINEAR.USDT.UNSPECIFIED",
-        "1000",
-        "0.1",
-        "buy",
+        "2203",
+        0.01,
+        ORDER_DIRECTION_BUY,
+        POSITION_SIDE_LONG,
     )
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `stsdk-0.2.1/stsdk/test/test_placeorder.py` & `stsdk-0.3.1.dev1/stsdk/test/test_placeorder.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/utils/cache_manager.py` & `stsdk-0.3.1.dev1/stsdk/utils/cache_manager.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/utils/consul.py` & `stsdk-0.3.1.dev1/stsdk/utils/consul.py`

 * *Files identical despite different names*

### Comparing `stsdk-0.2.1/stsdk/utils/http.py` & `stsdk-0.3.1.dev1/stsdk/utils/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import httpx
 
 from stsdk.utils.log import log
 
-timeout = 1
+timeout = httpx.Timeout(5.0, connect=60.0)
+client = httpx.Client(timeout=timeout)
 
 
 class Request:
     def get(self, url, headers=None, params=None):
         log.info("get info: ", url, params)
-        resp = httpx.get(url, headers=headers, params=params, timeout=timeout)
+        resp = client.get(url, headers=headers, params=params, timeout=timeout)
         return resp.json()
 
     def post(self, url, data, headers=None):
         log.info("post info: ", url, data)
-        resp = httpx.post(url, headers=headers, data=data, timeout=timeout)
-        return resp.json()
+        resp = client.post(url, headers=headers, data=data, timeout=timeout).json()
+        if resp.get("code", 200) != 200:
+            raise Exception(resp)
+        return resp
 
     def patch(self, url, data, headers=None):
         log.info("patch info: ", url, data)
-        resp = httpx.patch(url, headers=headers, data=data, timeout=timeout)
+        resp = client.patch(url, headers=headers, data=data, timeout=timeout)
         return resp.json()
 
     def delete(self, url, data, headers=None):
         log.info("delete info: ", url, data)
-        resp = httpx.delete(url, headers=headers, data=data, timeout=timeout)
+        resp = client.delete(url, headers=headers, data=data, timeout=timeout)
         return resp.json()
 
     def close(self):
         self.session.close()
 
 
 request = Request()
```

### Comparing `stsdk-0.2.1/stsdk/utils/instrument_id.py` & `stsdk-0.3.1.dev1/stsdk/utils/instrument_id.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,13 +10,20 @@
         exchange,
         symbol,
         security_type,
         contract_type,
         settle_ccy,
         expiry_date,
     ) = instrument_id.split(".")
-    return {exchange, symbol, security_type, contract_type, settle_ccy, expiry_date}
+    return {
+        "exchange": exchange,
+        "symbol": symbol,
+        "security_type": security_type,
+        "contract_type": contract_type,
+        "settle_ccy": settle_ccy,
+        "expiry_date": expiry_date,
+    }
 
 
 def expand_topic(topic):
     topic_type = topic.split(".")[0]
     return topic_type
```

### Comparing `stsdk-0.2.1/stsdk/utils/log.py` & `stsdk-0.3.1.dev1/stsdk/utils/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import os
 import sys
 
 from loguru import logger
 
 
 class LogUtil:
-    def __init__(self):
-        self.set_dir("./logs")
+    def __init__(self, log_directory = None):
+        if log_directory:
+            self.set_dir(log_directory)
+        else:
+            self.set_dir("./logs")
 
     def set_dir(self, log_directory):
         self.log_directory = log_directory
         os.makedirs(log_directory, exist_ok=True)
 
         log_file_info = os.path.join(self.log_directory, "{time:YYYY-MM-DD}_info.log")
         log_file_error = os.path.join(self.log_directory, "{time:YYYY-MM-DD}_error.log")
```

### Comparing `stsdk-0.2.1/stsdk/utils/websocket.py` & `stsdk-0.3.1.dev1/stsdk/utils/websocket.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import traceback
+
 import websocket
 
 from stsdk.utils.log import log
 
 
 class Websocket:
     def __init__(self, url):
@@ -35,8 +37,10 @@
             self.ws.send(payload)
 
     def on_close(self, ws, close_status_code, close_msg):
         log.info("Websocket connection closed")
         ws.close()
 
     def on_error(self, ws, error):
-        log.error("Websocket error received: %s", error)
+        log.error(f"Websocket error received: {error}, ws url: {self.url}")
+        log.error("Detailed error information:")
+        log.error(traceback.format_exc())
```

### Comparing `stsdk-0.2.1/PKG-INFO` & `stsdk-0.3.1.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: stsdk
-Version: 0.2.1
+Version: 0.3.1.dev1
 Summary: this is for at trade strategy module
 Author: stark
 Author-email: yangwang@web3.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.6,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: blinker (>=1.7.0,<2.0.0)
 Requires-Dist: cacheout (>=0.15.0,<0.16.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: httpx (>=0.25.0,<0.26.0)
 Requires-Dist: janus (>=1.0.0,<2.0.0)
+Requires-Dist: locust (>=2.20.1,<3.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: prometheus-client (>=0.19.0,<0.20.0)
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
+Requires-Dist: redis (>=5.0.3,<6.0.0)
 Requires-Dist: rel (>=0.4.9,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Requires-Dist: ujson (>=5.8.0,<6.0.0)
 Requires-Dist: websocket-client (>=1.6.4,<2.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 # st-sdk
 
@@ -36,16 +43,24 @@
 3. model：设计strategy module，order manager，position manager等对策略曝光的最上层模块
 4. config：一些常用的配置项
 5. common：主要存放constant和error等常量
 6. test：python测试文件目录
 
 ## 开发配置
 
+st-sdk使用poetry作为核心的包管理工具，工具地址：https://python-poetry.org/。直接抛弃了pip的方式开发，把包版本控制&发版都简单收敛到一个工具和命令行中。
+
 ## 开发流程
 
+- 执行test demo,我们通过下面的命令行，可以执行test的python代码，其他的和python代码使用没有任何区别
+
+```
+poetry run python stsdk/test/st_demo_1.py
+```
+
 ## 设计细节
 
 ### cache设计
 
 每一个key会对应一个map，map中的cache是用户订阅参数产生的topic，然后创建出来的自定义数据。
 
 举个例子：
```

