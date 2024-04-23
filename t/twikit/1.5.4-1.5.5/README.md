# Comparing `tmp/twikit-1.5.4.tar.gz` & `tmp/twikit-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.4.tar", last modified: Sat Apr 20 04:21:46 2024, max compression
+gzip compressed data, was "twikit-1.5.5.tar", last modified: Mon Apr 22 10:55:00 2024, max compression
```

## Comparing `twikit-1.5.4.tar` & `twikit-1.5.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.206078 twikit-1.5.4/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-20 04:21:46.203087 twikit-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 04:21:46.206078 twikit-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.129282 twikit-1.5.4/twikit/
--rw-rw-rw-   0        0        0      620 2024-04-20 03:59:36.000000 twikit-1.5.4/twikit/__init__.py
--rw-rw-rw-   0        0        0   135693 2024-04-20 03:58:46.000000 twikit-1.5.4/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.4/twikit/community.py
--rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.4/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.4/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.4/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.4/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/trend.py
--rw-rw-rw-   0        0        0    22342 2024-04-20 03:51:37.000000 twikit-1.5.4/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.199097 twikit-1.5.4/twikit/twikit_async/
--rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.4/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   137981 2024-04-20 03:59:02.000000 twikit-1.5.4/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.4/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.4/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    22211 2024-04-18 16:51:47.000000 twikit-1.5.4/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.4/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.4/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.4/twikit/user.py
--rw-rw-rw-   0        0        0    26321 2024-04-20 03:22:02.000000 twikit-1.5.4/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 04:21:46.149231 twikit-1.5.4/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-20 04:21:45.000000 twikit-1.5.4/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 10:55:00.152341 twikit-1.5.5/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-22 10:55:00.150341 twikit-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 10:55:00.152341 twikit-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:55:00.079531 twikit-1.5.5/twikit/
+-rw-rw-rw-   0        0        0      620 2024-04-22 10:54:44.000000 twikit-1.5.5/twikit/__init__.py
+-rw-rw-rw-   0        0        0   137023 2024-04-22 10:50:56.000000 twikit-1.5.5/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.5/twikit/community.py
+-rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.5/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.5/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-22 10:40:20.000000 twikit-1.5.5/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.5/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/trend.py
+-rw-rw-rw-   0        0        0    22706 2024-04-22 10:51:23.000000 twikit-1.5.5/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:55:00.146353 twikit-1.5.5/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.5/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   139325 2024-04-22 10:51:00.000000 twikit-1.5.5/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.5/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.5/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    22587 2024-04-22 10:52:12.000000 twikit-1.5.5/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.5/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.5/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.5/twikit/user.py
+-rw-rw-rw-   0        0        0    27911 2024-04-22 10:43:30.000000 twikit-1.5.5/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:55:00.098482 twikit-1.5.5/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-22 10:54:59.000000 twikit-1.5.5/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-22 10:54:59.000000 twikit-1.5.5/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 10:54:59.000000 twikit-1.5.5/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-22 10:54:59.000000 twikit-1.5.5/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 10:54:59.000000 twikit-1.5.5/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.4/LICENSE` & `twikit-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/PKG-INFO` & `twikit-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.4
+Version: 1.5.5
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.4/README.md` & `twikit-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/setup.py` & `twikit-1.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/__init__.py` & `twikit-1.5.5/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.4'
+__version__ = '1.5.5'
 
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
 from .list import List
```

### Comparing `twikit-1.5.4/twikit/client.py` & `twikit-1.5.5/twikit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     COMMUNITY_NOTE_FEATURES,
     JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     FEATURES,
     TOKEN,
     USER_FEATURES,
     NOTE_TWEET_FEATURES,
+    SIMILAR_POSTS_FEATURES,
     Endpoint,
     Flow,
     Result,
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
@@ -560,14 +561,52 @@
 
         return Result(
             results,
             partial(self.search_user, query, count, next_cursor),
             next_cursor
         )
 
