# Comparing `tmp/unitradeapi-0.119.tar.gz` & `tmp/unitradeapi-0.120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitradeapi-0.119.tar", last modified: Wed Feb 28 11:54:00 2024, max compression
+gzip compressed data, was "unitradeapi-0.120.tar", last modified: Tue Apr 23 12:41:31 2024, max compression
```

## Comparing `unitradeapi-0.119.tar` & `unitradeapi-0.120.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-02-28 11:54:00.775135 unitradeapi-0.119/
--rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.119/LICENSE.md
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-02-28 11:54:00.774923 unitradeapi-0.119/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.119/README.md
--rw-r--r--   0 andrey     (501) staff       (20)       38 2024-02-28 11:54:00.775184 unitradeapi-0.119/setup.cfg
--rw-r--r--   0 andrey     (501) staff       (20)      706 2024-02-28 11:53:24.000000 unitradeapi-0.119/setup.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-02-28 11:54:00.773767 unitradeapi-0.119/unitradeapi/
--rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.119/unitradeapi/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.119/unitradeapi/binance.py
--rw-r--r--   0 andrey     (501) staff       (20)    15246 2024-02-28 11:51:14.000000 unitradeapi-0.119/unitradeapi/bybit.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-02-28 11:54:00.774658 unitradeapi-0.119/unitradeapi.egg-info/
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-02-28 11:54:00.000000 unitradeapi-0.119/unitradeapi.egg-info/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      271 2024-02-28 11:54:00.000000 unitradeapi-0.119/unitradeapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrey     (501) staff       (20)        1 2024-02-28 11:54:00.000000 unitradeapi-0.119/unitradeapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrey     (501) staff       (20)       36 2024-02-28 11:54:00.000000 unitradeapi-0.119/unitradeapi.egg-info/requires.txt
--rw-r--r--   0 andrey     (501) staff       (20)       12 2024-02-28 11:54:00.000000 unitradeapi-0.119/unitradeapi.egg-info/top_level.txt
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.833402 unitradeapi-0.120/
+-rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.120/LICENSE.md
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-04-23 12:41:31.832971 unitradeapi-0.120/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.120/README.md
+-rw-r--r--   0 andrey     (501) staff       (20)       38 2024-04-23 12:41:31.833467 unitradeapi-0.120/setup.cfg
+-rw-r--r--   0 andrey     (501) staff       (20)      706 2024-04-23 12:41:18.000000 unitradeapi-0.120/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.831417 unitradeapi-0.120/unitradeapi/
+-rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.120/unitradeapi/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.120/unitradeapi/binance.py
+-rw-r--r--   0 andrey     (501) staff       (20)    15405 2024-04-23 12:36:18.000000 unitradeapi-0.120/unitradeapi/bybit.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.832523 unitradeapi-0.120/unitradeapi.egg-info/
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      271 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        1 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       36 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/requires.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       12 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/top_level.txt
```

### Comparing `unitradeapi-0.119/LICENSE.md` & `unitradeapi-0.120/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.119/PKG-INFO` & `unitradeapi-0.120/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.119
+Version: 0.120
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `unitradeapi-0.119/README.md` & `unitradeapi-0.120/README.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.119/setup.py` & `unitradeapi-0.120/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='unitradeapi',
-    version='0.119',
+    version='0.120',
     packages=find_packages(),
     description='Binance, Bybit API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='plv88',
     author_email='plv.andrey88@gmail.com',
     url='https://github.com/plv88/UniCryptTradeAPI',
```

### Comparing `unitradeapi-0.119/unitradeapi/binance.py` & `unitradeapi-0.120/unitradeapi/binance.py`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.119/unitradeapi/bybit.py` & `unitradeapi-0.120/unitradeapi/bybit.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,14 @@
                 break
             # Добавляем полученные логи в общий список
             all_logs.extend(response.get('list', []))
             # Обновляем курсор для следующего запроса
             cursor = response.get('nextPageCursor')
             if not cursor:
                 break  # Выход из цикла, если больше нет страниц для загрузки
-
         return all_logs
 
 
 #Websockets
 class SyncBybitWebsocketPublic:
     _dict_urls = {
         'spot': 'wss://stream.bybit.com/v5/public/spot',
@@ -331,19 +330,23 @@
 
     def send_heartbeat(self, _wsapp):
         while self._is_running:  # Проверьте, что соединение должно быть открыто
             try:
                 if _wsapp.sock and _wsapp.sock.connected:  # Проверьте, что сокет существует и соединение открыто
                     _wsapp.send(json.dumps({"req_id": "100001", "op": "ping"}))
                 else:
-                    print("WebSocket is not connected.")
+                    msg = "send_heartbeat, WebSocket is not connected."
+                    self._logger.warning(msg)
+                    print(msg)
                     break  # Выход из цикла, если соединение закрыто
                 time.sleep(20)
             except websocket.WebSocketConnectionClosedException:
-                print("WebSocket connection is closed, stopping heartbeat.")
+                msg = "WebSocket connection is closed, stopping heartbeat."
+                self._logger.warning(msg)
+                print(msg)
                 break
 
     def on_open(self, _wsapp):
         print("Connection opened")
         heartbeat_thread = threading.Thread(target=self.send_heartbeat, args=(_wsapp,))
         heartbeat_thread.start()
         data = {
```

### Comparing `unitradeapi-0.119/unitradeapi.egg-info/PKG-INFO` & `unitradeapi-0.120/unitradeapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.119
+Version: 0.120
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

