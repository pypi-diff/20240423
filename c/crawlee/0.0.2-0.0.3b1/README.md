# Comparing `tmp/crawlee-0.0.2.tar.gz` & `tmp/crawlee-0.0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.2.tar", max compression
+gzip compressed data, was "crawlee-0.0.3b1.tar", max compression
```

## Comparing `crawlee-0.0.2.tar` & `crawlee-0.0.3b1.tar`

### file list

```diff
@@ -1,65 +1,77 @@
--rw-r--r--   0        0        0    11355 2024-01-15 10:43:27.602910 crawlee-0.0.2/LICENSE
--rw-r--r--   0        0        0       17 2024-01-14 07:30:15.307605 crawlee-0.0.2/README.md
--rw-r--r--   0        0        0     5913 2024-04-11 07:59:00.206388 crawlee-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 16:55:10.812444 crawlee-0.0.2/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.269919 crawlee-0.0.2/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3376 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     2056 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-03-08 15:21:38.269919 crawlee-0.0.2/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1835 2024-03-08 15:28:15.522918 crawlee-0.0.2/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.270919 crawlee-0.0.2/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15881 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9174 2024-03-18 16:55:10.813444 crawlee-0.0.2/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      186 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    12621 2024-04-10 16:34:23.951009 crawlee-0.0.2/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4026 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2279 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0      420 2024-04-10 16:02:45.061422 crawlee-0.0.2/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0     1245 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/configuration.py
--rw-r--r--   0        0        0       91 2024-04-10 13:42:23.139187 crawlee-0.0.2/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7169 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     3004 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.2/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1264 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/types.py
--rw-r--r--   0        0        0       38 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2481 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      261 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-03-30 20:24:08.426839 crawlee-0.0.2/src/crawlee/log_config.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.2/src/crawlee/py.typed
--rw-r--r--   0        0        0     5512 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/request.py
--rw-r--r--   0        0        0      365 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/__init__.py
--rw-r--r--   0        0        0     5693 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/base_resource_client.py
--rw-r--r--   0        0        0     3436 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/base_resource_collection_client.py
--rw-r--r--   0        0        0    19760 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/dataset_client.py
--rw-r--r--   0        0        0     1545 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/dataset_collection_client.py
--rw-r--r--   0        0        0    20509 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_client.py
--rw-r--r--   0        0        0     1660 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_collection_client.py
--rw-r--r--   0        0        0        0 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/py.typed
--rw-r--r--   0        0        0    22531 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/request_queue_client.py
--rw-r--r--   0        0        0     1635 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/request_queue_collection_client.py
--rw-r--r--   0        0        0     1645 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      106 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/__init__.py
--rw-r--r--   0        0        0     1577 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/base_storage_client.py
--rw-r--r--   0        0        0    11486 2024-04-08 10:23:01.757507 crawlee-0.0.2/src/crawlee/storage_clients/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/py.typed
--rw-r--r--   0        0        0      150 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7240 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15488 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     5123 2024-04-11 07:59:09.551307 crawlee-0.0.2/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0        0 2024-04-04 15:33:46.944733 crawlee-0.0.2/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2611 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2741 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25804 2024-04-10 16:39:44.067022 crawlee-0.0.2/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0     3989 2024-04-10 08:51:04.116008 crawlee-0.0.2/src/crawlee/storages/types.py
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 crawlee-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-01-15 10:43:27.602910 crawlee-0.0.3b1/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-15 12:48:32.824597 crawlee-0.0.3b1/README.md
+-rw-r--r--   0        0        0     6331 2024-04-23 12:46:22.947137 crawlee-0.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 16:55:10.812444 crawlee-0.0.3b1/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.269919 crawlee-0.0.3b1/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-05 11:38:44.800791 crawlee-0.0.3b1/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-04-04 15:33:46.940733 crawlee-0.0.3b1/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-04-18 12:13:47.123107 crawlee-0.0.3b1/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-04-04 15:33:46.940733 crawlee-0.0.3b1/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-04-12 12:50:54.784754 crawlee-0.0.3b1/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     2056 2024-04-04 15:33:46.941733 crawlee-0.0.3b1/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-04-18 13:24:49.427217 crawlee-0.0.3b1/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-03-08 15:21:38.269919 crawlee-0.0.3b1/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1585 2024-04-12 12:51:35.336347 crawlee-0.0.3b1/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-04-04 15:33:46.941733 crawlee-0.0.3b1/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-04-05 11:38:44.800791 crawlee-0.0.3b1/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.270919 crawlee-0.0.3b1/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-04-18 14:10:07.138207 crawlee-0.0.3b1/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      186 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    14678 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     5315 2024-04-18 10:29:13.253131 crawlee-0.0.3b1/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2279 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0      815 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-04-18 10:29:13.253131 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     4017 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      462 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1246 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/configuration.py
+-rw-r--r--   0        0        0       91 2024-04-10 13:42:23.139187 crawlee-0.0.3b1/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2683 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.3b1/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     2031 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       38 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-04-17 08:37:58.250881 crawlee-0.0.3b1/src/crawlee/log_config.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.3b1/src/crawlee/py.typed
+-rw-r--r--   0        0        0     5506 2024-04-22 09:41:15.792175 crawlee-0.0.3b1/src/crawlee/request.py
+-rw-r--r--   0        0        0      365 2024-04-22 10:45:11.357161 crawlee-0.0.3b1/src/crawlee/resource_clients/__init__.py
+-rw-r--r--   0        0        0     5687 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_client.py
+-rw-r--r--   0        0        0     2980 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0        0        0    19714 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_client.py
+-rw-r--r--   0        0        0     1819 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_collection_client.py
+-rw-r--r--   0        0        0    20474 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_client.py
+-rw-r--r--   0        0        0     1936 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_collection_client.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:34:17.118301 crawlee-0.0.3b1/src/crawlee/resource_clients/py.typed
+-rw-r--r--   0        0        0    22426 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_client.py
+-rw-r--r--   0        0        0     1912 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_collection_client.py
+-rw-r--r--   0        0        0       67 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8155 2024-04-16 07:53:19.412180 crawlee-0.0.3b1/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-04-15 15:12:32.447960 crawlee-0.0.3b1/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0     1645 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      106 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/base_storage_client.py
+-rw-r--r--   0        0        0    11477 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/py.typed
+-rw-r--r--   0        0        0      150 2024-04-10 08:51:04.115008 crawlee-0.0.3b1/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7600 2024-04-18 18:02:48.825221 crawlee-0.0.3b1/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15526 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4999 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0     6489 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/models.py
+-rw-r--r--   0        0        0        0 2024-04-04 15:33:46.944733 crawlee-0.0.3b1/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2611 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2742 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25845 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-04-18 12:13:47.126107 crawlee-0.0.3b1/src/crawlee/types.py
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 crawlee-0.0.3b1/PKG-INFO
```

### Comparing `crawlee-0.0.2/LICENSE` & `crawlee-0.0.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/pyproject.toml` & `crawlee-0.0.3b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.2"
+version = "0.0.3b1"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -43,23 +43,27 @@
 # We use inclusive ordered comparison clauses for external packages intentionally in order to enhance Crawlee's
 # compatibility with external packages. This decision was discussed in detail in the following PR:
 # https://github.com/apify/apify-sdk-python/pull/154.
 [tool.poetry.dependencies]
 python = "^3.9"
 aiofiles = "^23.2.1"
 aioshutil = "^1.3"
+beautifulsoup4 = { version = "^4.12.3", optional = true }
 colorama = "^0.4.6"
-docutils = "^0.20.1" # HACK - prevent poetry from resolving version to 0.21.post1 which does not exist
-eval-type-backport = "^0.1.3"
+docutils = "^0.21.0"
+eval-type-backport = "^0.2.0"
+html5lib = { version = "^1.1", optional = true }
 httpx = "^0.27.0"
+lxml = { version = "^5.2.1", optional = true }
 more_itertools = "^10.2.0"
 psutil = "^5.9.8"
 pydantic = "^2.6.3"
 pydantic-settings = "^2.2.1"
 pyee = "^11.1.0"
+python-dateutil = "^2.9.0"
 sortedcollections = "^2.1.0"
 typing-extensions = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 build = "~1.2.0"
 filelock = "~3.13.1"
 mypy = "~1.9.0"
@@ -68,19 +72,23 @@
 pytest = "~8.1.0"
 pytest-asyncio = "~0.23.5"
 pytest-cov = "~5.0.0"
 pytest-only = "~2.1.0"
 pytest-timeout = "~2.3.0"
 pytest-xdist = "~3.5.0"
 respx = "~0.21.0"
-ruff = "~0.3.0"
-twine = "~5.0.0"
+ruff = "~0.4.0"
 types-aiofiles = "^23.2.0.20240106"
+types-beautifulsoup4 = "^4.12.0.20240229"
 types-colorama = "~0.4.15.20240106"
 types-psutil = "~5.9.5.20240205"
+types-python-dateutil = "^2.9.0.20240316"
+
+[tool.poetry.extras]
+beautifulsoup = ["beautifulsoup4", "lxml", "html5lib"]
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
@@ -138,14 +146,17 @@
     "TRY301",  # Abstract `raise` to an inner function
 ]
 
 [tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "single"
 
+[tool.ruff.lint.flake8-builtins]
+builtins-ignorelist = ["id"]
+
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.isort]
 known-local-folder = ["crawlee"]
 
 [tool.ruff.lint.pylint]
@@ -154,14 +165,15 @@
 [tool.pytest.ini_options]
 addopts = "-ra"
 asyncio_mode = "auto"
 timeout = 1200
 
 [tool.mypy]
 python_version = "3.9"
+plugins = ["pydantic.mypy"]
 files = ["scripts", "src", "tests"]
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
 disallow_untyped_defs = true
 no_implicit_optional = true
@@ -171,7 +183,10 @@
 warn_unused_ignores = true
 
 [tool.mypy-scrapy]
 ignore_missing_imports = true
 
 [tool.mypy-sortedcollections]
 ignore_missing_imports = true
+
+[tool.coverage.report]
+exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
```

### Comparing `crawlee-0.0.2/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.3b1/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/crypto.py` & `crawlee-0.0.3b1/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.3b1/src/crawlee/_utils/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime, timezone
 from enum import Enum
 from typing import TYPE_CHECKING, Any, NoReturn
 
 from crawlee._utils.file import ContentType, is_content_type
 
 if TYPE_CHECKING:
-    from crawlee.storages.types import StorageTypes
+    from crawlee.types import StorageTypes
 
 
 def filter_out_none_values_recursively(dictionary: dict, *, remove_empty_dicts: bool = False) -> dict | None:
     """Recursively filters out None values from a dictionary.
 
     Args:
         dictionary: The dictionary to filter.
@@ -89,11 +89,11 @@
 
 def raise_on_duplicate_storage(client_type: StorageTypes, key_name: str, value: str) -> NoReturn:
     """Raise an error indicating that a storage with the provided key name and value already exists."""
     client_type = maybe_extract_enum_member_value(client_type)
     raise ValueError(f'{client_type} with {key_name} "{value}" already exists.')
 
 
-def raise_on_non_existing_storage(client_type: StorageTypes, id_: str | None) -> NoReturn:
+def raise_on_non_existing_storage(client_type: StorageTypes, id: str | None) -> NoReturn:
     """Raise an error indicating that a storage with the provided id does not exist."""
     client_type = maybe_extract_enum_member_value(client_type)
-    raise ValueError(f'{client_type} with id "{id_}" does not exist.')
+    raise ValueError(f'{client_type} with id "{id}" does not exist.')
```

### Comparing `crawlee-0.0.2/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.3b1/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/file.py` & `crawlee-0.0.3b1/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.3b1/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/math.py` & `crawlee-0.0.3b1/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.3b1/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.3b1/src/crawlee/_utils/recurring_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,26 +23,22 @@
         logger.debug(f'Calling RecurringTask.__init__(func={func.__name__}, delay={delay})...')
         self.func = func
         self.delay = delay
         self.task: asyncio.Task | None = None
 
     async def _wrapper(self) -> None:
         """Internal method that repeatedly executes the provided function with the specified delay."""
-        logger.debug('Calling RecurringTask._wrapper()...')
         sleep_time_secs = self.delay.total_seconds()
         while True:
-            logger.debug('RecurringTask._wrapper(): calling self.func()...')
             await self.func() if asyncio.iscoroutinefunction(self.func) else self.func()
             await asyncio.sleep(sleep_time_secs)
 
     def start(self) -> None:
         """Start the recurring task execution."""
-        logger.debug('Calling RecurringTask.start()...')
         self.task = asyncio.create_task(self._wrapper(), name=f'Task-recurring-{self.func.__name__}')
 
     async def stop(self) -> None:
         """Stop the recurring task execution."""
-        logger.debug('Calling RecurringTask.stop()...')
         if self.task:
             self.task.cancel()
             # Ensure the task has a chance to properly handle the cancellation and any potential exceptions.
             await asyncio.gather(self.task, return_exceptions=True)
```

### Comparing `crawlee-0.0.2/src/crawlee/_utils/requests.py` & `crawlee-0.0.3b1/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/system.py` & `crawlee-0.0.3b1/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/_utils/wait.py` & `crawlee-0.0.3b1/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.3b1/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.3b1/src/crawlee/autoscaling/snapshotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,19 +90,15 @@
         self._max_used_cpu_ratio = max_used_cpu_ratio
         self._max_used_memory_ratio = max_used_memory_ratio
         self._max_client_errors = max_client_errors
         self._snapshot_history = snapshot_history
         self._reserve_memory_ratio = reserve_memory_ratio
         self._memory_warning_cooldown_period = memory_warning_cooldown_period
         self._client_rate_limit_error_retry_count = client_rate_limit_error_retry_count
-
-        if max_memory_size is None:
-            self._max_memory_size = self._get_default_max_memory_size()
-        else:
-            self._max_memory_size = max_memory_size
+        self._max_memory_size = max_memory_size or self._get_default_max_memory_size()
 
         self._cpu_snapshots: list[CpuSnapshot] = []
         self._event_loop_snapshots: list[EventLoopSnapshot] = []
         self._memory_snapshots: list[MemorySnapshot] = []
         self._client_snapshots: list[ClientSnapshot] = []
 
         self._snapshot_event_loop_task = RecurringTask(self._snapshot_event_loop, self._event_loop_snapshot_interval)
```

### Comparing `crawlee-0.0.2/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.3b1/src/crawlee/autoscaling/system_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,28 +77,28 @@
 
         Considers snapshots within the `_max_snapshot_age` timeframe and determines if the system is currently
         overloaded based on predefined thresholds for each resource type.
 
         Returns:
             An object representing the current system status.
         """
