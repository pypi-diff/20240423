# Comparing `tmp/benimang-0.5.23.tar.gz` & `tmp/benimang-0.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.5.23.tar", last modified: Wed Mar 27 01:41:26 2024, max compression
+gzip compressed data, was "benimang-0.5.24.tar", last modified: Tue Apr 23 07:52:07 2024, max compression
```

## Comparing `benimang-0.5.23.tar` & `benimang-0.5.24.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 01:41:26.531644 benimang-0.5.23/
--rw-rw-rw-   0        0        0       29 2024-01-16 03:49:18.000000 benimang-0.5.23/MANIFEST.in
--rw-rw-rw-   0        0        0      881 2024-03-27 01:41:26.530645 benimang-0.5.23/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.23/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 01:41:26.517127 benimang-0.5.23/beni/
--rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.23/beni/__init__.py
--rw-rw-rw-   0        0        0     6535 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bbyte.py
--rw-rw-rw-   0        0        0     1815 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bcache.py
--rw-rw-rw-   0        0        0     1812 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bcolor.py
--rw-rw-rw-   0        0        0     2796 2024-03-11 07:42:18.000000 benimang-0.5.23/beni/bcrypto.py
--rw-rw-rw-   0        0        0      436 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bdefine.py
--rw-rw-rw-   0        0        0     1594 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bexecute.py
--rw-rw-rw-   0        0        0     2697 2024-03-27 01:38:29.000000 benimang-0.5.23/beni/bfile.py
--rw-rw-rw-   0        0        0     6393 2024-03-27 01:25:11.000000 benimang-0.5.23/beni/bfunc.py
--rw-rw-rw-   0        0        0     5740 2024-03-19 08:01:51.000000 benimang-0.5.23/beni/bhttp.py
--rw-rw-rw-   0        0        0     2242 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/binput.py
--rw-rw-rw-   0        0        0     1708 2024-02-19 03:49:12.000000 benimang-0.5.23/beni/bjwt.py
--rw-rw-rw-   0        0        0     5021 2024-03-25 01:38:46.000000 benimang-0.5.23/beni/block.py
--rw-rw-rw-   0        0        0     4147 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/blog.py
--rw-rw-rw-   0        0        0     6115 2024-03-19 08:01:55.000000 benimang-0.5.23/beni/bmysql.py
--rw-rw-rw-   0        0        0     4023 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bpath.py
--rw-rw-rw-   0        0        0     1374 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bpathx.py
--rw-rw-rw-   0        0        0     2820 2024-01-17 09:05:37.000000 benimang-0.5.23/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1055 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bprogress.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bqiniu.py
--rw-rw-rw-   0        0        0     3982 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bstore.py
--rw-rw-rw-   0        0        0     4525 2024-03-08 08:49:47.000000 benimang-0.5.23/beni/btask.py
--rw-rw-rw-   0        0        0     1559 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/btime.py
--rw-rw-rw-   0        0        0      500 2024-02-08 08:49:32.000000 benimang-0.5.23/beni/btype.py
--rw-rw-rw-   0        0        0     2318 2024-01-16 03:49:31.000000 benimang-0.5.23/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2024-03-27 01:41:26.529645 benimang-0.5.23/benimang.egg-info/
--rw-rw-rw-   0        0        0      881 2024-03-27 01:41:26.000000 benimang-0.5.23/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2024-03-27 01:41:26.000000 benimang-0.5.23/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 01:41:26.000000 benimang-0.5.23/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      234 2024-03-27 01:41:26.000000 benimang-0.5.23/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-27 01:41:26.000000 benimang-0.5.23/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      833 2024-03-27 01:40:11.000000 benimang-0.5.23/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 01:41:26.531644 benimang-0.5.23/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-27 01:41:26.528644 benimang-0.5.23/test/
--rw-rw-rw-   0        0        0      398 2024-03-08 09:28:12.000000 benimang-0.5.23/test/test_bbyte.py
--rw-rw-rw-   0        0        0      420 2024-01-16 03:49:31.000000 benimang-0.5.23/test/test_bcache.py
--rw-rw-rw-   0        0        0      735 2024-02-19 03:32:56.000000 benimang-0.5.23/test/test_bcrypto.py
--rw-rw-rw-   0        0        0      406 2024-02-19 03:14:30.000000 benimang-0.5.23/test/test_bfile.py
--rw-rw-rw-   0        0        0      339 2024-02-20 06:12:13.000000 benimang-0.5.23/test/test_bfunc.py
--rw-rw-rw-   0        0        0      491 2024-03-11 06:44:11.000000 benimang-0.5.23/test/test_crypto.py
--rw-rw-rw-   0        0        0      485 2024-02-19 01:38:08.000000 benimang-0.5.23/test/test_mysql.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:52:07.493231 benimang-0.5.24/
+-rw-rw-rw-   0        0        0       29 2024-01-16 03:49:18.000000 benimang-0.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0      853 2024-04-23 07:52:07.492232 benimang-0.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.24/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 07:52:07.477854 benimang-0.5.24/beni/
+-rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.24/beni/__init__.py
+-rw-rw-rw-   0        0        0     6535 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bbyte.py
+-rw-rw-rw-   0        0        0     1815 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bcache.py
+-rw-rw-rw-   0        0        0     1812 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2796 2024-03-11 07:42:18.000000 benimang-0.5.24/beni/bcrypto.py
+-rw-rw-rw-   0        0        0      436 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bdefine.py
+-rw-rw-rw-   0        0        0     1594 2024-04-23 07:33:23.000000 benimang-0.5.24/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2697 2024-03-27 01:38:29.000000 benimang-0.5.24/beni/bfile.py
+-rw-rw-rw-   0        0        0     6638 2024-04-23 03:25:59.000000 benimang-0.5.24/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5740 2024-03-19 08:01:51.000000 benimang-0.5.24/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2242 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/binput.py
+-rw-rw-rw-   0        0        0     1473 2024-04-23 06:13:33.000000 benimang-0.5.24/beni/bjwt.py
+-rw-rw-rw-   0        0        0     3897 2024-04-23 03:17:09.000000 benimang-0.5.24/beni/block.py
+-rw-rw-rw-   0        0        0     4147 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/blog.py
+-rw-rw-rw-   0        0        0     6115 2024-03-19 08:01:55.000000 benimang-0.5.24/beni/bmysql.py
+-rw-rw-rw-   0        0        0     4023 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bpath.py
+-rw-rw-rw-   0        0        0     1374 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bpathx.py
+-rw-rw-rw-   0        0        0     2820 2024-01-17 09:05:37.000000 benimang-0.5.24/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1055 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     3982 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bstore.py
+-rw-rw-rw-   0        0        0     4514 2024-04-23 02:36:55.000000 benimang-0.5.24/beni/btask.py
+-rw-rw-rw-   0        0        0     1559 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/btime.py
+-rw-rw-rw-   0        0        0      500 2024-02-08 08:49:32.000000 benimang-0.5.24/beni/btype.py
+-rw-rw-rw-   0        0        0     2318 2024-01-16 03:49:31.000000 benimang-0.5.24/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:52:07.491234 benimang-0.5.24/benimang.egg-info/
+-rw-rw-rw-   0        0        0      853 2024-04-23 07:52:07.000000 benimang-0.5.24/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-04-23 07:52:07.000000 benimang-0.5.24/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:52:07.000000 benimang-0.5.24/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2024-04-23 07:52:07.000000 benimang-0.5.24/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-23 07:52:07.000000 benimang-0.5.24/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-04-23 07:46:11.000000 benimang-0.5.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:52:07.494231 benimang-0.5.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 07:52:07.489906 benimang-0.5.24/test/
+-rw-rw-rw-   0        0        0      398 2024-03-08 09:28:12.000000 benimang-0.5.24/test/test_bbyte.py
+-rw-rw-rw-   0        0        0      420 2024-01-16 03:49:31.000000 benimang-0.5.24/test/test_bcache.py
+-rw-rw-rw-   0        0        0      735 2024-02-19 03:32:56.000000 benimang-0.5.24/test/test_bcrypto.py
+-rw-rw-rw-   0        0        0      406 2024-02-19 03:14:30.000000 benimang-0.5.24/test/test_bfile.py
+-rw-rw-rw-   0        0        0      584 2024-04-23 03:29:36.000000 benimang-0.5.24/test/test_bfunc.py
+-rw-rw-rw-   0        0        0      491 2024-03-11 06:44:11.000000 benimang-0.5.24/test/test_crypto.py
+-rw-rw-rw-   0        0        0      485 2024-02-19 01:38:08.000000 benimang-0.5.24/test/test_mysql.py
+-rw-rw-rw-   0        0        0      501 2024-04-23 02:36:18.000000 benimang-0.5.24/test/test_portLock.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 02:52:47.000000 benimang-0.5.24/test/test_rwlock.py
```

### Comparing `benimang-0.5.23/PKG-INFO` & `benimang-0.5.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benimang
-Version: 0.5.23
+Version: 0.5.24
 Summary: Utils library for Beni
 Author-email: Beni Mang <benimang@126.com>
 Maintainer-email: Beni Mang <benimang@126.com>
 Keywords: benimang,beni
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiofiles
@@ -13,15 +13,14 @@
 Requires-Dist: async_timeout
 Requires-Dist: build
 Requires-Dist: chardet
 Requires-Dist: colorama
 Requires-Dist: cryptography
 Requires-Dist: nest-asyncio
 Requires-Dist: orjson