+    def get_similar_tweets(self, tweet_id: str) -> list[Tweet]:
+        """
+        Retrieves tweets similar to the specified tweet (Twitter premium only).
+
+        Parameters
+        ----------
+        tweet_id : :class:`str`
+            The ID of the tweet for which similar tweets are to be retrieved.
+
+        Returns
+        -------
+        list[:class:`Tweet`]
+            A list of Tweet objects representing tweets
+            similar to the specified tweet.
+        """
+        params = flatten_params({
+            'variables': {'tweet_id': tweet_id},
+            'features': SIMILAR_POSTS_FEATURES
+        })
+        response = self.http.get(
+            Endpoint.SIMILAR_POSTS,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        items = find_dict(response, 'entries')[0]
+        results = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            results.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        return results
+
     def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
         status_check_interval: float = 1.0,
         media_type: str | None = None,
         media_category: str | None = None
```

### Comparing `twikit-1.5.4/twikit/community.py` & `twikit-1.5.5/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/errors.py` & `twikit-1.5.5/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/group.py` & `twikit-1.5.5/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/http.py` & `twikit-1.5.5/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/list.py` & `twikit-1.5.5/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/message.py` & `twikit-1.5.5/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/notification.py` & `twikit-1.5.5/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/trend.py` & `twikit-1.5.5/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/tweet.py` & `twikit-1.5.5/twikit/tweet.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,14 +434,26 @@
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
         return self._client.get_favoriters(self.id, count, cursor)
 
+    def get_similar_tweets(self) -> list[Tweet]:
+        """
+        Retrieves tweets similar to the tweet (Twitter premium only).
+
+        Returns
+        -------
+        list[:class:`Tweet`]
+            A list of Tweet objects representing tweets
+            similar to the tweet.
+        """
+        return self._client.get_similar_tweets(self.id)
+
     def update(self) -> None:
         new = self._client.get_tweet_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
```

### Comparing `twikit-1.5.4/twikit/twikit_async/__init__.py` & `twikit-1.5.5/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/client.py` & `twikit-1.5.5/twikit/twikit_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     FEATURES,
     JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     TOKEN,
     USER_FEATURES,
+    SIMILAR_POSTS_FEATURES,
     NOTE_TWEET_FEATURES,
     Endpoint,
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
     get_query_id,
@@ -565,14 +566,52 @@
         return Result(
             results,
             partial(self.search_user,
                     query, count, next_cursor),
             next_cursor
         )
 
+    async def get_similar_tweets(self, tweet_id: str) -> list[Tweet]:
+        """
+        Retrieves tweets similar to the specified tweet (Twitter premium only).
+
+        Parameters
+        ----------
+        tweet_id : :class:`str`
+            The ID of the tweet for which similar tweets are to be retrieved.
+
+        Returns
+        -------
+        list[:class:`Tweet`]
+            A list of Tweet objects representing tweets
+            similar to the specified tweet.
+        """
+        params = flatten_params({
+            'variables': {'tweet_id': tweet_id},
+            'features': SIMILAR_POSTS_FEATURES
+        })
+        response = (await self.http.get(
+            Endpoint.SIMILAR_POSTS,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        items = find_dict(response, 'entries')[0]
+        results = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            results.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        return results
+
     async def upload_media(
         self,
         source: str | bytes,
         wait_for_completion: bool = False,
         status_check_interval: float = 1.0,
         media_type: str | None = None,
         media_category: str | None = None
```

### Comparing `twikit-1.5.4/twikit/twikit_async/community.py` & `twikit-1.5.5/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/errors.py` & `twikit-1.5.5/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/group.py` & `twikit-1.5.5/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/http.py` & `twikit-1.5.5/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/list.py` & `twikit-1.5.5/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/message.py` & `twikit-1.5.5/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/notification.py` & `twikit-1.5.5/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/trend.py` & `twikit-1.5.5/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/tweet.py` & `twikit-1.5.5/twikit/twikit_async/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,14 +431,26 @@
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
         return await self._client.get_favoriters(self.id, count, cursor)
 
+    async def get_similar_tweets(self) -> list[Tweet]:
+        """
+        Retrieves tweets similar to the tweet (Twitter premium only).
+
+        Returns
+        -------
+        list[:class:`Tweet`]
+            A list of Tweet objects representing tweets
+            similar to the tweet.
+        """
+        return await self._client.get_similar_tweets(self.id)
+
     async def update(self) -> None:
         new = await self._client.get_tweet_by_id(self.id)
         self.__dict__.update(new.__dict__)
 
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
```

### Comparing `twikit-1.5.4/twikit/twikit_async/user.py` & `twikit-1.5.5/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/twikit_async/utils.py` & `twikit-1.5.5/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/user.py` & `twikit-1.5.5/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.4/twikit/utils.py` & `twikit-1.5.5/twikit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,38 +106,66 @@
     'responsive_web_graphql_exclude_directive_enabled': True,
     'verified_phone_label_enabled': False,
     'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
     'responsive_web_graphql_timeline_navigation_enabled': True
 }
 
 NOTE_TWEET_FEATURES = {
-    "communities_web_enable_tweet_community_results_fetch": True,
-    "c9s_tweet_anatomy_moderator_badge_enabled": True,
-    "tweetypie_unmention_optimization_enabled": True,
-    "responsive_web_edit_tweet_api_enabled": True,
-    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
-    "view_counts_everywhere_api_enabled": True,
-    "longform_notetweets_consumption_enabled": True,
-    "responsive_web_twitter_article_tweet_consumption_enabled": True,
-    "tweet_awards_web_tipping_enabled": False,
-    "creator_subscriptions_quote_tweet_preview_enabled": False,
-    "longform_notetweets_rich_text_read_enabled": True,
-    "longform_notetweets_inline_media_enabled": True,
-    "articles_preview_enabled": False,
-    "rweb_video_timestamps_enabled": True,
-    "rweb_tipjar_consumption_enabled": True,
-    "responsive_web_graphql_exclude_directive_enabled": True,
-    "verified_phone_label_enabled": False,
-    "freedom_of_speech_not_reach_fetch_enabled": True,
-    "standardized_nudges_misinfo": True,
-    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
-    "tweet_with_visibility_results_prefer_gql_media_interstitial_enabled": True,
-    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
-    "responsive_web_graphql_timeline_navigation_enabled": True,
-    "responsive_web_enhance_cards_enabled": False
+    'communities_web_enable_tweet_community_results_fetch': True,
+    'c9s_tweet_anatomy_moderator_badge_enabled': True,
+    'tweetypie_unmention_optimization_enabled': True,
+    'responsive_web_edit_tweet_api_enabled': True,
+    'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+    'view_counts_everywhere_api_enabled': True,
+    'longform_notetweets_consumption_enabled': True,
+    'responsive_web_twitter_article_tweet_consumption_enabled': True,
+    'tweet_awards_web_tipping_enabled': False,
+    'creator_subscriptions_quote_tweet_preview_enabled': False,
+    'longform_notetweets_rich_text_read_enabled': True,
+    'longform_notetweets_inline_media_enabled': True,
+    'articles_preview_enabled': False,
+    'rweb_video_timestamps_enabled': True,
+    'rweb_tipjar_consumption_enabled': True,
+    'responsive_web_graphql_exclude_directive_enabled': True,
+    'verified_phone_label_enabled': False,
+    'freedom_of_speech_not_reach_fetch_enabled': True,
+    'standardized_nudges_misinfo': True,
+    'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': True,
+    'tweet_with_visibility_results_prefer_gql_media_interstitial_enabled': True,
+    'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+    'responsive_web_graphql_timeline_navigation_enabled': True,
+    'responsive_web_enhance_cards_enabled': False
+}
+
+SIMILAR_POSTS_FEATURES = {
+    'rweb_tipjar_consumption_enabled': True,
+    'responsive_web_graphql_exclude_directive_enabled': True,
+    'verified_phone_label_enabled': False,
+    'creator_subscriptions_tweet_preview_api_enabled': True,
+    'responsive_web_graphql_timeline_navigation_enabled': True,
+    'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+    'communities_web_enable_tweet_community_results_fetch': True,
+    'c9s_tweet_anatomy_moderator_badge_enabled': True,
+    'articles_preview_enabled': False,
+    'tweetypie_unmention_optimization_enabled': True,
+    'responsive_web_edit_tweet_api_enabled': True,
+    'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+    'view_counts_everywhere_api_enabled': True,
+    'longform_notetweets_consumption_enabled': True,
+    'responsive_web_twitter_article_tweet_consumption_enabled': True,
+    'tweet_awards_web_tipping_enabled': False,
+    'creator_subscriptions_quote_tweet_preview_enabled': False,
+    'freedom_of_speech_not_reach_fetch_enabled': True,
+    'standardized_nudges_misinfo': True,
+    'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': True,
+    'tweet_with_visibility_results_prefer_gql_media_interstitial_enabled': True,
+    'rweb_video_timestamps_enabled': True,
+    'longform_notetweets_rich_text_read_enabled': True,
+    'longform_notetweets_inline_media_enabled': True,
+    'responsive_web_enhance_cards_enabled': False
 }
 
 
 class Endpoint:
     """
     A class containing Twitter API endpoints.
     """
@@ -220,14 +248,15 @@
     COMMUNITIES_TIMELINE = 'https://twitter.com/i/api/graphql/4-4iuIdaLPpmxKnA3mr2LA/CommunitiesMainPageTimeline'
     JOIN_COMMUNITY = 'https://twitter.com/i/api/graphql/xZQLbDwbI585YTG0QIpokw/JoinCommunity'
     REQUEST_TO_JOIN_COMMUNITY = 'https://twitter.com/i/api/graphql/XwWChphD_6g7JnsFus2f2Q/RequestToJoinCommunity'
     LEAVE_COMMUNITY = 'https://twitter.com/i/api/graphql/OoS6Kd4-noNLXPZYHtygeA/LeaveCommunity'
     COMMUNITY_MEMBERS = 'https://twitter.com/i/api/graphql/KDAssJ5lafCy-asH4wm1dw/membersSliceTimeline_Query'
     COMMUNITY_MODERATORS = 'https://twitter.com/i/api/graphql/9KI_r8e-tgp3--N5SZYVjg/moderatorsSliceTimeline_Query'
     SEARCH_COMMUNITY_TWEET = 'https://twitter.com/i/api/graphql/5341rmzzvdjqfmPKfoHUBw/CommunityTweetSearchModuleQuery'
+    SIMILAR_POSTS = 'https://twitter.com/i/api/graphql/EToazR74i0rJyZYalfVEAQ/SimilarPosts'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
```

### Comparing `twikit-1.5.4/twikit.egg-info/PKG-INFO` & `twikit-1.5.5/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.4
+Version: 1.5.5
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.4/twikit.egg-info/SOURCES.txt` & `twikit-1.5.5/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

