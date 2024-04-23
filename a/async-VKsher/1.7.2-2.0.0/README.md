# Comparing `tmp/async_VKsher-1.7.2.tar.gz` & `tmp/async_VKsher-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_VKsher-1.7.2.tar", last modified: Sun Apr 21 17:41:52 2024, max compression
+gzip compressed data, was "async_VKsher-2.0.0.tar", last modified: Mon Apr 22 15:43:55 2024, max compression
```

## Comparing `async_VKsher-1.7.2.tar` & `async_VKsher-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.397068 async_VKsher-1.7.2/
--rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-1.7.2/LICENSE
--rw-rw-rw-   0        0        0    28118 2024-04-21 17:41:52.394479 async_VKsher-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0    27096 2024-04-20 15:22:35.000000 async_VKsher-1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.374927 async_VKsher-1.7.2/asyncVK/
--rw-rw-rw-   0        0        0     4050 2024-04-21 16:26:30.000000 async_VKsher-1.7.2/asyncVK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.376922 async_VKsher-1.7.2/asyncVK/asyncDB/
--rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-1.7.2/asyncVK/asyncDB/__init__.py
--rw-rw-rw-   0        0        0     1548 2024-04-21 15:33:16.000000 async_VKsher-1.7.2/asyncVK/chain.py
--rw-rw-rw-   0        0        0     1912 2021-12-13 12:57:10.000000 async_VKsher-1.7.2/asyncVK/condition.py
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.378880 async_VKsher-1.7.2/asyncVK/core/
--rw-rw-rw-   0        0        0     2364 2024-04-20 15:15:28.000000 async_VKsher-1.7.2/asyncVK/core/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-04-21 16:28:22.000000 async_VKsher-1.7.2/asyncVK/dispatcher.py
--rw-rw-rw-   0        0        0     2672 2024-04-21 15:29:06.000000 async_VKsher-1.7.2/asyncVK/handlers.py
--rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-1.7.2/asyncVK/keyboard.py
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.392379 async_VKsher-1.7.2/async_VKsher.egg-info/
--rw-rw-rw-   0        0        0    28118 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-21 17:41:52.000000 async_VKsher-1.7.2/async_VKsher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 17:41:52.397068 async_VKsher-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0      821 2024-04-21 17:41:31.000000 async_VKsher-1.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 17:41:52.389439 async_VKsher-1.7.2/upload/
--rw-rw-rw-   0        0        0      786 2024-04-21 17:36:26.000000 async_VKsher-1.7.2/upload/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.358429 async_VKsher-2.0.0/
+-rw-rw-rw-   0        0        0    35149 2022-07-25 16:43:52.000000 async_VKsher-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    30584 2024-04-22 15:43:55.357431 async_VKsher-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    29525 2024-04-22 15:43:21.000000 async_VKsher-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.335539 async_VKsher-2.0.0/asyncVK/
+-rw-rw-rw-   0        0        0     4050 2024-04-21 16:26:30.000000 async_VKsher-2.0.0/asyncVK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.337586 async_VKsher-2.0.0/asyncVK/asyncDB/
+-rw-rw-rw-   0        0        0     1199 2021-12-13 13:50:31.000000 async_VKsher-2.0.0/asyncVK/asyncDB/__init__.py
+-rw-rw-rw-   0        0        0     1548 2024-04-21 15:33:16.000000 async_VKsher-2.0.0/asyncVK/chain.py
+-rw-rw-rw-   0        0        0     1874 2024-04-22 15:43:03.000000 async_VKsher-2.0.0/asyncVK/condition.py
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.341826 async_VKsher-2.0.0/asyncVK/core/
+-rw-rw-rw-   0        0        0     2727 2024-04-22 14:59:33.000000 async_VKsher-2.0.0/asyncVK/core/__init__.py
+-rw-rw-rw-   0        0        0      895 2024-04-22 15:41:29.000000 async_VKsher-2.0.0/asyncVK/core/message.py
+-rw-rw-rw-   0        0        0     4525 2024-04-22 15:38:32.000000 async_VKsher-2.0.0/asyncVK/dispatcher.py
+-rw-rw-rw-   0        0        0     2672 2024-04-21 15:29:06.000000 async_VKsher-2.0.0/asyncVK/handlers.py
+-rw-rw-rw-   0        0        0      731 2021-02-02 06:00:48.000000 async_VKsher-2.0.0/asyncVK/keyboard.py
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.355401 async_VKsher-2.0.0/async_VKsher.egg-info/
+-rw-rw-rw-   0        0        0    30584 2024-04-22 15:43:55.000000 async_VKsher-2.0.0/async_VKsher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-22 15:43:55.000000 async_VKsher-2.0.0/async_VKsher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 15:43:55.000000 async_VKsher-2.0.0/async_VKsher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-22 15:43:55.000000 async_VKsher-2.0.0/async_VKsher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-22 15:43:55.000000 async_VKsher-2.0.0/async_VKsher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 15:43:55.358429 async_VKsher-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-04-22 15:43:40.000000 async_VKsher-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 15:43:55.352296 async_VKsher-2.0.0/upload/
+-rw-rw-rw-   0        0        0      786 2024-04-21 17:36:26.000000 async_VKsher-2.0.0/upload/__init__.py
```

### Comparing `async_VKsher-1.7.2/LICENSE` & `async_VKsher-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/PKG-INFO` & `async_VKsher-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.2
+Version: 2.0.0
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,21 +13,24 @@
 Requires-Dist: asyncio>=3
 Requires-Dist: aiohttp>=3
 Requires-Dist: aiofiles>=22
 
 asyncVK – асинхронный фреймворк для создания ботов ВК. Преимущества: удобство, скорость выигрываемая за счёт асинхронности.
 =
 