-Requires-Dist: portalocker
 Requires-Dist: pretty_errors
 Requires-Dist: prettytable
 Requires-Dist: pydantic
 Requires-Dist: pyjwt
 Requires-Dist: pyperclip
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
```

### Comparing `benimang-0.5.23/beni/bbyte.py` & `benimang-0.5.24/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bcache.py` & `benimang-0.5.24/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bcolor.py` & `benimang-0.5.24/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bcrypto.py` & `benimang-0.5.24/beni/bcrypto.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bexecute.py` & `benimang-0.5.24/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bfile.py` & `benimang-0.5.24/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bfunc.py` & `benimang-0.5.24/beni/bfunc.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,7 +252,15 @@
     half = len(chunks) // 2
     even_chunks = chunks[:half]
     odd_chunks = chunks[half:]
     if len(chunks) % 2 == 1:
         even_chunks.append(b'')
     deobfuscated = b''.join(sum(zip(even_chunks, odd_chunks), ())) + b''.join(even_chunks[len(odd_chunks):])
     return deobfuscated
+
+
+def shuffleSequence(data: AnyType) -> AnyType:
+    '打乱序列'
+    tempData = toAny(data)
+    size = len(tempData)
+    n = int(size / 3) - size % 10
+    return tempData[:size - n * 2] + tempData[size - n:] + tempData[size - n * 2:size - n]
```

### Comparing `benimang-0.5.23/beni/bhttp.py` & `benimang-0.5.24/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/binput.py` & `benimang-0.5.24/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bjwt.py` & `benimang-0.5.24/beni/bjwt.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 import uuid
 from typing import Any
 
 import jwt
 
 from beni import bfile