-        return self._get_system_info(self._max_snapshot_age)
+        return self._get_system_info(sample_duration=self._max_snapshot_age)
 
     def get_historical_system_info(self) -> SystemInfo:
         """Retrieves and evaluates the historical status of system resources.
 
         Considers the entire history of snapshots from the Snapshotter to assess long-term system performance and
         determines if the system has been historically overloaded.
 
         Returns:
             An object representing the historical system status.
         """
         return self._get_system_info()
 
-    def _get_system_info(self, sample_duration: timedelta | None = None) -> SystemInfo:
+    def _get_system_info(self, *, sample_duration: timedelta | None = None) -> SystemInfo:
         """Get system information based on the overload state of different resources within a specified duration.
 
         Args:
             sample_duration: Specific duration for which to evaluate the system status. If None, evaluates across
                 the entire history available in the snapshotter.
 
         Returns:
@@ -178,22 +178,24 @@
         Returns:
             An object with an `is_overloaded` property set to `True` if the sample is considered overloaded based
             on the specified threshold ratio. Otherwise, `is_overloaded` is set to `False`.
         """
         if not sample:
             return LoadRatioInfo(limit_ratio=threshold, actual_ratio=0)
 
+        if len(sample) == 1:
+            return LoadRatioInfo(limit_ratio=threshold, actual_ratio=float(sample[0].is_overloaded))
+
         weights, values = [], []
 
         for previous, current in pairwise(sample):
             weight = (current.created_at - previous.created_at).total_seconds() or 0.001  # Avoid zero
             value = float(current.is_overloaded)
             weights.append(weight)
             values.append(value)
 
         try:
             weighted_avg = compute_weighted_avg(values, weights)
-        except ValueError:
-            logger.warning('Total weight cannot be zero')
-            return LoadRatioInfo(limit_ratio=threshold, actual_ratio=0)
+        except ValueError as exc:
+            raise ValueError('Failed to compute weighted average for the sample.') from exc
 
         return LoadRatioInfo(limit_ratio=threshold, actual_ratio=round(weighted_avg, 3))
```

### Comparing `crawlee-0.0.2/src/crawlee/autoscaling/types.py` & `crawlee-0.0.3b1/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.3b1/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,35 @@
 from __future__ import annotations
 
 from datetime import timedelta
 from functools import partial
 from logging import getLogger
 from typing import TYPE_CHECKING, Awaitable, Callable, Generic, Union, cast
 
+import httpx
 from typing_extensions import TypeVar
 
 from crawlee._utils.wait import wait_for
 from crawlee.autoscaling import AutoscaledPool, ConcurrencySettings
 from crawlee.autoscaling.snapshotter import Snapshotter
 from crawlee.autoscaling.system_status import SystemStatus
-from crawlee.basic_crawler.context_pipeline import ContextPipeline, RequestHandlerError
+from crawlee.basic_crawler.context_pipeline import (
+    ContextPipeline,
+    ContextPipelineInitializationError,
+    RequestHandlerError,
+)
 from crawlee.basic_crawler.router import Router
-from crawlee.basic_crawler.types import BasicCrawlingContext, FinalStatistics
+from crawlee.basic_crawler.types import BasicCrawlingContext, FinalStatistics, SendRequestFunction
 from crawlee.configuration import Configuration
 from crawlee.events.local_event_manager import LocalEventManager
+from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.request import BaseRequestData, Request, RequestState
 
 if TYPE_CHECKING:
+    from crawlee.http_clients.base_http_client import BaseHttpClient, HttpResponse
     from crawlee.storages.request_provider import RequestProvider
 
 
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 ErrorHandler = Callable[[TCrawlingContext, Exception], Awaitable[Union[Request, None]]]
 FailedRequestHandler = Callable[[TCrawlingContext, Exception], Awaitable[None]]
 