-Бот создаётся за счёт шести структурных единиц: 
+Бот создаётся за счёт пяти основных структурных единиц: 
 1) Bot – это самая главная структурная единица. Это собственно сам бот, который подаёт ивенты     обработчикам.
 2) Handler – эта структурная единица отвечает за обработку ивентов. 
 3) Dispatcher – эта структурная единица отвечает за взаимодействие с ВК (ответы на сообщения, добавление комментариев). Она автоматически настраивается хандлерами.
-4) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
-5) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
-6) Chain - эта структурная единица позволяет создавать цепочки команд.
+4) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
+5) Chain - эта структурная единица позволяет создавать цепочки команд.
+
+Также есть такие второстепенные структурные единицы как:
+1) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
+2) Message - структура сообщения для облегчения работы с сообщениями.
 
 Как работать с библиотекой? Легко и интуитивно понятно! Для начала нужно импортировать саму библиотеку и создать бота:
 ```python
 from asyncVK import Handler, Bot, run_polling
 from asyncVK.dispatcher import Dispatcher
 from asyncVK.condition import Condition, And, Or
 import asyncVK.keyboard as keyboard
@@ -117,20 +120,41 @@
 
     dispatcher.answer – ответить в ЛС. Можно активировать при любом событии, отправит сообщение инициатору события. Список аргументов: 
 		text – текст сообщения.
 		attachment – вложение сообщения (в виде части ссылки такого рода: 
 		    от ссылки https://vk.com/id386746383?z=photo386746383_457256628%2Falbum386746383_0 
 		    берём только photo386746383_457256628 и передаём это в качестве аргумента). 
 		keyboard – кнопки ВК.
-		
-    dispatcher.send_message – ответить в том же чате. Список аргументов идентичен с answer.
+		Возвращает структуру Message вашего сообщения.
+
+    dispatcher.reply - ответить на сообщение пользователя. Список аргументов и возвращаемое значение идентичны с answer.
+    dispatcher.send_message – ответить в том же чате. Список аргументов и возвращаемое значение идентичны с answer.
     dispatcher.send_comment – ответить в комментариях. Список аргументов идентичен с answer, но аргумент keyboard отсутствует.
     dispatcher.mark_as_read – пометить сообщение как "прочитанное". Никаких аргументов не принимает.
     dispatcher.set_typing_status – установить статус на набор текста / запись голосового сообщения. Принимает один аргумент: 
-        typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+        	typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+    dispatcher.kick_user - удаляет участника из беседы
+        	member_id - id участника беседы (id сообщества пишется со знаком -)
+    dispatcher.edit_chat_name - изменяет название беседы
+        	title - новое название беседы
+
+Пример использования структуры Message:
+```python
+@bot.handle
+@Handler.on.message_new(Condition(command="прив"))
+async def handler(dispatcher: Dispatcher):
+    message = await dispatcher.reply("Это сообщение исчезнет через 3 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 2 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 1 секунду, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.delete()
+    await dispatcher.message.pin()
+```
 
 Как создать кнопки? Тоже несложно! Вот пример:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     buttons = keyboard.get_keyboard([
@@ -179,19 +203,32 @@
 Параметры диспетчера:
 
     dispatcher.token - ваш токен
     dispatcher.user_id - id инициировавшего событие пользователя
     dispatcher.peer_id - id чата (если это ЛС, то peer_id равен user_id)
     dispatcher.post_id - id записи на стене или обсуждения (если событие это новая запись на стене, новый комментарий на стене или в обсуждении)
     dispatcher.owner_id - если событие было внутри группы, то owner_id это id группы
+    dispatcher.object_id - id объекта события
     dispatcher.event - объект события
     dispatcher.text - если к примеру событие это новое сообщение, то text это текст сообщения, если это к примеру новый комментарий, то text это текст комментария и т.д.
     dispatcher.reply_text - текст отвеченного сообщения (если таковое имеется)
     dispatcher.reply_user_id - id пользователя написавшего отмеченное сообщение (если таковое имеется)
     dispatcher.reply_peer_id - id чата отмеченного сообщения (если таковое имеется)
+    dispatcher.reply_object_id - id объекта ответа
+    dispatcher.message - выдаёт структуру Message для сообщения из события
+    dispatcher.reply_message - выдаёт структуру Message для отвеченного сообщения из события
+
+Возможность структуры Message:
+
+    message.edit - изменить сообщение
+    		text - новый текст
+		attachment - вложение
+ 		keyboard - клавиатура
+    message.pin - закрепить сообщение
+    message.delete - удалить сообщение
 
 Если вы хотите выполнить сразу несколько запросов асинхронно, то можно просто воспользовать библиотекой `asyncio`. К примеру:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     tasks = [asyncio.create_task(dispatcher.mark_as_read()),
```

### Comparing `async_VKsher-1.7.2/README.md` & `async_VKsher-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 asyncVK – асинхронный фреймворк для создания ботов ВК. Преимущества: удобство, скорость выигрываемая за счёт асинхронности.
 =
 
-Бот создаётся за счёт шести структурных единиц: 
+Бот создаётся за счёт пяти основных структурных единиц: 
 1) Bot – это самая главная структурная единица. Это собственно сам бот, который подаёт ивенты     обработчикам.
 2) Handler – эта структурная единица отвечает за обработку ивентов. 
 3) Dispatcher – эта структурная единица отвечает за взаимодействие с ВК (ответы на сообщения, добавление комментариев). Она автоматически настраивается хандлерами.
