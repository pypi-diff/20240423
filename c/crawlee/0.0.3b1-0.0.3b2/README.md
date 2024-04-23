# Comparing `tmp/crawlee-0.0.3b1.tar.gz` & `tmp/crawlee-0.0.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.3b1.tar", max compression
+gzip compressed data, was "crawlee-0.0.3b2.tar", max compression
```

## Comparing `crawlee-0.0.3b1.tar` & `crawlee-0.0.3b2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11355 2024-01-15 10:43:27.602910 crawlee-0.0.3b1/LICENSE
--rw-r--r--   0        0        0       17 2024-04-15 12:48:32.824597 crawlee-0.0.3b1/README.md
--rw-r--r--   0        0        0     6331 2024-04-23 12:46:22.947137 crawlee-0.0.3b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 16:55:10.812444 crawlee-0.0.3b1/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.269919 crawlee-0.0.3b1/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-05 11:38:44.800791 crawlee-0.0.3b1/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-04-04 15:33:46.940733 crawlee-0.0.3b1/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-04-18 12:13:47.123107 crawlee-0.0.3b1/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-04-04 15:33:46.940733 crawlee-0.0.3b1/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-04-12 12:50:54.784754 crawlee-0.0.3b1/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     2056 2024-04-04 15:33:46.941733 crawlee-0.0.3b1/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-04-18 13:24:49.427217 crawlee-0.0.3b1/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-03-08 15:21:38.269919 crawlee-0.0.3b1/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1585 2024-04-12 12:51:35.336347 crawlee-0.0.3b1/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-04-04 15:33:46.941733 crawlee-0.0.3b1/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-04-05 11:38:44.800791 crawlee-0.0.3b1/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.270919 crawlee-0.0.3b1/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-04-18 14:10:07.138207 crawlee-0.0.3b1/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      186 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    14678 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     5315 2024-04-18 10:29:13.253131 crawlee-0.0.3b1/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2279 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0      815 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-04-18 10:29:13.253131 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     4017 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      462 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1246 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/configuration.py
--rw-r--r--   0        0        0       91 2024-04-10 13:42:23.139187 crawlee-0.0.3b1/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2683 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.3b1/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     2031 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       38 2024-04-10 08:51:04.114008 crawlee-0.0.3b1/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     3146 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-04-18 13:12:22.299220 crawlee-0.0.3b1/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-04-17 08:37:58.250881 crawlee-0.0.3b1/src/crawlee/log_config.py
--rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.3b1/src/crawlee/py.typed
--rw-r--r--   0        0        0     5506 2024-04-22 09:41:15.792175 crawlee-0.0.3b1/src/crawlee/request.py
--rw-r--r--   0        0        0      365 2024-04-22 10:45:11.357161 crawlee-0.0.3b1/src/crawlee/resource_clients/__init__.py
--rw-r--r--   0        0        0     5687 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_client.py
--rw-r--r--   0        0        0     2980 2024-04-18 12:13:47.124107 crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_collection_client.py
--rw-r--r--   0        0        0    19714 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_client.py
--rw-r--r--   0        0        0     1819 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_collection_client.py
--rw-r--r--   0        0        0    20474 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_client.py
--rw-r--r--   0        0        0     1936 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_collection_client.py
--rw-r--r--   0        0        0        0 2024-04-17 11:34:17.118301 crawlee-0.0.3b1/src/crawlee/resource_clients/py.typed
--rw-r--r--   0        0        0    22426 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_client.py
--rw-r--r--   0        0        0     1912 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_collection_client.py
--rw-r--r--   0        0        0       67 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-04-15 15:12:32.446961 crawlee-0.0.3b1/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8155 2024-04-16 07:53:19.412180 crawlee-0.0.3b1/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-04-15 15:12:32.447960 crawlee-0.0.3b1/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0     1645 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      106 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/base_storage_client.py
--rw-r--r--   0        0        0    11477 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-17 11:34:17.119301 crawlee-0.0.3b1/src/crawlee/storage_clients/py.typed
--rw-r--r--   0        0        0      150 2024-04-10 08:51:04.115008 crawlee-0.0.3b1/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7600 2024-04-18 18:02:48.825221 crawlee-0.0.3b1/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15526 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4999 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0     6489 2024-04-18 12:13:47.125107 crawlee-0.0.3b1/src/crawlee/storages/models.py
--rw-r--r--   0        0        0        0 2024-04-04 15:33:46.944733 crawlee-0.0.3b1/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2611 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2742 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25845 2024-04-22 10:45:11.358161 crawlee-0.0.3b1/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-04-18 12:13:47.126107 crawlee-0.0.3b1/src/crawlee/types.py
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 crawlee-0.0.3b1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-23 13:50:32.938953 crawlee-0.0.3b2/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-23 13:50:32.938953 crawlee-0.0.3b2/README.md
+-rw-r--r--   0        0        0     6331 2024-04-23 13:50:55.274863 crawlee-0.0.3b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     2056 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1585 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      186 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    14678 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     5315 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2279 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0      815 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     4017 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      462 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1246 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/configuration.py
+-rw-r--r--   0        0        0       91 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2683 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     2031 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       38 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/log_config.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/py.typed
+-rw-r--r--   0        0        0     5506 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/request.py
+-rw-r--r--   0        0        0      365 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/__init__.py
+-rw-r--r--   0        0        0     5687 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/base_resource_client.py
+-rw-r--r--   0        0        0     2980 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0        0        0    19714 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/dataset_client.py
+-rw-r--r--   0        0        0     1819 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/dataset_collection_client.py
+-rw-r--r--   0        0        0    20474 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/key_value_store_client.py
+-rw-r--r--   0        0        0     1936 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/key_value_store_collection_client.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/py.typed
+-rw-r--r--   0        0        0    22426 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/request_queue_client.py
+-rw-r--r--   0        0        0     1912 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/resource_clients/request_queue_collection_client.py
+-rw-r--r--   0        0        0       67 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8155 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0     1645 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      106 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storage_clients/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storage_clients/base_storage_client.py
+-rw-r--r--   0        0        0    11477 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storage_clients/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storage_clients/py.typed
+-rw-r--r--   0        0        0      150 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7600 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15526 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4999 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0     6489 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/models.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2611 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2742 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25845 2024-04-23 13:50:32.942953 crawlee-0.0.3b2/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-04-23 13:50:32.946953 crawlee-0.0.3b2/src/crawlee/types.py
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 crawlee-0.0.3b2/PKG-INFO
```

### Comparing `crawlee-0.0.3b1/LICENSE` & `crawlee-0.0.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/pyproject.toml` & `crawlee-0.0.3b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.3b1"
+version = "0.0.3b2"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.3b2/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/crypto.py` & `crawlee-0.0.3b2/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.3b2/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.3b2/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/file.py` & `crawlee-0.0.3b2/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.3b2/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/math.py` & `crawlee-0.0.3b2/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.3b2/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.3b2/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/requests.py` & `crawlee-0.0.3b2/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/system.py` & `crawlee-0.0.3b2/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/_utils/wait.py` & `crawlee-0.0.3b2/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.3b2/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.3b2/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.3b2/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/autoscaling/types.py` & `crawlee-0.0.3b2/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.3b2/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.3b2/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.3b2/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.3b2/src/crawlee/basic_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.3b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/configuration.py` & `crawlee-0.0.3b2/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/events/event_manager.py` & `crawlee-0.0.3b2/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.3b2/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/events/types.py` & `crawlee-0.0.3b2/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.3b2/src/crawlee/http_clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.3b2/src/crawlee/http_clients/httpx_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.3b2/src/crawlee/http_crawler/http_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/log_config.py` & `crawlee-0.0.3b2/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/request.py` & `crawlee-0.0.3b2/src/crawlee/request.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/base_resource_collection_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/dataset_collection_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/key_value_store_collection_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/resource_clients/request_queue_collection_client.py` & `crawlee-0.0.3b2/src/crawlee/resource_clients/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/sessions/models.py` & `crawlee-0.0.3b2/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/sessions/session.py` & `crawlee-0.0.3b2/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.3b2/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storage_client_manager.py` & `crawlee-0.0.3b2/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storage_clients/base_storage_client.py` & `crawlee-0.0.3b2/src/crawlee/storage_clients/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storage_clients/memory_storage_client.py` & `crawlee-0.0.3b2/src/crawlee/storage_clients/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/base_storage.py` & `crawlee-0.0.3b2/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/dataset.py` & `crawlee-0.0.3b2/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.3b2/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/models.py` & `crawlee-0.0.3b2/src/crawlee/storages/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/request_list.py` & `crawlee-0.0.3b2/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/request_provider.py` & `crawlee-0.0.3b2/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/storages/request_queue.py` & `crawlee-0.0.3b2/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/src/crawlee/types.py` & `crawlee-0.0.3b2/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b1/PKG-INFO` & `crawlee-0.0.3b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.3b1
+Version: 0.0.3b2
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```