-from beni.bfunc import toAny
-from beni.btype import AnyType, XPath
+from beni.bfunc import shuffleSequence
+from beni.btype import XPath
 
 _KEY_SALT = '_salt_@#%@#xafDGAz.nq'
 _KEY_TEXT = '_text_A!@$,FJ@#adsfkl'
 
 
 def encodeJson(data: dict[str, Any], secret: str, tips: str = '') -> str:
     tips = tips.strip()
     data[_KEY_SALT] = uuid.uuid4().hex
     result = jwt.encode(data, secret, algorithm='HS256')
-    result = _magicSequence(result)
+    result = shuffleSequence(result)
     if tips:
         result = f'{tips} {result}'
     return result
 
 
 def encodeText(text: str, secret: str, tips: str = '') -> str:
     tips = tips.strip()
@@ -35,15 +35,15 @@
     content = await bfile.readText(file)
     result = encodeText(content, secret, tips)
     await bfile.writeText(file, result)
 
 
 def decodeJson(content: str, secret: str) -> dict[str, Any]:
     content = content.split(' ')[-1]
-    content = _magicSequence(content)
+    content = shuffleSequence(content)
     data = jwt.decode(content, secret, algorithms=['HS256'])
     if _KEY_SALT in data:
         del data[_KEY_SALT]
     return data
 
 
 def decodeText(content: str, secret: str) -> str:
@@ -51,15 +51,7 @@
     return data[_KEY_TEXT]
 
 
 async def decodeFile(file: XPath, secret: str) -> None:
     content = await bfile.readText(file)
     result = decodeText(content, secret)
     await bfile.writeText(file, result)
-
-
-def _magicSequence(data: AnyType) -> AnyType:
-    '混淆'
-    tempData = toAny(data)
-    size = len(tempData)
-    n = int(size / 3) - size % 10
-    return tempData[:size - n * 2] + tempData[size - n:] + tempData[size - n * 2:size - n]
```

### Comparing `benimang-0.5.23/beni/block.py` & `benimang-0.5.24/beni/block.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,39 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
-from contextlib import asynccontextmanager
+import socket
+from contextlib import asynccontextmanager, contextmanager
 from functools import wraps