-4) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
-5) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
-6) Chain - эта структурная единица позволяет создавать цепочки команд.
+4) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
+5) Chain - эта структурная единица позволяет создавать цепочки команд.
+
+Также есть такие второстепенные структурные единицы как:
+1) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
+2) Message - структура сообщения для облегчения работы с сообщениями.
 
 Как работать с библиотекой? Легко и интуитивно понятно! Для начала нужно импортировать саму библиотеку и создать бота:
 ```python
 from asyncVK import Handler, Bot, run_polling
 from asyncVK.dispatcher import Dispatcher
 from asyncVK.condition import Condition, And, Or
 import asyncVK.keyboard as keyboard
@@ -101,20 +104,41 @@
 
     dispatcher.answer – ответить в ЛС. Можно активировать при любом событии, отправит сообщение инициатору события. Список аргументов: 
 		text – текст сообщения.
 		attachment – вложение сообщения (в виде части ссылки такого рода: 
 		    от ссылки https://vk.com/id386746383?z=photo386746383_457256628%2Falbum386746383_0 
 		    берём только photo386746383_457256628 и передаём это в качестве аргумента). 
 		keyboard – кнопки ВК.
-		
-    dispatcher.send_message – ответить в том же чате. Список аргументов идентичен с answer.
+		Возвращает структуру Message вашего сообщения.
+
+    dispatcher.reply - ответить на сообщение пользователя. Список аргументов и возвращаемое значение идентичны с answer.
+    dispatcher.send_message – ответить в том же чате. Список аргументов и возвращаемое значение идентичны с answer.
     dispatcher.send_comment – ответить в комментариях. Список аргументов идентичен с answer, но аргумент keyboard отсутствует.
     dispatcher.mark_as_read – пометить сообщение как "прочитанное". Никаких аргументов не принимает.
     dispatcher.set_typing_status – установить статус на набор текста / запись голосового сообщения. Принимает один аргумент: 
-        typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+        	typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+    dispatcher.kick_user - удаляет участника из беседы
+        	member_id - id участника беседы (id сообщества пишется со знаком -)
+    dispatcher.edit_chat_name - изменяет название беседы
+        	title - новое название беседы
+
+Пример использования структуры Message:
+```python
+@bot.handle
+@Handler.on.message_new(Condition(command="прив"))
+async def handler(dispatcher: Dispatcher):
+    message = await dispatcher.reply("Это сообщение исчезнет через 3 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 2 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 1 секунду, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.delete()
+    await dispatcher.message.pin()
+```
 
 Как создать кнопки? Тоже несложно! Вот пример:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     buttons = keyboard.get_keyboard([
@@ -163,19 +187,32 @@
 Параметры диспетчера:
 
     dispatcher.token - ваш токен
     dispatcher.user_id - id инициировавшего событие пользователя
     dispatcher.peer_id - id чата (если это ЛС, то peer_id равен user_id)
     dispatcher.post_id - id записи на стене или обсуждения (если событие это новая запись на стене, новый комментарий на стене или в обсуждении)
     dispatcher.owner_id - если событие было внутри группы, то owner_id это id группы
+    dispatcher.object_id - id объекта события
     dispatcher.event - объект события
     dispatcher.text - если к примеру событие это новое сообщение, то text это текст сообщения, если это к примеру новый комментарий, то text это текст комментария и т.д.
     dispatcher.reply_text - текст отвеченного сообщения (если таковое имеется)
     dispatcher.reply_user_id - id пользователя написавшего отмеченное сообщение (если таковое имеется)
     dispatcher.reply_peer_id - id чата отмеченного сообщения (если таковое имеется)
+    dispatcher.reply_object_id - id объекта ответа
+    dispatcher.message - выдаёт структуру Message для сообщения из события
+    dispatcher.reply_message - выдаёт структуру Message для отвеченного сообщения из события
+
+Возможность структуры Message:
+
+    message.edit - изменить сообщение
+    		text - новый текст
+		attachment - вложение
+ 		keyboard - клавиатура
+    message.pin - закрепить сообщение
+    message.delete - удалить сообщение
 
 Если вы хотите выполнить сразу несколько запросов асинхронно, то можно просто воспользовать библиотекой `asyncio`. К примеру:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     tasks = [asyncio.create_task(dispatcher.mark_as_read()),
```

### Comparing `async_VKsher-1.7.2/asyncVK/__init__.py` & `async_VKsher-2.0.0/asyncVK/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/asyncVK/asyncDB/__init__.py` & `async_VKsher-2.0.0/asyncVK/asyncDB/__init__.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/asyncVK/chain.py` & `async_VKsher-2.0.0/asyncVK/chain.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/asyncVK/condition.py` & `async_VKsher-2.0.0/asyncVK/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Union
 
-from .core import get_event_params
-
 
 class Condition:
-    def __init__(self, command: str = None, contains_command: str = None,
-                 user_id: int = None, peer_id: int = None, post_id: int = None, owner_id: int = None):
+    def __init__(self, command: str = None, contains_command: str = None, user_id: int = None,
+                 peer_id: int = None, post_id: int = None, owner_id: int = None):
         self.command = command
         self.contains_command = contains_command
         self.user_id = user_id
         self.peer_id = peer_id
         self.post_id = post_id
         self.owner_id = owner_id
```

### Comparing `async_VKsher-1.7.2/asyncVK/core/__init__.py` & `async_VKsher-2.0.0/asyncVK/core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,39 +3,44 @@
 
 def get_event_params(event: dict, event_type: str) -> dict:
     text = None
     user_id = None
     peer_id = None
     post_id = None
     owner_id = None
-    reply_message = {}
+    object_id = None
+    reply = {}
 
     try:
         if event_type == "message_new":
             text = event["object"]["message"]["text"]
             peer_id = event["object"]["message"]["peer_id"]
             user_id = event["object"]["message"]["from_id"]
+            object_id = event["object"]["message"]["conversation_message_id"]
 
             if "reply_message" in event["object"]["message"]:
-                reply_message = {
+                reply = {
                     "text": event["object"]["message"]["reply_message"]["text"],
                     "peer_id": event["object"]["message"]["reply_message"]["peer_id"],
-                    "user_id": event["object"]["message"]["reply_message"]["from_id"]
+                    "user_id": event["object"]["message"]["reply_message"]["from_id"],
+                    "object_id": event["object"]["message"]["reply_message"]["conversation_message_id"]
                 }
 
         elif event_type == "message_edit":
             text = event["object"]["text"]
             peer_id = event["object"]["peer_id"]
             user_id = event["object"]["from_id"]
+            object_id = event["object"]["conversation_message_id"]
 
             if "reply_message" in event["object"]:
-                reply_message = {
+                reply = {
                     "text": event["object"]["reply_message"]["text"],
                     "peer_id": event["object"]["reply_message"]["peer_id"],
-                    "user_id": event["object"]["reply_message"]["from_id"]
+                    "user_id": event["object"]["reply_message"]["from_id"],
+                    "object_id": event["object"]["reply_message"]["conversation_message_id"]
                 }
 
         elif event_type in ("wall_reply_new", "wall_reply_edit"):
             text = event["object"]["text"]
             owner_id = event["object"]["owner_id"]
             user_id = event["object"]["from_id"]
             post_id = event["object"]["post_id"]
@@ -58,9 +63,10 @@
     return {
         "type": event_type,
         "text": text,
         "user_id": user_id,
         "peer_id": peer_id,
         "post_id": post_id,
         "owner_id": owner_id,
-        "reply_message": reply_message
+        "object_id": object_id,
+        "reply": reply
     }
```

### Comparing `async_VKsher-1.7.2/asyncVK/handlers.py` & `async_VKsher-2.0.0/asyncVK/handlers.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/asyncVK/keyboard.py` & `async_VKsher-2.0.0/asyncVK/keyboard.py`

 * *Files identical despite different names*

### Comparing `async_VKsher-1.7.2/async_VKsher.egg-info/PKG-INFO` & `async_VKsher-2.0.0/async_VKsher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_VKsher
-Version: 1.7.2
+Version: 2.0.0
 Summary: asyncVK is asynchronous library for creating a bot in VK
 Home-page: https://github.com/Ekventor/asyncVK
 Author: Kulenov Islam
 Author-email: kit.werr34@gmail.com
 Keywords: vk vkontakte вк вконтакте бот bot
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,21 +13,24 @@
 Requires-Dist: asyncio>=3
 Requires-Dist: aiohttp>=3
 Requires-Dist: aiofiles>=22
 
 asyncVK – асинхронный фреймворк для создания ботов ВК. Преимущества: удобство, скорость выигрываемая за счёт асинхронности.
 =
 
-Бот создаётся за счёт шести структурных единиц: 
+Бот создаётся за счёт пяти основных структурных единиц: 
 1) Bot – это самая главная структурная единица. Это собственно сам бот, который подаёт ивенты     обработчикам.
 2) Handler – эта структурная единица отвечает за обработку ивентов. 
 3) Dispatcher – эта структурная единица отвечает за взаимодействие с ВК (ответы на сообщения, добавление комментариев). Она автоматически настраивается хандлерами.