@@ -48,25 +55,27 @@
     def __init__(
         self,
         *,
         request_provider: RequestProvider,
         router: Callable[[TCrawlingContext], Awaitable[None]] | None = None,
         # TODO: make request_provider optional (and instantiate based on configuration if None is supplied)
         # https://github.com/apify/crawlee-py/issues/83
+        http_client: BaseHttpClient | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         max_request_retries: int = 3,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
         """Initialize the BasicCrawler.
 
         Args:
             request_provider: Provides requests to be processed
             router: A callable to which request handling is delegated
+            http_client: HTTP client to be used for `BasicCrawlingContext.send_request` and HTTP-only crawling.
             concurrency_settings: Allows fine-tuning concurrency levels
             max_request_retries: Maximum amount of attempts at processing a request
             configuration: Crawler configuration
             request_handler_timeout: How long is a single request handler allowed to run
             _context_pipeline: Allows extending the request lifecycle and modifying the crawling context.
                 This parameter is meant to be used by child classes, not when BasicCrawler is instantiated directly.
         """
@@ -74,14 +83,16 @@
 
         if isinstance(cast(Router, router), Router):
             self._router = cast(Router[TCrawlingContext], router)
         elif router is not None:
             self._router = None
             self.router.default_handler(router)
 
+        self._http_client = http_client or HttpxClient()
+
         self._context_pipeline = _context_pipeline or ContextPipeline()
 
         self._error_handler: ErrorHandler[TCrawlingContext] | None = None
         self._failed_request_handler: FailedRequestHandler[TCrawlingContext] | None = None
 
         self._max_request_retries = max_request_retries
 
@@ -158,24 +169,25 @@
             await self.add_requests(requests)
 
         async with self._event_manager, self._snapshotter:
             await self._pool.run()
 
         return FinalStatistics()
 
-    async def _handle_request_error(self, crawling_context: TCrawlingContext, error: Exception) -> None:
+    def _should_retry_request(self, crawling_context: BasicCrawlingContext) -> bool:
         max_request_retries = crawling_context.request.max_retries
         if max_request_retries is None:
             max_request_retries = self._max_request_retries
 
-        should_retry_request = (
+        return (
             not crawling_context.request.no_retry and (crawling_context.request.retry_count + 1) < max_request_retries
         )
 
-        if should_retry_request:
+    async def _handle_request_error(self, crawling_context: TCrawlingContext, error: Exception) -> None:
+        if self._should_retry_request(crawling_context):
             request = crawling_context.request
             request.retry_count += 1
 
             if self._error_handler:
                 try:
                     new_request = await self._error_handler(crawling_context, error)
                 except Exception as e:
@@ -201,14 +213,20 @@
 
         if self._failed_request_handler:
             try:
                 await self._failed_request_handler(crawling_context, error)
             except Exception as e:
                 raise UserDefinedErrorHandlerError('Exception thrown in user-defined failed request handler') from e
 
+    def _prepare_send_request_function(self) -> SendRequestFunction:
+        async def send_request(url: str, *, method: str = 'get', headers: dict[str, str] | None = None) -> HttpResponse:
+            return await self._http_client.send_request(url, method=method, headers=httpx.Headers(headers))
+
+        return send_request
+
     async def __is_finished_function(self) -> bool:
         return await self._request_provider.is_finished()
 
     async def __is_task_ready_function(self) -> bool:
         return not await self._request_provider.is_empty()
 
     async def __run_task_function(self) -> None:
@@ -220,31 +238,31 @@
             max_retries=3,
         )
 
         if request is None:
             return
 
         # TODO: fetch session from the session pool
-        # https://github.com/apify/crawlee-py/issues/78
+        # https://github.com/apify/crawlee-py/issues/110
 
-        crawling_context = BasicCrawlingContext(request=request)
+        crawling_context = BasicCrawlingContext(request=request, send_request=self._prepare_send_request_function())
 
         try:
             request.state = RequestState.REQUEST_HANDLER
 
             await wait_for(
                 lambda: self.__run_request_handler(crawling_context),
                 timeout=self._request_handler_timeout,
                 timeout_message='Request handler timed out after '
                 f'{self._request_handler_timeout.total_seconds()} seconds',
                 logger=logger,
             )
 
             await wait_for(
-                lambda: self._request_provider.mark_request_as_handled(request),
+                lambda: self._request_provider.mark_request_as_handled(crawling_context.request),
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
 
@@ -275,14 +293,36 @@
                 logger.exception(
                     'An exception occurred during handling of failed request. This places the crawler '
                     'and its underlying storages into an unknown state and crawling will be terminated.',
                     exc_info=secondary_error,
                 )
                 request.state = RequestState.ERROR
                 raise
+        except ContextPipelineInitializationError as initialization_error:
+            if self._should_retry_request(crawling_context):
+                logger.debug(
+                    'An exception occured during the initialization of crawling context, a retry is in order',
+                    exc_info=initialization_error,
+                )
+
+                request = crawling_context.request
+                request.retry_count += 1
+                request.state = RequestState.DONE
+                await self._request_provider.reclaim_request(request)
+            else:
+                logger.exception('Request failed and reached maximum retries', exc_info=initialization_error)
+
+                await wait_for(
+                    lambda: self._request_provider.mark_request_as_handled(crawling_context.request),
+                    timeout=self._internal_timeout,
+                    timeout_message='Marking request as handled timed out after '
+                    f'{self._internal_timeout.total_seconds()} seconds',
+                    logger=logger,
+                    max_retries=3,
+                )
         except Exception as internal_error:
             logger.exception(
                 'An exception occurred during handling of a request. This places the crawler '
                 'and its underlying storages into an unknown state and crawling will be terminated.',
                 exc_info=internal_error,
             )
             raise
```

### Comparing `crawlee-0.0.2/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.3b1/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,36 @@
     """Wraps an exception thrown from a request handler (router) and extends it with crawling context."""
 
     def __init__(self, wrapped_exception: Exception, crawling_context: TCrawlingContext) -> None:
         self.wrapped_exception = wrapped_exception
         self.crawling_context = crawling_context
 
 
+class ContextPipelineInitializationError(Exception):
+    """Wraps an exception thrown in the initialization step of a context pipeline middleware.
+
+    We may not have the complete context at this point, so only `BasicCrawlingContext` is provided.
+    """
+
+    def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
+        self.wrapped_exception = wrapped_exception
+        self.crawling_context = crawling_context
+
+
+class ContextPipelineFinalizationError(Exception):
+    """Wraps an exception thrown in the finalization step of a context pipeline middleware.
+
+    We may not have the complete context at this point, so only `BasicCrawlingContext` is provided.
+    """
+
+    def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
+        self.wrapped_exception = wrapped_exception
+        self.crawling_context = crawling_context
+
+
 class ContextPipeline(Generic[TCrawlingContext]):
     """Encapsulates the logic of gradually enhancing the crawling context with additional information and utilities.
 
     The enhancement is done by a chain of middlewares that are added to the pipeline after it's creation.
     """
 
     def __init__(
@@ -51,37 +73,42 @@
         """Run a crawling context through the middleware chain and pipe it into a consumer function.
 
         Exceptions from the consumer function are wrapped together with the final crawling context.
         """
         chain = list(self._middleware_chain())
         cleanup_stack = list[AsyncGenerator]()
 
-        for member in reversed(chain):
-            if member._middleware:  # noqa: SLF001
-                middleware_instance = member._middleware(crawling_context)  # noqa: SLF001
-                try:
-                    result = await middleware_instance.__anext__()
-                except StopAsyncIteration as e:
-                    raise RuntimeError('The middleware did not yield') from e
-
-                crawling_context = result
-                cleanup_stack.append(middleware_instance)
-
         try:
-            await final_context_consumer(cast(TCrawlingContext, crawling_context))
-        except Exception as e:
-            raise RequestHandlerError(e, crawling_context) from e
+            for member in reversed(chain):
+                if member._middleware:  # noqa: SLF001
+                    middleware_instance = member._middleware(crawling_context)  # noqa: SLF001
+                    try:
+                        result = await middleware_instance.__anext__()
+                    except StopAsyncIteration as e:
+                        raise RuntimeError('The middleware did not yield') from e
+                    except Exception as e:
+                        raise ContextPipelineInitializationError(e, crawling_context) from e
+
+                    crawling_context = result
+                    cleanup_stack.append(middleware_instance)
 
-        for middleware_instance in reversed(cleanup_stack):
             try:
-                result = await middleware_instance.__anext__()
-            except StopAsyncIteration:  # noqa: PERF203
-                pass
-            else:
-                raise RuntimeError('The middleware yielded more than once')
+                await final_context_consumer(cast(TCrawlingContext, crawling_context))
+            except Exception as e:
+                raise RequestHandlerError(e, crawling_context) from e
+        finally:
+            for middleware_instance in reversed(cleanup_stack):
+                try:
+                    result = await middleware_instance.__anext__()
+                except StopAsyncIteration:  # noqa: PERF203
+                    pass
+                except Exception as e:
+                    raise ContextPipelineFinalizationError(e, crawling_context) from e
+                else:
+                    raise RuntimeError('The middleware yielded more than once')
 
     def compose(
         self,
         middleware: Callable[
             [TCrawlingContext],
             AsyncGenerator[TMiddlewareCrawlingContext, None],
         ],
```

### Comparing `crawlee-0.0.2/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.3b1/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/configuration.py` & `crawlee-0.0.3b1/src/crawlee/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # ruff: noqa: TCH003 TCH002
+
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import Annotated
 
 from pydantic import Field
 from pydantic_settings import BaseSettings
```

### Comparing `crawlee-0.0.2/src/crawlee/events/event_manager.py` & `crawlee-0.0.3b1/src/crawlee/events/event_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,55 +9,77 @@
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 from pyee.asyncio import AsyncIOEventEmitter
 
 if TYPE_CHECKING:
     from datetime import timedelta
+    from types import TracebackType
 
     from crawlee.events.types import Event, EventData, Listener, WrappedListener
 
 logger = getLogger(__name__)
 
 
 class EventManager:
     """Event manager for registering, emitting, and managing event listeners.
 
     Event manager allows you to register event listeners, emit events, and wait for event listeners to complete
     their execution. It is built on top of the `pyee.asyncio.AsyncIOEventEmitter` class.
     """
 
-    def __init__(self) -> None:
-        logger.debug('Calling EventManager.__init__()...')
+    def __init__(self, close_timeout: timedelta | None = None) -> None:
+        """Create a new instance.
+
+        Args:
+            close_timeout: Optional timeout after which the pending event listeners are canceled.
+        """
+        self._close_timeout = close_timeout
 
         # Asynchronous event emitter for handle events and invoke the event listeners.
         self._event_emitter = AsyncIOEventEmitter()
 
         # Listeners are wrapped inside asyncio.Task. Store their references here so that we can wait for them to finish.
         self._listener_tasks: set[asyncio.Task] = set()
 
         # Store the mapping between events, listeners and their wrappers in the following way:
         #   event -> listener -> [wrapped_listener_1, wrapped_listener_2, ...]
         self._listeners_to_wrappers: dict[Event, dict[Listener, list[WrappedListener]]] = defaultdict(
             lambda: defaultdict(list),
         )
 
+    async def __aenter__(self) -> EventManager:
+        """Initializes the event manager upon entering the async context."""
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        exc_traceback: TracebackType | None,
+    ) -> None:
+        """Closes the local event manager upon exiting the async context.
+
+        This will stop listening for the events, and it will wait for all the event listeners to finish.
+        """
+        await self.wait_for_all_listeners_to_complete(timeout=self._close_timeout)
+        self._event_emitter.remove_all_listeners()
+        self._listener_tasks.clear()
+        self._listeners_to_wrappers.clear()
+
     def on(self, *, event: Event, listener: Listener) -> None:
         """Add an event listener to the event manager.
 
         Args:
             event: The Actor event for which to listen to.
             listener: The function (sync or async) which is to be called when the event is emitted.
         """
-        logger.debug('Calling EventManager.on()...')
 
         @wraps(listener)
         async def listener_wrapper(event_data: EventData) -> None:
-            logger.debug('Calling EventManager.on.listener_wrapper()...')
-
             # If the listener is a coroutine function, just call it, otherwise, run it in a separate thread
             # to avoid blocking the event loop
             coro = (
                 listener(event_data)
                 if asyncio.iscoroutinefunction(listener)
                 else asyncio.to_thread(listener, event_data)
             )
@@ -88,16 +110,14 @@
         """Remove a listener, or all listeners, from an Actor event.
 
         Args:
             event: The Actor event for which to remove listeners.
             listener: The listener which is supposed to be removed. If not passed, all listeners of this event
                 are removed.
         """
-        logger.debug('Calling EventManager.off()...')
-
         if listener:
             for listener_wrapper in self._listeners_to_wrappers[event][listener]:
                 self._event_emitter.remove_listener(event.value, listener_wrapper)
             self._listeners_to_wrappers[event][listener] = []
         else:
             self._listeners_to_wrappers[event] = defaultdict(list)
             self._event_emitter.remove_all_listeners(event.value)
@@ -105,39 +125,23 @@
     def emit(self, *, event: Event, event_data: EventData) -> None:
         """Emit an event.
 
         Args:
             event: The event which will be emitted.
             event_data: The data which will be passed to the event listeners.
         """
-        logger.debug('Calling EventManager.emit()...')
         self._event_emitter.emit(event.value, event_data)
 
-    async def close(self, *, timeout: timedelta | None = None) -> None:
-        """Close the event manager.
-
-        This will stop listening for the events, and it will wait for all the event listeners to finish.
-
-        Args:
-            timeout: Optional timeout after which the pending event listeners are canceled.
-        """
-        logger.debug('Calling EventManager.close()...')
-        await self._wait_for_all_listeners_to_complete(timeout=timeout)
-        self._event_emitter.remove_all_listeners()
-        self._listener_tasks.clear()
-        self._listeners_to_wrappers.clear()
-
-    async def _wait_for_all_listeners_to_complete(self, *, timeout: timedelta | None = None) -> None:
+    async def wait_for_all_listeners_to_complete(self, *, timeout: timedelta | None = None) -> None:
         """Wait for all currently executing event listeners to complete.
 
         Args:
             timeout: The maximum time to wait for the event listeners to finish. If they do not complete within
                 the specified timeout, they will be canceled.
         """
-        logger.debug('Calling EventManager.wait_for_all_listeners_to_complete()...')
 
         async def wait_for_listeners() -> None:
             """Gathers all listener tasks and awaits their completion, logging any exceptions encountered."""
             results = await asyncio.gather(*self._listener_tasks, return_exceptions=True)
             for result in results:
                 if isinstance(result, Exception):
                     logger.exception('Event listener raised an exception.', exc_info=result)
```

### Comparing `crawlee-0.0.2/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.3b1/src/crawlee/events/local_event_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,64 +21,58 @@
 class LocalEventManager(EventManager):
     """Local event manager for emitting system info events."""
 
     def __init__(
         self,
         *,
         system_info_interval: timedelta = timedelta(seconds=60),
-        close_timeout: timedelta | None = None,
     ) -> None:
         """Create a new instance.
 
         Args:
             system_info_interval: Interval at which `SystemInfo` events are emitted.
             close_timeout: Optional timeout for closing the event manager.
         """
-        logger.debug('Calling LocalEventManager.__init__()...')
-
         self._system_info_interval = system_info_interval
-        self._close_timeout = close_timeout
 
         # Recurring task for emitting system info events.
         self._emit_system_info_event_rec_task: RecurringTask | None = None
 
         super().__init__()
 
     async def __aenter__(self) -> LocalEventManager:
         """Initializes the local event manager upon entering the async context.
 
         It starts emitting system info events at regular intervals.
         """
-        logger.debug('Calling LocalEventManager.__aenter__()...')
+        await super().__aenter__()
+
         self._emit_system_info_event_rec_task = RecurringTask(
             func=self._emit_system_info_event,
             delay=self._system_info_interval,
         )
         self._emit_system_info_event_rec_task.start()
+
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_traceback: TracebackType | None,
     ) -> None:
         """Closes the local event manager upon exiting the async context.
 
         It stops emitting system info events and closes the event manager.
         """
-        logger.debug('Calling LocalEventManager.__aexit__()...')
-
         if self._emit_system_info_event_rec_task is not None:
             await self._emit_system_info_event_rec_task.stop()
 
-        await super().close(timeout=self._close_timeout)
+        await super().__aexit__(exc_type, exc_value, exc_traceback)
 
     async def _emit_system_info_event(self) -> None:
         """Emits a system info event with the current CPU and memory usage."""
-        logger.debug('Calling LocalEventManager._emit_system_info_event()...')
-
         cpu_info = await asyncio.to_thread(get_cpu_info)
         memory_info = await asyncio.to_thread(get_memory_info)
 
         event_data = EventSystemInfoData(cpu_info=cpu_info, memory_info=memory_info)
         self.emit(event=Event.SYSTEM_INFO, event_data=event_data)
```

### Comparing `crawlee-0.0.2/src/crawlee/events/types.py` & `crawlee-0.0.3b1/src/crawlee/events/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """Enum of all possible events that can be emitted."""
 
     PERSIST_STATE = 'persistState'
     SYSTEM_INFO = 'systemInfo'
     MIGRATING = 'migrating'
     ABORTING = 'aborting'
     EXIT = 'exit'
+    SESSION_RETIRED = 'sessionRetired'
 
 
 @dataclass
 class EventPersistStateData:
     """Data for the persist state event."""
 
     is_migrating: bool
```

### Comparing `crawlee-0.0.2/src/crawlee/log_config.py` & `crawlee-0.0.3b1/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/request.py` & `crawlee-0.0.3b1/src/crawlee/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,26 +77,26 @@
 
     @classmethod
     def from_url(
         cls,
         url: str,
         *,
         unique_key: str | None = None,
-        id_: str | None = None,
+        id: str | None = None,
         **kwargs: Any,
     ) -> Self:
         """Create a new `RequestData` instance from a URL."""
         unique_key = unique_key or compute_unique_key(url)
-        id_ = id_ or unique_key_to_request_id(unique_key)
-        return cls(url=url, unique_key=unique_key, id=id_, **kwargs)
+        id = id or unique_key_to_request_id(unique_key)
+        return cls(url=url, unique_key=unique_key, id=id, **kwargs)
 
     @classmethod
-    def from_base_request_data(cls, base_request_data: BaseRequestData, *, id_: str | None = None) -> Self:
+    def from_base_request_data(cls, base_request_data: BaseRequestData, *, id: str | None = None) -> Self:
         """Create a complete Request object based on a BaseRequestData instance."""
-        return cls(**base_request_data.model_dump(), id=id_ or unique_key_to_request_id(base_request_data.unique_key))
+        return cls(**base_request_data.model_dump(), id=id or unique_key_to_request_id(base_request_data.unique_key))
 
     @property
     def crawlee_data(self) -> CrawleeRequestData:
         """Crawlee-specific configuration stored in the user_data."""
         return CrawleeRequestData.model_validate(self.user_data.get('__crawlee', {}) if self.user_data else {})
 
     @property
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/base_resource_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from crawlee.storage_clients import MemoryStorageClient
-    from crawlee.storages.types import BaseResourceInfo
+    from crawlee.storages.models import BaseStorageMetadata
 
 
 class BaseResourceClient(ABC):
     """Base class for resource clients."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> None:
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
-        self.id = id_
+        self.id = id
         self.name = name
 
     @property
     @abstractmethod
-    def resource_info(self) -> BaseResourceInfo:
+    def resource_info(self) -> BaseStorageMetadata:
         """Get the resource info for the storage client."""
 
     @abstractmethod
-    async def get(self) -> BaseResourceInfo | None:
+    async def get(self) -> BaseStorageMetadata | None:
         """Get the info about the storage client.
 
         Returns:
             The storage client info or None if it does not exist.
         """
 
     @classmethod
@@ -53,58 +53,58 @@
 
     @classmethod
     @abstractmethod
     def _create_from_directory(
         cls,
         storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> Self:
         """Create a new resource client from a directory."""
 
     @classmethod
     def find_or_create_client_by_id_or_name(
         cls,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> Self | None:
         """Locates or creates a new storage client based on the given ID or name.
 
         This method attempts to find a storage client in the memory cache first. If not found,
         it tries to locate a storage directory by name. If still not found, it searches through
         storage directories for a matching ID or name in their metadata. If none exists, and the
         specified ID is 'default', it checks for a default storage directory. If a storage client
         is found or created, it is added to the memory cache. If no storage client can be located or
         created, the method returns None.
 
         Args:
             memory_storage_client: The memory storage client used to store and retrieve storage clients.
-            id_: The unique identifier for the storage client. Defaults to None.
+            id: The unique identifier for the storage client. Defaults to None.
             name: The name of the storage client. Defaults to None.
 
         Raises:
-            ValueError: If both id_ and name are None.
+            ValueError: If both id and name are None.
 
         Returns:
             The found or created storage client, or None if no client could be found or created.
         """
-        if id_ is None and name is None:
-            raise ValueError('Either id_ or name must be specified.')
+        if id is None and name is None:
+            raise ValueError('Either id or name must be specified.')
 
         storage_client_cache = cls._get_storage_client_cache(memory_storage_client)
         storages_dir = cls._get_storages_dir(memory_storage_client)
 
         # First check memory cache
         found = next(
             (
                 storage_client
                 for storage_client in storage_client_cache
-                if storage_client.id == id_
+                if storage_client.id == id
                 or (storage_client.name and name and storage_client.name.lower() == name.lower())
             ),
             None,
         )
 
         if found is not None:
             return found
@@ -123,31 +123,31 @@
                 if not entry.is_dir():
                     continue
                 metadata_path = os.path.join(entry.path, '__metadata__.json')
                 if not os.access(metadata_path, os.F_OK):
                     continue
                 with open(metadata_path, encoding='utf-8') as metadata_file:
                     metadata = json.load(metadata_file)
-                if id_ and id_ == metadata.get('id'):
+                if id and id == metadata.get('id'):
                     storage_path = entry.path
                     name = metadata.get(name)
                     break
                 if name and name == metadata.get('name'):
                     storage_path = entry.path
-                    id_ = metadata.get(id_)
+                    id = metadata.get(id)
                     break
 
         # As a last resort, try to check if the accessed storage is the default one,
         # and the folder has no metadata
         # TODO: make this respect the APIFY_DEFAULT_XXX_ID env var
         # https://github.com/apify/apify-sdk-python/issues/149
-        if id_ == 'default':
-            possible_storage_path = os.path.join(storages_dir, id_)
+        if id == 'default':
+            possible_storage_path = os.path.join(storages_dir, id)
             if os.access(possible_storage_path, os.F_OK):
                 storage_path = possible_storage_path
 
         if not storage_path:
             return None
 
-        resource_client = cls._create_from_directory(storage_path, memory_storage_client, id_, name)
+        resource_client = cls._create_from_directory(storage_path, memory_storage_client, id, name)
         storage_client_cache.append(resource_client)
         return resource_client
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/base_resource_collection_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_collection_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from crawlee._utils.file import persist_metadata_if_enabled
 from crawlee.resource_clients.base_resource_client import BaseResourceClient
-from crawlee.storages.types import BaseResourceInfo, ListPage
 
 if TYPE_CHECKING:
     from crawlee.storage_clients import MemoryStorageClient
+    from crawlee.storages.models import BaseListPage, BaseStorageMetadata
 
 ResourceClientType = TypeVar('ResourceClientType', bound=BaseResourceClient, contravariant=True)  # noqa: PLC0105
 
 
 class BaseResourceCollectionClient(ABC, Generic[ResourceClientType]):
     """Base class for resource collection clients."""
 
@@ -30,74 +30,60 @@
     def _client_class(self) -> type[ResourceClientType]:
         """Get the class of the resource clients."""
 
     @abstractmethod
     def _get_storage_client_cache(self) -> list[ResourceClientType]:
         """Get the storage client cache."""
 
-    async def list(self) -> ListPage:
+    @abstractmethod
+    async def list(self) -> BaseListPage:
         """List the available storages.
 
         Returns:
             The list of available storages matching the specified filters.
         """
-        storage_client_cache = self._get_storage_client_cache()
-
-        items = [storage.resource_info for storage in storage_client_cache]
-
-        return ListPage(
-            total=len(items),
-            count=len(items),
-            offset=0,
-            limit=len(items),
-            desc=False,
-            items=sorted(items, key=lambda item: item.created_at),
-        )
 
     async def get_or_create(
         self,
         *,
         name: str | None = None,
         schema: dict | None = None,  # noqa: ARG002
-        id_: str | None = None,
-    ) -> BaseResourceInfo:
+        id: str | None = None,
+    ) -> BaseStorageMetadata:
         """Retrieve a named storage, or create a new one when it doesn't exist.
 
         Args:
             name: The name of the storage to retrieve or create.
             schema: The schema of the storage
-            id_: ID of the storage to retrieve or create
+            id: ID of the storage to retrieve or create
 
         Returns:
             The retrieved or newly-created storage.
         """
         resource_client_class = self._client_class
         storage_client_cache = self._get_storage_client_cache()
 
-        if name or id_:
+        if name or id:
             found = resource_client_class.find_or_create_client_by_id_or_name(
                 memory_storage_client=self._memory_storage_client,
                 name=name,
-                id_=id_,
+                id=id,
             )
             if found:
                 return found.resource_info
 
         new_resource = resource_client_class(
-            id_=id_,
+            id=id,
             name=name,
             base_storage_directory=self._base_storage_directory,
             memory_storage_client=self._memory_storage_client,
         )
         storage_client_cache.append(new_resource)
 
-        resource_info = new_resource.resource_info
-        data = resource_info.__dict__ if isinstance(resource_info, BaseResourceInfo) else resource_info
-
         # Write to the disk
         await persist_metadata_if_enabled(
-            data=data,
+            data=new_resource.resource_info.model_dump(),
             entity_directory=new_resource.resource_directory,  # type: ignore
             write_metadata=self._memory_storage_client.write_metadata,
         )
 
-        return resource_info
+        return new_resource.resource_info
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/dataset_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import os
 from datetime import datetime, timezone
+from logging import getLogger
 from typing import TYPE_CHECKING, Any, AsyncIterator
 
 import aiofiles
 import aioshutil
 from aiofiles.os import makedirs
 from typing_extensions import override
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.data_processing import raise_on_duplicate_storage, raise_on_non_existing_storage
 from crawlee._utils.file import force_rename, json_dumps, persist_metadata_if_enabled
 from crawlee.resource_clients.base_resource_client import BaseResourceClient
-from crawlee.storages.types import DatasetResourceInfo, ListPage, StorageTypes
+from crawlee.storages.models import DatasetItemsListPage, DatasetMetadata
+from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.storage_clients import MemoryStorageClient
-    from crawlee.storages.types import JSONSerializable
+    from crawlee.types import JSONSerializable
+
+logger = getLogger(__name__)
 
 
 class DatasetClient(BaseResourceClient):
     """Sub-client for manipulating a single dataset."""
 
     _LIST_ITEMS_LIMIT = 999_999_999_999
     """This is what API returns in the x-apify-pagination-limit header when no limit query parameter is used."""
@@ -32,39 +36,39 @@
     """Number of characters of the dataset item file names, e.g.: 000000019.json - 9 digits."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
         created_at: datetime | None = None,
         accessed_at: datetime | None = None,
         modified_at: datetime | None = None,
         item_count: int = 0,
     ) -> None:
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
-        self.id = id_ or crypto_random_object_id()
+        self.id = id or crypto_random_object_id()
         self.name = name
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
 
         self.resource_directory = os.path.join(self._base_storage_directory, self.name or self.id)
         self.dataset_entries: dict[str, dict] = {}
         self.file_operation_lock = asyncio.Lock()
         self.item_count = item_count
 
     @property
     @override
-    def resource_info(self) -> DatasetResourceInfo:
+    def resource_info(self) -> DatasetMetadata:
         """Get the resource info for the dataset client."""
-        return DatasetResourceInfo(
+        return DatasetMetadata(
             id=str(self.id),
             name=str(self.name),
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             item_count=self.item_count,
         )
@@ -84,96 +88,99 @@
 
     @classmethod
     @override
     def _create_from_directory(
         cls,
         storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> DatasetClient:
         item_count = 0
         created_at = datetime.now(timezone.utc)
         accessed_at = datetime.now(timezone.utc)
         modified_at = datetime.now(timezone.utc)
-        entries: dict[str, dict] = {}
 
+        # Load metadata if it exists
+        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
+
+        if os.path.exists(metadata_filepath):
+            with open(metadata_filepath, encoding='utf-8') as f:
+                json_content = json.load(f)
+                resource_info = DatasetMetadata(**json_content)
+
+            id = resource_info.id
+            name = resource_info.name
+            item_count = resource_info.item_count
+            created_at = resource_info.created_at
+            accessed_at = resource_info.accessed_at
+            modified_at = resource_info.modified_at
+
+        # Load dataset entries
+        entries: dict[str, dict] = {}
         has_seen_metadata_file = False
 
-        # Access the dataset folder
         for entry in os.scandir(storage_directory):
             if entry.is_file():
                 if entry.name == '__metadata__.json':
                     has_seen_metadata_file = True
-
-                    # We have found the dataset's metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                        metadata = json.load(f)
-                    id_ = metadata['id']
-                    name = metadata['name']
-                    item_count = metadata['itemCount']
-                    created_at = datetime.fromisoformat(metadata['createdAt'])
-                    accessed_at = datetime.fromisoformat(metadata['accessedAt'])
-                    modified_at = datetime.fromisoformat(metadata['modifiedAt'])
-
                     continue
 
                 with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
                     entry_content = json.load(f)
-                entry_name = entry.name.split('.')[0]
 
+                entry_name = entry.name.split('.')[0]
                 entries[entry_name] = entry_content
 
                 if not has_seen_metadata_file:
                     item_count += 1
 
+        # Create new dataset client
         new_client = DatasetClient(
             base_storage_directory=memory_storage_client.datasets_directory,
             memory_storage_client=memory_storage_client,
-            id_=id_,
+            id=id,
             name=name,
             created_at=created_at,
             accessed_at=accessed_at,
             modified_at=modified_at,
             item_count=item_count,
         )
 
-        for entry_id, content in entries.items():
-            new_client.dataset_entries[entry_id] = content
-
+        new_client.dataset_entries.update(entries)
         return new_client
 
     @override
-    async def get(self) -> DatasetResourceInfo | None:
+    async def get(self) -> DatasetMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if found:
             async with found.file_operation_lock:
                 await found.update_timestamps(has_been_modified=False)
                 return found.resource_info
 
         return None
 
-    async def update(self, *, name: str | None = None) -> DatasetResourceInfo:
+    async def update(self, *, name: str | None = None) -> DatasetMetadata:
         """Update the dataset with specified fields.
 
         Args:
             name: The new name for the dataset
 
         Returns:
             The updated dataset
         """
         # Check by id
         existing_dataset_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_dataset_by_id is None:
             raise_on_non_existing_storage(StorageTypes.DATASET, self.id)
 
         # Skip if no changes
@@ -234,15 +241,15 @@
         fields: list[str] | None = None,  # noqa: ARG002
         omit: list[str] | None = None,  # noqa: ARG002
         unwind: str | None = None,  # noqa: ARG002
         skip_empty: bool = False,  # noqa: ARG002
         skip_hidden: bool = False,  # noqa: ARG002
         flatten: list[str] | None = None,  # noqa: ARG002
         view: str | None = None,  # noqa: ARG002
-    ) -> ListPage:
+    ) -> DatasetItemsListPage:
         """Retrieves a paginated list of items from a dataset based on various filtering parameters.
 
         This method provides the flexibility to filter, sort, and modify the appearance of dataset items when listed.
         Each parameter modifies the result set according to its purpose. The method also supports pagination
         through 'offset' and 'limit' parameters.
 
         Args:
@@ -272,15 +279,15 @@
         Returns:
             An object containing the list of filtered, sorted, and paginated dataset items,
                 as well as additional pagination details.
         """
         # Check by id
         existing_dataset_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_dataset_by_id is None:
             raise_on_non_existing_storage(StorageTypes.DATASET, self.id)
 
         async with existing_dataset_by_id.file_operation_lock:
@@ -298,15 +305,15 @@
                 items.append(existing_dataset_by_id.dataset_entries[entry_number])
 
             await existing_dataset_by_id.update_timestamps(has_been_modified=False)
 
             if desc:
                 items.reverse()
 
-            return ListPage(
+            return DatasetItemsListPage(
                 count=len(items),
                 desc=desc or False,
                 items=items,
                 limit=limit or self._LIST_ITEMS_LIMIT,
                 offset=offset or 0,
                 total=existing_dataset_by_id.item_count,
             )
@@ -350,15 +357,14 @@
             skip_empty: If set to True, omits items that are empty after other filters have been applied.
 
             skip_hidden: If set to True, omits fields starting with the '#' character from the output.
 
         Yields:
             An asynchronous iterator of dictionary objects, each representing a dataset item after applying
             the specified filters and transformations.
-
         """
         cache_size = 1000
         first_item = offset
 
         # If there is no limit, set last_item to None until we get the total from the first API response
         last_item = None if limit is None else offset + limit
 
@@ -393,15 +399,15 @@
         Args:
             items: The items which to push in the dataset. Either a stringified JSON, a dictionary,
                 or a list of strings or dictionaries.
         """
         # Check by id
         existing_dataset_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_dataset_by_id is None:
             raise_on_non_existing_storage(StorageTypes.DATASET, self.id)
 
         normalized = self._normalize_items(items)
@@ -410,15 +416,15 @@
         for entry in normalized:
             existing_dataset_by_id.item_count += 1
             idx = self._generate_local_entry_name(existing_dataset_by_id.item_count)
 
             existing_dataset_by_id.dataset_entries[idx] = entry
             added_ids.append(idx)
 
-        data_entries = [(id_, existing_dataset_by_id.dataset_entries[id_]) for id_ in added_ids]
+        data_entries = [(id, existing_dataset_by_id.dataset_entries[id]) for id in added_ids]
 
         async with existing_dataset_by_id.file_operation_lock:
             await existing_dataset_by_id.update_timestamps(has_been_modified=True)
 
             await self._persist_dataset_items_to_disk(
                 data=data_entries,
                 entity_directory=existing_dataset_by_id.resource_directory,
@@ -461,19 +467,16 @@
     async def update_timestamps(self, *, has_been_modified: bool) -> None:
         """Update the timestamps of the dataset."""
         self._accessed_at = datetime.now(timezone.utc)
 
         if has_been_modified:
             self._modified_at = datetime.now(timezone.utc)
 
-        dataset_info = self.resource_info
-        dataset_info_as_dict = dataset_info.__dict__
-
         await persist_metadata_if_enabled(
-            data=dataset_info_as_dict,
+            data=self.resource_info.model_dump(),
             entity_directory=self.resource_directory,
             write_metadata=self._memory_storage_client.write_metadata,
         )
 
     def get_start_and_end_indexes(self, offset: int, limit: int | None = None) -> tuple[int, int]:
         """Calculate the start and end indexes for listing items."""
         actual_limit = limit or self.item_count
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/dataset_collection_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_collection_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,50 +2,57 @@
 
 from typing import TYPE_CHECKING
 
 from typing_extensions import override
 
 from crawlee.resource_clients.base_resource_collection_client import BaseResourceCollectionClient
 from crawlee.resource_clients.dataset_client import DatasetClient
+from crawlee.storages.models import DatasetsListPage
 
 if TYPE_CHECKING:
-    from crawlee.storages.types import BaseResourceInfo, ListPage
+    from crawlee.storages.models import BaseStorageMetadata
 
 
 class DatasetCollectionClient(BaseResourceCollectionClient):
     """Sub-client for manipulating datasets."""
 
     @property
     @override
     def _client_class(self) -> type[DatasetClient]:
         return DatasetClient
 
     @override
     def _get_storage_client_cache(self) -> list[DatasetClient]:
         return self._memory_storage_client.datasets_handled
 
-    async def list(self) -> ListPage:
-        """List the available datasets.
-
-        Returns:
-            The list of available datasets matching the specified filters.
-        """
-        return await super().list()
+    @override
+    async def list(self) -> DatasetsListPage:
+        storage_client_cache = self._get_storage_client_cache()
+        items = [storage.resource_info for storage in storage_client_cache]
+
+        return DatasetsListPage(
+            total=len(items),
+            count=len(items),
+            offset=0,
+            limit=len(items),
+            desc=False,
+            items=sorted(items, key=lambda item: item.created_at),
+        )
 
     async def get_or_create(
         self,
         *,
         name: str | None = None,
         schema: dict | None = None,
-        id_: str | None = None,
-    ) -> BaseResourceInfo:
+        id: str | None = None,
+    ) -> BaseStorageMetadata:
         """Retrieve a named dataset, or create a new one when it doesn't exist.
 
         Args:
             name: The name of the dataset to retrieve or create.
             schema: The schema of the dataset
-            id_: ID of the dataset to retrieve or create
+            id: ID of the dataset to retrieve or create
 
         Returns:
             The retrieved or newly-created dataset.
         """
-        return await super().get_or_create(name=name, schema=schema, id_=id_)
+        return await super().get_or_create(name=name, schema=schema, id=id)
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,22 @@
     force_remove,
     force_rename,
     is_file_or_bytes,
     json_dumps,
     persist_metadata_if_enabled,
 )
 from crawlee.resource_clients.base_resource_client import BaseResourceClient
-from crawlee.storages.types import (
-    KeyValueStoreListKeysOutput,
+from crawlee.storages.models import (
+    KeyValueStoreKeyInfo,
+    KeyValueStoreListKeysPage,
+    KeyValueStoreMetadata,
     KeyValueStoreRecord,
-    KeyValueStoreRecordInfo,
-    KeyValueStoreResourceInfo,
-    StorageTypes,
+    KeyValueStoreRecordMetadata,
 )
+from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.storage_clients import MemoryStorageClient
 
 logger = getLogger(__name__)
 
 
@@ -44,37 +45,38 @@
     """Sub-client for manipulating a single key-value store."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
         created_at: datetime | None = None,
         accessed_at: datetime | None = None,
         modified_at: datetime | None = None,
     ) -> None:
+        self.id = id or crypto_random_object_id()
+        self.name = name
+
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
-        self.id = id_ or crypto_random_object_id()
-        self.name = name
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
 
         self.resource_directory = os.path.join(base_storage_directory, self.name or self.id)
         self.records: dict[str, KeyValueStoreRecord] = {}
         self.file_operation_lock = asyncio.Lock()
 
     @property
     @override
-    def resource_info(self) -> KeyValueStoreResourceInfo:
+    def resource_info(self) -> KeyValueStoreMetadata:
         """Get the resource info for the key-value store client."""
-        return KeyValueStoreResourceInfo(
+        return KeyValueStoreMetadata(
             id=str(self.id),
             name=str(self.name),
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             user_id='1',
         )
@@ -82,144 +84,141 @@
     @classmethod
     @override
     def _get_storages_dir(cls, memory_storage_client: MemoryStorageClient) -> str:
         return memory_storage_client.key_value_stores_directory
 
     @classmethod
     @override
-    def _get_storage_client_cache(
-        cls,
-        memory_storage_client: MemoryStorageClient,
-    ) -> list[KeyValueStoreClient]:
+    def _get_storage_client_cache(cls, memory_storage_client: MemoryStorageClient) -> list[KeyValueStoreClient]:
         return memory_storage_client.key_value_stores_handled
 
     @classmethod
     @override
     def _create_from_directory(
         cls,
         storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> KeyValueStoreClient:
         created_at = datetime.now(timezone.utc)
         accessed_at = datetime.now(timezone.utc)
         modified_at = datetime.now(timezone.utc)
 
-        store_metadata_path = os.path.join(storage_directory, '__metadata__.json')
-        if os.path.exists(store_metadata_path):
-            with open(store_metadata_path, encoding='utf-8') as f:
-                metadata = json.load(f)
-            id_ = metadata['id']
-            name = metadata['name']
-            created_at = datetime.fromisoformat(metadata['createdAt'])
-            accessed_at = datetime.fromisoformat(metadata['accessedAt'])
-            modified_at = datetime.fromisoformat(metadata['modifiedAt'])
+        # Load metadata if it exists
+        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
+
+        if os.path.exists(metadata_filepath):
+            with open(metadata_filepath, encoding='utf-8') as f:
+                json_content = json.load(f)
+                resource_info = KeyValueStoreMetadata(**json_content)
+
+            id = resource_info.id
+            name = resource_info.name
+            created_at = resource_info.created_at
+            accessed_at = resource_info.accessed_at
+            modified_at = resource_info.modified_at
 
+        # Create new KVS client
         new_client = KeyValueStoreClient(
             base_storage_directory=memory_storage_client.key_value_stores_directory,
             memory_storage_client=memory_storage_client,
-            id_=id_,
+            id=id,
             name=name,
             accessed_at=accessed_at,
             created_at=created_at,
             modified_at=modified_at,
         )
 
-        # Scan the key value store folder, check each entry in there and parse it as a store record
+        # Scan the KVS folder, check each entry in there and parse it as a store record
         for entry in os.scandir(storage_directory):
             if not entry.is_file():
                 continue
 
             # Ignore metadata files on their own
             if entry.name.endswith('__metadata__.json'):
                 continue
 
-            with open(os.path.join(storage_directory, entry.name), 'rb') as f:
-                file_content = f.read()
-
             # Try checking if this file has a metadata file associated with it
-            metadata = None
-            if os.path.exists(os.path.join(storage_directory, entry.name + '.__metadata__.json')):
-                with open(
-                    os.path.join(storage_directory, entry.name + '.__metadata__.json'), encoding='utf-8'
-                ) as metadata_file:
-                    try:
-                        metadata = json.load(metadata_file)
-
-                        if metadata.get('key') is None:
-                            raise ValueError('Metadata missing required "key".')  # noqa: TRY301
+            record_metadata = None
+            record_metadata_filepath = os.path.join(storage_directory, f'{entry.name}.__metadata__.json')
 
-                        if metadata.get('contentType') is None:
-                            raise ValueError('Metadata missing required "contentType".')  # noqa: TRY301
+            if os.path.exists(record_metadata_filepath):
+                with open(record_metadata_filepath, encoding='utf-8') as metadata_file:
+                    try:
+                        json_content = json.load(metadata_file)
+                        record_metadata = KeyValueStoreRecordMetadata(**json_content)
 
                     except Exception:
                         logger.warning(
                             f'Metadata of key-value store entry "{entry.name}" for store {name or id} could '
                             'not be parsed. The metadata file will be ignored.',
                             exc_info=True,
                         )
 
-            if not metadata:
+            if not record_metadata:
                 content_type, _ = mimetypes.guess_type(entry.name)
                 if content_type is None:
                     content_type = 'application/octet-stream'
 
-                metadata = {
-                    'key': pathlib.Path(entry.name).stem,
-                    'contentType': content_type,
-                }
+                record_metadata = KeyValueStoreRecordMetadata(
+                    key=pathlib.Path(entry.name).stem,
+                    content_type=content_type,
+                )
+
+            with open(os.path.join(storage_directory, entry.name), 'rb') as f:
+                file_content = f.read()
 
             try:
-                maybe_parse_body(file_content, metadata['contentType'])
+                maybe_parse_body(file_content, record_metadata.content_type)
             except Exception:
-                metadata['contentType'] = 'application/octet-stream'
+                record_metadata.content_type = 'application/octet-stream'
                 logger.warning(
-                    f"""Key-value store entry "{metadata['key']}" for store {name or id} could not be parsed."""
+                    f'Key-value store entry "{record_metadata.key}" for store {name or id} could not be parsed.'
                     'The entry will be assumed as binary.',
                     exc_info=True,
                 )
 
-            new_client.records[metadata['key']] = KeyValueStoreRecord(
-                key=metadata['key'],
-                content_type=metadata['contentType'],
+            new_client.records[record_metadata.key] = KeyValueStoreRecord(
+                key=record_metadata.key,
+                content_type=record_metadata.content_type,
                 filename=entry.name,
                 value=file_content,
             )
 
         return new_client
 
     @override
-    async def get(self) -> KeyValueStoreResourceInfo | None:
+    async def get(self) -> KeyValueStoreMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if found:
             async with found.file_operation_lock:
                 await found.update_timestamps(has_been_modified=False)
                 return found.resource_info
 
         return None
 
-    async def update(self, *, name: str | None = None) -> KeyValueStoreResourceInfo:
+    async def update(self, *, name: str | None = None) -> KeyValueStoreMetadata:
         """Update the key-value store with specified fields.
 
         Args:
             name: The new name for key-value store
 
         Returns:
             The updated key-value store
         """
         # Check by id
         existing_store_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_store_by_id is None:
             raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
 
         # Skip if no changes
@@ -271,42 +270,42 @@
                     await aioshutil.rmtree(store.resource_directory)
 
     async def list_keys(
         self,
         *,
         limit: int = 1000,
         exclusive_start_key: str | None = None,
-    ) -> KeyValueStoreListKeysOutput:
+    ) -> KeyValueStoreListKeysPage:
         """List the keys in the key-value store.
 
         Args:
             limit: Number of keys to be returned. Maximum value is 1000.
             exclusive_start_key: All keys up to this one (including) are skipped from the result.
 
         Returns:
             The list of keys in the key-value store matching the given arguments.
         """
         # Check by id
         existing_store_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_store_by_id is None:
             raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
 
-        items: list[KeyValueStoreRecordInfo] = []
+        items: list[KeyValueStoreKeyInfo] = []
 
         for record in existing_store_by_id.records.values():
             size = len(record.value)
-            items.append(KeyValueStoreRecordInfo(key=record.key, size=size))
+            items.append(KeyValueStoreKeyInfo(key=record.key, size=size))
 
         if len(items) == 0:
-            return KeyValueStoreListKeysOutput(
+            return KeyValueStoreListKeysPage(
                 count=len(items),
                 limit=limit,
                 exclusive_start_key=exclusive_start_key,
                 is_truncated=False,
                 next_exclusive_start_key=None,
                 items=items,
             )
@@ -326,61 +325,23 @@
         last_selected_item = limited_items[-1]
         is_last_selected_item_absolutely_last = last_item_in_store == last_selected_item
         next_exclusive_start_key = None if is_last_selected_item_absolutely_last else last_selected_item.key
 
         async with existing_store_by_id.file_operation_lock:
             await existing_store_by_id.update_timestamps(has_been_modified=False)
 
-        return KeyValueStoreListKeysOutput(
+        return KeyValueStoreListKeysPage(
             count=len(items),
             limit=limit,
             exclusive_start_key=exclusive_start_key,
             is_truncated=not is_last_selected_item_absolutely_last,
             next_exclusive_start_key=next_exclusive_start_key,
             items=limited_items,
         )
 
-    async def _get_record_internal(
-        self,
-        key: str,
-        *,
-        as_bytes: bool = False,
-    ) -> KeyValueStoreRecord | None:
-        # Check by id
-        existing_store_by_id = self.find_or_create_client_by_id_or_name(
-            memory_storage_client=self._memory_storage_client,
-            id_=self.id,
-            name=self.name,
-        )
-
-        if existing_store_by_id is None:
-            raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
-
-        stored_record = existing_store_by_id.records.get(key)
-
-        if stored_record is None:
-            return None
-
-        record = KeyValueStoreRecord(
-            key=stored_record.key,
-            value=stored_record.value,
-            content_type=stored_record.content_type,
-        )
-
-        if not as_bytes:
-            try:
-                record.value = maybe_parse_body(record.value, str(record.content_type))
-            except ValueError:
-                logger.exception('Error parsing key-value store record')
-
-        async with existing_store_by_id.file_operation_lock:
-            await existing_store_by_id.update_timestamps(has_been_modified=False)
-
-        return record
-
     async def get_record(self, key: str) -> KeyValueStoreRecord | None:
         """Retrieve the given record from the key-value store.
 
         Args:
             key: Key of the record to retrieve
 
         Returns:
@@ -410,15 +371,15 @@
             key: The key of the record to save the value to
             value: The value to save into the record
             content_type: The content type of the saved value
         """
         # Check by id
         existing_store_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_store_by_id is None:
             raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
 
         if isinstance(value, io.IOBase):
@@ -434,66 +395,64 @@
 
         if 'application/json' in content_type and not is_file_or_bytes(value) and not isinstance(value, str):
             s = await json_dumps(value)
             value = s.encode('utf-8')
 
         async with existing_store_by_id.file_operation_lock:
             await existing_store_by_id.update_timestamps(has_been_modified=True)
-            record = KeyValueStoreRecord(
-                key=key,
-                value=value,
-                content_type=content_type,
-            )
+            record = KeyValueStoreRecord(key=key, value=value, content_type=content_type, filename=None)
 
             old_record = existing_store_by_id.records.get(key)
             existing_store_by_id.records[key] = record
 
             if self._memory_storage_client.persist_storage:
                 record_filename = self._filename_from_record(record)
+                record.filename = record_filename
 
                 if old_record is not None and self._filename_from_record(old_record) != record_filename:
                     await existing_store_by_id.delete_persisted_record(old_record)
 
                 await existing_store_by_id.persist_record(record)
 
     async def persist_record(self, record: KeyValueStoreRecord) -> None:
         """Persist the specified record to the key-value store."""
         store_directory = self.resource_directory
         record_filename = self._filename_from_record(record)
         record.filename = record_filename
+        record.content_type = record.content_type or 'application/octet-stream'
 
         # Ensure the directory for the entity exists
         await makedirs(store_directory, exist_ok=True)
 
         # Create files for the record
         record_path = os.path.join(store_directory, record_filename)
-        record_metadata_path = os.path.join(store_directory, record_filename + '.__metadata__.json')
+        record_metadata_path = os.path.join(store_directory, f'{record_filename}.__metadata__.json')
 
         # Convert to bytes if string
         if isinstance(record.value, str):
             record.value = record.value.encode('utf-8')
 
         async with aiofiles.open(record_path, mode='wb') as f:
             await f.write(record.value)
 
         if self._memory_storage_client.write_metadata:
             async with aiofiles.open(record_metadata_path, mode='wb') as f:
-                s = await json_dumps({'key': record.key, 'contentType': record.content_type})
-                await f.write(s.encode('utf-8'))
+                record_metadata = KeyValueStoreRecordMetadata(key=record.key, content_type=record.content_type)
+                await f.write(record_metadata.model_dump_json(indent=2).encode('utf-8'))
 
     async def delete_record(self, key: str) -> None:
         """Delete the specified record from the key-value store.
 
         Args:
             key: The key of the record which to delete
         """
         # Check by id
         existing_store_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_store_by_id is None:
             raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
 
         record = existing_store_by_id.records.get(key)
@@ -523,23 +482,59 @@
     async def update_timestamps(self, *, has_been_modified: bool) -> None:
         """Update the timestamps of the key-value store."""
         self._accessed_at = datetime.now(timezone.utc)
 
         if has_been_modified:
             self._modified_at = datetime.now(timezone.utc)
 
-        kv_store_info = self.resource_info
-        kv_store_info_as_dict = kv_store_info.__dict__
-
         await persist_metadata_if_enabled(
-            data=kv_store_info_as_dict,
+            data=self.resource_info.model_dump(),
             entity_directory=self.resource_directory,
             write_metadata=self._memory_storage_client.write_metadata,
         )
 
+    async def _get_record_internal(
+        self,
+        key: str,
+        *,
+        as_bytes: bool = False,
+    ) -> KeyValueStoreRecord | None:
+        # Check by id
+        existing_store_by_id = self.find_or_create_client_by_id_or_name(
+            memory_storage_client=self._memory_storage_client,
+            id=self.id,
+            name=self.name,
+        )
+
+        if existing_store_by_id is None:
+            raise_on_non_existing_storage(StorageTypes.KEY_VALUE_STORE, self.id)
+
+        stored_record = existing_store_by_id.records.get(key)
+
+        if stored_record is None:
+            return None
+
+        record = KeyValueStoreRecord(
+            key=stored_record.key,
+            value=stored_record.value,
+            content_type=stored_record.content_type,
+            filename=stored_record.filename,
+        )
+
+        if not as_bytes:
+            try:
+                record.value = maybe_parse_body(record.value, str(record.content_type))
+            except ValueError:
+                logger.exception('Error parsing key-value store record')
+
+        async with existing_store_by_id.file_operation_lock:
+            await existing_store_by_id.update_timestamps(has_been_modified=False)
+
+        return record
+
     def _filename_from_record(self, record: KeyValueStoreRecord) -> str:
         if record.filename is not None:
             return record.filename
 
         if not record.content_type or record.content_type == 'application/octet-stream':
             return record.key
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_collection_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_collection_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,57 @@
 
 from typing import TYPE_CHECKING
 
 from typing_extensions import override
 
 from crawlee.resource_clients.base_resource_collection_client import BaseResourceCollectionClient
 from crawlee.resource_clients.key_value_store_client import KeyValueStoreClient
+from crawlee.storages.models import KeyValueStoresListPage
 
 if TYPE_CHECKING:
-    from crawlee.storages.types import BaseResourceInfo, ListPage
+    from crawlee.storages.models import BaseStorageMetadata
 
 
 class KeyValueStoreCollectionClient(BaseResourceCollectionClient):
     """Sub-client for manipulating key-value stores."""
 
     @property
     @override
     def _client_class(self) -> type[KeyValueStoreClient]:
         return KeyValueStoreClient
 
     @override
     def _get_storage_client_cache(self) -> list[KeyValueStoreClient]:
         return self._memory_storage_client.key_value_stores_handled
 
-    async def list(self) -> ListPage:
-        """List the available key-value stores.
-
-        Returns:
-            The list of available key-value stores matching the specified filters.
-        """
-        return await super().list()
+    @override
+    async def list(self) -> KeyValueStoresListPage:
+        storage_client_cache = self._get_storage_client_cache()
+        items = [storage.resource_info for storage in storage_client_cache]
+
+        return KeyValueStoresListPage(
+            total=len(items),
+            count=len(items),
+            offset=0,
+            limit=len(items),
+            desc=False,
+            items=sorted(items, key=lambda item: item.created_at),
+        )
 
     async def get_or_create(
         self,
         *,
         name: str | None = None,
         schema: dict | None = None,
-        id_: str | None = None,
-    ) -> BaseResourceInfo:
+        id: str | None = None,
+    ) -> BaseStorageMetadata:
         """Retrieve a named key-value store, or create a new one when it doesn't exist.
 
         Args:
             name: The name of the key-value store to retrieve or create.
             schema: The schema of the key-value store
-            id_: The id of the key-value store to retrieve or create.
+            id: The id of the key-value store to retrieve or create.
 
         Returns:
             The retrieved or newly-created key-value store.
         """
-        return await super().get_or_create(name=name, schema=schema, id_=id_)
+        return await super().get_or_create(name=name, schema=schema, id=id)
```

### Comparing `crawlee-0.0.2/src/crawlee/resource_clients/request_queue_client.py` & `crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,70 +15,61 @@
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.data_processing import (
     filter_out_none_values_recursively,
     raise_on_duplicate_storage,
     raise_on_non_existing_storage,
 )
-from crawlee._utils.file import (
-    force_remove,
-    force_rename,
-    json_dumps,
-    persist_metadata_if_enabled,
-)
+from crawlee._utils.file import force_remove, force_rename, json_dumps, persist_metadata_if_enabled
 from crawlee._utils.requests import unique_key_to_request_id
 from crawlee.request import Request
 from crawlee.resource_clients.base_resource_client import BaseResourceClient
-from crawlee.storages.types import (
-    RequestQueueHeadResponse,
-    RequestQueueOperationInfo,
-    RequestQueueResourceInfo,
-    StorageTypes,
-)
+from crawlee.storages.models import RequestQueueHead, RequestQueueMetadata, RequestQueueOperationInfo
+from crawlee.types import StorageTypes
 
 if TYPE_CHECKING:
     from crawlee.storage_clients import MemoryStorageClient
 
 
 class RequestQueueClient(BaseResourceClient):
     """Sub-client for manipulating a single request queue."""
 
     def __init__(
         self,
         *,
         base_storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
         created_at: datetime | None = None,
         accessed_at: datetime | None = None,
         modified_at: datetime | None = None,
         handled_request_count: int = 0,
         pending_request_count: int = 0,
     ) -> None:
         self._base_storage_directory = base_storage_directory
         self._memory_storage_client = memory_storage_client
-        self.id = id_ or crypto_random_object_id()
+        self.id = id or crypto_random_object_id()
         self.name = name
         self._created_at = created_at or datetime.now(timezone.utc)
         self._accessed_at = accessed_at or datetime.now(timezone.utc)
         self._modified_at = modified_at or datetime.now(timezone.utc)
         self.handled_request_count = handled_request_count
         self.pending_request_count = pending_request_count
 
         self.resource_directory = os.path.join(base_storage_directory, name or self.id)
         self.requests = ValueSortedDict(lambda request: request.order_no or -float('inf'))
         self.file_operation_lock = asyncio.Lock()
         self._last_used_timestamp = Decimal(0.0)
 
     @property
     @override
-    def resource_info(self) -> RequestQueueResourceInfo:
+    def resource_info(self) -> RequestQueueMetadata:
         """Get the resource info for the request queue client."""
-        return RequestQueueResourceInfo(
+        return RequestQueueMetadata(
             id=str(self.id),
             name=str(self.name),
             accessed_at=self._accessed_at,
             created_at=self._created_at,
             modified_at=self._modified_at,
             had_multiple_clients=False,
             handled_request_count=self.handled_request_count,
@@ -101,92 +92,101 @@
 
     @classmethod
     @override
     def _create_from_directory(
         cls,
         storage_directory: str,
         memory_storage_client: MemoryStorageClient,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> RequestQueueClient:
         created_at = datetime.now(timezone.utc)
         accessed_at = datetime.now(timezone.utc)
         modified_at = datetime.now(timezone.utc)
         handled_request_count = 0
         pending_request_count = 0
-        entries: list[dict] = []
 
-        # Access the request queue folder
+        # Load metadata if it exists
+        metadata_filepath = os.path.join(storage_directory, '__metadata__.json')
+
+        if os.path.exists(metadata_filepath):
+            with open(metadata_filepath, encoding='utf-8') as f:
+                json_content = json.load(f)
+                resource_info = RequestQueueMetadata(**json_content)
+
+            id = resource_info.id
+            name = resource_info.name
+            created_at = resource_info.created_at
+            accessed_at = resource_info.accessed_at
+            modified_at = resource_info.modified_at
+            handled_request_count = resource_info.handled_request_count
+            pending_request_count = resource_info.pending_request_count
+
+        # Load request entries
+        entries: dict[str, Request] = {}
+
         for entry in os.scandir(storage_directory):
             if entry.is_file():
                 if entry.name == '__metadata__.json':
-                    # We have found the queue's metadata file, build out information based on it
-                    with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                        metadata = json.load(f)
-
-                    id_ = metadata['id']
-                    name = metadata['name']
-                    created_at = datetime.fromisoformat(metadata['createdAt'])
-                    accessed_at = datetime.fromisoformat(metadata['accessedAt'])
-                    modified_at = datetime.fromisoformat(metadata['modifiedAt'])
-                    handled_request_count = metadata['handledRequestCount']
-                    pending_request_count = metadata['pendingRequestCount']
                     continue
 
                 with open(os.path.join(storage_directory, entry.name), encoding='utf-8') as f:
-                    request = json.load(f)
-                    if request.order_no:
-                        request.order_no = Decimal(request.order_no)
-                entries.append(request)
+                    content = json.load(f)
 
-        new_client = cls(
+                request = Request(**content)
+                order_no = request.order_no
+                if order_no:
+                    request.order_no = Decimal(order_no)
+
+                entries[request.id] = request
+
+        # Create new RQ client
+        new_client = RequestQueueClient(
             base_storage_directory=memory_storage_client.request_queues_directory,
             memory_storage_client=memory_storage_client,
-            id_=id_,
+            id=id,
             name=name,
             accessed_at=accessed_at,
             created_at=created_at,
             modified_at=modified_at,
             handled_request_count=handled_request_count,
             pending_request_count=pending_request_count,
         )
 
-        for request in entries:
-            new_client.requests[request['id']] = request
-
+        new_client.requests.update(entries)
         return new_client
 
     @override
-    async def get(self) -> RequestQueueResourceInfo | None:
+    async def get(self) -> RequestQueueMetadata | None:
         found = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if found:
             async with found.file_operation_lock:
                 await found.update_timestamps(has_been_modified=False)
                 return found.resource_info
 
         return None
 
-    async def update(self, *, name: str | None = None) -> RequestQueueResourceInfo:
+    async def update(self, *, name: str | None = None) -> RequestQueueMetadata:
         """Update the request queue with specified fields.
 
         Args:
             name: The new name for the request queue
 
         Returns:
             The updated request queue
         """
         # Check by id
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         # Skip if no changes
@@ -234,26 +234,26 @@
                 queue.pending_request_count = 0
                 queue.handled_request_count = 0
                 queue.requests.clear()
 
                 if os.path.exists(queue.resource_directory):
                     await aioshutil.rmtree(queue.resource_directory)
 
-    async def list_head(self, *, limit: int | None = None) -> RequestQueueHeadResponse:
+    async def list_head(self, *, limit: int | None = None) -> RequestQueueHead:
         """Retrieve a given number of requests from the beginning of the queue.
 
         Args:
             limit: How many requests to retrieve
 
         Returns:
             The desired number of requests from the beginning of the queue.
         """
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         async with existing_queue_by_id.file_operation_lock:
@@ -275,15 +275,15 @@
                 # Check that the request still exists and was not handled,
                 # in case something deleted it or marked it as handled concurrenctly
                 if request and request.order_no:
                     requests.append(request)
 
             items = [request for item in requests if (request := self._json_to_request(item.json_))]
 
-            return RequestQueueHeadResponse(
+            return RequestQueueHead(
                 limit=limit,
                 had_multiple_clients=False,
                 queue_modified_at=existing_queue_by_id._modified_at,  # noqa: SLF001
                 items=items,
             )
 
     async def add_request(
@@ -299,15 +299,15 @@
             forefront: Whether to add the request to the head or the end of the queue
 
         Returns:
             The added request.
         """
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         request_model = await self._create_internal_request(request, forefront)
@@ -354,15 +354,15 @@
             request_id: ID of the request to retrieve
 
         Returns:
             The retrieved request, or None, if it did not exist.
         """
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         async with existing_queue_by_id.file_operation_lock:
@@ -384,15 +384,15 @@
             forefront: Whether to put the updated request in the beginning or the end of the queue
 
         Returns:
             The updated request
         """
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         request_model = await self._create_internal_request(request, forefront)
@@ -438,15 +438,15 @@
         """Delete a request from the queue.
 
         Args:
             request_id: ID of the request to delete.
         """
         existing_queue_by_id = self.find_or_create_client_by_id_or_name(
             memory_storage_client=self._memory_storage_client,
-            id_=self.id,
+            id=self.id,
             name=self.name,
         )
 
         if existing_queue_by_id is None:
             raise_on_non_existing_storage(StorageTypes.REQUEST_QUEUE, self.id)
 
         async with existing_queue_by_id.file_operation_lock:
@@ -488,15 +488,15 @@
 
         # Ensure the directory for the entity exists
         await makedirs(entity_directory, exist_ok=True)
 
         # Write the request to the file
         file_path = os.path.join(entity_directory, f'{request.id}.json')
         async with aiofiles.open(file_path, mode='wb') as f:
-            s = await json_dumps(request)
+            s = await json_dumps(request.model_dump())
             await f.write(s.encode('utf-8'))
 
     async def _delete_request_file_from_storage(self, *, request_id: str, entity_directory: str) -> None:
         """Deletes a specific request item from the disk.
 
         This function removes a file representing a request, identified by the request's ID, from a
         specified directory. Before attempting to remove the file, it ensures that the target directory
@@ -515,43 +515,40 @@
     async def update_timestamps(self, *, has_been_modified: bool) -> None:
         """Update the timestamps of the request queue."""
         self._accessed_at = datetime.now(timezone.utc)
 
         if has_been_modified:
             self._modified_at = datetime.now(timezone.utc)
 
-        request_queue_info = self.resource_info
-        request_queue_info_as_dict = request_queue_info.__dict__
-
         await persist_metadata_if_enabled(
-            data=request_queue_info_as_dict,
+            data=self.resource_info.model_dump(),
             entity_directory=self.resource_directory,
             write_metadata=self._memory_storage_client.write_metadata,
         )
 
     def _json_to_request(self, request_json: str | None) -> Request | None:
         if request_json is None:
             return None
         request_dict = filter_out_none_values_recursively(json.loads(request_json))
         if request_dict is None:
             return None
         return Request(**request_dict)
 
     async def _create_internal_request(self, request: Request, forefront: bool | None) -> Request:
         order_no = self._calculate_order_no(request, forefront)
-        id_ = unique_key_to_request_id(request.unique_key)
+        id = unique_key_to_request_id(request.unique_key)
 
-        if request.id is not None and request.id != id_:
+        if request.id is not None and request.id != id:
             raise ValueError('Request ID does not match its unique_key.')
 
-        json_request = await json_dumps({**(request.__dict__), 'id': id_})
+        json_request = await json_dumps({**(request.model_dump()), 'id': id})
         return Request(
             url=request.url,
             unique_key=request.unique_key,
-            id=id_,
+            id=id,
             method=request.method,
             retry_count=request.retry_count,
             order_no=order_no,
             json_=json_request,
         )
 
     def _calculate_order_no(self, request: Request, forefront: bool | None) -> Decimal | None:
```

### Comparing `crawlee-0.0.2/src/crawlee/storage_client_manager.py` & `crawlee-0.0.3b1/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/storage_clients/base_storage_client.py` & `crawlee-0.0.3b1/src/crawlee/storage_clients/base_storage_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
     """Defines an abstract base for storage clients.
 
     It offers interfaces to get clients for interacting with storage resources like datasets, key-value stores,
     and request queues.
     """
 
     @abstractmethod
-    def dataset(self, id_: str) -> DatasetClient:
+    def dataset(self, id: str) -> DatasetClient:
         """Gets a client for a specific dataset by its ID."""
 
     @abstractmethod
     def datasets(self) -> DatasetCollectionClient:
         """Gets a client for dataset collection operations."""
 
     @abstractmethod
-    def key_value_store(self, id_: str) -> KeyValueStoreClient:
+    def key_value_store(self, id: str) -> KeyValueStoreClient:
         """Gets a client for a specific key-value store by its ID."""
 
     @abstractmethod
     def key_value_stores(self) -> KeyValueStoreCollectionClient:
         """Gets a client for key-value store collection operations."""
 
     @abstractmethod
-    def request_queue(self, id_: str) -> RequestQueueClient:
+    def request_queue(self, id: str) -> RequestQueueClient:
         """Gets a client for a specific request queue by its ID."""
 
     @abstractmethod
     def request_queues(self) -> RequestQueueCollectionClient:
         """Gets a client for request queue collection operations."""
```

### Comparing `crawlee-0.0.2/src/crawlee/storage_clients/memory_storage_client.py` & `crawlee-0.0.3b1/src/crawlee/storage_clients/memory_storage_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,49 +82,49 @@
 
     @property
     def request_queues_directory(self) -> str:
         """Path to the directory containing request queues."""
         return os.path.join(self._local_data_directory, 'request_queues')
 
     @override
-    def dataset(self, id_: str) -> DatasetClient:
+    def dataset(self, id: str) -> DatasetClient:
         return DatasetClient(
             base_storage_directory=self.datasets_directory,
             memory_storage_client=self,
-            id_=id_,
+            id=id,
         )
 
     @override
     def datasets(self) -> DatasetCollectionClient:
         return DatasetCollectionClient(
             base_storage_directory=self.datasets_directory,
             memory_storage_client=self,
         )
 
     @override
-    def key_value_store(self, id_: str) -> KeyValueStoreClient:
+    def key_value_store(self, id: str) -> KeyValueStoreClient:
         return KeyValueStoreClient(
             base_storage_directory=self.key_value_stores_directory,
             memory_storage_client=self,
-            id_=id_,
+            id=id,
         )
 
     @override
     def key_value_stores(self) -> KeyValueStoreCollectionClient:
         return KeyValueStoreCollectionClient(
             base_storage_directory=self.key_value_stores_directory,
             memory_storage_client=self,
         )
 
     @override
-    def request_queue(self, id_: str) -> RequestQueueClient:
+    def request_queue(self, id: str) -> RequestQueueClient:
         return RequestQueueClient(
             base_storage_directory=self.request_queues_directory,
             memory_storage_client=self,
-            id_=id_,
+            id=id,
         )
 
     @override
     def request_queues(self) -> RequestQueueCollectionClient:
         return RequestQueueCollectionClient(
             base_storage_directory=self.request_queues_directory,
             memory_storage_client=self,
```

### Comparing `crawlee-0.0.2/src/crawlee/storages/base_storage.py` & `crawlee-0.0.3b1/src/crawlee/storages/base_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from abc import ABC, abstractmethod
+from logging import getLogger
 from typing import TYPE_CHECKING, Generic, TypeVar, cast
 
 from typing_extensions import Self
 
 from crawlee.configuration import Configuration
 
 if TYPE_CHECKING:
@@ -15,65 +16,67 @@
 
     BaseResourceClientType = TypeVar('BaseResourceClientType', bound=BaseResourceClient)
     BaseResourceCollectionClientType = TypeVar('BaseResourceCollectionClientType', bound=BaseResourceCollectionClient)
 else:
     BaseResourceClientType = TypeVar('BaseResourceClientType')
     BaseResourceCollectionClientType = TypeVar('BaseResourceCollectionClientType')
 
+logger = getLogger(__name__)
+
 
 class BaseStorage(ABC, Generic[BaseResourceClientType, BaseResourceCollectionClientType]):
     """A class for managing storages."""
 
     _purge_on_start: bool
     cache_by_id: dict | None = None
     cache_by_name: dict | None = None
     _storage_creating_lock: asyncio.Lock | None = None
 
     def __init__(
         self,
-        id_: str,
+        id: str,
         name: str | None,
         configuration: Configuration,
         client: MemoryStorageClient,
     ) -> None:
         """Create a new instance.
 
         Args:
-            id_: ID of the storage.
+            id: ID of the storage.
             name: Name of the storage.
             configuration: The configuration settings.
             client: The underlying storage client to be used.
         """
-        self.id = id_
+        self.id = id
         self._name = name
         self._configuration = configuration
         self._storage_client = client
 
     @property
     def name(self) -> str | None:
         """Name of the storage."""
         return self._name
 
     @classmethod
     async def open(
         cls,
         *,
         configuration: Configuration | None = None,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
     ) -> Self:
         """Opens a storage instance based on provided identifiers or returns a previously opened instance from cache.
 
         This method facilitates the retrieval or initialization of a storage instance using specified configuration
         details. If an instance corresponding to the given `id` or `name` was previously opened, this method returns
         the cached instance. Otherwise, it initializes a new storage instance. When neither `id` nor `name` is provided,
         the default storage associated with the current actor run is utilized.
 
         Args:
-            id_: Identifier for the specific storage to open. An error is raised if no matching storage is found.
+            id: Identifier for the specific storage to open. An error is raised if no matching storage is found.
             name: Name for the specific storage to open or create.
             configuration: Configuration instance to use. If omitted, the global configuration is applied.
 
         Returns:
             The opened or retrieved storage instance.
         """
         from crawlee.storage_client_manager import StorageClientManager
@@ -83,31 +86,31 @@
 
         if cls.cache_by_id is None:
             raise AttributeError("The 'cache_by_id' attribute must not be None.")
 
         if cls.cache_by_name is None:
             raise AttributeError("The 'cache_by_name' attribute must not be None.")
 
-        if id_ and name:
-            raise ValueError("Either 'id_' or 'name' must be provided, not both.")
+        if id and name:
+            raise ValueError("Either 'id' or 'name' must be provided, not both.")
 
         used_config = configuration or Configuration()
         used_client = StorageClientManager.get_storage_client()
 
         is_default_storage_on_local = False
         # Fetch default ID if no ID or name was passed
-        if not id_ and not name:
+        if not id and not name:
             if isinstance(used_client, MemoryStorageClient):
                 is_default_storage_on_local = True
-            id_ = cls._get_default_id(used_config)
+            id = cls._get_default_id(used_config)
 
         # Try to get the storage instance from cache
         cached_storage = None
-        if id_:
-            cached_storage = cls.cache_by_id.get(id_)
+        if id:
+            cached_storage = cls.cache_by_id.get(id)
         elif name:
             cached_storage = cls.cache_by_name.get(name)
 
         if cached_storage is not None:
             # This cast is needed since MyPy doesn't understand very well that Self and Storage are the same
             return cast(Self, cached_storage)
 
@@ -116,29 +119,29 @@
             await used_client.purge_on_start()
 
         if cls._storage_creating_lock is None:
             raise AttributeError('cls._storage_creating_lock must be initialized before calling open.')
 
         async with cls._storage_creating_lock:
             # Create the storage
-            if id_ and not is_default_storage_on_local:
-                single_storage_client = cls._get_single_storage_client(id_, used_client)
+            if id and not is_default_storage_on_local:
+                single_storage_client = cls._get_single_storage_client(id, used_client)
                 storage_info = await single_storage_client.get()
                 if not storage_info:
                     storage_label = cls._get_human_friendly_label()
-                    raise RuntimeError(f'{storage_label} with id "{id_}" does not exist!')
+                    raise RuntimeError(f'{storage_label} with id "{id}" does not exist!')
             elif is_default_storage_on_local:
                 storage_collection_client = cls._get_storage_collection_client(used_client)
-                storage_info = await storage_collection_client.get_or_create(name=name, id_=id_)
+                storage_info = await storage_collection_client.get_or_create(name=name, id=id)
             else:
                 storage_collection_client = cls._get_storage_collection_client(used_client)
                 storage_info = await storage_collection_client.get_or_create(name=name)
 
             storage = cls(
-                id_=storage_info.id,
+                id=storage_info.id,
                 name=storage_info.name,
                 configuration=used_config,
                 client=used_client,
             )
 
             # Cache by id and name
             cls.cache_by_id[storage.id] = storage
@@ -155,15 +158,15 @@
     @classmethod
     @abstractmethod
     def _get_default_id(cls, configuration: Configuration) -> str:
         """Get the default storage ID."""
 
     @classmethod
     @abstractmethod
-    def _get_single_storage_client(cls, id_: str, client: MemoryStorageClient) -> BaseResourceClientType:
+    def _get_single_storage_client(cls, id: str, client: MemoryStorageClient) -> BaseResourceClientType:
         """Get the single storage client for the given ID."""
 
     @classmethod
     @abstractmethod
     def _get_storage_collection_client(cls, client: MemoryStorageClient) -> BaseResourceCollectionClientType:
         """Get the storage collection client."""
 
@@ -174,11 +177,17 @@
         if cls.cache_by_name is None:
             cls.cache_by_name = {}
         if cls._storage_creating_lock is None:
             cls._storage_creating_lock = asyncio.Lock()
 
     def _remove_from_cache(self) -> None:
         if self.__class__.cache_by_id is not None:
-            del self.__class__.cache_by_id[self.id]
+            try:
+                del self.__class__.cache_by_id[self.id]
+            except KeyError as exc:
+                raise RuntimeError(f'Storage with provided ID was not found ({self.id}).') from exc
 
         if self.name and self.__class__.cache_by_name is not None:
-            del self.__class__.cache_by_name[self.name]
+            try:
+                del self.__class__.cache_by_name[self.name]
+            except KeyError as exc:
+                raise RuntimeError(f'Storage with provided name was not found ({self.name}).') from exc
```

### Comparing `crawlee-0.0.2/src/crawlee/storages/dataset.py` & `crawlee-0.0.3b1/src/crawlee/storages/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,69 +11,70 @@
 from crawlee.storages.base_storage import BaseStorage
 from crawlee.storages.key_value_store import KeyValueStore
 
 if TYPE_CHECKING:
     from crawlee.configuration import Configuration
     from crawlee.resource_clients import DatasetClient, DatasetCollectionClient
     from crawlee.storage_clients import MemoryStorageClient
-    from crawlee.storages.types import DatasetResourceInfo, JSONSerializable, ListPage
+    from crawlee.storages.models import DatasetItemsListPage, DatasetMetadata
+    from crawlee.types import JSONSerializable
 
 
 class Dataset(BaseStorage):
     """Represents an append-only structured storage, ideal for tabular data akin to database tables.
 
     Represents a structured data store similar to a table, where each object (row) has consistent attributes (columns).
     Datasets operate on an append-only basis, allowing for the addition of new records without the modification or
     removal of existing ones. This class is typically used for storing crawling results.
 
     Data can be stored locally or in the cloud, with local storage paths formatted as:
     `{CRAWLEE_LOCAL_STORAGE_DIR}/datasets/{DATASET_ID}/{INDEX}.json`. Here, `{DATASET_ID}` is either "default" or
     a specific dataset ID, and `{INDEX}` represents the zero-based index of the item in the dataset.
 
-    To open a dataset, use the `open` class method with an `id_`, `name`, or `config`. If unspecified, the default
-    dataset for the current crawler run is used. Opening a non-existent dataset by `id_` raises an error, while
+    To open a dataset, use the `open` class method with an `id`, `name`, or `config`. If unspecified, the default
+    dataset for the current crawler run is used. Opening a non-existent dataset by `id` raises an error, while
     by `name`, it is created.
 
     Usage:
-        dataset = await Dataset.open(id_='my_dataset_id')
+        dataset = await Dataset.open(id='my_dataset_id')
     """
 
     _MAX_PAYLOAD_SIZE = ByteSize.from_mb(9)
     """Maximum size for a single payload."""
 
     _SAFETY_BUFFER_PERCENT = 0.01 / 100  # 0.01%
     """Percentage buffer to reduce payload limit slightly for safety."""
 
     _EFFECTIVE_LIMIT_SIZE = _MAX_PAYLOAD_SIZE - (_MAX_PAYLOAD_SIZE * _SAFETY_BUFFER_PERCENT)
     """Calculated payload limit considering safety buffer."""
 
     def __init__(
         self,
-        id_: str,
+        id: str,
         name: str | None,
         configuration: Configuration,
         client: MemoryStorageClient,
     ) -> None:
-        super().__init__(id_=id_, name=name, client=client, configuration=configuration)
+        super().__init__(id=id, name=name, client=client, configuration=configuration)
         self._dataset_client = client.dataset(self.id)
 
     @classmethod
     @override
     def _get_human_friendly_label(cls) -> str:
         return 'Dataset'
 
     @classmethod
     @override
     def _get_default_id(cls, configuration: Configuration) -> str:
         return configuration.default_dataset_id
 
     @classmethod
     @override
-    def _get_single_storage_client(cls, id_: str, client: MemoryStorageClient) -> DatasetClient:
-        return client.dataset(id_)
+    def _get_single_storage_client(cls, id: str, client: MemoryStorageClient) -> DatasetClient:
+        return client.dataset(id)
 
     @classmethod
     @override
     def _get_storage_collection_client(cls, client: MemoryStorageClient) -> DatasetCollectionClient:
         return client.datasets()
 
     async def push_data(self, data: JSONSerializable) -> None:
@@ -111,15 +112,15 @@
         fields: list[str] | None = None,
         omit: list[str] | None = None,
         unwind: str | None = None,
         skip_empty: bool = False,
         skip_hidden: bool = False,
         flatten: list[str] | None = None,
         view: str | None = None,
-    ) -> ListPage:
+    ) -> DatasetItemsListPage:
         """Retrieves dataset items based on filtering, sorting, and pagination parameters.
 
         This method allows customization of the data retrieval process from a dataset, supporting operations such as
         field selection, ordering, and skipping specific records based on provided parameters.
 
         Args:
             offset: Skips the specified number of items at the start.
@@ -131,15 +132,15 @@
             unwind: Unwinds items by a specified array field, turning each element into a separate item.
             skip_empty: Excludes empty items from the results if True.
             skip_hidden: Excludes fields starting with '#' if True.
             flatten: Fields to be flattened in returned items.
             view: Specifies the dataset view to be used.
 
         Returns:
-            ListPage containing filtered and paginated dataset items.
+            List page containing filtered and paginated dataset items.
         """
         # TODO: Improve error handling here
         # https://github.com/apify/apify-sdk-python/issues/140
         return await self._dataset_client.list_items(
             offset=offset,
             limit=limit,
             desc=desc,
@@ -207,15 +208,15 @@
         await self._export_to(
             key,
             to_key_value_store_id=to_key_value_store_id,
             to_key_value_store_name=to_key_value_store_name,
             content_type='text/csv',
         )
 
-    async def get_info(self) -> DatasetResourceInfo | None:
+    async def get_info(self) -> DatasetMetadata | None:
         """Get an object containing general information about the dataset.
 
         Returns:
             Object returned by calling the GET dataset API endpoint.
         """
         return await self._dataset_client.get()
 
@@ -286,15 +287,15 @@
 
             to_key_value_store_name: The name of the key-value store in which the result will be saved. You must
                 specify only one of `to_key_value_store_id` and `to_key_value_store_name` arguments. If you omit both,
                 it uses the default key-value store.
 
             content_type: Either 'text/csv' or 'application/json'. Defaults to JSON.
         """
-        key_value_store = await KeyValueStore.open(id_=to_key_value_store_id, name=to_key_value_store_name)
+        key_value_store = await KeyValueStore.open(id=to_key_value_store_id, name=to_key_value_store_name)
         items: list[dict] = []
         limit = 1000
         offset = 0
         while True:
             list_items = await self._dataset_client.list_items(limit=limit, offset=offset)
             items.extend(list_items.items)
             if list_items.total <= offset + list_items.count:
```

### Comparing `crawlee-0.0.2/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.3b1/src/crawlee/storages/key_value_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, AsyncIterator, TypeVar, overload
 
 from typing_extensions import override
 
 from crawlee.storages.base_storage import BaseStorage
-from crawlee.storages.types import KeyValueStoreRecordInfo
+from crawlee.storages.models import KeyValueStoreKeyInfo
 
 if TYPE_CHECKING:
     from crawlee.configuration import Configuration
     from crawlee.resource_clients import KeyValueStoreClient, KeyValueStoreCollectionClient
     from crawlee.storage_clients import MemoryStorageClient
 
 T = TypeVar('T')
@@ -24,46 +24,46 @@
     The data can be stored on a local filesystem or in the cloud, determined by the `CRAWLEE_LOCAL_STORAGE_DIR`
     environment variable.
 
     By default, data is stored in `{CRAWLEE_LOCAL_STORAGE_DIR}/key_value_stores/{STORE_ID}/{INDEX}.{EXT}`, where
     `{STORE_ID}` is either "default" or specified by `CRAWLEE_DEFAULT_KEY_VALUE_STORE_ID`, `{KEY}` is the record key,
     and `{EXT}` is the MIME type.
 
-    To open a key-value store, use the class method `open`, providing either an `id_` or `name` along with optional
+    To open a key-value store, use the class method `open`, providing either an `id` or `name` along with optional
     `config`. If neither is provided, the default store for the crawler run is used. Opening a non-existent store by
-    `id_` raises an error, while a non-existent store by `name` is created.
+    `id` raises an error, while a non-existent store by `name` is created.
 
     Usage:
-        kvs = await KeyValueStore.open(id_='my_kvs_id')
+        kvs = await KeyValueStore.open(id='my_kvs_id')
     """
 
     def __init__(
         self,
-        id_: str,
+        id: str,
         name: str | None,
         configuration: Configuration,
         client: MemoryStorageClient,
     ) -> None:
-        super().__init__(id_=id_, name=name, client=client, configuration=configuration)
+        super().__init__(id=id, name=name, client=client, configuration=configuration)
         self._key_value_store_client = client.key_value_store(self.id)
 
     @classmethod
     @override
     def _get_human_friendly_label(cls) -> str:
         return 'Key-value store'
 
     @classmethod
     @override
     def _get_default_id(cls, configuration: Configuration) -> str:
         return configuration.default_key_value_store_id
 
     @classmethod
     @override
-    def _get_single_storage_client(cls, id_: str, client: MemoryStorageClient) -> KeyValueStoreClient:
-        return client.key_value_store(id_)
+    def _get_single_storage_client(cls, id: str, client: MemoryStorageClient) -> KeyValueStoreClient:
+        return client.key_value_store(id)
 
     @classmethod
     @override
     def _get_storage_collection_client(cls, client: MemoryStorageClient) -> KeyValueStoreCollectionClient:
         return client.key_value_stores()
 
     @overload
@@ -84,28 +84,27 @@
 
         Returns:
             Any: The value associated with the given key. `default_value` is used in case the record does not exist.
         """
         record = await self._key_value_store_client.get_record(key)
         return record.value if record else default_value
 
-    async def iterate_keys(self, exclusive_start_key: str | None = None) -> AsyncIterator[KeyValueStoreRecordInfo]:
+    async def iterate_keys(self, exclusive_start_key: str | None = None) -> AsyncIterator[KeyValueStoreKeyInfo]:
         """Iterate over the keys in the key-value store.
 
         Args:
             exclusive_start_key: All keys up to this one (including) are skipped from the result.
 
         Yields:
-            An object, where `key` is the record key, and `info` is an object that contains a single property `size`
-                indicating size of the record.
+            Information about a key-value store record.
         """
         while True:
             list_keys = await self._key_value_store_client.list_keys(exclusive_start_key=exclusive_start_key)
             for item in list_keys.items:
-                yield KeyValueStoreRecordInfo(key=item.key, size=item.size)
+                yield KeyValueStoreKeyInfo(key=item.key, size=item.size)
 
             if not list_keys.is_truncated:
                 break
             exclusive_start_key = list_keys.next_exclusive_start_key
 
     async def set_value(
         self,
```

### Comparing `crawlee-0.0.2/src/crawlee/storages/request_list.py` & `crawlee-0.0.3b1/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.2/src/crawlee/storages/request_provider.py` & `crawlee-0.0.3b1/src/crawlee/storages/request_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
     from crawlee.request import BaseRequestData, Request
-    from crawlee.storages.types import RequestQueueOperationInfo
+    from crawlee.storages.models import RequestQueueOperationInfo
 
 
 class RequestProvider(ABC):
     """Provides access to a queue of crawling requests."""
 
     @property
     @abstractmethod
```

### Comparing `crawlee-0.0.2/src/crawlee/storages/request_queue.py` & `crawlee-0.0.3b1/src/crawlee/storages/request_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 from typing_extensions import override
 
 from crawlee._utils.crypto import crypto_random_object_id
 from crawlee._utils.lru_cache import LRUCache
 from crawlee._utils.requests import unique_key_to_request_id
 from crawlee.request import Request
 from crawlee.storages.base_storage import BaseStorage
+from crawlee.storages.models import RequestQueueHeadState, RequestQueueOperationInfo
 from crawlee.storages.request_provider import RequestProvider
-from crawlee.storages.types import BaseResourceInfo, RequestQueueOperationInfo, RequestQueueSnapshot
 
 if TYPE_CHECKING:
     from crawlee.configuration import Configuration
     from crawlee.request import BaseRequestData
     from crawlee.resource_clients import RequestQueueClient, RequestQueueCollectionClient
     from crawlee.storage_clients import MemoryStorageClient
+    from crawlee.storages.models import BaseStorageMetadata
 
 logger = getLogger(__name__)
 
 
 class RequestQueue(BaseStorage, RequestProvider):
     """Represents a queue storage for HTTP requests to crawl.
 
@@ -39,15 +40,15 @@
     queue's ID (default or specified) and `{REQUEST_ID}` is the request's ID.
 
     Usage includes creating or opening existing queues by ID or name, with named queues retained indefinitely and
     unnamed queues expiring after 7 days unless specified otherwise. Supports mutable operations—URLs can be added
     and deleted.
 
     Usage:
-        rq = await RequestQueue.open(id_='my_rq_id')
+        rq = await RequestQueue.open(id='my_rq_id')
     """
 
     _API_PROCESSED_REQUESTS_DELAY = timedelta(seconds=10)
     """Delay threshold to assume consistency of queue head operations after queue modifications."""
 
     _MAX_CACHED_REQUESTS = 1_000_000
     """Maximum number of requests that can be cached."""
@@ -68,20 +69,20 @@
     """Cache size for recently handled requests."""
 
     _STORAGE_CONSISTENCY_DELAY = timedelta(seconds=3)
     """Expected delay for storage to achieve consistency, guiding the timing of subsequent read operations."""
 
     def __init__(
         self,
-        id_: str,
+        id: str,
         name: str | None,
         configuration: Configuration,
         client: MemoryStorageClient,
     ) -> None:
-        super().__init__(id_=id_, name=name, client=client, configuration=configuration)
+        super().__init__(id=id, name=name, client=client, configuration=configuration)
 
         self._client_key = crypto_random_object_id()
         self._internal_timeout_seconds = 5 * 60
         self._assumed_total_count = 0
         self._assumed_handled_count = 0
         self._request_queue_client = client.request_queue(self.id)
         self._queue_head_dict: OrderedDictType[str, str] = OrderedDict()
@@ -92,19 +93,19 @@
         self._requests_cache: LRUCache[dict] = LRUCache(max_length=self._MAX_CACHED_REQUESTS)
 
     @classmethod
     @override
     async def open(
         cls,
         *,
-        id_: str | None = None,
+        id: str | None = None,
         name: str | None = None,
         configuration: Configuration | None = None,
     ) -> RequestQueue:
-        rq = await super().open(id_=id_, name=name, configuration=configuration)
+        rq = await super().open(id=id, name=name, configuration=configuration)
         await rq.ensure_head_is_non_empty()
         return rq
 
     @classmethod
     @override
     def _get_human_friendly_label(cls) -> str:
         return 'Request queue'
@@ -114,18 +115,18 @@
     def _get_default_id(cls, configuration: Configuration) -> str:
         return configuration.default_request_queue_id
 
     @classmethod
     @override
     def _get_single_storage_client(
         cls,
-        id_: str,
+        id: str,
         client: MemoryStorageClient,
     ) -> RequestQueueClient:
-        return client.request_queue(id_)
+        return client.request_queue(id)
 
     @classmethod
     @override
     def _get_storage_collection_client(
         cls,
         client: MemoryStorageClient,
     ) -> RequestQueueCollectionClient:
@@ -418,15 +419,15 @@
         return is_head_consistent and len(self._queue_head_dict) == 0 and self._in_progress_count() == 0
 
     async def drop(self) -> None:
         """Remove the request queue either from the Apify cloud storage or from the local directory."""
         await self._request_queue_client.delete()
         self._remove_from_cache()
 
-    async def get_info(self) -> BaseResourceInfo | None:
+    async def get_info(self) -> BaseStorageMetadata | None:
         """Get an object containing general information about the request queue.
 
         Returns:
             Object returned by calling the GET request queue API endpoint.
         """
         return await self._request_queue_client.get()
 
@@ -452,15 +453,15 @@
 
         if limit is None:
             limit = max(self._in_progress_count() * self._QUERY_HEAD_BUFFER, self._QUERY_HEAD_MIN_LENGTH)
 
         if self._query_queue_head_task is None:
             self._query_queue_head_task = asyncio.Task(self._queue_query_head(limit))
 
-        queue_head: RequestQueueSnapshot = await self._query_queue_head_task
+        queue_head: RequestQueueHeadState = await self._query_queue_head_task
 
         # TODO: I feel this code below can be greatly simplified... (comes from TS implementation *wink*)
         # https://github.com/apify/apify-sdk-python/issues/142
 
         # If queue is still empty then one of the following holds:
         # - the other calls waiting for this task already consumed all the returned requests
         # - the limit was too low and contained only requests in progress
@@ -532,15 +533,15 @@
         self._requests_cache[cache_key] = {
             'id': operation_info.request_id,
             'isHandled': operation_info.was_already_handled,
             'uniqueKey': operation_info.request_unique_key,
             'wasAlreadyHandled': operation_info.was_already_handled,
         }
 
-    async def _queue_query_head(self, limit: int) -> RequestQueueSnapshot:
+    async def _queue_query_head(self, limit: int) -> RequestQueueHeadState:
         query_started_at = datetime.now(timezone.utc)
 
         list_head = await self._request_queue_client.list_head(limit=limit)
         list_head_items: list[Request] = list_head.items
 
         for request in list_head_items:
             # Queue head index might be behind the main table, so ensure we don't recycle requests
@@ -562,15 +563,15 @@
                     request_unique_key=request.unique_key,
                 ),
             )
 
         # This is needed so that the next call to _ensureHeadIsNonEmpty() will fetch the queue head again.
         self._query_queue_head_task = None
 
-        return RequestQueueSnapshot(
+        return RequestQueueHeadState(
             was_limit_reached=len(list_head.items) >= limit,
             prev_limit=limit,
             queue_modified_at=list_head.queue_modified_at,
             query_started_at=query_started_at,
             had_multiple_clients=list_head.had_multiple_clients,
         )
```

### Comparing `crawlee-0.0.2/PKG-INFO` & `crawlee-0.0.3b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.2
+Version: 0.0.3b1
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,25 +13,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: beautifulsoup
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aioshutil (>=1.3,<2.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ; extra == "beautifulsoup"
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: docutils (>=0.20.1,<0.21.0)
-Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0)
+Requires-Dist: docutils (>=0.21.0,<0.22.0)
+Requires-Dist: eval-type-backport (>=0.2.0,<0.3.0)
+Requires-Dist: html5lib (>=1.1,<2.0) ; extra == "beautifulsoup"
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0) ; extra == "beautifulsoup"
 Requires-Dist: more_itertools (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: sortedcollections (>=2.1.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/crawlee-py/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://todo.com/
 Project-URL: Homepage, https://todo.com/
 Project-URL: Issue Tracker, https://github.com/apify/crawlee-py/issues
```