-from pathlib import Path
 from typing import Any
 
-from beni import bpath
-from beni.bfunc import crcStr, toAny
+from beni.bfunc import toAny
 from beni.btype import AsyncFuncType, Func
 
-
-@asynccontextmanager
-async def useFileLock(*keys: str, timeout: float = 0):
-    import portalocker
-    lock_list: list[portalocker.Lock] = []
-    keyfile_list: list[Path] = []
-    for key in keys:
-        lock, keyfile = await _lock_acquire(key, timeout)
-        lock_list.append(lock)
-        keyfile_list.append(keyfile)
-    try:
-        yield
-    finally:
-        for lock in lock_list:
-            lock.release()
-        for keyfile in keyfile_list:
-            try:
-                bpath.remove(keyfile)
-            except:
-                pass
+# ------------------------------------------------------------------------------------------------------------------------
+# 根据端口限制多开
 
 
-async def _lock_acquire(key: str, timeout: float = 0):
-    '''不对外部提供，只提供给 async_keylock 方法使用'''
-    keyfile = bpath.workspace(f'.lock/{crcStr(key)}.lock')
-    bpath.make(keyfile.parent)
-    import portalocker
+@contextmanager
+def portLock(port: int, errMsg: str = '程序禁止多开'):
+    assert 60000 <= port <= 65535, '端口范围为 60000 ~ 65535'
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
-        lock = portalocker.Lock(keyfile, timeout=timeout, fail_when_locked=timeout == 0)
-        f = lock.acquire()
-        f.write(key)
-        f.flush()
+        sock.bind(('localhost', port))
+        sock.listen(1)
+        yield
     except:
-        raise Exception(f'程序不允许重复执行')
-    return lock, keyfile
+        raise Exception(errMsg)
+    finally:
+        sock.close()
 
 
 # ------------------------------------------------------------------------------------------------------------------------
-
+# 限制并执行数量
 
 def limit(value: int = 1):
     def wraperfun(func: AsyncFuncType) -> AsyncFuncType:
         @wraps(func)
         async def wraper(*args: Any, **kwargs: Any):
             funid = id(inspect.unwrap(func))
             if funid not in _limitDict:
@@ -105,69 +85,48 @@
         while self._running + self._queue.qsize() > self._limit:
             if self._queue.empty():
                 break
             await self._queue.get()
 
 
 # ------------------------------------------------------------------------------------------------------------------------
-
+# 读写锁
 
 class RWLock():
+    def __init__(self) -> None:
+        self._readLock: asyncio.Lock = asyncio.Lock()
+        self._writeLock: asyncio.Lock = asyncio.Lock()
+        self._readers: int = 0
+
+    async def acquireRead(self) -> None:
+        async with self._readLock:
+            self._readers += 1
+            if self._readers == 1:
+                await self._writeLock.acquire()
+
+    async def releaseRead(self) -> None:
+        async with self._readLock:
+            self._readers -= 1
+            if self._readers == 0:
+                self._writeLock.release()
 
-    def __init__(self, maxNum: int) -> None:
-        self._maxNum = maxNum
-        self._readNum = 0
-        self._writeNum = 0
-        self._onReadFinished = asyncio.Event()
-        self._onWriteFinished = asyncio.Event()
-
-    def _getNum(self):
-        return self._readNum + self._writeNum
-
-    async def getRead(self):
-        while True:
-            if self._writeNum:
-                self._onWriteFinished.clear()
-                await self._onWriteFinished.wait()
-            elif self._getNum() >= self._maxNum:
-                self._onReadFinished.clear()
-                await self._onReadFinished.wait()
-            else:
-                self._readNum += 1
-                break
+    async def acquireWrite(self) -> None:
+        await self._writeLock.acquire()
 
-    def releaseRead(self):
-        self._readNum -= 1
-        if not self._readNum:
-            self._onReadFinished.set()
+    async def releaseWrite(self) -> None:
+        self._writeLock.release()
 
     @asynccontextmanager
     async def useRead(self):
-        await self.getRead()
+        await self.acquireRead()
         try:
             yield
         finally:
-            self.releaseRead()
-
-    async def getWrite(self):
-        while True:
-            if self._readNum:
-                self._onReadFinished.clear()
-                await self._onReadFinished.wait()
-            elif self._writeNum:
-                self._onWriteFinished.clear()
-                await self._onWriteFinished.wait()
-            else:
-                self._writeNum += 1
-                break
-
-    def releaseWrite(self):
-        self._writeNum -= 1
-        self._onWriteFinished.set()
+            await self.releaseRead()
 
     @asynccontextmanager
     async def useWrite(self):
-        await self.getWrite()
+        await self.acquireWrite()
         try:
             yield
         finally:
-            self.releaseWrite()
+            await self.releaseWrite()
```

### Comparing `benimang-0.5.23/beni/blog.py` & `benimang-0.5.24/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bmysql.py` & `benimang-0.5.24/beni/bmysql.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bpath.py` & `benimang-0.5.24/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bpathx.py` & `benimang-0.5.24/beni/bpathx.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bplaywright.py` & `benimang-0.5.24/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bprogress.py` & `benimang-0.5.24/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bqiniu.py` & `benimang-0.5.24/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bstore.py` & `benimang-0.5.24/beni/bstore.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/btask.py` & `benimang-0.5.24/beni/btask.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 app = Typer()
 
 nest_asyncio.apply()
 
 
 @dataclass
 class _Options:
-    lock: str = 'btask'
+    lock: int = 60001
     logPath: Path = Null
     binPath: Path = Null
     logFilesLimit: int = 100
 
 
 options: Final = _Options()
 isShowSummary: bool = False
@@ -60,15 +60,15 @@
 
 
 @asynccontextmanager
 async def _task():
     # bfunc.sysUtf8() # 由于不是每次都需要用到，界面显示了不美观 Active code page: 65001
     if options.binPath:
         bfunc.addEnvPath(options.binPath)
-    async with block.useFileLock(options.lock):
+    with block.portLock(options.lock):
         start_time = Datetime.now()
         bfunc.initErrorFormat()
         if options.logPath:
             logFile = bpath.get(options.logPath, btime.datetimeStr('%Y%m%d_%H%M%S.log'))
             assert logFile.is_file(), f'日志文件创建失败（已存在） {logFile}'
         else:
             logFile = None
```

### Comparing `benimang-0.5.23/beni/btime.py` & `benimang-0.5.24/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/beni/bzip.py` & `benimang-0.5.24/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.23/benimang.egg-info/PKG-INFO` & `benimang-0.5.24/benimang.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benimang
-Version: 0.5.23
+Version: 0.5.24
 Summary: Utils library for Beni
 Author-email: Beni Mang <benimang@126.com>
 Maintainer-email: Beni Mang <benimang@126.com>
 Keywords: benimang,beni
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiofiles
@@ -13,15 +13,14 @@
 Requires-Dist: async_timeout
 Requires-Dist: build
 Requires-Dist: chardet
 Requires-Dist: colorama
 Requires-Dist: cryptography
 Requires-Dist: nest-asyncio
 Requires-Dist: orjson
-Requires-Dist: portalocker
 Requires-Dist: pretty_errors
 Requires-Dist: prettytable
 Requires-Dist: pydantic
 Requires-Dist: pyjwt
 Requires-Dist: pyperclip
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
```

### Comparing `benimang-0.5.23/benimang.egg-info/SOURCES.txt` & `benimang-0.5.24/benimang.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -33,8 +33,10 @@
 benimang.egg-info/top_level.txt
 test/test_bbyte.py
 test/test_bcache.py
 test/test_bcrypto.py
 test/test_bfile.py
 test/test_bfunc.py
 test/test_crypto.py
-test/test_mysql.py
+test/test_mysql.py
+test/test_portLock.py
+test/test_rwlock.py
```

### Comparing `benimang-0.5.23/pyproject.toml` & `benimang-0.5.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://peps.python.org/pep-0621/#example
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 
 [project]
 name = "benimang"
-version = "0.5.23"
+version = "0.5.24"
 description = "Utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 maintainers = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 
 dependencies = [
@@ -19,15 +19,14 @@
   'build',
   'chardet',
   'colorama',
   'cryptography',
   'nest-asyncio',
   'orjson',
   # 'playwright',
-  'portalocker',
   'pretty_errors',
   'prettytable',
   'pydantic',
   'pyjwt',
   'pyperclip',
   'pytest',
   'pytest-asyncio',
```

### Comparing `benimang-0.5.23/test/test_bcrypto.py` & `benimang-0.5.24/test/test_bcrypto.py`

 * *Files identical despite different names*