-4) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
-5) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
-6) Chain - эта структурная единица позволяет создавать цепочки команд.
+4) Condition (Condition, And, Or) – эта структурная единица отвечает за условия. С помощью неё можно строить сложные условия для хандлеров.
+5) Chain - эта структурная единица позволяет создавать цепочки команд.
+
+Также есть такие второстепенные структурные единицы как:
+1) Keyboard – это второстепенная структурная единица. Она отвечает за создание кнопок в ВК.
+2) Message - структура сообщения для облегчения работы с сообщениями.
 
 Как работать с библиотекой? Легко и интуитивно понятно! Для начала нужно импортировать саму библиотеку и создать бота:
 ```python
 from asyncVK import Handler, Bot, run_polling
 from asyncVK.dispatcher import Dispatcher
 from asyncVK.condition import Condition, And, Or
 import asyncVK.keyboard as keyboard
@@ -117,20 +120,41 @@
 
     dispatcher.answer – ответить в ЛС. Можно активировать при любом событии, отправит сообщение инициатору события. Список аргументов: 
 		text – текст сообщения.
 		attachment – вложение сообщения (в виде части ссылки такого рода: 
 		    от ссылки https://vk.com/id386746383?z=photo386746383_457256628%2Falbum386746383_0 
 		    берём только photo386746383_457256628 и передаём это в качестве аргумента). 
 		keyboard – кнопки ВК.
-		
-    dispatcher.send_message – ответить в том же чате. Список аргументов идентичен с answer.
+		Возвращает структуру Message вашего сообщения.
+
+    dispatcher.reply - ответить на сообщение пользователя. Список аргументов и возвращаемое значение идентичны с answer.
+    dispatcher.send_message – ответить в том же чате. Список аргументов и возвращаемое значение идентичны с answer.
     dispatcher.send_comment – ответить в комментариях. Список аргументов идентичен с answer, но аргумент keyboard отсутствует.
     dispatcher.mark_as_read – пометить сообщение как "прочитанное". Никаких аргументов не принимает.
     dispatcher.set_typing_status – установить статус на набор текста / запись голосового сообщения. Принимает один аргумент: 
-        typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+        	typing_status. Его значение по умолчанию "typing" (набор текста). Можно изменить на "audiomessage" – запись голосового сообщения.
+    dispatcher.kick_user - удаляет участника из беседы
+        	member_id - id участника беседы (id сообщества пишется со знаком -)
+    dispatcher.edit_chat_name - изменяет название беседы
+        	title - новое название беседы
+
+Пример использования структуры Message:
+```python
+@bot.handle
+@Handler.on.message_new(Condition(command="прив"))
+async def handler(dispatcher: Dispatcher):
+    message = await dispatcher.reply("Это сообщение исчезнет через 3 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 2 секунды, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.edit("Это сообщение исчезнет через 1 секунду, а твоё сообщение будет закреплено")
+    await asyncio.sleep(1)
+    await message.delete()
+    await dispatcher.message.pin()
+```
 
 Как создать кнопки? Тоже несложно! Вот пример:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     buttons = keyboard.get_keyboard([
@@ -179,19 +203,32 @@
 Параметры диспетчера:
 
     dispatcher.token - ваш токен
     dispatcher.user_id - id инициировавшего событие пользователя
     dispatcher.peer_id - id чата (если это ЛС, то peer_id равен user_id)
     dispatcher.post_id - id записи на стене или обсуждения (если событие это новая запись на стене, новый комментарий на стене или в обсуждении)
     dispatcher.owner_id - если событие было внутри группы, то owner_id это id группы
+    dispatcher.object_id - id объекта события
     dispatcher.event - объект события
     dispatcher.text - если к примеру событие это новое сообщение, то text это текст сообщения, если это к примеру новый комментарий, то text это текст комментария и т.д.
     dispatcher.reply_text - текст отвеченного сообщения (если таковое имеется)
     dispatcher.reply_user_id - id пользователя написавшего отмеченное сообщение (если таковое имеется)
     dispatcher.reply_peer_id - id чата отмеченного сообщения (если таковое имеется)
+    dispatcher.reply_object_id - id объекта ответа
+    dispatcher.message - выдаёт структуру Message для сообщения из события
+    dispatcher.reply_message - выдаёт структуру Message для отвеченного сообщения из события
+
+Возможность структуры Message:
+
+    message.edit - изменить сообщение
+    		text - новый текст
+		attachment - вложение
+ 		keyboard - клавиатура
+    message.pin - закрепить сообщение
+    message.delete - удалить сообщение
 
 Если вы хотите выполнить сразу несколько запросов асинхронно, то можно просто воспользовать библиотекой `asyncio`. К примеру:
 ```python
 @bot.handle
 @Handler.on.message_new(Condition(contains_command="прив"), is_lower=True)
 async def handler(dispatcher: Dispatcher):
     tasks = [asyncio.create_task(dispatcher.mark_as_read()),
```

### Comparing `async_VKsher-1.7.2/setup.py` & `async_VKsher-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 requirements = ["asyncio>=3", "aiohttp>=3", "aiofiles>=22"]
 
 
 setup(
     name="async_VKsher",
-    version="1.7.2",
+    version="2.0.0",
     author="Kulenov Islam",
     author_email="kit.werr34@gmail.com",
     description="asyncVK is asynchronous library for creating a bot in VK",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/Ekventor/asyncVK",
     packages=find_packages(),
```

### Comparing `async_VKsher-1.7.2/upload/__init__.py` & `async_VKsher-2.0.0/upload/__init__.py`

 * *Files identical despite different names*

