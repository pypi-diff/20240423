# Comparing `tmp/xgne-0.0.8.tar.gz` & `tmp/xgne-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgne-0.0.8.tar", last modified: Wed Mar 20 16:08:45 2024, max compression
+gzip compressed data, was "xgne-0.0.9.tar", last modified: Tue Apr 23 09:30:45 2024, max compression
```

## Comparing `xgne-0.0.8.tar` & `xgne-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 16:08:45.277890 xgne-0.0.8/
--rw-rw-rw-   0        0        0      431 2024-03-20 16:08:45.276893 xgne-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       34 2024-03-20 13:14:18.000000 xgne-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 16:08:45.278889 xgne-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1168 2024-03-20 16:08:08.000000 xgne-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 16:08:45.235007 xgne-0.0.8/xgne/
--rw-rw-rw-   0        0        0     5371 2024-03-20 16:08:08.000000 xgne-0.0.8/xgne/__init__.py
--rw-rw-rw-   0        0        0    17118 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/defaults.py
-drwxrwxrwx   0        0        0        0 2024-03-20 16:08:45.249966 xgne-0.0.8/xgne/dom/
--rw-rw-rw-   0        0        0     5195 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/dom/DomHandler.py
--rw-rw-rw-   0        0        0       25 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/dom/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 16:08:45.273901 xgne-0.0.8/xgne/extractor/
--rw-rw-rw-   0        0        0    13396 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/ArticleBodyExtractor.py
--rw-rw-rw-   0        0        0     7596 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/AuthorExtractor.py
--rw-rw-rw-   0        0        0     9653 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/ContentExtractor.py
--rw-rw-rw-   0        0        0     3134 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/HeadMetaExtractor.py
--rw-rw-rw-   0        0        0     8799 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/ImageExtractor.py
--rw-rw-rw-   0        0        0     2234 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/LangExtractor.py
--rw-rw-rw-   0        0        0     1408 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/ListExtractor.py
--rw-rw-rw-   0        0        0    22789 2024-03-20 15:07:09.000000 xgne-0.0.8/xgne/extractor/TimeExtractor.py
--rw-rw-rw-   0        0        0     2726 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/TitleExtractor.py
--rw-rw-rw-   0        0        0      312 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/extractor/__init__.py
--rw-rw-rw-   0        0        0    10391 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/parsers.py
--rw-rw-rw-   0        0        0     5777 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/text.py
--rw-rw-rw-   0        0        0     8809 2024-03-20 13:14:18.000000 xgne-0.0.8/xgne/utils.py
--rw-rw-rw-   0        0        0      182 2024-03-20 16:08:08.000000 xgne-0.0.8/xgne/version.py
-drwxrwxrwx   0        0        0        0 2024-03-20 16:08:45.245976 xgne-0.0.8/xgne.egg-info/
--rw-rw-rw-   0        0        0      431 2024-03-20 16:08:45.000000 xgne-0.0.8/xgne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2024-03-20 16:08:45.000000 xgne-0.0.8/xgne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 16:08:45.000000 xgne-0.0.8/xgne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-03-20 16:08:45.000000 xgne-0.0.8/xgne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-20 16:08:45.000000 xgne-0.0.8/xgne.egg-info/top_level.txt
+drwxr-xr-x   0 brucelong   (501) staff       (20)        0 2024-04-23 09:30:45.668647 xgne-0.0.9/
+-rw-r--r--   0 brucelong   (501) staff       (20)      410 2024-04-23 09:30:45.668382 xgne-0.0.9/PKG-INFO
+-rw-r--r--   0 brucelong   (501) staff       (20)       32 2023-12-24 07:19:44.000000 xgne-0.0.9/README.md
+-rw-r--r--   0 brucelong   (501) staff       (20)       38 2024-04-23 09:30:45.668717 xgne-0.0.9/setup.cfg
+-rw-r--r--   0 brucelong   (501) staff       (20)     1137 2024-04-23 09:26:26.000000 xgne-0.0.9/setup.py
+drwxr-xr-x   0 brucelong   (501) staff       (20)        0 2024-04-23 09:30:45.663639 xgne-0.0.9/xgne/
+-rw-r--r--   0 brucelong   (501) staff       (20)     5320 2024-04-23 09:25:09.000000 xgne-0.0.9/xgne/__init__.py
+-rw-------   0 brucelong   (501) staff       (20)    16736 2024-03-20 05:30:42.000000 xgne-0.0.9/xgne/defaults.py
+drwxr-xr-x   0 brucelong   (501) staff       (20)        0 2024-04-23 09:30:45.664799 xgne-0.0.9/xgne/dom/
+-rw-r--r--   0 brucelong   (501) staff       (20)     5066 2024-03-20 05:18:40.000000 xgne-0.0.9/xgne/dom/DomHandler.py
+-rw-r--r--   0 brucelong   (501) staff       (20)       24 2024-03-20 02:09:54.000000 xgne-0.0.9/xgne/dom/__init__.py
+drwxr-xr-x   0 brucelong   (501) staff       (20)        0 2024-04-23 09:30:45.667967 xgne-0.0.9/xgne/extractor/
+-rw-r--r--   0 brucelong   (501) staff       (20)    13054 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/extractor/ArticleBodyExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     7418 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/extractor/AuthorExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     9426 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/extractor/ContentExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     3047 2023-12-29 13:09:50.000000 xgne-0.0.9/xgne/extractor/HeadMetaExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     8554 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/extractor/ImageExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)      686 2023-12-29 08:57:17.000000 xgne-0.0.9/xgne/extractor/InformationExtractor.py
+-rw-------   0 brucelong   (501) staff       (20)     2175 2023-12-27 13:29:41.000000 xgne-0.0.9/xgne/extractor/LangExtractor.py
+-rw-------   0 brucelong   (501) staff       (20)     1367 2023-12-24 07:21:07.000000 xgne-0.0.9/xgne/extractor/ListExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)    22278 2024-03-21 02:06:01.000000 xgne-0.0.9/xgne/extractor/TimeExtractor.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     2661 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/extractor/TitleExtractor.py
+-rw-------   0 brucelong   (501) staff       (20)      306 2023-12-29 13:08:51.000000 xgne-0.0.9/xgne/extractor/__init__.py
+-rw-r--r--   0 brucelong   (501) staff       (20)    10046 2023-12-29 13:28:53.000000 xgne-0.0.9/xgne/parsers.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     5586 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/text.py
+-rw-r--r--   0 brucelong   (501) staff       (20)     8511 2024-03-20 08:35:03.000000 xgne-0.0.9/xgne/utils.py
+-rw-r--r--   0 brucelong   (501) staff       (20)      175 2024-04-23 09:26:26.000000 xgne-0.0.9/xgne/version.py
+drwxr-xr-x   0 brucelong   (501) staff       (20)        0 2024-04-23 09:30:45.664365 xgne-0.0.9/xgne.egg-info/
+-rw-r--r--   0 brucelong   (501) staff       (20)      410 2024-04-23 09:30:45.000000 xgne-0.0.9/xgne.egg-info/PKG-INFO
+-rw-r--r--   0 brucelong   (501) staff       (20)      666 2024-04-23 09:30:45.000000 xgne-0.0.9/xgne.egg-info/SOURCES.txt
+-rw-r--r--   0 brucelong   (501) staff       (20)        1 2024-04-23 09:30:45.000000 xgne-0.0.9/xgne.egg-info/dependency_links.txt
+-rw-r--r--   0 brucelong   (501) staff       (20)       66 2024-04-23 09:30:45.000000 xgne-0.0.9/xgne.egg-info/requires.txt
+-rw-r--r--   0 brucelong   (501) staff       (20)        5 2024-04-23 09:30:45.000000 xgne-0.0.9/xgne.egg-info/top_level.txt
```

### Comparing `xgne-0.0.8/xgne/__init__.py` & `xgne-0.0.9/xgne/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,113 @@
-from lxml.etree import tostring
-
-from .utils import pre_parse, remove_noise_node, config, html2element, normalize_text
-from .extractor import ContentExtractor, TitleExtractor, TimeExtractor, AuthorExtractor, ListExtractor, LangExtractor, \
-    HeadMetaExtractor
-from newspaper import Config, Article
-
-
-class GeneralNewsExtractor:
-    def __init__(self):
-        # 配置 newspaper
-        self.config = Config()
-
-    def extract(self,
-                html,
-                title_xpath='',
-                author_xpath='',
-                publish_time_xpath='',
-                host='',
-                body_xpath='',
-                noise_node_list=None,
-                with_body_html=False,
-                use_visiable_info=False):
-        article = Article('')
-        try:
-            # 对 HTML 进行预处理可能会破坏 HTML 原有的结构，导致根据原始 HTML 编写的 XPath 不可用
-            # 因此，如果指定了 title_xpath/author_xpath/publish_time_xpath，那么需要先提取再进行
-            article.set_html(html)
-            article.parse()
-            # 输出已解析的信息
-            info_dict = {
-                'movies': article.movies,
-                'keywords': article.keywords,
-                'meta_keywords': article.meta_keywords,
-                'meta_description': article.meta_description,
-                'summary': article.summary,
-                'tags': article.tags or [],
-                'canonical_link': article.canonical_link,
-                'source_url': article.source_url,
-            }
-            body_html = ''
-            if article.clean_top_node:
-                body_html = tostring(article.clean_top_node, encoding="unicode", method="html")
-            try:
-                # 预处理
-                normal_html = normalize_text(html)
-                element = html2element(normal_html)
-                lang = LangExtractor().language(html)
-                headmeta = HeadMetaExtractor().extractor(element)
-                title = TitleExtractor().extract(element, title_xpath=title_xpath)
-                author = AuthorExtractor().extractor(element, author_xpath=author_xpath) or article.authors
-                element = pre_parse(element)
-                remove_noise_node(element, noise_node_list)
-                if not host:
-                    host = headmeta.get('host')
-                content = ContentExtractor().extract(element,
-                                                     host=host,
-                                                     with_body_html=with_body_html,
-                                                     body_xpath=body_xpath,
-                                                     use_visiable_info=use_visiable_info)
-                publish_time = TimeExtractor().extractor(element,
-                                                         publish_time_xpath=publish_time_xpath,
-                                                         normal_html=normal_html,
-                                                         title=title,
-                                                         content=content[0][1]['text'],
-                                                         html=html,
-                                                         npp_pt=article.publish_date
-                                                         )
-                text = content[0][1]['text']
-                npp_text = article.text
-                if npp_text and len(npp_text) > len(text):
-                    text = npp_text
-                else:
-                    body_html = content[0][1]['body_html']
-                result = {'title': title,
-                          'author': author,
-                          'publish_time': publish_time,
-                          'lang': lang,
-                          'content': text,
-                          'images': content[0][1]['images'],
-                          'headmeta': headmeta,
-                          'top_image': headmeta.pop('top_image'),
-                          'website': headmeta.pop('host')
-                          }
-            except:
-                publish_time_temp = article.publish_date
-                publish_time = TimeExtractor().deal_publish_time_dtt(publish_time_temp)
-                result = {
-                    'title': article.title,
-                    'author': article.authors,
-                    'publish_time': publish_time,
-                    'lang': article.meta_lang,
-                    'content': article.text,
-                    'images': article.imgs,
-                    'headmeta': dict(article.meta_data),
-                    'top_image': article.top_image,
-                    'website': host
-                }
-            if with_body_html or config.get('with_body_html', False):
-                result['body_html'] = body_html
-            result = dict(result, **info_dict)
-            return result
-        except Exception as e:
-            return {'error': "parser error," + str(e)}
-
-
-class ListPageExtractor:
-    def extract(self, html, feature):
-        normalize_html = normalize_text(html)
-        element = html2element(normalize_html)
-        extractor = ListExtractor()
-        return extractor.extract(element, feature)
+from lxml.etree import tostring
+
+from .utils import pre_parse, remove_noise_node, config, html2element, normalize_text
+from .extractor import ContentExtractor, TitleExtractor, TimeExtractor, AuthorExtractor, ListExtractor, LangExtractor, \
+    HeadMetaExtractor
+from newspaper import Config, Article
+
+
+class GeneralNewsExtractor:
+    def __init__(self):
+        # 配置 newspaper
+        self.config = Config()
+        self.config.fetch_images = False
+
+    def extract(self,
+                html,
+                title_xpath='',
+                author_xpath='',
+                publish_time_xpath='',
+                host='',
+                body_xpath='',
+                noise_node_list=None,
+                with_body_html=False,
+                use_visiable_info=False):
+        article = Article('', config=self.config)
+        try:
+            # 对 HTML 进行预处理可能会破坏 HTML 原有的结构，导致根据原始 HTML 编写的 XPath 不可用
+            # 因此，如果指定了 title_xpath/author_xpath/publish_time_xpath，那么需要先提取再进行
+            article.set_html(html)
+            article.parse()
+            # 输出已解析的信息
+            info_dict = {
+                'movies': article.movies,
+                'keywords': article.keywords,
+                'meta_keywords': article.meta_keywords,
+                'meta_description': article.meta_description,
+                'summary': article.summary,
+                'tags': article.tags or [],
+                'canonical_link': article.canonical_link,
+                'source_url': article.source_url,
+            }
+            body_html = ''
+            if article.clean_top_node:
+                body_html = tostring(article.clean_top_node, encoding="unicode", method="html")
+            try:
+                # 预处理
+                normal_html = normalize_text(html)
+                element = html2element(normal_html)
+                lang = LangExtractor().language(html)
+                headmeta = HeadMetaExtractor().extractor(element)
+                title = TitleExtractor().extract(element, title_xpath=title_xpath)
+                author = AuthorExtractor().extractor(element, author_xpath=author_xpath) or article.authors
+                element = pre_parse(element)
+                remove_noise_node(element, noise_node_list)
+                if not host:
+                    host = headmeta.get('host')
+                content = ContentExtractor().extract(element,
+                                                     host=host,
+                                                     with_body_html=with_body_html,
+                                                     body_xpath=body_xpath,
+                                                     use_visiable_info=use_visiable_info)
+                publish_time = TimeExtractor().extractor(element,
+                                                         publish_time_xpath=publish_time_xpath,
+                                                         normal_html=normal_html,
+                                                         title=title,
+                                                         content=content[0][1]['text'],
+                                                         html=html,
+                                                         npp_pt=article.publish_date
+                                                         )
+                text = content[0][1]['text']
+                npp_text = article.text
+                if npp_text and len(npp_text) > len(text):
+                    text = npp_text
+                else:
+                    body_html = content[0][1]['body_html']
+                result = {'title': title,
+                          'author': author,
+                          'publish_time': publish_time,
+                          'lang': lang,
+                          'content': text,
+                          'images': content[0][1]['images'],
+                          'headmeta': headmeta,
+                          'top_image': headmeta.pop('top_image'),
+                          'website': headmeta.pop('host')
+                          }
+            except:
+                publish_time_temp = article.publish_date
+                publish_time = TimeExtractor().deal_publish_time_dtt(publish_time_temp)
+                result = {
+                    'title': article.title,
+                    'author': article.authors,
+                    'publish_time': publish_time,
+                    'lang': article.meta_lang,
+                    'content': article.text,
+                    'images': article.imgs,
+                    'headmeta': dict(article.meta_data),
+                    'top_image': article.top_image,
+                    'website': host
+                }
+            if with_body_html or config.get('with_body_html', False):
+                result['body_html'] = body_html
+            result = dict(result, **info_dict)
+            return result
+        except Exception as e:
+            return {'error': "parser error," + str(e)}
+
+
+class ListPageExtractor:
+    def extract(self, html, feature):
+        normalize_html = normalize_text(html)
+        element = html2element(normalize_html)
+        extractor = ListExtractor()
+        return extractor.extract(element, feature)
```

### Comparing `xgne-0.0.8/xgne/defaults.py` & `xgne-0.0.9/xgne/defaults.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,382 +1,382 @@
-# *********************************作者配置信息********************************
-import re
-
-AUTHOR_PATTERN = [
-    "责编[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "责任编辑[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "作者[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "编辑[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "文[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "原创[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "撰文[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
-    "来源[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：|<]",
-    # 以下正则表达式需要进一步测试
-    # '(作者[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
-    # '(记者[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
-    # '(原创[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
-    # '(撰文[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
-    # '(文/图[：|:| |丨|/]?\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
-]
-
-AUTHOR_ATTRS = ["name", "rel", "itemprop", "class", "id", "property"]
-AUTHOR_VALS = [
-    "author",
-    "byline",
-    "dc.creator",
-    "byl",
-    "article:author",
-    "story-byline",
-    "article-author",
-]
-AUTHOR_STOP_WORDS = [
-    "By",
-    "Reuters",
-    "IANS",
-    "AP",
-    "AFP",
-    "PTI",
-    "IANS",
-    "ANI",
-    "DPA",
-    "Senior Reporter",
-    "Reporter",
-    "Writer",
-    "Opinion Writer",
-]
-# *********************************时间相关配置信息********************************
-DATETIME_PATTERN = [
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{4})",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
-    "(\d{4}年\d{1,2}月\d{1,2}日)",
-    "(\d{1,2}月(\.| |-|,)*\d{1,2}(\.| |-|,)*\d{4})",  # 4月 30, 2018
-    "((\d{4})(\.|,| |\|)*年(\.|,| |\|)*\d{1,2}(\.|,| |\|)*月(\.|,| |\|)*\d{1,2}日)",  # 年月日中间带有空格.和,
-    "(\d{2}年\d{1,2}月\d{1,2}日)",
-    "(\d{1,2}月\d{1,2}日)"
-]
-
-PUBLISH_TIME_META = [  # 部分特别规范的新闻网站，可以直接从 HTML 的 meta 数据中获得发布时间
-    '//meta[starts-with(@property, "rnews:datePublished")]/@content',
-    '//meta[starts-with(@property, "article:published_time")]/@content',
-    '//meta[starts-with(@property, "og:published_time")]/@content',
-    '//meta[starts-with(@property, "og:release_date")]/@content',
-    '//meta[starts-with(@itemprop, "datePublished")]/@content',
-    '//meta[starts-with(@itemprop, "dateUpdate")]/@content',
-    '//meta[starts-with(@name, "OriginalPublicationDate")]/@content',
-    '//meta[starts-with(@name, "article_date_original")]/@content',
-    '//meta[starts-with(@name, "og:time")]/@content',
-    '//meta[starts-with(@name, "apub:time")]/@content',
-    '//meta[starts-with(@name, "publication_date")]/@content',
-    '//meta[starts-with(@name, "sailthru.date")]/@content',
-    '//meta[starts-with(@name, "PublishDate")]/@content',
-    '//meta[starts-with(@name, "publishdate")]/@content',
-    '//meta[starts-with(@name, "PubDate")]/@content',
-    '//meta[starts-with(@name, "pubtime")]/@content',
-    '//meta[starts-with(@name, "_pubtime")]/@content',
-    '//meta[starts-with(@name, "weibo: article:create_at")]/@content',
-    '//meta[starts-with(@pubdate, "pubdate")]/@content',
-]
-JW_DATETIME_PATTERN = [
-    "(((\d{1,2}:\d{1,2}:\d{1,2})(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})))",
-    "((\d{1,2}:\d{1,2})(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4}))",
-    "(\d{1,4}(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
-    "((January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
-    "(\d{1,4}(\.|,| |\||/|-|—|\[|\])*(Januari|Februari|Maret|April|Mei|Juni|Juli|Agustus|September|Oktober|November|Desember)(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
-    "((Januari|Februari|Maret|April|Mei|Juni|Juli|Agustus|September|Oktober|November|Desember)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
-    # 印度尼西亚月份
-
-    "(\d{1,2}) ?(minutes|hours|day|days) ?(ago)",  # 3 days ago
-    "\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}Z$",  # 标准utc 时间
-    '\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d+Z$'  # 带毫秒的utc 时间 2023-03-27T10:00:22.260993Z
-    "(\d{4}(\.| |\|)*\d{1,2}(\.| |\|)*\d{1,2}(\.| |\|)*\d{2}:\d{2}:\d{2})",  # 2016. 9. 20. 15:01:01
-    "(\d{4}(\.| |\|)*\d{1,2}(\.| |\|)*\d{1,2}(\.| |\|)*\d{2}:\d{2})",  # 2016. 9. 20. 15:01
-
-]
-DATETIME_PATTERN.extend(JW_DATETIME_PATTERN)
-# *********************************标题配置信息********************************
-TITLE_HTAG_XPATH = '//h1//text() | //h2//text() | //h3//text() | //h4//text()'
-
-TITLE_SPLIT_CHAR_PATTERN = '[-_|]'
-
-USELESS_TAG = ['style', 'script', 'link', 'video', 'iframe', 'source', 'picture', 'header', 'blockquote',
-               'footer']
-
-# if one tag in the follow list does not contain any child node nor content, it could be removed
-TAGS_CAN_BE_REMOVE_IF_EMPTY = ['section', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'span']
-
-USELESS_ATTR = {
-    'share',
-    'contribution',
-    'copyright',
-    'copy-right',
-    'disclaimer',
-    'recommend',
-    'related',
-    'footer',
-    'comment',
-    'social',
-    'submeta',
-    'report-infor'
-}
-
-# *********************************正文配置信息********************************
-HIGH_WEIGHT_ARRT_KEYWORD = ['content',
-                            'article',
-                            'news_txt',
-                            'post_text']
-
-# *********************************Meta配置信息********************************
-META_IMAGE_TAGS = [
-    {"tag": "meta", "field": 'meta[property="og:image"]', "score": 10},
-    {"tag": "link", "attr": "rel", "value": "image_src|img_src", "score": 8},
-    {"tag": "meta", "field": 'meta[name="og:image"]', "score": 8},
-    {"tag": "link", "attr": "rel", "value": "icon", "score": 5},
-]
-
-ARTICLE_BODY_TAGS = [
-    {"tag": "article", "role": "article"},
-    {"itemprop": "articleBody"},
-    {"itemtype": "https://schema.org/Article"},
-    {"itemtype": "https://schema.org/NewsArticle"},
-    {"itemtype": "https://schema.org/BlogPosting"},
-    {"itemtype": "https://schema.org/ScholarlyArticle"},
-    {"itemtype": "https://schema.org/SocialMediaPosting"},
-    {"itemtype": "https://schema.org/TechArticle"},
-]
-
-ALLOWED_TYPES = [
-    "html",
-    "htm",
-    "md",
-    "rst",
-    "aspx",
-    "jsp",
-    "rhtml",
-    "cgi",
-    "xhtml",
-    "jhtml",
-    "asp",
-    "shtml",
-]
-TOP_IMAGE_SETTINGS = {
-    "min_width": 300,
-    "min_height": 200,
-    "min_area": 10000,
-    "max_retries": 2,
-}
-TIME_TOKEN = ['发布时间', '发表时间', '发布日期', '时间:', '时间：', '日期：', '更新時間：',
-              'Updated:', 'Published:', 'published about', 'issue', 'issued', '當前報紙', '發表於', 'Updated', 'Published on ',
-              'Published: '
-              ]
-
-INLINE_TAG = ['span', 'a', 'em', 'b', 'i', 'small', 'strong']
-MAYBEIS = ['and', 'article', 'body', 'column', 'main', 'shadow']
-
-DATETIME_PATTERN_COMPARE = [
-    # "((((\.|,| |\||/|-|—)*)?)(\d{1,2}:\d{1,2}((:\d{1,2})?))?(((\.|,| |\||/|-|—)*)?)(\d{1,4})?(((\.|,| |\||/|-|—)*)?)(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(((\.|,| |\||/|-|—)*)?)((\d{2,4})?)(((\.|,| |\||/|-|—)*)?)((\d{2,4})?)(((\.|,| |\||/|-|—)*)?)(\d{1,2}:\d{1,2}((:\d{1,2})?))?(((\.|,| |\||/|-|—)*)?)\w+(([\+-]\d)?))",
-    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 2020-04-05 12:23:23
-    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 2020-04-05 12:23
-    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 2020-04-05 12时23分05秒
-    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 2020-04-05 12时23分
-    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 20-04-05 12:23:23
-    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 20-04-05 12:23
-    "([1-2]\d{3}年\s*\d{1,2}月\s*\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 2020年3月12日  12:23:23
-    "([1-2]\d{3}年\s*\d{1,2}月\s*\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 2020年3月12日  12:23
-    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 2020年3月12日  12时23分45秒
-    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 2020年3月12日  12时23分
-    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 20年3月12日  12:23:23
-    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?星期.\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 20年3月12日  12:23
-    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 20年3月12日  12时23分45秒
-    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 20年3月12日  12时23分
-    "(\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 3月12日  12:23:23
-    "(\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 3月12日  12:23
-    "(\d{1,2}[-|/|.]\d{1,2}\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 04-05 12:23:23
-    "(\d{1,2}[-|/|.]\d{1,2}\s+[0-2]?[0-9]:[0-5]?[0-9])",  # 04-05 12:23
-    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",  # 2020-3-12
-    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",  # 20-3-12
-    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?)",  # 2020年3月12日
-    "([0-2]\d{1}年\d{1,2}月\d{1,2}日?)",  # 20年3月12日
-
-]
-
-
-def jp_sub_func(match):
-    if match.group(1) == '令和':
-
-        if str(match.group(2)).isdigit():
-            return str(2018 + int(match.group(2))) + '年'
-        elif match.group(2) == '元':
-            return str(2019) + '年'
-
-    elif match.group(1) == '平成':
-        if str(match.group(2)).isdigit():
-            return str(2018 + int(match.group(2))) + '年'
-        elif match.group(2) == '元':
-            return str(1989) + '年'
-
-    else:
-        return match.group()
-
-
-def sub_st(match):
-    if match.group(0).strip() in ['august', 'Agustus']:
-        return match.group(0)
-    else:
-        return ' '
-
-
-RE_SUB_MAP = {
-    '(Monday|Tuesday|Wednesday|Thursday|Friday|Saturday|Sunday)': ' ',
-    '(Mon|Tues|Wed|Thur|Fri|Sat|Sun)': ' ',
-    '(Mon|Tue|Wed|Thu|Fri|Sat|Sun)': ' ',
-    '(Mon.|Tues.|Wed.|Thur.|Fri.|Sat.|Sun.)': ' ',
-    # '(AM|PM|a.m.|p.m.)': ' ',
-    '(on|at)': ' ',
-    '(nd|rd|th)': ' ',
-    '(平成|令和)(\S+)年': jp_sub_func,
-    '.*?st.*?': sub_st,
-    '時': '时'
-
-}
-# name itemprop property
-
-MATA_TIME_TOKEN = {
-    'article:published_time',
-    'datePublished',
-    'dateUpdate',
-    'pubDate',
-    'pubdate',
-    'date',
-    'og:published_time',
-    'og:article:published_time',
-    'og:release_date',
-    'og:time',
-    'render_timestamp',
-    'weibo: article:create_at',
-    '_pubtime',
-    'cXenseParse:recs:publishtime',
-    'pubtime',
-    'PubDate',
-    'publishdate',
-    'PublishDate',
-    'publishDate',
-    'sailthru.date',
-    'publication_date',
-    'apub:time',
-    'article_date_original',
-    'OriginalPublicationDate',
-    'dcterms.date',
-    'nv:news:date',
-    'parsely-pub-date',
-    'citation_publication_date',
-    'article:published_time',
-    'issueDate',
-    'date.release'
-}
-PUBLISH_TIME_META_EXTRA = [
-    '//meta[starts-with(@pubdate, "pubdate")]/@content',
-    '//meta[contains(@name, "date")]/@content',
-    '//meta[contains(@name, "publish")]/@content',
-    '//meta[contains(@name, "published")]/@content',
-    '//meta[contains(@property, "published")]/@content',
-    '//meta[contains(@property, "publish")]/@content',
-    '//meta[contains(@property, "date")]/@content',
-    '//meta[contains(@itemprop, "date")]/@content',
-    '//meta[contains(@itemprop, "publish")]/@content',
-    '//meta[contains(@itemprop, "published")]/@content',
-]
-
-
-def generate_meta_xpath():
-    for prop in ['name', 'itemprop', 'property']:
-        for class_name in MATA_TIME_TOKEN:
-            pattern = '//meta[starts-with(@%s, "%s")]/@content'
-            PUBLISH_TIME_META.append(pattern % (prop, class_name))
-    PUBLISH_TIME_META.extend(PUBLISH_TIME_META_EXTRA)
-
-
-STOPWORDS_DIR = ''
-
-generate_meta_xpath()
-
-PUBLISH_TIME_TAG = [
-    '//time/@datetime',  # h5 time 标签
-    '//time/@dateTime',  # h5 time 标签
-    '//relative-time/@datetime',  # h5 time 标签
-    '//*[@id="story_date"]/text()',
-    '//*[@class="time"]/text()',
-    '//time/@content',
-    '//*[@class="date"]/text()',
-    '//*[contains(@class,"date-time")]/text()',
-    '//*[contains(@class,"updated-date-time")]/text()',
-    '//*[contains(@class,"num_date")]/text()',
-    '//*[contains(@class,"se_date")]/text()',
-    '//*[contains(@class,"post-date")]/text()',
-    '//*[contains(@class,"teaser-byline-text-date")]/text()',
-    '//*[contains(@class,"date_posted")]/text()',
-    '//*[@itemprop="datePublished"]/@content',
-    '//time/text()',
-    '//*[@class="time"]/text()',
-    '//*[contains(@class,"date")]/text()',
-    '//*[contains(@class,"time")]/text()',
-]
-
-SCRIPT_TIME_RE = [
-
-]
-
-## 只取group 1 的这个要注意
-BASE_SCRIPT_TIME_RE = """["\']?%s *["\']? *: *["\']?(.*?)["\']"""
-SCRIPT_TIME_RE_TOKEN = [
-    'datePublished',
-    'publishedDate',
-    'created_date',
-    'publish_date',
-    'publishedDateCro',
-    'publishedDateUtc',
-    'publishedAtDate',
-    'articlePublishTime',
-    'ep_contentdata_delivered_date',
-    'deliveredDate',
-    "createdAt",
-    'dateModified',
-]
-SCRIPT_TIME_RE_EXTRA = [
-
-]
-
-
-def generate_script_re():
-    for token in SCRIPT_TIME_RE_TOKEN:
-        SCRIPT_TIME_RE.append(re.compile(BASE_SCRIPT_TIME_RE % token, re.I))
-    SCRIPT_TIME_RE.extend(SCRIPT_TIME_RE_EXTRA)
-
-
-generate_script_re()
-
-USELESS_TAG_TO_TIME = ['style', 'link', 'iframe', 'blockquote']
+# *********************************作者配置信息********************************
+import re
+
+AUTHOR_PATTERN = [
+    "责编[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "责任编辑[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "作者[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "编辑[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "文[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "原创[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "撰文[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：]",
+    "来源[：|:| |丨|/]\s*([\u4E00-\u9FA5a-zA-Z]{2,20})[^\u4E00-\u9FA5|:|：|<]",
+    # 以下正则表达式需要进一步测试
+    # '(作者[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
+    # '(记者[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
+    # '(原创[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
+    # '(撰文[：|:| |丨|/]\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
+    # '(文/图[：|:| |丨|/]?\s*[\u4E00-\u9FA5a-zA-Z、 ]{2,20})[）】)]]?[^\u4E00-\u9FA5|:|：]',
+]
+
+AUTHOR_ATTRS = ["name", "rel", "itemprop", "class", "id", "property"]
+AUTHOR_VALS = [
+    "author",
+    "byline",
+    "dc.creator",
+    "byl",
+    "article:author",
+    "story-byline",
+    "article-author",
+]
+AUTHOR_STOP_WORDS = [
+    "By",
+    "Reuters",
+    "IANS",
+    "AP",
+    "AFP",
+    "PTI",
+    "IANS",
+    "ANI",
+    "DPA",
+    "Senior Reporter",
+    "Reporter",
+    "Writer",
+    "Opinion Writer",
+]
+# *********************************时间相关配置信息********************************
+DATETIME_PATTERN = [
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    "(\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{4})",
+    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
+    "(\d{4}年\d{1,2}月\d{1,2}日)",
+    "(\d{1,2}月(\.| |-|,)*\d{1,2}(\.| |-|,)*\d{4})",  # 4月 30, 2018
+    "((\d{4})(\.|,| |\|)*年(\.|,| |\|)*\d{1,2}(\.|,| |\|)*月(\.|,| |\|)*\d{1,2}日)",  # 年月日中间带有空格.和,
+    "(\d{2}年\d{1,2}月\d{1,2}日)",
+    "(\d{1,2}月\d{1,2}日)"
+]
+
+PUBLISH_TIME_META = [  # 部分特别规范的新闻网站，可以直接从 HTML 的 meta 数据中获得发布时间
+    '//meta[starts-with(@property, "rnews:datePublished")]/@content',
+    '//meta[starts-with(@property, "article:published_time")]/@content',
+    '//meta[starts-with(@property, "og:published_time")]/@content',
+    '//meta[starts-with(@property, "og:release_date")]/@content',
+    '//meta[starts-with(@itemprop, "datePublished")]/@content',
+    '//meta[starts-with(@itemprop, "dateUpdate")]/@content',
+    '//meta[starts-with(@name, "OriginalPublicationDate")]/@content',
+    '//meta[starts-with(@name, "article_date_original")]/@content',
+    '//meta[starts-with(@name, "og:time")]/@content',
+    '//meta[starts-with(@name, "apub:time")]/@content',
+    '//meta[starts-with(@name, "publication_date")]/@content',
+    '//meta[starts-with(@name, "sailthru.date")]/@content',
+    '//meta[starts-with(@name, "PublishDate")]/@content',
+    '//meta[starts-with(@name, "publishdate")]/@content',
+    '//meta[starts-with(@name, "PubDate")]/@content',
+    '//meta[starts-with(@name, "pubtime")]/@content',
+    '//meta[starts-with(@name, "_pubtime")]/@content',
+    '//meta[starts-with(@name, "weibo: article:create_at")]/@content',
+    '//meta[starts-with(@pubdate, "pubdate")]/@content',
+]
+JW_DATETIME_PATTERN = [
+    "(((\d{1,2}:\d{1,2}:\d{1,2})(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})))",
+    "((\d{1,2}:\d{1,2})(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4}))",
+    "(\d{1,4}(\.|,| |\||/|-|—|\[|\])*(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
+    "((January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
+    "(\d{1,4}(\.|,| |\||/|-|—|\[|\])*(Januari|Februari|Maret|April|Mei|Juni|Juli|Agustus|September|Oktober|November|Desember)(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
+    "((Januari|Februari|Maret|April|Mei|Juni|Juli|Agustus|September|Oktober|November|Desember)(\.|,| |\||/|-|—|\[|\])*\d{1,4}(\.|,| |\||/|-|—|\[|\])*(\d{2,4})(\.|,| |\||/|-|—|\[|\])*(\d{1,2}:\d{1,2}((:\d{1,2})?))?)",
+    # 印度尼西亚月份
+
+    "(\d{1,2}) ?(minutes|hours|day|days) ?(ago)",  # 3 days ago
+    "\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}Z$",  # 标准utc 时间
+    '\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d+Z$'  # 带毫秒的utc 时间 2023-03-27T10:00:22.260993Z
+    "(\d{4}(\.| |\|)*\d{1,2}(\.| |\|)*\d{1,2}(\.| |\|)*\d{2}:\d{2}:\d{2})",  # 2016. 9. 20. 15:01:01
+    "(\d{4}(\.| |\|)*\d{1,2}(\.| |\|)*\d{1,2}(\.| |\|)*\d{2}:\d{2})",  # 2016. 9. 20. 15:01
+
+]
+DATETIME_PATTERN.extend(JW_DATETIME_PATTERN)
+# *********************************标题配置信息********************************
+TITLE_HTAG_XPATH = '//h1//text() | //h2//text() | //h3//text() | //h4//text()'
+
+TITLE_SPLIT_CHAR_PATTERN = '[-_|]'
+
+USELESS_TAG = ['style', 'script', 'link', 'video', 'iframe', 'source', 'picture', 'header', 'blockquote',
+               'footer']
+
+# if one tag in the follow list does not contain any child node nor content, it could be removed
+TAGS_CAN_BE_REMOVE_IF_EMPTY = ['section', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'span']
+
+USELESS_ATTR = {
+    'share',
+    'contribution',
+    'copyright',
+    'copy-right',
+    'disclaimer',
+    'recommend',
+    'related',
+    'footer',
+    'comment',
+    'social',
+    'submeta',
+    'report-infor'
+}
+
+# *********************************正文配置信息********************************
+HIGH_WEIGHT_ARRT_KEYWORD = ['content',
+                            'article',
+                            'news_txt',
+                            'post_text']
+
+# *********************************Meta配置信息********************************
+META_IMAGE_TAGS = [
+    {"tag": "meta", "field": 'meta[property="og:image"]', "score": 10},
+    {"tag": "link", "attr": "rel", "value": "image_src|img_src", "score": 8},
+    {"tag": "meta", "field": 'meta[name="og:image"]', "score": 8},
+    {"tag": "link", "attr": "rel", "value": "icon", "score": 5},
+]
+
+ARTICLE_BODY_TAGS = [
+    {"tag": "article", "role": "article"},
+    {"itemprop": "articleBody"},
+    {"itemtype": "https://schema.org/Article"},
+    {"itemtype": "https://schema.org/NewsArticle"},
+    {"itemtype": "https://schema.org/BlogPosting"},
+    {"itemtype": "https://schema.org/ScholarlyArticle"},
+    {"itemtype": "https://schema.org/SocialMediaPosting"},
+    {"itemtype": "https://schema.org/TechArticle"},
+]
+
+ALLOWED_TYPES = [
+    "html",
+    "htm",
+    "md",
+    "rst",
+    "aspx",
+    "jsp",
+    "rhtml",
+    "cgi",
+    "xhtml",
+    "jhtml",
+    "asp",
+    "shtml",
+]
+TOP_IMAGE_SETTINGS = {
+    "min_width": 300,
+    "min_height": 200,
+    "min_area": 10000,
+    "max_retries": 2,
+}
+TIME_TOKEN = ['发布时间', '发表时间', '发布日期', '时间:', '时间：', '日期：', '更新時間：',
+              'Updated:', 'Published:', 'published about', 'issue', 'issued', '當前報紙', '發表於', 'Updated', 'Published on ',
+              'Published: '
+              ]
+
+INLINE_TAG = ['span', 'a', 'em', 'b', 'i', 'small', 'strong']
+MAYBEIS = ['and', 'article', 'body', 'column', 'main', 'shadow']
+
+DATETIME_PATTERN_COMPARE = [
+    # "((((\.|,| |\||/|-|—)*)?)(\d{1,2}:\d{1,2}((:\d{1,2})?))?(((\.|,| |\||/|-|—)*)?)(\d{1,4})?(((\.|,| |\||/|-|—)*)?)(January|February|March|April|May|June|July|August|September|October|November|December|Jan|Feb|Mar|Apr|Aug|Sept|Oct|Nov|Dec)(((\.|,| |\||/|-|—)*)?)((\d{2,4})?)(((\.|,| |\||/|-|—)*)?)((\d{2,4})?)(((\.|,| |\||/|-|—)*)?)(\d{1,2}:\d{1,2}((:\d{1,2})?))?(((\.|,| |\||/|-|—)*)?)\w+(([\+-]\d)?))",
+    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 2020-04-05 12:23:23
+    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 2020-04-05 12:23
+    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 2020-04-05 12时23分05秒
+    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 2020-04-05 12时23分
+    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 20-04-05 12:23:23
+    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2}/?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 20-04-05 12:23
+    "([1-2]\d{3}年\s*\d{1,2}月\s*\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 2020年3月12日  12:23:23
+    "([1-2]\d{3}年\s*\d{1,2}月\s*\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 2020年3月12日  12:23
+    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 2020年3月12日  12时23分45秒
+    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 2020年3月12日  12时23分
+    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 20年3月12日  12:23:23
+    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?星期.\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 20年3月12日  12:23
+    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9][时|点][0-5]?[0-9]分[0-5]?[0-9]秒)",  # 20年3月12日  12时23分45秒
+    "([1-2]\d{1}年\d{1,2}月\d{1,2}日?\s*?[[0-2]?[0-9][时|点][0-5]?[0-9]分)",  # 20年3月12日  12时23分
+    "(\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 3月12日  12:23:23
+    "(\d{1,2}月\d{1,2}日?\s*?[0-2]?[0-9]:[0-5]?[0-9])",  # 3月12日  12:23
+    "(\d{1,2}[-|/|.]\d{1,2}\s*?[0-2]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",  # 04-05 12:23:23
+    "(\d{1,2}[-|/|.]\d{1,2}\s+[0-2]?[0-9]:[0-5]?[0-9])",  # 04-05 12:23
+    "([1-2]\d{3}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",  # 2020-3-12
+    "([1-2]\d{1}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",  # 20-3-12
+    "([1-2]\d{3}年\d{1,2}月\d{1,2}日?)",  # 2020年3月12日
+    "([0-2]\d{1}年\d{1,2}月\d{1,2}日?)",  # 20年3月12日
+
+]
+
+
+def jp_sub_func(match):
+    if match.group(1) == '令和':
+
+        if str(match.group(2)).isdigit():
+            return str(2018 + int(match.group(2))) + '年'
+        elif match.group(2) == '元':
+            return str(2019) + '年'
+
+    elif match.group(1) == '平成':
+        if str(match.group(2)).isdigit():
+            return str(2018 + int(match.group(2))) + '年'
+        elif match.group(2) == '元':
+            return str(1989) + '年'
+
+    else:
+        return match.group()
+
+
+def sub_st(match):
+    if match.group(0).strip() in ['august', 'Agustus']:
+        return match.group(0)
+    else:
+        return ' '
+
+
+RE_SUB_MAP = {
+    '(Monday|Tuesday|Wednesday|Thursday|Friday|Saturday|Sunday)': ' ',
+    '(Mon|Tues|Wed|Thur|Fri|Sat|Sun)': ' ',
+    '(Mon|Tue|Wed|Thu|Fri|Sat|Sun)': ' ',
+    '(Mon.|Tues.|Wed.|Thur.|Fri.|Sat.|Sun.)': ' ',
+    # '(AM|PM|a.m.|p.m.)': ' ',
+    '(on|at)': ' ',
+    '(nd|rd|th)': ' ',
+    '(平成|令和)(\S+)年': jp_sub_func,
+    '.*?st.*?': sub_st,
+    '時': '时'
+
+}
+# name itemprop property
+
+MATA_TIME_TOKEN = {
+    'article:published_time',
+    'datePublished',
+    'dateUpdate',
+    'pubDate',
+    'pubdate',
+    'date',
+    'og:published_time',
+    'og:article:published_time',
+    'og:release_date',
+    'og:time',
+    'render_timestamp',
+    'weibo: article:create_at',
+    '_pubtime',
+    'cXenseParse:recs:publishtime',
+    'pubtime',
+    'PubDate',
+    'publishdate',
+    'PublishDate',
+    'publishDate',
+    'sailthru.date',
+    'publication_date',
+    'apub:time',
+    'article_date_original',
+    'OriginalPublicationDate',
+    'dcterms.date',
+    'nv:news:date',
+    'parsely-pub-date',
+    'citation_publication_date',
+    'article:published_time',
+    'issueDate',
+    'date.release'
+}
+PUBLISH_TIME_META_EXTRA = [
+    '//meta[starts-with(@pubdate, "pubdate")]/@content',
+    '//meta[contains(@name, "date")]/@content',
+    '//meta[contains(@name, "publish")]/@content',
+    '//meta[contains(@name, "published")]/@content',
+    '//meta[contains(@property, "published")]/@content',
+    '//meta[contains(@property, "publish")]/@content',
+    '//meta[contains(@property, "date")]/@content',
+    '//meta[contains(@itemprop, "date")]/@content',
+    '//meta[contains(@itemprop, "publish")]/@content',
+    '//meta[contains(@itemprop, "published")]/@content',
+]
+
+
+def generate_meta_xpath():
+    for prop in ['name', 'itemprop', 'property']:
+        for class_name in MATA_TIME_TOKEN:
+            pattern = '//meta[starts-with(@%s, "%s")]/@content'
+            PUBLISH_TIME_META.append(pattern % (prop, class_name))
+    PUBLISH_TIME_META.extend(PUBLISH_TIME_META_EXTRA)
+
+
+STOPWORDS_DIR = ''
+
+generate_meta_xpath()
+
+PUBLISH_TIME_TAG = [
+    '//time/@datetime',  # h5 time 标签
+    '//time/@dateTime',  # h5 time 标签
+    '//relative-time/@datetime',  # h5 time 标签
+    '//*[@id="story_date"]/text()',
+    '//*[@class="time"]/text()',
+    '//time/@content',
+    '//*[@class="date"]/text()',
+    '//*[contains(@class,"date-time")]/text()',
+    '//*[contains(@class,"updated-date-time")]/text()',
+    '//*[contains(@class,"num_date")]/text()',
+    '//*[contains(@class,"se_date")]/text()',
+    '//*[contains(@class,"post-date")]/text()',
+    '//*[contains(@class,"teaser-byline-text-date")]/text()',
+    '//*[contains(@class,"date_posted")]/text()',
+    '//*[@itemprop="datePublished"]/@content',
+    '//time/text()',
+    '//*[@class="time"]/text()',
+    '//*[contains(@class,"date")]/text()',
+    '//*[contains(@class,"time")]/text()',
+]
+
+SCRIPT_TIME_RE = [
+
+]
+
+## 只取group 1 的这个要注意
+BASE_SCRIPT_TIME_RE = """["\']?%s *["\']? *: *["\']?(.*?)["\']"""
+SCRIPT_TIME_RE_TOKEN = [
+    'datePublished',
+    'publishedDate',
+    'created_date',
+    'publish_date',
+    'publishedDateCro',
+    'publishedDateUtc',
+    'publishedAtDate',
+    'articlePublishTime',
+    'ep_contentdata_delivered_date',
+    'deliveredDate',
+    "createdAt",
+    'dateModified',
+]
+SCRIPT_TIME_RE_EXTRA = [
+
+]
+
+
+def generate_script_re():
+    for token in SCRIPT_TIME_RE_TOKEN:
+        SCRIPT_TIME_RE.append(re.compile(BASE_SCRIPT_TIME_RE % token, re.I))
+    SCRIPT_TIME_RE.extend(SCRIPT_TIME_RE_EXTRA)
+
+
+generate_script_re()
+
+USELESS_TAG_TO_TIME = ['style', 'link', 'iframe', 'blockquote']
```

### Comparing `xgne-0.0.8/xgne/extractor/ArticleBodyExtractor.py` & `xgne-0.0.9/xgne/extractor/ArticleBodyExtractor.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,342 @@
-import copy
-
-from lxml.html import Element
-
-from ..defaults import ARTICLE_BODY_TAGS
-from ..parsers import Parser
-
-
-class ArticleBodyExtractor:
-    def __init__(self, config):
-        self.top_node = None
-        self.top_node_complemented = None
-        self.parser = Parser()
-        self.stopwords_class = config.stopwords_class
-        self.language = config.language
-
-    def parse(self, doc: Element):
-        """_summary_
-
-        Args:
-            doc (Element): _description_
-        """
-        self.top_node = self.calculate_best_node(doc)
-        self.top_node_complemented = self.complement_with_siblings(self.top_node)
-
-    def calculate_best_node(self, doc):
-        top_node = None
-        nodes_to_check = self.nodes_to_check(doc)
-        self.boost_highly_likely_nodes(doc)
-        starting_boost = float(1.0)
-        cnt = 0
-        i = 0
-        parent_nodes = []
-        nodes_with_text = []
-
-        for node in nodes_to_check:
-            text_node = self.parser.getText(node)
-            word_stats = self.stopwords_class(
-                language=self.language
-            ).get_stopword_count(text_node)
-            high_link_density = self.is_highlink_density(node)
-            if word_stats.stop_word_count > 2 and not high_link_density:
-                nodes_with_text.append(node)
-
-        nodes_number = len(nodes_with_text)
-        negative_scoring = 0
-        bottom_negativescore_nodes = float(nodes_number) * 0.25
-
-        for node in nodes_with_text:
-            boost_score = float(0)
-            # boost
-            if self.is_boostable(node):
-                if cnt >= 0:
-                    boost_score = float((1.0 / starting_boost) * 50)
-                    starting_boost += 1
-            # nodes_number
-            if nodes_number > 15:
-                if (nodes_number - i) <= bottom_negativescore_nodes:
-                    booster = float(bottom_negativescore_nodes - (nodes_number - i))
-                    boost_score = float(-pow(booster, float(2)))
-                    negscore = abs(boost_score) + negative_scoring
-                    if negscore > 40:
-                        boost_score = float(5)
-
-            text_node = self.parser.getText(node)
-            word_stats = self.stopwords_class(
-                language=self.language
-            ).get_stopword_count(text_node)
-            upscore = int(word_stats.stop_word_count + boost_score)
-
-            parent_node = self.parser.getParent(node)
-            self.update_score(parent_node, upscore)
-            self.update_node_count(parent_node, 1)
-
-            if parent_node not in parent_nodes:
-                parent_nodes.append(parent_node)
-
-            # Parent of parent node
-            parent_parent_node = self.parser.getParent(parent_node)
-            if parent_parent_node is not None:
-                self.update_node_count(parent_parent_node, 1)
-                self.update_score(parent_parent_node, upscore / 2)
-                if parent_parent_node not in parent_nodes:
-                    parent_nodes.append(parent_parent_node)
-            cnt += 1
-            i += 1
-
-        if parent_nodes:
-            parent_nodes.sort(key=self.get_score, reverse=True)
-            top_node = parent_nodes[0]
-
-        return top_node
-
-    def nodes_to_check(self, doc):
-        """Returns a list of nodes we want to search
-        on like paragraphs and tables
-        """
-        nodes_to_check = []
-        for tag in ["p", "pre", "td", "article", "div"]:
-            if tag == "div":
-                items = []
-                for id_ in ["article-body", "article", "story", "article-content"]:
-                    items += self.parser.getElementsByTag(
-                        doc, tag=tag, attr="id", value=id_
-                    )
-            else:
-                items = self.parser.getElementsByTag(doc, tag=tag)
-            nodes_to_check += items
-        return nodes_to_check
-
-    def is_boostable(self, node):
-        """A lot of times the first paragraph might be the caption under an image
-        so we'll want to make sure if we're going to boost a parent node that
-        it should be connected to other paragraphs, at least for the first n
-        paragraphs so we'll want to make sure that the next sibling is a
-        paragraph and has at least some substantial weight to it.
-        """
-        para = "p"
-        steps_away = 0
-        minimum_stopword_count = 5
-        max_stepsaway_from_node = 3
-
-        nodes = self.walk_siblings(node)
-        for current_node in nodes:
-            # <p>
-            current_node_tag = self.parser.getTag(current_node)
-            if current_node_tag == para:
-                if steps_away >= max_stepsaway_from_node:
-                    return False
-                paragraph_text = self.parser.getText(current_node)
-                word_stats = self.stopwords_class(
-                    language=self.language
-                ).get_stopword_count(paragraph_text)
-                if word_stats.stop_word_count > minimum_stopword_count:
-                    return True
-                steps_away += 1
-        return False
-
-    def is_highlink_density(self, e):
-        """Checks the density of links within a node, if there is a high
-        link to text ratio, then the text is less likely to be relevant
-        """
-        links = self.parser.getElementsByTag(e, tag="a")
-        if not links:
-            return False
-
-        text = self.parser.getText(e)
-        words = [word for word in text.split() if word.isalnum()]
-        if not words:
-            return True
-        words_number = float(len(words))
-        sb = []
-        for link in links:
-            sb.append(self.parser.getText(link))
-
-        link_text = "".join(sb)
-        link_words = link_text.split()
-        num_link_words = float(len(link_words))
-        num_links = float(len(links))
-        link_divisor = float(num_link_words / words_number)
-        score = float(link_divisor * num_links)
-        if score >= 1.0:
-            return True
-        return False
-        # return True if score > 1.0 else False
-
-    def boost_highly_likely_nodes(self, doc: Element):
-        """Set a bias score for all nodes under most likely
-        article containers. This way we can find articles
-        that have little text.
-
-        Args:
-            doc (Element): Document to be checked
-        """
-        candidates = []
-        for tag in ["p", "pre", "td", "article", "div"]:
-            candidates.extend(self.parser.getElementsByTag(doc, tag=tag))
-
-        for e in candidates:
-            if self.is_highly_likly(e):
-                for child in e.iterdescendants():
-                    self.update_score(child, 25)  # TODO: find an optimum value
-
-    def is_highly_likly(self, node: Element) -> bool:
-        """Checks if the node is a well known tag + attributes combination
-        for article body containers. This way we can deliver even small
-        article bodies with high link density
-        see: https://finance.yahoo.com/m/
-            0edc9aaa-e3ba-3178-be5a-f8c16fbffff2/warren-buffett-stocks-shaky.html
-
-        Args:
-            node (Element): Node to check
-
-        Returns:
-            bool: True if node could be an article body top node
-        """
-
-        def is_tag_match(node, tag_dict):
-            if node.tag != tag_dict.get("tag", node.tag):
-                return False
-            for k, v in tag_dict.items():
-                if k == "tag":
-                    continue
-                if node.get(k) != v:
-                    return False
-            return True
-
-        for tag in ARTICLE_BODY_TAGS:
-            if is_tag_match(node, tag):
-                return True
-
-        return False
-
-    def update_score(self, node, add_to_score):
-        """Adds a score to the gravityScore Attribute we put on divs
-        we'll get the current score then add the score we're passing
-        in to the current.
-        """
-        current_score = 0
-        score_string = self.parser.getAttribute(node, "gravityScore")
-        if score_string:
-            current_score = float(score_string)
-
-        new_score = current_score + add_to_score
-        self.parser.setAttribute(node, "gravityScore", str(new_score))
-
-    def update_node_count(self, node, add_to_count):
-        """Stores how many decent nodes are under a parent node"""
-        current_score = 0
-        count_string = self.parser.getAttribute(node, "gravityNodes")
-        if count_string:
-            current_score = int(count_string)
-
-        new_score = current_score + add_to_count
-        self.parser.setAttribute(node, "gravityNodes", str(new_score))
-
-    def add_siblings(self, top_node):
-        res_node = copy.deepcopy(top_node)
-        baseline_score_siblings_para = self.get_siblings_score(top_node)
-        results = self.walk_siblings(top_node)
-        for current_node in results:
-            ps = self.get_siblings_content(current_node, baseline_score_siblings_para)
-            for p in ps:
-                res_node.insert(0, p)
-        return res_node
-
-    def get_siblings_content(self, current_sibling, baseline_score_siblings_para):
-        """Adds any siblings that may have a decent score to this node"""
-        if current_sibling.tag == "p" and len(self.parser.getText(current_sibling)) > 0:
-            e0 = current_sibling
-            if e0.tail:
-                e0 = copy.deepcopy(e0)
-                e0.tail = ""
-            return [e0]
-        else:
-            potential_paragraphs = self.parser.getElementsByTag(
-                current_sibling, tag="p"
-            )
-            if potential_paragraphs is None:
-                return None
-            else:
-                ps = []
-                for first_paragraph in potential_paragraphs:
-                    text = self.parser.getText(first_paragraph)
-                    if len(text) > 0:
-                        word_stats = self.stopwords_class(
-                            language=self.language
-                        ).get_stopword_count(text)
-                        paragraph_score = word_stats.stop_word_count
-                        sibling_baseline_score = float(0.30)
-                        high_link_density = self.is_highlink_density(first_paragraph)
-                        score = float(
-                            baseline_score_siblings_para * sibling_baseline_score
-                        )
-                        if score < paragraph_score and not high_link_density:
-                            p = self.parser.createElement(tag="p", text=text, tail=None)
-                            ps.append(p)
-                return ps
-
-    def get_siblings_score(self, top_node):
-        """We could have long articles that have tons of paragraphs
-        so if we tried to calculate the base score against
-        the total text score of those paragraphs it would be unfair.
-        So we need to normalize the score based on the average scoring
-        of the paragraphs within the top node.
-        For example if our total score of 10 paragraphs was 1000
-        but each had an average value of 100 then 100 should be our base.
-        """
-        base = 100000
-        paragraphs_number = 0
-        paragraphs_score = 0
-        nodes_to_check = self.parser.getElementsByTag(top_node, tag="p")
-
-        for node in nodes_to_check:
-            text_node = self.parser.getText(node)
-            word_stats = self.stopwords_class(
-                language=self.language
-            ).get_stopword_count(text_node)
-            high_link_density = self.is_highlink_density(node)
-            if word_stats.stop_word_count > 2 and not high_link_density:
-                paragraphs_number += 1
-                paragraphs_score += word_stats.stop_word_count
-
-        if paragraphs_number > 0:
-            base = paragraphs_score / paragraphs_number
-
-        return base
-
-    def walk_siblings(self, node):
-        return self.parser.previousSiblings(node)
-
-    def get_node_gravity_score(self, node):
-        gravity_score = self.parser.getAttribute(node, "gravityScore")
-        if not gravity_score:
-            return None
-        return float(gravity_score)
-
-    def get_score(self, node):
-        """Returns the gravityScore as an integer from this node"""
-        return self.get_node_gravity_score(node) or 0
-
-    def complement_with_siblings(self, node: Element) -> Element:
-        """Adds surrounding relevant siblings to the top node.
-        Attention, it generates off-the-tree node.
-
-        Args:
-            node (Element): Top node detected
-
-        Returns:
-            Element: off the tree node complemented with siblings
-        """
-        if node is None:
-            return node
-        node_complemented = self.add_siblings(
-            node
-        )  # TODO: test if there is a problem with siblings AFTER the top node
-        for e in self.parser.getChildren(node_complemented):
-            e_tag = self.parser.getTag(e)
-            if e_tag != "p":
-                if self.is_highlink_density(e):
-                    self.parser.remove(e)
-        return node_complemented
+import copy
+
+from lxml.html import Element
+
+from ..defaults import ARTICLE_BODY_TAGS
+from ..parsers import Parser
+
+
+class ArticleBodyExtractor:
+    def __init__(self, config):
+        self.top_node = None
+        self.top_node_complemented = None
+        self.parser = Parser()
+        self.stopwords_class = config.stopwords_class
+        self.language = config.language
+
+    def parse(self, doc: Element):
+        """_summary_
+
+        Args:
+            doc (Element): _description_
+        """
+        self.top_node = self.calculate_best_node(doc)
+        self.top_node_complemented = self.complement_with_siblings(self.top_node)
+
+    def calculate_best_node(self, doc):
+        top_node = None
+        nodes_to_check = self.nodes_to_check(doc)
+        self.boost_highly_likely_nodes(doc)
+        starting_boost = float(1.0)
+        cnt = 0
+        i = 0
+        parent_nodes = []
+        nodes_with_text = []
+
+        for node in nodes_to_check:
+            text_node = self.parser.getText(node)
+            word_stats = self.stopwords_class(
+                language=self.language
+            ).get_stopword_count(text_node)
+            high_link_density = self.is_highlink_density(node)
+            if word_stats.stop_word_count > 2 and not high_link_density:
+                nodes_with_text.append(node)
+
+        nodes_number = len(nodes_with_text)
+        negative_scoring = 0
+        bottom_negativescore_nodes = float(nodes_number) * 0.25
+
+        for node in nodes_with_text:
+            boost_score = float(0)
+            # boost
+            if self.is_boostable(node):
+                if cnt >= 0:
+                    boost_score = float((1.0 / starting_boost) * 50)
+                    starting_boost += 1
+            # nodes_number
+            if nodes_number > 15:
+                if (nodes_number - i) <= bottom_negativescore_nodes:
+                    booster = float(bottom_negativescore_nodes - (nodes_number - i))
+                    boost_score = float(-pow(booster, float(2)))
+                    negscore = abs(boost_score) + negative_scoring
+                    if negscore > 40:
+                        boost_score = float(5)
+
+            text_node = self.parser.getText(node)
+            word_stats = self.stopwords_class(
+                language=self.language
+            ).get_stopword_count(text_node)
+            upscore = int(word_stats.stop_word_count + boost_score)
+
+            parent_node = self.parser.getParent(node)
+            self.update_score(parent_node, upscore)
+            self.update_node_count(parent_node, 1)
+
+            if parent_node not in parent_nodes:
+                parent_nodes.append(parent_node)
+
+            # Parent of parent node
+            parent_parent_node = self.parser.getParent(parent_node)
+            if parent_parent_node is not None:
+                self.update_node_count(parent_parent_node, 1)
+                self.update_score(parent_parent_node, upscore / 2)
+                if parent_parent_node not in parent_nodes:
+                    parent_nodes.append(parent_parent_node)
+            cnt += 1
+            i += 1
+
+        if parent_nodes:
+            parent_nodes.sort(key=self.get_score, reverse=True)
+            top_node = parent_nodes[0]
+
+        return top_node
+
+    def nodes_to_check(self, doc):
+        """Returns a list of nodes we want to search
+        on like paragraphs and tables
+        """
+        nodes_to_check = []
+        for tag in ["p", "pre", "td", "article", "div"]:
+            if tag == "div":
+                items = []
+                for id_ in ["article-body", "article", "story", "article-content"]:
+                    items += self.parser.getElementsByTag(
+                        doc, tag=tag, attr="id", value=id_
+                    )
+            else:
+                items = self.parser.getElementsByTag(doc, tag=tag)
+            nodes_to_check += items
+        return nodes_to_check
+
+    def is_boostable(self, node):
+        """A lot of times the first paragraph might be the caption under an image
+        so we'll want to make sure if we're going to boost a parent node that
+        it should be connected to other paragraphs, at least for the first n
+        paragraphs so we'll want to make sure that the next sibling is a
+        paragraph and has at least some substantial weight to it.
+        """
+        para = "p"
+        steps_away = 0
+        minimum_stopword_count = 5
+        max_stepsaway_from_node = 3
+
+        nodes = self.walk_siblings(node)
+        for current_node in nodes:
+            # <p>
+            current_node_tag = self.parser.getTag(current_node)
+            if current_node_tag == para:
+                if steps_away >= max_stepsaway_from_node:
+                    return False
+                paragraph_text = self.parser.getText(current_node)
+                word_stats = self.stopwords_class(
+                    language=self.language
+                ).get_stopword_count(paragraph_text)
+                if word_stats.stop_word_count > minimum_stopword_count:
+                    return True
+                steps_away += 1
+        return False
+
+    def is_highlink_density(self, e):
+        """Checks the density of links within a node, if there is a high
+        link to text ratio, then the text is less likely to be relevant
+        """
+        links = self.parser.getElementsByTag(e, tag="a")
+        if not links:
+            return False
+
+        text = self.parser.getText(e)
+        words = [word for word in text.split() if word.isalnum()]
+        if not words:
+            return True
+        words_number = float(len(words))
+        sb = []
+        for link in links:
+            sb.append(self.parser.getText(link))
+
+        link_text = "".join(sb)
+        link_words = link_text.split()
+        num_link_words = float(len(link_words))
+        num_links = float(len(links))
+        link_divisor = float(num_link_words / words_number)
+        score = float(link_divisor * num_links)
+        if score >= 1.0:
+            return True
+        return False
+        # return True if score > 1.0 else False
+
+    def boost_highly_likely_nodes(self, doc: Element):
+        """Set a bias score for all nodes under most likely
+        article containers. This way we can find articles
+        that have little text.
+
+        Args:
+            doc (Element): Document to be checked
+        """
+        candidates = []
+        for tag in ["p", "pre", "td", "article", "div"]:
+            candidates.extend(self.parser.getElementsByTag(doc, tag=tag))
+
+        for e in candidates:
+            if self.is_highly_likly(e):
+                for child in e.iterdescendants():
+                    self.update_score(child, 25)  # TODO: find an optimum value
+
+    def is_highly_likly(self, node: Element) -> bool:
+        """Checks if the node is a well known tag + attributes combination
+        for article body containers. This way we can deliver even small
+        article bodies with high link density
+        see: https://finance.yahoo.com/m/
+            0edc9aaa-e3ba-3178-be5a-f8c16fbffff2/warren-buffett-stocks-shaky.html
+
+        Args:
+            node (Element): Node to check
+
+        Returns:
+            bool: True if node could be an article body top node
+        """
+
+        def is_tag_match(node, tag_dict):
+            if node.tag != tag_dict.get("tag", node.tag):
+                return False
+            for k, v in tag_dict.items():
+                if k == "tag":
+                    continue
+                if node.get(k) != v:
+                    return False
+            return True
+
+        for tag in ARTICLE_BODY_TAGS:
+            if is_tag_match(node, tag):
+                return True
+
+        return False
+
+    def update_score(self, node, add_to_score):
+        """Adds a score to the gravityScore Attribute we put on divs
+        we'll get the current score then add the score we're passing
+        in to the current.
+        """
+        current_score = 0
+        score_string = self.parser.getAttribute(node, "gravityScore")
+        if score_string:
+            current_score = float(score_string)
+
+        new_score = current_score + add_to_score
+        self.parser.setAttribute(node, "gravityScore", str(new_score))
+
+    def update_node_count(self, node, add_to_count):
+        """Stores how many decent nodes are under a parent node"""
+        current_score = 0
+        count_string = self.parser.getAttribute(node, "gravityNodes")
+        if count_string:
+            current_score = int(count_string)
+
+        new_score = current_score + add_to_count
+        self.parser.setAttribute(node, "gravityNodes", str(new_score))
+
+    def add_siblings(self, top_node):
+        res_node = copy.deepcopy(top_node)
+        baseline_score_siblings_para = self.get_siblings_score(top_node)
+        results = self.walk_siblings(top_node)
+        for current_node in results:
+            ps = self.get_siblings_content(current_node, baseline_score_siblings_para)
+            for p in ps:
+                res_node.insert(0, p)
+        return res_node
+
+    def get_siblings_content(self, current_sibling, baseline_score_siblings_para):
+        """Adds any siblings that may have a decent score to this node"""
+        if current_sibling.tag == "p" and len(self.parser.getText(current_sibling)) > 0:
+            e0 = current_sibling
+            if e0.tail:
+                e0 = copy.deepcopy(e0)
+                e0.tail = ""
+            return [e0]
+        else:
+            potential_paragraphs = self.parser.getElementsByTag(
+                current_sibling, tag="p"
+            )
+            if potential_paragraphs is None:
+                return None
+            else:
+                ps = []
+                for first_paragraph in potential_paragraphs:
+                    text = self.parser.getText(first_paragraph)
+                    if len(text) > 0:
+                        word_stats = self.stopwords_class(
+                            language=self.language
+                        ).get_stopword_count(text)
+                        paragraph_score = word_stats.stop_word_count
+                        sibling_baseline_score = float(0.30)
+                        high_link_density = self.is_highlink_density(first_paragraph)
+                        score = float(
+                            baseline_score_siblings_para * sibling_baseline_score
+                        )
+                        if score < paragraph_score and not high_link_density:
+                            p = self.parser.createElement(tag="p", text=text, tail=None)
+                            ps.append(p)
+                return ps
+
+    def get_siblings_score(self, top_node):
+        """We could have long articles that have tons of paragraphs
+        so if we tried to calculate the base score against
+        the total text score of those paragraphs it would be unfair.
+        So we need to normalize the score based on the average scoring
+        of the paragraphs within the top node.
+        For example if our total score of 10 paragraphs was 1000
+        but each had an average value of 100 then 100 should be our base.
+        """
+        base = 100000
+        paragraphs_number = 0
+        paragraphs_score = 0
+        nodes_to_check = self.parser.getElementsByTag(top_node, tag="p")
+
+        for node in nodes_to_check:
+            text_node = self.parser.getText(node)
+            word_stats = self.stopwords_class(
+                language=self.language
+            ).get_stopword_count(text_node)
+            high_link_density = self.is_highlink_density(node)
+            if word_stats.stop_word_count > 2 and not high_link_density:
+                paragraphs_number += 1
+                paragraphs_score += word_stats.stop_word_count
+
+        if paragraphs_number > 0:
+            base = paragraphs_score / paragraphs_number
+
+        return base
+
+    def walk_siblings(self, node):
+        return self.parser.previousSiblings(node)
+
+    def get_node_gravity_score(self, node):
+        gravity_score = self.parser.getAttribute(node, "gravityScore")
+        if not gravity_score:
+            return None
+        return float(gravity_score)
+
+    def get_score(self, node):
+        """Returns the gravityScore as an integer from this node"""
+        return self.get_node_gravity_score(node) or 0
+
+    def complement_with_siblings(self, node: Element) -> Element:
+        """Adds surrounding relevant siblings to the top node.
+        Attention, it generates off-the-tree node.
+
+        Args:
+            node (Element): Top node detected
+
+        Returns:
+            Element: off the tree node complemented with siblings
+        """
+        if node is None:
+            return node
+        node_complemented = self.add_siblings(
+            node
+        )  # TODO: test if there is a problem with siblings AFTER the top node
+        for e in self.parser.getChildren(node_complemented):
+            e_tag = self.parser.getTag(e)
+            if e_tag != "p":
+                if self.is_highlink_density(e):
+                    self.parser.remove(e)
+        return node_complemented
```

### Comparing `xgne-0.0.8/xgne/extractor/AuthorExtractor.py` & `xgne-0.0.9/xgne/extractor/AuthorExtractor.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-import re
-from copy import deepcopy
-from typing import List, Union
-from collections import OrderedDict
-
-from lxml.html import HtmlElement
-
-from ..utils import config
-from ..parsers import Parser
-from ..defaults import AUTHOR_PATTERN, AUTHOR_ATTRS, AUTHOR_STOP_WORDS, AUTHOR_VALS
-
-
-class AuthorExtractor:
-    def __init__(self):
-        self.author_pattern = AUTHOR_PATTERN
-        self.parser = Parser()
-        self.authors: List[str] = []
-
-    def extractor(self, element: HtmlElement, author_xpath='') -> List[str]:
-        # 如果提供了自定义的作者 XPath，则直接使用该 XPath 进行提取
-        author_xpath = author_xpath or config.get('author', {}).get('xpath')
-        if author_xpath:
-            self.authors = element.xpath(author_xpath)
-        # 否则，从文本中提取作者信息
-        text = ''.join(element.xpath('.//text()'))
-        for pattern in self.author_pattern:
-            author_obj = re.search(pattern, text)
-            if author_obj:
-                self.authors = self.authors + [author_obj.group(0)]
-        self.authors = [i.strip() for i in self.authors if i.strip()]
-        # 如果未成功提取作者信息，则尝试从 JSON-LD 数据和其他元素中提取
-        if not self.authors:
-            _digits = re.compile(r"\d")
-            author_stopwords_patt = [re.escape(x) for x in AUTHOR_STOP_WORDS]
-            author_stopwords = re.compile(
-                r"\b(" + "|".join(author_stopwords_patt) + r")\b", flags=re.IGNORECASE
-            )
-
-            def contains_digits(d):
-                return bool(_digits.search(d))
-
-            def uniqify_list(lst: List[str]) -> List[str]:
-                """
-                从提供的字符串列表中去除重复项但保持原始顺序。
-                忽略末尾空格和大小写。
-
-                Args:
-                    lst (List[str]): 输入的字符串列表，可能包含重复项
-
-                Returns:
-                    List[str]: 输出的字符串列表，已删除重复项
-                """
-                seen = OrderedDict()
-                for item in lst:
-                    seen[item.lower().strip()] = item.strip()
-                return [seen[item] for item in seen.keys() if item]
-
-            def parse_byline(search_str):
-                """
-                解析候选行的 HTML 或文本，并以列表形式提取出名字
-                """
-                # 移除 HTML 标签
-                search_str = re.sub("<[^<]+?>", "", search_str)
-                search_str = re.sub("[\n\t\r\xa0]", " ", search_str)
-
-                # 移除原始的 "By" 语句
-                m = re.search(r"\b(by|from)[:\s](.*)", search_str, flags=re.IGNORECASE)
-                if m:
-                    search_str = m.group(2)
-
-                search_str = search_str.strip()
-
-                # 使用非字母数字字符分割行
-                name_tokens = re.split(r"[·,\|]|\sand\s|\set\s|\sund\s|/", search_str)
-                # 一些合理性检查
-                name_tokens = [s.strip() for s in name_tokens if not contains_digits(s)]
-                name_tokens = [s for s in name_tokens if 5 > len(re.findall(r"\w+", s)) > 1]
-
-                return name_tokens
-
-            # Try 1: Search popular author tags for authors
-
-            matches = []
-            authors = []
-
-            json_ld_scripts = self.parser.get_ld_json_object(element)
-
-            def get_authors(vals):
-                if isinstance(vals, dict):
-                    if isinstance(vals.get("name"), str):
-                        authors.append(vals.get("name"))
-                    elif isinstance(vals.get("name"), list):
-                        authors.extend(vals.get("name"))
-                elif isinstance(vals, list):
-                    for val in vals:
-                        if isinstance(val, dict):
-                            authors.append(val.get("name"))
-                        elif isinstance(val, str):
-                            authors.append(val)
-                elif isinstance(vals, str):
-                    authors.append(vals)
-
-            for script_tag in json_ld_scripts:
-                if "@graph" in script_tag:
-                    g = script_tag.get("@graph", [])
-                    for item in g:
-                        if not isinstance(item, dict):
-                            continue
-                        if item.get("@type") == "Person":
-                            authors.append(item.get("name"))
-                        if "author" in item:
-                            get_authors(item["author"])
-                else:
-                    if "author" in script_tag:
-                        get_authors(script_tag["author"])
-
-            def get_text_from_element(node: HtmlElement) -> str:
-                """
-                从元素中提取文本，包括其子元素的文本
-                """
-                if node is None:
-                    return ""
-                if node.tag in ["script", "style", "time"]:
-                    return ""
-
-                node = deepcopy(node)
-                for tag in ["script", "style", "time"]:
-                    for el in node.xpath(f".//{tag}"):
-                        el.getparent().remove(el)
-                text = list(node.itertext())
-                text = " ".join(text)
-                return text
-
-            authors = [re.sub("[\n\t\r\xa0]", " ", x) for x in authors if x]
-            doc_root = element.getroottree()
-
-            def getpath(node):
-                if doc_root is not None:
-                    return doc_root.getpath(node)
-
-            # TODO: be more specific, not a combination of all attributes and values
-            for attr in AUTHOR_ATTRS:
-                for val in AUTHOR_VALS:
-                    found = self.parser.get_element_by_attribs(element, attribs={attr: val})
-                    matches.extend([(found, getpath(found)) for found in found])
-
-            matches.sort(
-                key=lambda x: x[1], reverse=True
-            )  # 按 XPath 排序，以获取最特定的匹配项
-            matches_reduced = []
-            for m in matches:
-                if len(matches_reduced) == 0:
-                    matches_reduced.append(m)
-                elif not matches_reduced[-1][1].startswith(
-                        m[1]
-                ):  # 移除前一个节点的父节点
-                    matches_reduced.append(m)
-            matches_reduced.sort(
-                key=lambda x: x[1]
-            )  # 保留一些作者的排序
-
-            for match, _ in matches_reduced:
-                content: Union[str, List] = ""
-                if match.tag == "meta":
-                    mm = match.xpath("@content")
-                    if len(mm) > 0:
-                        content = mm[0]
-                else:
-                    # 忽略 <time> 标签或带有 "on ..." 的标签
-                    # 移除 <style> 标签 https://washingtonindependent.com/how-to-apply-for-reseller-permit-in-washington-state/
-                    content = get_text_from_element(match)
-                if len(content) > 0:
-                    authors.extend(parse_byline(content))
-
-            # 输出的字符串列表，已删除重复项
-            authors = [re.sub(author_stopwords, "", x).strip(" .,-/") for x in authors]
-            self.authors = uniqify_list(authors)
-        return self.authors
+import re
+from copy import deepcopy
+from typing import List, Union
+from collections import OrderedDict
+
+from lxml.html import HtmlElement
+
+from ..utils import config
+from ..parsers import Parser
+from ..defaults import AUTHOR_PATTERN, AUTHOR_ATTRS, AUTHOR_STOP_WORDS, AUTHOR_VALS
+
+
+class AuthorExtractor:
+    def __init__(self):
+        self.author_pattern = AUTHOR_PATTERN
+        self.parser = Parser()
+        self.authors: List[str] = []
+
+    def extractor(self, element: HtmlElement, author_xpath='') -> List[str]:
+        # 如果提供了自定义的作者 XPath，则直接使用该 XPath 进行提取
+        author_xpath = author_xpath or config.get('author', {}).get('xpath')
+        if author_xpath:
+            self.authors = element.xpath(author_xpath)
+        # 否则，从文本中提取作者信息
+        text = ''.join(element.xpath('.//text()'))
+        for pattern in self.author_pattern:
+            author_obj = re.search(pattern, text)
+            if author_obj:
+                self.authors = self.authors + [author_obj.group(0)]
+        self.authors = [i.strip() for i in self.authors if i.strip()]
+        # 如果未成功提取作者信息，则尝试从 JSON-LD 数据和其他元素中提取
+        if not self.authors:
+            _digits = re.compile(r"\d")
+            author_stopwords_patt = [re.escape(x) for x in AUTHOR_STOP_WORDS]
+            author_stopwords = re.compile(
+                r"\b(" + "|".join(author_stopwords_patt) + r")\b", flags=re.IGNORECASE
+            )
+
+            def contains_digits(d):
+                return bool(_digits.search(d))
+
+            def uniqify_list(lst: List[str]) -> List[str]:
+                """
+                从提供的字符串列表中去除重复项但保持原始顺序。
+                忽略末尾空格和大小写。
+
+                Args:
+                    lst (List[str]): 输入的字符串列表，可能包含重复项
+
+                Returns:
+                    List[str]: 输出的字符串列表，已删除重复项
+                """
+                seen = OrderedDict()
+                for item in lst:
+                    seen[item.lower().strip()] = item.strip()
+                return [seen[item] for item in seen.keys() if item]
+
+            def parse_byline(search_str):
+                """
+                解析候选行的 HTML 或文本，并以列表形式提取出名字
+                """
+                # 移除 HTML 标签
+                search_str = re.sub("<[^<]+?>", "", search_str)
+                search_str = re.sub("[\n\t\r\xa0]", " ", search_str)
+
+                # 移除原始的 "By" 语句
+                m = re.search(r"\b(by|from)[:\s](.*)", search_str, flags=re.IGNORECASE)
+                if m:
+                    search_str = m.group(2)
+
+                search_str = search_str.strip()
+
+                # 使用非字母数字字符分割行
+                name_tokens = re.split(r"[·,\|]|\sand\s|\set\s|\sund\s|/", search_str)
+                # 一些合理性检查
+                name_tokens = [s.strip() for s in name_tokens if not contains_digits(s)]
+                name_tokens = [s for s in name_tokens if 5 > len(re.findall(r"\w+", s)) > 1]
+
+                return name_tokens
+
+            # Try 1: Search popular author tags for authors
+
+            matches = []
+            authors = []
+
+            json_ld_scripts = self.parser.get_ld_json_object(element)
+
+            def get_authors(vals):
+                if isinstance(vals, dict):
+                    if isinstance(vals.get("name"), str):
+                        authors.append(vals.get("name"))
+                    elif isinstance(vals.get("name"), list):
+                        authors.extend(vals.get("name"))
+                elif isinstance(vals, list):
+                    for val in vals:
+                        if isinstance(val, dict):
+                            authors.append(val.get("name"))
+                        elif isinstance(val, str):
+                            authors.append(val)
+                elif isinstance(vals, str):
+                    authors.append(vals)
+
+            for script_tag in json_ld_scripts:
+                if "@graph" in script_tag:
+                    g = script_tag.get("@graph", [])
+                    for item in g:
+                        if not isinstance(item, dict):
+                            continue
+                        if item.get("@type") == "Person":
+                            authors.append(item.get("name"))
+                        if "author" in item:
+                            get_authors(item["author"])
+                else:
+                    if "author" in script_tag:
+                        get_authors(script_tag["author"])
+
+            def get_text_from_element(node: HtmlElement) -> str:
+                """
+                从元素中提取文本，包括其子元素的文本
+                """
+                if node is None:
+                    return ""
+                if node.tag in ["script", "style", "time"]:
+                    return ""
+
+                node = deepcopy(node)
+                for tag in ["script", "style", "time"]:
+                    for el in node.xpath(f".//{tag}"):
+                        el.getparent().remove(el)
+                text = list(node.itertext())
+                text = " ".join(text)
+                return text
+
+            authors = [re.sub("[\n\t\r\xa0]", " ", x) for x in authors if x]
+            doc_root = element.getroottree()
+
+            def getpath(node):
+                if doc_root is not None:
+                    return doc_root.getpath(node)
+
+            # TODO: be more specific, not a combination of all attributes and values
+            for attr in AUTHOR_ATTRS:
+                for val in AUTHOR_VALS:
+                    found = self.parser.get_element_by_attribs(element, attribs={attr: val})
+                    matches.extend([(found, getpath(found)) for found in found])
+
+            matches.sort(
+                key=lambda x: x[1], reverse=True
+            )  # 按 XPath 排序，以获取最特定的匹配项
+            matches_reduced = []
+            for m in matches:
+                if len(matches_reduced) == 0:
+                    matches_reduced.append(m)
+                elif not matches_reduced[-1][1].startswith(
+                        m[1]
+                ):  # 移除前一个节点的父节点
+                    matches_reduced.append(m)
+            matches_reduced.sort(
+                key=lambda x: x[1]
+            )  # 保留一些作者的排序
+
+            for match, _ in matches_reduced:
+                content: Union[str, List] = ""
+                if match.tag == "meta":
+                    mm = match.xpath("@content")
+                    if len(mm) > 0:
+                        content = mm[0]
+                else:
+                    # 忽略 <time> 标签或带有 "on ..." 的标签
+                    # 移除 <style> 标签 https://washingtonindependent.com/how-to-apply-for-reseller-permit-in-washington-state/
+                    content = get_text_from_element(match)
+                if len(content) > 0:
+                    authors.extend(parse_byline(content))
+
+            # 输出的字符串列表，已删除重复项
+            authors = [re.sub(author_stopwords, "", x).strip(" .,-/") for x in authors]
+            self.authors = uniqify_list(authors)
+        return self.authors
```

### Comparing `xgne-0.0.8/xgne/extractor/ContentExtractor.py` & `xgne-0.0.9/xgne/extractor/ContentExtractor.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-import re
-import json
-import numpy as np
-from lxml.html import etree, tostring
-from html import unescape
-from ..utils import iter_node, pad_host_for_images, config, get_high_weight_keyword_pattern, universal_filter
-
-
-class ContentExtractor:
-    def __init__(self, content_tag='p'):
-        """
-
-        :param content_tag: 正文内容在哪个标签里面
-        """
-        self.content_tag = content_tag
-        self.node_info = {}
-        self.high_weight_keyword_pattern = get_high_weight_keyword_pattern()
-        self.punctuation = set('''！，。？、；：“”‘’《》%（）,.?:;'"!%()''')  # 常见的中英文标点符号
-        self.element_text_cache = {}
-
-    def extract(self, selector, host='', body_xpath='', with_body_html=False, use_visiable_info=False):
-        body_xpath = body_xpath or config.get('body', {}).get('xpath', '')
-        use_visiable_info = use_visiable_info or config.get('use_visiable_info', False)
-        if body_xpath:
-            body = selector.xpath(body_xpath)[0]
-        else:
-            body = selector.xpath('//body')[0]
-        for node_index, node in enumerate(iter_node(body)):
-            if use_visiable_info:
-                if not node.attrib.get('is_visiable', True):
-                    continue
-                coordinate_json = node.attrib.get('coordinate', '{}')
-                coordinate = json.loads(coordinate_json)
-                if coordinate.get('height', 0) < 150:  # 正文块的高度应该要大于150px
-                    continue
-            node_hash = hash(node)
-            density_info = self.calc_text_density(node)
-            text_density = density_info['density']
-            ti_text = density_info['ti_text']
-            text_tag_count = self.count_text_tag(node, tag='p')
-            sbdi = self.calc_sbdi(ti_text, density_info['ti'], density_info['lti'])
-            images_list = [
-                i.xpath('./@data-src')[0]
-                if i.xpath('./@data-src') and ';base64,' in i.xpath('./@src')[0]
-                else i.xpath('./@src')[0]
-                for i in node.xpath('.//img')
-            ]
-            host = host or config.get('host', '')
-            if host:
-                images_list = [pad_host_for_images(host, url) for url in images_list]
-            node_info = {'ti': density_info['ti'],
-                         'lti': density_info['lti'],
-                         'tgi': density_info['tgi'],
-                         'ltgi': density_info['ltgi'],
-                         'node': node,
-                         'node_index': node_index,
-                         'density': text_density,
-                         'text': ti_text,
-                         'images': images_list,
-                         'text_tag_count': text_tag_count,
-                         'sbdi': sbdi}
-            if use_visiable_info:
-                node_info['is_visiable'] = node.attrib['is_visiable']
-                node_info['coordinate'] = node.attrib.get('coordinate', '')
-            if with_body_html or config.get('with_body_html', False):
-                body_source_code = unescape(etree.tostring(node, encoding='utf-8').decode())
-                node_info['body_html'] = universal_filter(body_source_code)
-            self.node_info[node_hash] = node_info
-        self.calc_new_score()
-        result = sorted(self.node_info.items(), key=lambda x: x[1]['score'], reverse=True)
-        return result
-
-    def count_text_tag(self, element, tag='p'):
-        """
-        当前标签下面的 text()和 p 标签，都应该进行统计
-        :param element:
-        :param tag:
-        :return:
-        """
-        tag_num = len(element.xpath(f'.//{tag}'))
-        direct_text = len(element.xpath('text()'))
-        return tag_num + direct_text
-
-    def get_all_text_of_element(self, element_list):
-        if not isinstance(element_list, list):
-            element_list = [element_list]
-
-        text_list = []
-        for element in element_list:
-            element_flag = element.getroottree().getpath(element)
-            if element_flag in self.element_text_cache:  # 直接读取缓存的数据，而不是再重复提取一次
-                text_list.extend(self.element_text_cache[element_flag])
-            else:
-                element_text_list = []
-                for text in element.xpath('.//text()'):
-                    text = text.strip()
-                    if not text:
-                        continue
-                    clear_text = re.sub(' +', ' ', text, flags=re.S)
-                    element_text_list.append(clear_text.replace('\n', ''))
-                self.element_text_cache[element_flag] = element_text_list
-                text_list.extend(element_text_list)
-        return text_list
-
-    def need_skip_ltgi(self, ti, lti):
-        """
-        有时候，会出现像维基百科一样，在文字里面加a 标签关键词的情况，例如：
-
-        <div>
-        我是正文我是正文我是正文<a href="xxx">关键词1</a>我是正文我是正文我是正文我是正文
-        我是正文我是正文我是正文我是正文我是正文<a href="xxx">关键词2</a>我是正文我是正文
-        我是正文
-        </div>
-
-        在这种情况下，tgi = ltgi = 2，计算公式的分母为0. 为了把这种情况和列表页全是链接的
-        情况区分出来，所以要做一下判断。检查节点下面所有 a 标签的超链接中的文本数量与本节点
-        下面所有文本数量的比值。如果超链接的文本数量占比极少，那么此时，ltgi 应该忽略
-        :param ti: 节点 i 的字符串字数
-        :param lti: 节点 i 的带链接的字符串字数
-        :return: bool
-        """
-        if lti == 0:
-            return False
-
-        return ti // lti > 10  # 正文的字符数量是链接字符数量的十倍以上
-
-    def calc_text_density(self, element):
-        """
-        根据公式：
-
-               Ti - LTi
-        TDi = -----------
-              TGi - LTGi
-
-
-        Ti:节点 i 的字符串字数
-        LTi：节点 i 的带链接的字符串字数
-        TGi：节点 i 的标签数
-        LTGi：节点 i 的带连接的标签数
-
-
-        :return:
-        """
-        ti_text = '\n'.join(self.get_all_text_of_element(element))
-        ti = len(ti_text)
-        ti = self.increase_tag_weight(ti, element)
-        a_tag_list = element.xpath('.//a')
-
-        lti = len(''.join(self.get_all_text_of_element(a_tag_list)))
-        tgi = len(element.xpath('.//*'))
-        ltgi = len(a_tag_list)
-        if (tgi - ltgi) == 0:
-            if not self.need_skip_ltgi(ti, lti):
-                return {'density': 0, 'ti_text': ti_text, 'ti': ti, 'lti': lti, 'tgi': tgi, 'ltgi': ltgi}
-            else:
-                ltgi = 0
-        density = (ti - lti) / (tgi - ltgi)
-        return {'density': density, 'ti_text': ti_text, 'ti': ti, 'lti': lti, 'tgi': tgi, 'ltgi': ltgi}
-
-    def increase_tag_weight(self, ti, element):
-        tag_class = element.get('class', '')
-        tag_id = element.get('id', '')
-        if self.high_weight_keyword_pattern.search(tag_id):
-            return 2 * ti
-        if self.high_weight_keyword_pattern.search(tag_class):
-            return 2 * ti
-        return ti
-
-    def calc_sbdi(self, text, ti, lti):
-        """
-                Ti - LTi
-        SbDi = --------------
-                 Sbi + 1
-
-        SbDi: 符号密度
-        Sbi：符号数量
-
-        :return:
-        """
-        sbi = self.count_punctuation_num(text)
-        sbdi = (ti - lti) / (sbi + 1)
-        return sbdi or 1  # sbdi 不能为0，否则会导致求对数时报错。
-
-    def count_punctuation_num(self, text):
-        count = 0
-        for char in text:
-            if char in self.punctuation:
-                count += 1
-        return count
-
-    def calc_new_score(self):
-        """
-        score = 1 * ndi * log10(text_tag_count + 2) * log(sbdi)
-
-        1：在论文里面，这里使用的是 log(std)，但是每一个密度都乘以相同的对数，他们的相对大小是不会改变的，所以我们没有必要计算
-        ndi：节点 i 的文本密度
-        text_tag_count: 正文所在标签数。例如正文在<p></p>标签里面，这里就是 p 标签数，如果正文在<div></div>标签，这里就是 div 标签数
-        sbdi：节点 i 的符号密度
-        :param std:
-        :return:
-        """
-        for node_hash, node_info in self.node_info.items():
-            score = node_info['density'] * np.log10(node_info['text_tag_count'] + 2) * np.log(
-                node_info['sbdi'])
-            self.node_info[node_hash]['score'] = score
-
-    def xpath_extract_content(self, element, content_xpath='', encoding='utf-8', clear_attrib=True, pretty_print=False,
-                              method='html'):
-        """
-        提取带标签的内容
-        :param element:
-        :param content_xpath:
-        :param encoding:
-        :param clear_attrib:
-        :param pretty_print:
-        :param method:
-        :return:
-        """
-        content = element.xpath(content_xpath)
-        news_content = ''
-        if content:
-            for element_ in content:
-                if clear_attrib:
-                    element_.attrib.clear()
-                news_content += bytes.decode(
-                    tostring(element_, encoding=encoding, pretty_print=pretty_print, method=method))
-        return news_content
+import re
+import json
+import numpy as np
+from lxml.html import etree, tostring
+from html import unescape
+from ..utils import iter_node, pad_host_for_images, config, get_high_weight_keyword_pattern, universal_filter
+
+
+class ContentExtractor:
+    def __init__(self, content_tag='p'):
+        """
+
+        :param content_tag: 正文内容在哪个标签里面
+        """
+        self.content_tag = content_tag
+        self.node_info = {}
+        self.high_weight_keyword_pattern = get_high_weight_keyword_pattern()
+        self.punctuation = set('''！，。？、；：“”‘’《》%（）,.?:;'"!%()''')  # 常见的中英文标点符号
+        self.element_text_cache = {}
+
+    def extract(self, selector, host='', body_xpath='', with_body_html=False, use_visiable_info=False):
+        body_xpath = body_xpath or config.get('body', {}).get('xpath', '')
+        use_visiable_info = use_visiable_info or config.get('use_visiable_info', False)
+        if body_xpath:
+            body = selector.xpath(body_xpath)[0]
+        else:
+            body = selector.xpath('//body')[0]
+        for node_index, node in enumerate(iter_node(body)):
+            if use_visiable_info:
+                if not node.attrib.get('is_visiable', True):
+                    continue
+                coordinate_json = node.attrib.get('coordinate', '{}')
+                coordinate = json.loads(coordinate_json)
+                if coordinate.get('height', 0) < 150:  # 正文块的高度应该要大于150px
+                    continue
+            node_hash = hash(node)
+            density_info = self.calc_text_density(node)
+            text_density = density_info['density']
+            ti_text = density_info['ti_text']
+            text_tag_count = self.count_text_tag(node, tag='p')
+            sbdi = self.calc_sbdi(ti_text, density_info['ti'], density_info['lti'])
+            images_list = [
+                i.xpath('./@data-src')[0]
+                if i.xpath('./@data-src') and ';base64,' in i.xpath('./@src')[0]
+                else i.xpath('./@src')[0]
+                for i in node.xpath('.//img')
+            ]
+            host = host or config.get('host', '')
+            if host:
+                images_list = [pad_host_for_images(host, url) for url in images_list]
+            node_info = {'ti': density_info['ti'],
+                         'lti': density_info['lti'],
+                         'tgi': density_info['tgi'],
+                         'ltgi': density_info['ltgi'],
+                         'node': node,
+                         'node_index': node_index,
+                         'density': text_density,
+                         'text': ti_text,
+                         'images': images_list,
+                         'text_tag_count': text_tag_count,
+                         'sbdi': sbdi}
+            if use_visiable_info:
+                node_info['is_visiable'] = node.attrib['is_visiable']
+                node_info['coordinate'] = node.attrib.get('coordinate', '')
+            if with_body_html or config.get('with_body_html', False):
+                body_source_code = unescape(etree.tostring(node, encoding='utf-8').decode())
+                node_info['body_html'] = universal_filter(body_source_code)
+            self.node_info[node_hash] = node_info
+        self.calc_new_score()
+        result = sorted(self.node_info.items(), key=lambda x: x[1]['score'], reverse=True)
+        return result
+
+    def count_text_tag(self, element, tag='p'):
+        """
+        当前标签下面的 text()和 p 标签，都应该进行统计
+        :param element:
+        :param tag:
+        :return:
+        """
+        tag_num = len(element.xpath(f'.//{tag}'))
+        direct_text = len(element.xpath('text()'))
+        return tag_num + direct_text
+
+    def get_all_text_of_element(self, element_list):
+        if not isinstance(element_list, list):
+            element_list = [element_list]
+
+        text_list = []
+        for element in element_list:
+            element_flag = element.getroottree().getpath(element)
+            if element_flag in self.element_text_cache:  # 直接读取缓存的数据，而不是再重复提取一次
+                text_list.extend(self.element_text_cache[element_flag])
+            else:
+                element_text_list = []
+                for text in element.xpath('.//text()'):
+                    text = text.strip()
+                    if not text:
+                        continue
+                    clear_text = re.sub(' +', ' ', text, flags=re.S)
+                    element_text_list.append(clear_text.replace('\n', ''))
+                self.element_text_cache[element_flag] = element_text_list
+                text_list.extend(element_text_list)
+        return text_list
+
+    def need_skip_ltgi(self, ti, lti):
+        """
+        有时候，会出现像维基百科一样，在文字里面加a 标签关键词的情况，例如：
+
+        <div>
+        我是正文我是正文我是正文<a href="xxx">关键词1</a>我是正文我是正文我是正文我是正文
+        我是正文我是正文我是正文我是正文我是正文<a href="xxx">关键词2</a>我是正文我是正文
+        我是正文
+        </div>
+
+        在这种情况下，tgi = ltgi = 2，计算公式的分母为0. 为了把这种情况和列表页全是链接的
+        情况区分出来，所以要做一下判断。检查节点下面所有 a 标签的超链接中的文本数量与本节点
+        下面所有文本数量的比值。如果超链接的文本数量占比极少，那么此时，ltgi 应该忽略
+        :param ti: 节点 i 的字符串字数
+        :param lti: 节点 i 的带链接的字符串字数
+        :return: bool
+        """
+        if lti == 0:
+            return False
+
+        return ti // lti > 10  # 正文的字符数量是链接字符数量的十倍以上
+
+    def calc_text_density(self, element):
+        """
+        根据公式：
+
+               Ti - LTi
+        TDi = -----------
+              TGi - LTGi
+
+
+        Ti:节点 i 的字符串字数
+        LTi：节点 i 的带链接的字符串字数
+        TGi：节点 i 的标签数
+        LTGi：节点 i 的带连接的标签数
+
+
+        :return:
+        """
+        ti_text = '\n'.join(self.get_all_text_of_element(element))
+        ti = len(ti_text)
+        ti = self.increase_tag_weight(ti, element)
+        a_tag_list = element.xpath('.//a')
+
+        lti = len(''.join(self.get_all_text_of_element(a_tag_list)))
+        tgi = len(element.xpath('.//*'))
+        ltgi = len(a_tag_list)
+        if (tgi - ltgi) == 0:
+            if not self.need_skip_ltgi(ti, lti):
+                return {'density': 0, 'ti_text': ti_text, 'ti': ti, 'lti': lti, 'tgi': tgi, 'ltgi': ltgi}
+            else:
+                ltgi = 0
+        density = (ti - lti) / (tgi - ltgi)
+        return {'density': density, 'ti_text': ti_text, 'ti': ti, 'lti': lti, 'tgi': tgi, 'ltgi': ltgi}
+
+    def increase_tag_weight(self, ti, element):
+        tag_class = element.get('class', '')
+        tag_id = element.get('id', '')
+        if self.high_weight_keyword_pattern.search(tag_id):
+            return 2 * ti
+        if self.high_weight_keyword_pattern.search(tag_class):
+            return 2 * ti
+        return ti
+
+    def calc_sbdi(self, text, ti, lti):
+        """
+                Ti - LTi
+        SbDi = --------------
+                 Sbi + 1
+
+        SbDi: 符号密度
+        Sbi：符号数量
+
+        :return:
+        """
+        sbi = self.count_punctuation_num(text)
+        sbdi = (ti - lti) / (sbi + 1)
+        return sbdi or 1  # sbdi 不能为0，否则会导致求对数时报错。
+
+    def count_punctuation_num(self, text):
+        count = 0
+        for char in text:
+            if char in self.punctuation:
+                count += 1
+        return count
+
+    def calc_new_score(self):
+        """
+        score = 1 * ndi * log10(text_tag_count + 2) * log(sbdi)
+
+        1：在论文里面，这里使用的是 log(std)，但是每一个密度都乘以相同的对数，他们的相对大小是不会改变的，所以我们没有必要计算
+        ndi：节点 i 的文本密度
+        text_tag_count: 正文所在标签数。例如正文在<p></p>标签里面，这里就是 p 标签数，如果正文在<div></div>标签，这里就是 div 标签数
+        sbdi：节点 i 的符号密度
+        :param std:
+        :return:
+        """
+        for node_hash, node_info in self.node_info.items():
+            score = node_info['density'] * np.log10(node_info['text_tag_count'] + 2) * np.log(
+                node_info['sbdi'])
+            self.node_info[node_hash]['score'] = score
+
+    def xpath_extract_content(self, element, content_xpath='', encoding='utf-8', clear_attrib=True, pretty_print=False,
+                              method='html'):
+        """
+        提取带标签的内容
+        :param element:
+        :param content_xpath:
+        :param encoding:
+        :param clear_attrib:
+        :param pretty_print:
+        :param method:
+        :return:
+        """
+        content = element.xpath(content_xpath)
+        news_content = ''
+        if content:
+            for element_ in content:
+                if clear_attrib:
+                    element_.attrib.clear()
+                news_content += bytes.decode(
+                    tostring(element_, encoding=encoding, pretty_print=pretty_print, method=method))
+        return news_content
```

### Comparing `xgne-0.0.8/xgne/extractor/HeadMetaExtractor.py` & `xgne-0.0.9/xgne/extractor/HeadMetaExtractor.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import re
-
-from lxml.html import HtmlElement, Element
-from collections import Counter
-
-from ..defaults import META_IMAGE_TAGS
-from ..parsers import Parser
-
-
-class HeadMetaExtractor:
-    def __init__(self):
-        # 定义用于匹配 URL 的正则表达式
-        # self.url_pattern = re.compile(r'https?://\S+')
-        self.url_pattern = re.compile(r'https?://[^\s/]+')
-        self.parser = Parser()
-
-    def extract_host(self, head_meta):
-        # 提取所有可能的 host
-        potential_hosts = []
-        for key, value in head_meta.items():
-            # 使用正则表达式检查值是否是有效的 URL
-            matches = self.url_pattern.findall(value)
-            for match in matches:
-                potential_hosts.append(match)
-
-        # 如果有有效的 host，选择出现次数最多的作为最终的 host
-        if potential_hosts:
-            most_common_host = Counter(potential_hosts).most_common(1)[0][0]
-            return most_common_host
-        else:
-            return None
-
-    def extractor(self, element: HtmlElement):
-        # 选择包含 meta 元素的标签
-        meta_tags = element.xpath('//head/meta')
-
-        # 遍历每个 meta 元素
-        head_meta = {}
-        for tag in meta_tags:
-            # 获取 meta 元素的属性
-            property_value = tag.get('property')
-            name_value = tag.get('name')
-            content_value = tag.get('content')
-
-            # 构建字典
-            if property_value and content_value:
-                head_meta[property_value] = content_value
-            elif name_value and content_value:
-                head_meta[name_value] = content_value
-        # 提取 host
-        host = self.extract_host(head_meta)
-
-        # 将 host 添加到 head_meta 中
-        head_meta['host'] = host
-        head_meta['top_image'] = self._get_meta_image(element)
-
-        return head_meta
-
-    def _get_meta_image(self, element: Element) -> str:
-        """从文档中获取可能的图片标签。"""
-        candidates = []
-        for elem in META_IMAGE_TAGS:
-            if elem["tag"] == "meta":
-                candidates.append(
-                    (self._get_meta_field(element, elem["field"]), elem["score"])
-                )
-            else:
-                img = self.parser.getElementsByTag(
-                    element,
-                    attr=elem["attr"],
-                    value=elem["value"],
-                    use_regex=("|" in elem["value"]),
-                )
-                if img:
-                    candidates.append((img[0].get("href"), elem["score"]))
-        candidates = [c for c in candidates if c[0]]
-
-        candidates.sort(key=lambda x: x[1], reverse=True)
-
-        return candidates[0][0] if candidates else ""
-
-    def _get_meta_field(self, element: Element, field: str) -> str:
-        """从文档中提取给定的 meta 字段。"""
-        metafield = self.parser.css_select(element, field)
-        if metafield:
-            return metafield[0].get("content", "").strip()
-        return ""
+import re
+
+from lxml.html import HtmlElement, Element
+from collections import Counter
+
+from ..defaults import META_IMAGE_TAGS
+from ..parsers import Parser
+
+
+class HeadMetaExtractor:
+    def __init__(self):
+        # 定义用于匹配 URL 的正则表达式
+        # self.url_pattern = re.compile(r'https?://\S+')
+        self.url_pattern = re.compile(r'https?://[^\s/]+')
+        self.parser = Parser()
+
+    def extract_host(self, head_meta):
+        # 提取所有可能的 host
+        potential_hosts = []
+        for key, value in head_meta.items():
+            # 使用正则表达式检查值是否是有效的 URL
+            matches = self.url_pattern.findall(value)
+            for match in matches:
+                potential_hosts.append(match)
+
+        # 如果有有效的 host，选择出现次数最多的作为最终的 host
+        if potential_hosts:
+            most_common_host = Counter(potential_hosts).most_common(1)[0][0]
+            return most_common_host
+        else:
+            return None
+
+    def extractor(self, element: HtmlElement):
+        # 选择包含 meta 元素的标签
+        meta_tags = element.xpath('//head/meta')
+
+        # 遍历每个 meta 元素
+        head_meta = {}
+        for tag in meta_tags:
+            # 获取 meta 元素的属性
+            property_value = tag.get('property')
+            name_value = tag.get('name')
+            content_value = tag.get('content')
+
+            # 构建字典
+            if property_value and content_value:
+                head_meta[property_value] = content_value
+            elif name_value and content_value:
+                head_meta[name_value] = content_value
+        # 提取 host
+        host = self.extract_host(head_meta)
+
+        # 将 host 添加到 head_meta 中
+        head_meta['host'] = host
+        head_meta['top_image'] = self._get_meta_image(element)
+
+        return head_meta
+
+    def _get_meta_image(self, element: Element) -> str:
+        """从文档中获取可能的图片标签。"""
+        candidates = []
+        for elem in META_IMAGE_TAGS:
+            if elem["tag"] == "meta":
+                candidates.append(
+                    (self._get_meta_field(element, elem["field"]), elem["score"])
+                )
+            else:
+                img = self.parser.getElementsByTag(
+                    element,
+                    attr=elem["attr"],
+                    value=elem["value"],
+                    use_regex=("|" in elem["value"]),
+                )
+                if img:
+                    candidates.append((img[0].get("href"), elem["score"]))
+        candidates = [c for c in candidates if c[0]]
+
+        candidates.sort(key=lambda x: x[1], reverse=True)
+
+        return candidates[0][0] if candidates else ""
+
+    def _get_meta_field(self, element: Element, field: str) -> str:
+        """从文档中提取给定的 meta 字段。"""
+        metafield = self.parser.css_select(element, field)
+        if metafield:
+            return metafield[0].get("content", "").strip()
+        return ""
```

### Comparing `xgne-0.0.8/xgne/extractor/LangExtractor.py` & `xgne-0.0.9/xgne/extractor/LangExtractor.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import re
-import locale
-import langid
-from lxml import html
-
-
-class LangExtractor:
-    def __init__(self):
-        self.name = "langid"
-        # 用于提取语言代码的正则表达式模式
-        self.langcode_pattern = re.compile(r'\b[a-zA-Z]{2}(?=([-_]|\b))')
-
-    def language(self, response):
-        try:
-            root = html.fromstring(response)
-        except ValueError:
-            root = html.fromstring(response.encode("utf-8"))
-
-        # 从不同的源提取语言
-        lang = self.extract_from_attributes(root) or \
-               self.extract_from_meta_tags(root) or \
-               self.extract_from_articles(root) or \
-               self.extract_from_body(root)
-
-        if lang:
-            lang = self.normalize_language(lang)
-
-        return lang
-
-    def extract_from_attributes(self, root):
-        # 从 HTML 属性中提取语言代码
-        lang = root.get('lang') or root.get('xml:lang')
-        return lang
-
-    def extract_from_meta_tags(self, root):
-        # 从 meta 标签中提取语言代码
-        lang = root.xpath('string(//meta[@name="language"]/@content)') or \
-               root.xpath('string(//meta[@property="og:locale"]/@content)')
-        return lang.strip() if lang else None
-
-    def extract_from_articles(self, root):
-        # 从文章中提取语言代码，选择最长的文章
-        article_texts = [re.sub(r'\s+', ' ', article.text_content().strip()) for article in root.xpath('//article')]
-        longest_article = max(article_texts, key=len, default='')
-        return langid.classify(longest_article)[0] if longest_article else None
-
-    def extract_from_body(self, root):
-        # 从整个 HTML 主体中提取语言代码
-        return langid.classify(root.text_content().strip())[0]
-
-    def normalize_language(self, lang):
-        # 规范化语言代码的输出
-        matches = self.langcode_pattern.search(lang)
-        if matches:
-            return matches.group(0)
-        else:
-            normalized = locale.normalize(re.split(r'\s|;|,', lang.strip())[0])
-            matches = self.langcode_pattern.search(normalized)
-            return matches.group(0) if matches else None
+import re
+import locale
+import langid
+from lxml import html
+
+
+class LangExtractor:
+    def __init__(self):
+        self.name = "langid"
+        # 用于提取语言代码的正则表达式模式
+        self.langcode_pattern = re.compile(r'\b[a-zA-Z]{2}(?=([-_]|\b))')
+
+    def language(self, response):
+        try:
+            root = html.fromstring(response)
+        except ValueError:
+            root = html.fromstring(response.encode("utf-8"))
+
+        # 从不同的源提取语言
+        lang = self.extract_from_attributes(root) or \
+               self.extract_from_meta_tags(root) or \
+               self.extract_from_articles(root) or \
+               self.extract_from_body(root)
+
+        if lang:
+            lang = self.normalize_language(lang)
+
+        return lang
+
+    def extract_from_attributes(self, root):
+        # 从 HTML 属性中提取语言代码
+        lang = root.get('lang') or root.get('xml:lang')
+        return lang
+
+    def extract_from_meta_tags(self, root):
+        # 从 meta 标签中提取语言代码
+        lang = root.xpath('string(//meta[@name="language"]/@content)') or \
+               root.xpath('string(//meta[@property="og:locale"]/@content)')
+        return lang.strip() if lang else None
+
+    def extract_from_articles(self, root):
+        # 从文章中提取语言代码，选择最长的文章
+        article_texts = [re.sub(r'\s+', ' ', article.text_content().strip()) for article in root.xpath('//article')]
+        longest_article = max(article_texts, key=len, default='')
+        return langid.classify(longest_article)[0] if longest_article else None
+
+    def extract_from_body(self, root):
+        # 从整个 HTML 主体中提取语言代码
+        return langid.classify(root.text_content().strip())[0]
+
+    def normalize_language(self, lang):
+        # 规范化语言代码的输出
+        matches = self.langcode_pattern.search(lang)
+        if matches:
+            return matches.group(0)
+        else:
+            normalized = locale.normalize(re.split(r'\s|;|,', lang.strip())[0])
+            matches = self.langcode_pattern.search(normalized)
+            return matches.group(0) if matches else None
```

### Comparing `xgne-0.0.8/xgne/extractor/ListExtractor.py` & `xgne-0.0.9/xgne/extractor/ListExtractor.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from collections import deque
-from lxml.html import HtmlElement
-
-
-class ListExtractor:
-    def extract(self, element: HtmlElement, feature):
-        result = []
-        if feature.startswith('/'):
-            feature_element = element.xpath(feature)
-        else:
-            feature_element = element.xpath(f'//*[contains(text(), "{feature}")]')
-
-        if not feature_element:
-            print('找不到 feature！')
-            return result
-
-        parent = feature_element[0]
-        leaf_class = parent.attrib.get('class', '')
-        if leaf_class:
-            leaf_node = f'{parent.tag}[@class="{leaf_class}"]'
-        else:
-            leaf_node = parent.tag
-        is_a_tag = parent.tag == 'a'
-        sub_path_queue = deque([leaf_node])
-        while parent is not None:
-            parent = parent.getparent()
-            if parent is None:
-                break
-            path = '/'.join(sub_path_queue)
-            item_list = parent.xpath(path)
-            if len(item_list) > 3:
-                for item in item_list:
-                    item_info = {'title': ''.join(item.xpath('text()'))}
-                    if is_a_tag:
-                        item_info['url'] = ''.join(item.xpath('@href'))
-                    result.append(item_info)
-                return result
-            sub_path_queue.insert(0, parent.tag)
-        return result
-
-
+from collections import deque
+from lxml.html import HtmlElement
+
+
+class ListExtractor:
+    def extract(self, element: HtmlElement, feature):
+        result = []
+        if feature.startswith('/'):
+            feature_element = element.xpath(feature)
+        else:
+            feature_element = element.xpath(f'//*[contains(text(), "{feature}")]')
+
+        if not feature_element:
+            print('找不到 feature！')
+            return result
+
+        parent = feature_element[0]
+        leaf_class = parent.attrib.get('class', '')
+        if leaf_class:
+            leaf_node = f'{parent.tag}[@class="{leaf_class}"]'
+        else:
+            leaf_node = parent.tag
+        is_a_tag = parent.tag == 'a'
+        sub_path_queue = deque([leaf_node])
+        while parent is not None:
+            parent = parent.getparent()
+            if parent is None:
+                break
+            path = '/'.join(sub_path_queue)
+            item_list = parent.xpath(path)
+            if len(item_list) > 3:
+                for item in item_list:
+                    item_info = {'title': ''.join(item.xpath('text()'))}
+                    if is_a_tag:
+                        item_info['url'] = ''.join(item.xpath('@href'))
+                    result.append(item_info)
+                return result
+            sub_path_queue.insert(0, parent.tag)
+        return result
+
+
```

### Comparing `xgne-0.0.8/xgne/extractor/TitleExtractor.py` & `xgne-0.0.9/xgne/extractor/TitleExtractor.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import re
-from ..utils import config, get_longest_common_sub_string
-from lxml.html import HtmlElement
-from ..defaults import TITLE_HTAG_XPATH, TITLE_SPLIT_CHAR_PATTERN
-
-
-class TitleExtractor:
-    def extract_by_xpath(self, element, title_xpath):
-        if title_xpath:
-            title_list = element.xpath(title_xpath)
-            if title_list:
-                return title_list[0]
-            else:
-                return ''
-        return ''
-
-    def extract_by_title(self, element):
-        title_list = element.xpath('//title/text()')
-        if not title_list:
-            return ''
-        title = re.split(TITLE_SPLIT_CHAR_PATTERN, title_list[0])
-        if title:
-            if len(title[0]) >= 4:
-                return title[0]
-            return title_list[0]
-        else:
-            return ''
-
-    def extract_by_htag(self, element):
-        title_list = element.xpath(TITLE_HTAG_XPATH)
-        if not title_list:
-            return ''
-        return title_list[0]
-
-    def extract_by_htag_and_title(self, element: HtmlElement) -> str:
-        """
-        一般来说，我们可以认为 title 中包含新闻标题，但是可能也含有其他文字，例如：
-        GNE 成为全球最好的新闻提取模块-今日头条
-        新华网：GNE 成为全球最好的新闻提取模块
-
-        同时，新闻的某个 <h>标签中也会包含这个新闻标题。
-
-        因此，通过 h 标签与 title 的文字双向匹配，找到最适合作为新闻标题的字符串。
-        但是，需要考虑到 title 与 h 标签中的文字可能均含有特殊符号，因此，不能直接通过
-        判断 h 标签中的文字是否在 title 中来判断，这里需要中最长公共子串。
-        :param element:
-        :return:
-        """
-        h_tag_texts_list = element.xpath('(//h1//text() | //h2//text() | //h3//text() | //h4//text() | //h5//text())')
-        title_text = ''.join(element.xpath('//title/text()'))
-        news_title = ''
-        for h_tag_text in h_tag_texts_list:
-            lcs = get_longest_common_sub_string(title_text, h_tag_text)
-            if len(lcs) > len(news_title):
-                news_title = lcs
-        return news_title if len(news_title) > 4 else ''
-
-    def extract(self, element: HtmlElement, title_xpath: str = '') -> str:
-        title_xpath = title_xpath or config.get('title', {}).get('xpath')
-        title = (self.extract_by_xpath(element, title_xpath)
-                 or self.extract_by_htag_and_title(element)
-                 or self.extract_by_title(element)
-                 or self.extract_by_htag(element)
-                 )
-        return title.strip()
+import re
+from ..utils import config, get_longest_common_sub_string
+from lxml.html import HtmlElement
+from ..defaults import TITLE_HTAG_XPATH, TITLE_SPLIT_CHAR_PATTERN
+
+
+class TitleExtractor:
+    def extract_by_xpath(self, element, title_xpath):
+        if title_xpath:
+            title_list = element.xpath(title_xpath)
+            if title_list:
+                return title_list[0]
+            else:
+                return ''
+        return ''
+
+    def extract_by_title(self, element):
+        title_list = element.xpath('//title/text()')
+        if not title_list:
+            return ''
+        title = re.split(TITLE_SPLIT_CHAR_PATTERN, title_list[0])
+        if title:
+            if len(title[0]) >= 4:
+                return title[0]
+            return title_list[0]
+        else:
+            return ''
+
+    def extract_by_htag(self, element):
+        title_list = element.xpath(TITLE_HTAG_XPATH)
+        if not title_list:
+            return ''
+        return title_list[0]
+
+    def extract_by_htag_and_title(self, element: HtmlElement) -> str:
+        """
+        一般来说，我们可以认为 title 中包含新闻标题，但是可能也含有其他文字，例如：
+        GNE 成为全球最好的新闻提取模块-今日头条
+        新华网：GNE 成为全球最好的新闻提取模块
+
+        同时，新闻的某个 <h>标签中也会包含这个新闻标题。
+
+        因此，通过 h 标签与 title 的文字双向匹配，找到最适合作为新闻标题的字符串。
+        但是，需要考虑到 title 与 h 标签中的文字可能均含有特殊符号，因此，不能直接通过
+        判断 h 标签中的文字是否在 title 中来判断，这里需要中最长公共子串。
+        :param element:
+        :return:
+        """
+        h_tag_texts_list = element.xpath('(//h1//text() | //h2//text() | //h3//text() | //h4//text() | //h5//text())')
+        title_text = ''.join(element.xpath('//title/text()'))
+        news_title = ''
+        for h_tag_text in h_tag_texts_list:
+            lcs = get_longest_common_sub_string(title_text, h_tag_text)
+            if len(lcs) > len(news_title):
+                news_title = lcs
+        return news_title if len(news_title) > 4 else ''
+
+    def extract(self, element: HtmlElement, title_xpath: str = '') -> str:
+        title_xpath = title_xpath or config.get('title', {}).get('xpath')
+        title = (self.extract_by_xpath(element, title_xpath)
+                 or self.extract_by_htag_and_title(element)
+                 or self.extract_by_title(element)
+                 or self.extract_by_htag(element)
+                 )
+        return title.strip()
```

### Comparing `xgne-0.0.8/xgne/parsers.py` & `xgne-0.0.9/xgne/parsers.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-# -*- coding: utf-8 -*-
-# Much of the code here was forked from https://github.com/codelucas/newspaper
-# Copyright (c) Lucas Ou-Yang (codelucas)
-
-"""
-Newspaper uses a lot of python-goose's parsing code. View theirlicense:
-https://github.com/codelucas/newspaper/blob/master/GOOSE-LICENSE.txt
-
-Parser objects will only contain operations that manipulate
-or query an lxml or soup dom object generated from an article's html.
-"""
-import json
-import re
-import logging
-import string
-from copy import deepcopy
-from typing import List, Dict
-import lxml.etree
-import lxml.html
-import lxml.html.clean
-from html import unescape
-
-from bs4 import UnicodeDammit
-
-from . import text
-
-log = logging.getLogger(__name__)
-
-
-class Parser:
-    @classmethod
-    def xpath_re(cls, node, expression):
-        regexp_namespace = "http://exslt.org/regular-expressions"
-        items = node.xpath(expression, namespaces={"re": regexp_namespace})
-        return items
-
-    @classmethod
-    def drop_tag(cls, nodes):
-        if isinstance(nodes, list):
-            for node in nodes:
-                node.drop_tag()
-        else:
-            nodes.drop_tag()
-
-    @classmethod
-    def css_select(cls, node, selector):
-        return node.cssselect(selector)
-
-    @classmethod
-    def get_unicode_html(cls, html):
-        if isinstance(html, str):
-            return html
-        if not html:
-            return html
-        converted = UnicodeDammit(html, is_html=True)
-        if not converted.unicode_markup:
-            raise ValueError(
-                "Failed to detect encoding of article HTML, tried: %s"
-                % ", ".join(converted.tried_encodings)
-            )
-        html = converted.unicode_markup
-        return html
-
-    @classmethod
-    def fromstring(cls, html):
-        html = cls.get_unicode_html(html)
-        # Enclosed in a `try` to prevent bringing the entire library
-        # down due to one article (out of potentially many in a `Source`)
-        try:
-            # lxml does not play well with <? ?> encoding tags
-            if html.startswith("<?"):
-                html = re.sub(r"^\<\?.*?\?\>", "", html, flags=re.DOTALL)
-            cls.doc = lxml.html.fromstring(html)
-            return cls.doc
-        except Exception:
-            log.warning("fromstring() returned an invalid string: %s...", html[:20])
-            return
-
-    @classmethod
-    def clean_article_html(cls, node):
-        article_cleaner = lxml.html.clean.Cleaner()
-        article_cleaner.javascript = True
-        article_cleaner.style = True
-        article_cleaner.allow_tags = [
-            "a",
-            "span",
-            "p",
-            "br",
-            "strong",
-            "b",
-            "em",
-            "i",
-            "tt",
-            "code",
-            "pre",
-            "blockquote",
-            "img",
-            "h1",
-            "h2",
-            "h3",
-            "h4",
-            "h5",
-            "h6",
-            "ul",
-            "ol",
-            "li",
-            "dl",
-            "dt",
-            "dd",
-        ]
-        article_cleaner.remove_unknown_tags = False
-        return article_cleaner.clean_html(node)
-
-    @classmethod
-    def nodeToString(cls, node):
-        """`decode` is needed at the end because `etree.tostring`
-        returns a python bytestring
-        """
-        return lxml.etree.tostring(node, method="html").decode()
-
-    @classmethod
-    def replaceTag(cls, node, tag):
-        node.tag = tag
-
-    @classmethod
-    def stripTags(cls, node, *tags):
-        lxml.etree.strip_tags(node, *tags)
-
-    @classmethod
-    def getElementById(cls, node, idd):
-        selector = '//*[@id="%s"]' % idd
-        elems = node.xpath(selector)
-        if elems:
-            return elems[0]
-        return None
-
-    @classmethod
-    def getElementsByTag(
-        cls, node, tag=None, attr=None, value=None, children=False, use_regex=False
-    ) -> list:
-        NS = None
-        # selector = tag or '*'
-        selector = "descendant-or-self::%s" % (tag or "*")
-        if attr and value:
-            if use_regex:
-                NS = {"re": "http://exslt.org/regular-expressions"}
-                selector = '%s[re:test(@%s, "%s", "i")]' % (selector, attr, value)
-            else:
-                trans = 'translate(@%s, "%s", "%s")' % (
-                    attr,
-                    string.ascii_uppercase,
-                    string.ascii_lowercase,
-                )
-                selector = '%s[contains(%s, "%s")]' % (selector, trans, value.lower())
-        elems = node.xpath(selector, namespaces=NS)
-        # remove the root node
-        # if we have a selection tag
-        if node in elems and (tag or children):
-            elems.remove(node)
-        return elems
-
-    @classmethod
-    def get_element_by_attribs(
-        cls, node, attribs: Dict[str, str]
-    ) -> List[lxml.html.Element]:
-        """Get list of elements with matching attributes
-
-        Args:
-            attribs (Dict[str,str]): dictionary containing attributes to match.
-                e.g. {"class":"foo", "id":"bar"}
-
-        Returns:
-            List[lxml.html.Element]: Elements matching the attributes
-        """
-        sel_list = []
-        for k, v in attribs.items():
-            trans = 'translate(@%s, "%s", "%s")' % (
-                k,
-                string.ascii_uppercase,
-                string.ascii_lowercase,
-            )
-            selector = '%s="%s"' % (trans, v.lower())
-            sel_list.append(selector)
-        selector = "descendant-or-self::*[%s]" % " and ".join(sel_list)
-        elems = node.xpath(selector)
-        return elems
-
-    @classmethod
-    def appendChild(cls, node, child):
-        node.append(child)
-
-    @classmethod
-    def childNodes(cls, node):
-        return list(node)
-
-    @classmethod
-    def childNodesWithText(cls, node):
-        root = node
-        # create the first text node
-        # if we have some text in the node
-        if root.text:
-            t = lxml.html.HtmlElement()
-            t.text = root.text
-            t.tag = "text"
-            root.text = None
-            root.insert(0, t)
-        # loop children
-        for c, n in enumerate(list(root)):
-            idx = root.index(n)
-            # don't process texts nodes
-            if n.tag == "text":
-                continue
-            # create a text node for tail
-            if n.tail:
-                t = cls.createElement(tag="text", text=n.tail, tail=None)
-                root.insert(idx + 1, t)
-        return list(root)
-
-    @classmethod
-    def textToPara(cls, text):
-        return cls.fromstring(text)
-
-    @classmethod
-    def getChildren(cls, node):
-        return node.getchildren()
-
-    @classmethod
-    def getElementsByTags(cls, node, tags):
-        selector = "descendant::*[%s]" % (" or ".join("self::%s" % tag for tag in tags))
-        elems = node.xpath(selector)
-        return elems
-
-    @classmethod
-    def createElement(cls, tag="p", text=None, tail=None):
-        t = lxml.html.HtmlElement()
-        t.tag = tag
-        t.text = text
-        t.tail = tail
-        return t
-
-    @classmethod
-    def getComments(cls, node):
-        return node.xpath("//comment()")
-
-    @classmethod
-    def getParent(cls, node):
-        return node.getparent()
-
-    @classmethod
-    def remove(cls, node):
-        parent = node.getparent()
-        if parent is not None:
-            if node.tail:
-                prev = node.getprevious()
-                if prev is None:
-                    if not parent.text:
-                        parent.text = ""
-                    parent.text += " " + node.tail
-                else:
-                    if not prev.tail:
-                        prev.tail = ""
-                    prev.tail += " " + node.tail
-            node.clear()
-            parent.remove(node)
-
-    @classmethod
-    def getTag(cls, node):
-        return node.tag
-
-    @classmethod
-    def getText(cls, node):
-        txts = [i for i in node.itertext()]
-        return text.innerTrim(" ".join(txts).strip())
-
-    @classmethod
-    def previousSiblings(cls, node):
-        """
-        returns preceding siblings in reverse order (nearest sibling is first)
-        """
-        return [n for n in node.itersiblings(preceding=True)]
-
-    @classmethod
-    def previousSibling(cls, node):
-        return node.getprevious()
-
-    @classmethod
-    def nextSibling(cls, node):
-        return node.getnext()
-
-    @classmethod
-    def isTextNode(cls, node):
-        return True if node.tag == "text" else False
-
-    @classmethod
-    def getAttribute(cls, node, attr=None):
-        if attr:
-            attr = node.attrib.get(attr, None)
-        if attr:
-            attr = unescape(attr)
-        return attr
-
-    @classmethod
-    def delAttribute(cls, node, attr=None):
-        if attr:
-            _attr = node.attrib.get(attr, None)
-            if _attr:
-                del node.attrib[attr]
-
-    @classmethod
-    def setAttribute(cls, node, attr=None, value=None):
-        if attr and value:
-            # Check if immutable attribute
-            if isinstance(
-                node, (lxml.etree.CommentBase, lxml.etree.EntityBase, lxml.etree.PIBase)
-            ):
-                return
-            node.set(attr, value)
-
-    @classmethod
-    def outerHtml(cls, node):
-        e0 = node
-        if e0.tail:
-            e0 = deepcopy(e0)
-            e0.tail = None
-        return cls.nodeToString(e0)
-
-    @classmethod
-    def get_ld_json_object(cls, node):
-        """Get the JSON-LD object from the node"""
-        # yoast seo structured data
-        json_ld = cls.getElementsByTag(
-            node, tag="script", attr="type", value="application/ld+json"
-        )
-        res = []
-        if json_ld:
-            for script_tag in json_ld:
-                try:
-                    schema_json = json.loads(script_tag.text)
-                except Exception:
-                    continue
-                if isinstance(schema_json, list):
-                    res.extend(schema_json)
-                else:
-                    res.append(schema_json)
-
+# -*- coding: utf-8 -*-
+# Much of the code here was forked from https://github.com/codelucas/newspaper
+# Copyright (c) Lucas Ou-Yang (codelucas)
+
+"""
+Newspaper uses a lot of python-goose's parsing code. View theirlicense:
+https://github.com/codelucas/newspaper/blob/master/GOOSE-LICENSE.txt
+
+Parser objects will only contain operations that manipulate
+or query an lxml or soup dom object generated from an article's html.
+"""
+import json
+import re
+import logging
+import string
+from copy import deepcopy
+from typing import List, Dict
+import lxml.etree
+import lxml.html
+import lxml.html.clean
+from html import unescape
+
+from bs4 import UnicodeDammit
+
+from . import text
+
+log = logging.getLogger(__name__)
+
+
+class Parser:
+    @classmethod
+    def xpath_re(cls, node, expression):
+        regexp_namespace = "http://exslt.org/regular-expressions"
+        items = node.xpath(expression, namespaces={"re": regexp_namespace})
+        return items
+
+    @classmethod
+    def drop_tag(cls, nodes):
+        if isinstance(nodes, list):
+            for node in nodes:
+                node.drop_tag()
+        else:
+            nodes.drop_tag()
+
+    @classmethod
+    def css_select(cls, node, selector):
+        return node.cssselect(selector)
+
+    @classmethod
+    def get_unicode_html(cls, html):
+        if isinstance(html, str):
+            return html
+        if not html:
+            return html
+        converted = UnicodeDammit(html, is_html=True)
+        if not converted.unicode_markup:
+            raise ValueError(
+                "Failed to detect encoding of article HTML, tried: %s"
+                % ", ".join(converted.tried_encodings)
+            )
+        html = converted.unicode_markup
+        return html
+
+    @classmethod
+    def fromstring(cls, html):
+        html = cls.get_unicode_html(html)
+        # Enclosed in a `try` to prevent bringing the entire library
+        # down due to one article (out of potentially many in a `Source`)
+        try:
+            # lxml does not play well with <? ?> encoding tags
+            if html.startswith("<?"):
+                html = re.sub(r"^\<\?.*?\?\>", "", html, flags=re.DOTALL)
+            cls.doc = lxml.html.fromstring(html)
+            return cls.doc
+        except Exception:
+            log.warning("fromstring() returned an invalid string: %s...", html[:20])
+            return
+
+    @classmethod
+    def clean_article_html(cls, node):
+        article_cleaner = lxml.html.clean.Cleaner()
+        article_cleaner.javascript = True
+        article_cleaner.style = True
+        article_cleaner.allow_tags = [
+            "a",
+            "span",
+            "p",
+            "br",
+            "strong",
+            "b",
+            "em",
+            "i",
+            "tt",
+            "code",
+            "pre",
+            "blockquote",
+            "img",
+            "h1",
+            "h2",
+            "h3",
+            "h4",
+            "h5",
+            "h6",
+            "ul",
+            "ol",
+            "li",
+            "dl",
+            "dt",
+            "dd",
+        ]
+        article_cleaner.remove_unknown_tags = False
+        return article_cleaner.clean_html(node)
+
+    @classmethod
+    def nodeToString(cls, node):
+        """`decode` is needed at the end because `etree.tostring`
+        returns a python bytestring
+        """
+        return lxml.etree.tostring(node, method="html").decode()
+
+    @classmethod
+    def replaceTag(cls, node, tag):
+        node.tag = tag
+
+    @classmethod
+    def stripTags(cls, node, *tags):
+        lxml.etree.strip_tags(node, *tags)
+
+    @classmethod
+    def getElementById(cls, node, idd):
+        selector = '//*[@id="%s"]' % idd
+        elems = node.xpath(selector)
+        if elems:
+            return elems[0]
+        return None
+
+    @classmethod
+    def getElementsByTag(
+        cls, node, tag=None, attr=None, value=None, children=False, use_regex=False
+    ) -> list:
+        NS = None
+        # selector = tag or '*'
+        selector = "descendant-or-self::%s" % (tag or "*")
+        if attr and value:
+            if use_regex:
+                NS = {"re": "http://exslt.org/regular-expressions"}
+                selector = '%s[re:test(@%s, "%s", "i")]' % (selector, attr, value)
+            else:
+                trans = 'translate(@%s, "%s", "%s")' % (
+                    attr,
+                    string.ascii_uppercase,
+                    string.ascii_lowercase,
+                )
+                selector = '%s[contains(%s, "%s")]' % (selector, trans, value.lower())
+        elems = node.xpath(selector, namespaces=NS)
+        # remove the root node
+        # if we have a selection tag
+        if node in elems and (tag or children):
+            elems.remove(node)
+        return elems
+
+    @classmethod
+    def get_element_by_attribs(
+        cls, node, attribs: Dict[str, str]
+    ) -> List[lxml.html.Element]:
+        """Get list of elements with matching attributes
+
+        Args:
+            attribs (Dict[str,str]): dictionary containing attributes to match.
+                e.g. {"class":"foo", "id":"bar"}
+
+        Returns:
+            List[lxml.html.Element]: Elements matching the attributes
+        """
+        sel_list = []
+        for k, v in attribs.items():
+            trans = 'translate(@%s, "%s", "%s")' % (
+                k,
+                string.ascii_uppercase,
+                string.ascii_lowercase,
+            )
+            selector = '%s="%s"' % (trans, v.lower())
+            sel_list.append(selector)
+        selector = "descendant-or-self::*[%s]" % " and ".join(sel_list)
+        elems = node.xpath(selector)
+        return elems
+
+    @classmethod
+    def appendChild(cls, node, child):
+        node.append(child)
+
+    @classmethod
+    def childNodes(cls, node):
+        return list(node)
+
+    @classmethod
+    def childNodesWithText(cls, node):
+        root = node
+        # create the first text node
+        # if we have some text in the node
+        if root.text:
+            t = lxml.html.HtmlElement()
+            t.text = root.text
+            t.tag = "text"
+            root.text = None
+            root.insert(0, t)
+        # loop children
+        for c, n in enumerate(list(root)):
+            idx = root.index(n)
+            # don't process texts nodes
+            if n.tag == "text":
+                continue
+            # create a text node for tail
+            if n.tail:
+                t = cls.createElement(tag="text", text=n.tail, tail=None)
+                root.insert(idx + 1, t)
+        return list(root)
+
+    @classmethod
+    def textToPara(cls, text):
+        return cls.fromstring(text)
+
+    @classmethod
+    def getChildren(cls, node):
+        return node.getchildren()
+
+    @classmethod
+    def getElementsByTags(cls, node, tags):
+        selector = "descendant::*[%s]" % (" or ".join("self::%s" % tag for tag in tags))
+        elems = node.xpath(selector)
+        return elems
+
+    @classmethod
+    def createElement(cls, tag="p", text=None, tail=None):
+        t = lxml.html.HtmlElement()
+        t.tag = tag
+        t.text = text
+        t.tail = tail
+        return t
+
+    @classmethod
+    def getComments(cls, node):
+        return node.xpath("//comment()")
+
+    @classmethod
+    def getParent(cls, node):
+        return node.getparent()
+
+    @classmethod
+    def remove(cls, node):
+        parent = node.getparent()
+        if parent is not None:
+            if node.tail:
+                prev = node.getprevious()
+                if prev is None:
+                    if not parent.text:
+                        parent.text = ""
+                    parent.text += " " + node.tail
+                else:
+                    if not prev.tail:
+                        prev.tail = ""
+                    prev.tail += " " + node.tail
+            node.clear()
+            parent.remove(node)
+
+    @classmethod
+    def getTag(cls, node):
+        return node.tag
+
+    @classmethod
+    def getText(cls, node):
+        txts = [i for i in node.itertext()]
+        return text.innerTrim(" ".join(txts).strip())
+
+    @classmethod
+    def previousSiblings(cls, node):
+        """
+        returns preceding siblings in reverse order (nearest sibling is first)
+        """
+        return [n for n in node.itersiblings(preceding=True)]
+
+    @classmethod
+    def previousSibling(cls, node):
+        return node.getprevious()
+
+    @classmethod
+    def nextSibling(cls, node):
+        return node.getnext()
+
+    @classmethod
+    def isTextNode(cls, node):
+        return True if node.tag == "text" else False
+
+    @classmethod
+    def getAttribute(cls, node, attr=None):
+        if attr:
+            attr = node.attrib.get(attr, None)
+        if attr:
+            attr = unescape(attr)
+        return attr
+
+    @classmethod
+    def delAttribute(cls, node, attr=None):
+        if attr:
+            _attr = node.attrib.get(attr, None)
+            if _attr:
+                del node.attrib[attr]
+
+    @classmethod
+    def setAttribute(cls, node, attr=None, value=None):
+        if attr and value:
+            # Check if immutable attribute
+            if isinstance(
+                node, (lxml.etree.CommentBase, lxml.etree.EntityBase, lxml.etree.PIBase)
+            ):
+                return
+            node.set(attr, value)
+
+    @classmethod
+    def outerHtml(cls, node):
+        e0 = node
+        if e0.tail:
+            e0 = deepcopy(e0)
+            e0.tail = None
+        return cls.nodeToString(e0)
+
+    @classmethod
+    def get_ld_json_object(cls, node):
+        """Get the JSON-LD object from the node"""
+        # yoast seo structured data
+        json_ld = cls.getElementsByTag(
+            node, tag="script", attr="type", value="application/ld+json"
+        )
+        res = []
+        if json_ld:
+            for script_tag in json_ld:
+                try:
+                    schema_json = json.loads(script_tag.text)
+                except Exception:
+                    continue
+                if isinstance(schema_json, list):
+                    res.extend(schema_json)
+                else:
+                    res.append(schema_json)
+
         return res
```

### Comparing `xgne-0.0.8/xgne/text.py` & `xgne-0.0.9/xgne/text.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-# -*- coding: utf-8 -*-
-# Much of the code here was forked from https://github.com/codelucas/newspaper
-# Copyright (c) Lucas Ou-Yang (codelucas)
-
-"""
-Stopword extraction and stopword classes.
-"""
-
-from dataclasses import dataclass, field
-from pathlib import Path
-import re
-import string
-from typing import Dict, List
-
-
-from .utils import FileHelper
-
-
-def innerTrim(value):
-    if isinstance(value, str):
-        # remove tab and white space
-        value = re.sub(r"[\s\t]+", " ", value)
-        value = "".join(value.splitlines())
-        return value.strip()
-    return ""
-
-
-@dataclass
-class WordStats:
-    """Holds the number of stop words and total words in an article"""
-
-    stop_word_count: int = 0
-    word_count: int = 0
-    stop_words: List[str] = field(default_factory=list)
-
-
-class StopWords:
-    TRANS_TABLE = str.maketrans("", "")
-    _cached_stop_words: Dict[str, str] = {}
-
-    def __init__(self, language="en"):
-        if language not in self._cached_stop_words:
-            stopwordsFile = Path(STOPWORDS_DIR) / f"stopwords-{language}.txt"
-            self._cached_stop_words[language] = set(
-                FileHelper.loadResourceFile(stopwordsFile).splitlines()
-            )
-        self.STOP_WORDS = self._cached_stop_words[language]
-
-    def remove_punctuation(self, content):
-        # code taken form
-        # http://stackoverflow.com/questions/265960/best-way-to-strip-punctuation-from-a-string-in-python
-        content_is_unicode = isinstance(content, str)
-        if content_is_unicode:
-            content = content.encode("utf-8")
-        trans_table = {ord(c): None for c in string.punctuation}
-        stripped_input = content.decode("utf-8").translate(trans_table)
-
-        return stripped_input
-
-    def candidate_words(self, stripped_input):
-        return stripped_input.split(" ")
-
-    def get_stopword_count(self, content):
-        if not content:
-            return WordStats()
-        ws = WordStats()
-        stripped_input = self.remove_punctuation(content)
-        candidate_words = self.candidate_words(stripped_input.lower())
-        overlapping_stopwords = []
-        c = 0
-        for w in candidate_words:
-            c += 1
-            if w in self.STOP_WORDS:
-                overlapping_stopwords.append(w)
-
-        ws.word_count = c
-        ws.stop_word_count = len(overlapping_stopwords)
-        ws.stop_words = overlapping_stopwords
-        return ws
-
-
-class StopWordsChinese(StopWords):
-    """Chinese segmentation"""
-
-    def __init__(self, language="zh"):
-        super(StopWordsChinese, self).__init__(language="zh")
-
-    def candidate_words(self, stripped_input):
-        # jieba builds a tree that takes a while. avoid building
-        # this tree if we don't use the chinese language
-        import jieba
-
-        return jieba.cut(stripped_input, cut_all=True)
-
-
-class StopWordsArabic(StopWords):
-    """Arabic segmentation"""
-
-    def __init__(self, language="ar"):
-        # force ar language code
-        super(StopWordsArabic, self).__init__(language="ar")
-
-    def remove_punctuation(self, content):
-        return content
-
-    def candidate_words(self, stripped_input):
-        import nltk
-
-        s = nltk.stem.isri.ISRIStemmer()
-        words = []
-        for word in nltk.tokenize.wordpunct_tokenize(stripped_input):
-            words.append(s.stem(word))
-        return words
-
-
-class StopWordsKorean(StopWords):
-    """Korean segmentation"""
-
-    def __init__(self, language="ko"):
-        super(StopWordsKorean, self).__init__(language="ko")
-
-    def get_stopword_count(self, content):
-        if not content:
-            return WordStats()
-        ws = WordStats()
-        stripped_input = self.remove_punctuation(content)
-        candidate_words = self.candidate_words(stripped_input)
-        overlapping_stopwords = []
-        c = 0
-        for w in candidate_words:
-            c += 1
-            for s in self.STOP_WORDS:
-                if w.endswith(s):
-                    overlapping_stopwords.append(w)
-
-        ws.word_count = c
-        ws.stop_word_count = len(overlapping_stopwords)
-        ws.stop_words = overlapping_stopwords
-        return ws
-
-
-class StopWordsHindi(StopWords):
-    """Hindi segmentation"""
-
-    def __init__(self, language="hi"):
-        super(StopWordsHindi, self).__init__(language="hi")
-
-    def get_stopword_count(self, content):
-        if not content:
-            return WordStats()
-        ws = WordStats()
-        stripped_input = self.remove_punctuation(content)
-        candidate_words = self.candidate_words(stripped_input)
-        overlapping_stopwords = []
-        c = 0
-        for w in candidate_words:
-            c += 1
-            for stop_word in self.STOP_WORDS:
-                overlapping_stopwords.append(stop_word)
-
-        ws.word_count = c
-        ws.stop_word_count = len(overlapping_stopwords)
-        ws.stop_words = overlapping_stopwords
-        return ws
-
-
-class StopWordsJapanese(StopWords):
-    """Japanese segmentation"""
-
-    def __init__(self, language="ja"):
-        super(StopWordsJapanese, self).__init__(language="ja")
-
-    def candidate_words(self, stripped_input):
-        import tinysegmenter
-
-        segmenter = tinysegmenter.TinySegmenter()
-        tokens = segmenter.tokenize(stripped_input)
-        return tokens
-
-
-class StopWordsThai(StopWords):
-    """Thai segmentation"""
-
-    def __init__(self, language="th"):
-        super(StopWordsThai, self).__init__(language="th")
-
-    def candidate_words(self, stripped_input):
-        import pythainlp
-
-        tokens = pythainlp.word_tokenize(stripped_input)
-        return tokens
+# -*- coding: utf-8 -*-
+# Much of the code here was forked from https://github.com/codelucas/newspaper
+# Copyright (c) Lucas Ou-Yang (codelucas)
+
+"""
+Stopword extraction and stopword classes.
+"""
+
+from dataclasses import dataclass, field
+from pathlib import Path
+import re
+import string
+from typing import Dict, List
+
+
+from .utils import FileHelper
+
+
+def innerTrim(value):
+    if isinstance(value, str):
+        # remove tab and white space
+        value = re.sub(r"[\s\t]+", " ", value)
+        value = "".join(value.splitlines())
+        return value.strip()
+    return ""
+
+
+@dataclass
+class WordStats:
+    """Holds the number of stop words and total words in an article"""
+
+    stop_word_count: int = 0
+    word_count: int = 0
+    stop_words: List[str] = field(default_factory=list)
+
+
+class StopWords:
+    TRANS_TABLE = str.maketrans("", "")
+    _cached_stop_words: Dict[str, str] = {}
+
+    def __init__(self, language="en"):
+        if language not in self._cached_stop_words:
+            stopwordsFile = Path(STOPWORDS_DIR) / f"stopwords-{language}.txt"
+            self._cached_stop_words[language] = set(
+                FileHelper.loadResourceFile(stopwordsFile).splitlines()
+            )
+        self.STOP_WORDS = self._cached_stop_words[language]
+
+    def remove_punctuation(self, content):
+        # code taken form
+        # http://stackoverflow.com/questions/265960/best-way-to-strip-punctuation-from-a-string-in-python
+        content_is_unicode = isinstance(content, str)
+        if content_is_unicode:
+            content = content.encode("utf-8")
+        trans_table = {ord(c): None for c in string.punctuation}
+        stripped_input = content.decode("utf-8").translate(trans_table)
+
+        return stripped_input
+
+    def candidate_words(self, stripped_input):
+        return stripped_input.split(" ")
+
+    def get_stopword_count(self, content):
+        if not content:
+            return WordStats()
+        ws = WordStats()
+        stripped_input = self.remove_punctuation(content)
+        candidate_words = self.candidate_words(stripped_input.lower())
+        overlapping_stopwords = []
+        c = 0
+        for w in candidate_words:
+            c += 1
+            if w in self.STOP_WORDS:
+                overlapping_stopwords.append(w)
+
+        ws.word_count = c
+        ws.stop_word_count = len(overlapping_stopwords)
+        ws.stop_words = overlapping_stopwords
+        return ws
+
+
+class StopWordsChinese(StopWords):
+    """Chinese segmentation"""
+
+    def __init__(self, language="zh"):
+        super(StopWordsChinese, self).__init__(language="zh")
+
+    def candidate_words(self, stripped_input):
+        # jieba builds a tree that takes a while. avoid building
+        # this tree if we don't use the chinese language
+        import jieba
+
+        return jieba.cut(stripped_input, cut_all=True)
+
+
+class StopWordsArabic(StopWords):
+    """Arabic segmentation"""
+
+    def __init__(self, language="ar"):
+        # force ar language code
+        super(StopWordsArabic, self).__init__(language="ar")
+
+    def remove_punctuation(self, content):
+        return content
+
+    def candidate_words(self, stripped_input):
+        import nltk
+
+        s = nltk.stem.isri.ISRIStemmer()
+        words = []
+        for word in nltk.tokenize.wordpunct_tokenize(stripped_input):
+            words.append(s.stem(word))
+        return words
+
+
+class StopWordsKorean(StopWords):
+    """Korean segmentation"""
+
+    def __init__(self, language="ko"):
+        super(StopWordsKorean, self).__init__(language="ko")
+
+    def get_stopword_count(self, content):
+        if not content:
+            return WordStats()
+        ws = WordStats()
+        stripped_input = self.remove_punctuation(content)
+        candidate_words = self.candidate_words(stripped_input)
+        overlapping_stopwords = []
+        c = 0
+        for w in candidate_words:
+            c += 1
+            for s in self.STOP_WORDS:
+                if w.endswith(s):
+                    overlapping_stopwords.append(w)
+
+        ws.word_count = c
+        ws.stop_word_count = len(overlapping_stopwords)
+        ws.stop_words = overlapping_stopwords
+        return ws
+
+
+class StopWordsHindi(StopWords):
+    """Hindi segmentation"""
+
+    def __init__(self, language="hi"):
+        super(StopWordsHindi, self).__init__(language="hi")
+
+    def get_stopword_count(self, content):
+        if not content:
+            return WordStats()
+        ws = WordStats()
+        stripped_input = self.remove_punctuation(content)
+        candidate_words = self.candidate_words(stripped_input)
+        overlapping_stopwords = []
+        c = 0
+        for w in candidate_words:
+            c += 1
+            for stop_word in self.STOP_WORDS:
+                overlapping_stopwords.append(stop_word)
+
+        ws.word_count = c
+        ws.stop_word_count = len(overlapping_stopwords)
+        ws.stop_words = overlapping_stopwords
+        return ws
+
+
+class StopWordsJapanese(StopWords):
+    """Japanese segmentation"""
+
+    def __init__(self, language="ja"):
+        super(StopWordsJapanese, self).__init__(language="ja")
+
+    def candidate_words(self, stripped_input):
+        import tinysegmenter
+
+        segmenter = tinysegmenter.TinySegmenter()
+        tokens = segmenter.tokenize(stripped_input)
+        return tokens
+
+
+class StopWordsThai(StopWords):
+    """Thai segmentation"""
+
+    def __init__(self, language="th"):
+        super(StopWordsThai, self).__init__(language="th")
+
+    def candidate_words(self, stripped_input):
+        import pythainlp
+
+        tokens = pythainlp.word_tokenize(stripped_input)
+        return tokens
```

### Comparing `xgne-0.0.8/xgne/utils.py` & `xgne-0.0.9/xgne/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-import codecs
-import logging
-import os
-import re
-import yaml
-import unicodedata
-from lxml.html import fromstring, HtmlElement
-from lxml.html import etree
-from urllib.parse import urlparse, urljoin
-from http.cookiejar import CookieJar as cj
-
-from .version import __version__
-
-from .defaults import USELESS_TAG, TAGS_CAN_BE_REMOVE_IF_EMPTY, USELESS_ATTR, HIGH_WEIGHT_ARRT_KEYWORD, ALLOWED_TYPES
-
-log = logging.getLogger(__name__)
-log.setLevel(logging.DEBUG)
-
-
-def normalize_node(element: HtmlElement):
-    etree.strip_elements(element, *USELESS_TAG)
-    for node in iter_node(element):
-        # inspired by readability.
-        if node.tag.lower() in TAGS_CAN_BE_REMOVE_IF_EMPTY and is_empty_element(node):
-            remove_node(node)
-
-        # merge text in span or strong to parent p tag
-        if node.tag.lower() == 'p':
-            etree.strip_tags(node, 'span')
-            etree.strip_tags(node, 'strong')
-
-        # if a div tag does not contain any sub node, it could be converted to p node.
-        if node.tag.lower() == 'div' and not node.getchildren():
-            node.tag = 'p'
-
-        if node.tag.lower() == 'span' and not node.getchildren():
-            node.tag = 'p'
-
-        # remove empty p tag
-        if node.tag.lower() == 'p' and not node.xpath('.//img'):
-            if not (node.text and node.text.strip()):
-                drop_tag(node)
-
-        class_name = node.get('class')
-        if class_name:
-            if class_name in USELESS_ATTR:
-                remove_node(node)
-                break
-
-
-def html2element(html):
-    html = re.sub('</?br.*?>', '', html)
-    element = fromstring(html)
-    return element
-
-
-def pre_parse(element):
-    normalize_node(element)
-
-    return element
-
-
-def remove_noise_node(element, noise_xpath_list):
-    noise_xpath_list = noise_xpath_list or config.get('noise_node_list')
-    if not noise_xpath_list:
-        return
-    for noise_xpath in noise_xpath_list:
-        nodes = element.xpath(noise_xpath)
-        for node in nodes:
-            remove_node(node)
-    return element
-
-
-def iter_node(element: HtmlElement):
-    yield element
-    for sub_element in element:
-        if isinstance(sub_element, HtmlElement):
-            yield from iter_node(sub_element)
-
-
-def remove_node(node: HtmlElement):
-    """
-    this is a in-place operation, not necessary to return
-    :param node:
-    :return:
-    """
-    parent = node.getparent()
-    if parent is not None:
-        parent.remove(node)
-
-
-def drop_tag(node: HtmlElement):
-    """
-    only delete the tag, but merge its text to parent.
-    :param node:
-    :return:
-    """
-    parent = node.getparent()
-    if parent is not None:
-        node.drop_tag()
-
-
-def is_empty_element(node: HtmlElement):
-    return not node.getchildren() and not node.text
-
-
-def pad_host_for_images(host, url):
-    """
-    网站上的图片可能有如下几种格式：
-
-    完整的绝对路径：https://xxx.com/1.jpg
-    完全不含 host 的相对路径： /1.jpg
-    含 host 但是不含 scheme:  xxx.com/1.jpg 或者  ://xxx.com/1.jpg
-
-    :param host:
-    :param url:
-    :return:
-    """
-    if url.startswith('http'):
-        return url
-    parsed_uri = urlparse(host)
-    scheme = parsed_uri.scheme
-    if url.startswith(':'):
-        return f'{scheme}{url}'
-    if url.startswith('//'):
-        return f'{scheme}:{url}'
-    return urljoin(host, url)
-
-
-def read_config():
-    if os.path.exists('.xgne'):
-        with open('.xgne', encoding='utf-8') as f:
-            config_text = f.read()
-        config = yaml.safe_load(config_text)
-        return config
-    return {}
-
-
-def get_high_weight_keyword_pattern():
-    return re.compile('|'.join(HIGH_WEIGHT_ARRT_KEYWORD), flags=re.I)
-
-
-def get_longest_common_sub_string(str1: str, str2: str) -> str:
-    """
-    获取两个字符串的最长公共子串。
-
-    构造一个矩阵，横向是字符串1，纵向是字符串2，例如：
-
-      BL是天才！？
-    听0 0 0 0 00 0
-    说0 0 0 0 00 0
-    B1 0 0 0 00 0
-    L0 1 0 0 00 0
-    是0 0 1 0 00 0
-    天0 0 0 1 00 0
-    才0 0 0 0 10 0
-    ！0 0 0 0 01 0
-
-    显然，只要斜对角线最长的就是最长公共子串
-
-    :param str1: 第一个字符串
-    :param str2: 第二个字符串
-    :return: 最长公共子串
-    """
-    if not all([str1, str2]):
-        return ''
-
-    # 构造一个矩阵，横向是字符串1，纵向是字符串2
-    matrix = [[0] * (len(str2) + 1) for _ in range(len(str1) + 1)]
-    max_length = 0
-    start_position = 0
-
-    for index_of_str1 in range(1, len(str1) + 1):
-        for index_of_str2 in range(1, len(str2) + 1):
-            if str1[index_of_str1 - 1] == str2[index_of_str2 - 1]:
-                matrix[index_of_str1][index_of_str2] = matrix[index_of_str1 - 1][index_of_str2 - 1] + 1
-                if matrix[index_of_str1][index_of_str2] > max_length:
-                    max_length = matrix[index_of_str1][index_of_str2]
-                    start_position = index_of_str1 - max_length
-            else:
-                matrix[index_of_str1][index_of_str2] = 0
-
-    return str1[start_position: start_position + max_length]
-
-
-def normalize_text(html):
-    """
-    使用 NFKC 对网页源代码进行归一化，把特殊符号转换为普通符号
-    :param html:
-    :return:
-    """
-    return unicodedata.normalize('NFKC', html)
-
-
-def urljoin_if_valid(base_url: str, url: str) -> str:
-    """拼接基本URL和可能是相对URL的地址，防止由于解析导致的无效URL。
-
-    Args:
-        base_url (str): 基本URL（即文章的URL）
-        url (str): 相对或绝对URL
-
-    Returns:
-        str: 如果有效则返回拼接的URL，否则返回空字符串
-    """
-
-    try:
-        res = urljoin(base_url, url)
-        return res
-    except ValueError:
-        return ""
-
-
-def url_to_filetype(abs_url: str) -> None:
-    """
-    输入一个URL，输出由URL指定的文件的文件类型。对于没有文件类型的情况，返回None。
-    'http://blahblah/images/car.jpg' -> 'jpg'
-    'http://yahoo.com'               -> None
-    """
-    path = urlparse(abs_url).path.rstrip('/')
-    path_chunks = [x for x in path.split("/") if x]
-    last_chunk = path_chunks[-1].split('.')  # 最后一块通常是文件
-    if len(last_chunk) < 2:
-        return None
-    file_type = last_chunk[-1]
-    # 假设文件扩展名最多为5个字符长
-    return file_type.lower() if len(file_type) <= 5 or file_type.lower() in ALLOWED_TYPES else None
-
-
-def get_requests_params():
-    '''
-    获取请求头的参数
-    :return:
-    '''
-    return {
-        "timeout": 7,
-        "proxies": {},
-        "headers": {
-            "User-Agent": f"xgne/{__version__}",
-        },
-        "cookies": cj(),
-    }
-
-
-# 通用文本过滤
-def universal_filter(text):
-    if text:
-        # \u1234
-        text = text.replace(u'\u200b', '')
-        text = text.replace(u'\u2002', '')
-        text = text.replace(u'\u3000', '')
-        text = text.replace(u'\ufeff', '')
-        # \x??
-        text = text.replace(u'\xa0', '')
-        text = text.replace(u'\x7f', '')
-        # &??
-        text = text.replace('&nbsp', ' ')
-        text = text.replace('&ldquo;', '"')
-        text = text.replace('&rdquo;', '"')
-        text = text.replace('&bull;', '•')
-        text = text.replace('&mdash;', '—')
-        text = text.replace('&lsquo;', "'")
-        text = text.replace('&rsquo;', "'")
-        text = text.replace('&hellip;', '…')
-        text = text.replace('&middot;', '·')
-        text = text.replace('&quot;', '"')
-        text = text.replace('&amp;', '&')
-        text = text.replace('&#39;', "'")
-        text = text.replace('&deg;', "°")
-        text = text.replace('&times;', "×")
-        text = text.replace('&beta;', "β")
-        text = text.replace('&ndash;', "–")
-        # \n, \r, \t
-        text = text.replace('\n', '')
-        text = text.replace('\r', '')
-        text = text.replace('\t', '')
-        # '  ?  '
-        text = text.strip()
-    return text
-
-
-class FileHelper(object):
-    @staticmethod
-    def loadResourceFile(filename):
-        if not os.path.isabs(filename):
-            dirpath = os.path.abspath(os.path.dirname(__file__))
-            path = os.path.join(dirpath, 'resources', filename)
-        else:
-            path = filename
-        try:
-            f = codecs.open(path, 'r', 'utf-8')
-            content = f.read()
-            f.close()
-            return content
-        except IOError:
-            raise IOError("Couldn't open file %s" % path)
-
-
-config = read_config()
+import codecs
+import logging
+import os
+import re
+import yaml
+import unicodedata
+from lxml.html import fromstring, HtmlElement
+from lxml.html import etree
+from urllib.parse import urlparse, urljoin
+from http.cookiejar import CookieJar as cj
+
+from .version import __version__
+
+from .defaults import USELESS_TAG, TAGS_CAN_BE_REMOVE_IF_EMPTY, USELESS_ATTR, HIGH_WEIGHT_ARRT_KEYWORD, ALLOWED_TYPES
+
+log = logging.getLogger(__name__)
+log.setLevel(logging.DEBUG)
+
+
+def normalize_node(element: HtmlElement):
+    etree.strip_elements(element, *USELESS_TAG)
+    for node in iter_node(element):
+        # inspired by readability.
+        if node.tag.lower() in TAGS_CAN_BE_REMOVE_IF_EMPTY and is_empty_element(node):
+            remove_node(node)
+
+        # merge text in span or strong to parent p tag
+        if node.tag.lower() == 'p':
+            etree.strip_tags(node, 'span')
+            etree.strip_tags(node, 'strong')
+
+        # if a div tag does not contain any sub node, it could be converted to p node.
+        if node.tag.lower() == 'div' and not node.getchildren():
+            node.tag = 'p'
+
+        if node.tag.lower() == 'span' and not node.getchildren():
+            node.tag = 'p'
+
+        # remove empty p tag
+        if node.tag.lower() == 'p' and not node.xpath('.//img'):
+            if not (node.text and node.text.strip()):
+                drop_tag(node)
+
+        class_name = node.get('class')
+        if class_name:
+            if class_name in USELESS_ATTR:
+                remove_node(node)
+                break
+
+
+def html2element(html):
+    html = re.sub('</?br.*?>', '', html)
+    element = fromstring(html)
+    return element
+
+
+def pre_parse(element):
+    normalize_node(element)
+
+    return element
+
+
+def remove_noise_node(element, noise_xpath_list):
+    noise_xpath_list = noise_xpath_list or config.get('noise_node_list')
+    if not noise_xpath_list:
+        return
+    for noise_xpath in noise_xpath_list:
+        nodes = element.xpath(noise_xpath)
+        for node in nodes:
+            remove_node(node)
+    return element
+
+
+def iter_node(element: HtmlElement):
+    yield element
+    for sub_element in element:
+        if isinstance(sub_element, HtmlElement):
+            yield from iter_node(sub_element)
+
+
+def remove_node(node: HtmlElement):
+    """
+    this is a in-place operation, not necessary to return
+    :param node:
+    :return:
+    """
+    parent = node.getparent()
+    if parent is not None:
+        parent.remove(node)
+
+
+def drop_tag(node: HtmlElement):
+    """
+    only delete the tag, but merge its text to parent.
+    :param node:
+    :return:
+    """
+    parent = node.getparent()
+    if parent is not None:
+        node.drop_tag()
+
+
+def is_empty_element(node: HtmlElement):
+    return not node.getchildren() and not node.text
+
+
+def pad_host_for_images(host, url):
+    """
+    网站上的图片可能有如下几种格式：
+
+    完整的绝对路径：https://xxx.com/1.jpg
+    完全不含 host 的相对路径： /1.jpg
+    含 host 但是不含 scheme:  xxx.com/1.jpg 或者  ://xxx.com/1.jpg
+
+    :param host:
+    :param url:
+    :return:
+    """
+    if url.startswith('http'):
+        return url
+    parsed_uri = urlparse(host)
+    scheme = parsed_uri.scheme
+    if url.startswith(':'):
+        return f'{scheme}{url}'
+    if url.startswith('//'):
+        return f'{scheme}:{url}'
+    return urljoin(host, url)
+
+
+def read_config():
+    if os.path.exists('.xgne'):
+        with open('.xgne', encoding='utf-8') as f:
+            config_text = f.read()
+        config = yaml.safe_load(config_text)
+        return config
+    return {}
+
+
+def get_high_weight_keyword_pattern():
+    return re.compile('|'.join(HIGH_WEIGHT_ARRT_KEYWORD), flags=re.I)
+
+
+def get_longest_common_sub_string(str1: str, str2: str) -> str:
+    """
+    获取两个字符串的最长公共子串。
+
+    构造一个矩阵，横向是字符串1，纵向是字符串2，例如：
+
+      BL是天才！？
+    听0 0 0 0 00 0
+    说0 0 0 0 00 0
+    B1 0 0 0 00 0
+    L0 1 0 0 00 0
+    是0 0 1 0 00 0
+    天0 0 0 1 00 0
+    才0 0 0 0 10 0
+    ！0 0 0 0 01 0
+
+    显然，只要斜对角线最长的就是最长公共子串
+
+    :param str1: 第一个字符串
+    :param str2: 第二个字符串
+    :return: 最长公共子串
+    """
+    if not all([str1, str2]):
+        return ''
+
+    # 构造一个矩阵，横向是字符串1，纵向是字符串2
+    matrix = [[0] * (len(str2) + 1) for _ in range(len(str1) + 1)]
+    max_length = 0
+    start_position = 0
+
+    for index_of_str1 in range(1, len(str1) + 1):
+        for index_of_str2 in range(1, len(str2) + 1):
+            if str1[index_of_str1 - 1] == str2[index_of_str2 - 1]:
+                matrix[index_of_str1][index_of_str2] = matrix[index_of_str1 - 1][index_of_str2 - 1] + 1
+                if matrix[index_of_str1][index_of_str2] > max_length:
+                    max_length = matrix[index_of_str1][index_of_str2]
+                    start_position = index_of_str1 - max_length
+            else:
+                matrix[index_of_str1][index_of_str2] = 0
+
+    return str1[start_position: start_position + max_length]
+
+
+def normalize_text(html):
+    """
+    使用 NFKC 对网页源代码进行归一化，把特殊符号转换为普通符号
+    :param html:
+    :return:
+    """
+    return unicodedata.normalize('NFKC', html)
+
+
+def urljoin_if_valid(base_url: str, url: str) -> str:
+    """拼接基本URL和可能是相对URL的地址，防止由于解析导致的无效URL。
+
+    Args:
+        base_url (str): 基本URL（即文章的URL）
+        url (str): 相对或绝对URL
+
+    Returns:
+        str: 如果有效则返回拼接的URL，否则返回空字符串
+    """
+
+    try:
+        res = urljoin(base_url, url)
+        return res
+    except ValueError:
+        return ""
+
+
+def url_to_filetype(abs_url: str) -> None:
+    """
+    输入一个URL，输出由URL指定的文件的文件类型。对于没有文件类型的情况，返回None。
+    'http://blahblah/images/car.jpg' -> 'jpg'
+    'http://yahoo.com'               -> None
+    """
+    path = urlparse(abs_url).path.rstrip('/')
+    path_chunks = [x for x in path.split("/") if x]
+    last_chunk = path_chunks[-1].split('.')  # 最后一块通常是文件
+    if len(last_chunk) < 2:
+        return None
+    file_type = last_chunk[-1]
+    # 假设文件扩展名最多为5个字符长
+    return file_type.lower() if len(file_type) <= 5 or file_type.lower() in ALLOWED_TYPES else None
+
+
+def get_requests_params():
+    '''
+    获取请求头的参数
+    :return:
+    '''
+    return {
+        "timeout": 7,
+        "proxies": {},
+        "headers": {
+            "User-Agent": f"xgne/{__version__}",
+        },
+        "cookies": cj(),
+    }
+
+
+# 通用文本过滤
+def universal_filter(text):
+    if text:
+        # \u1234
+        text = text.replace(u'\u200b', '')
+        text = text.replace(u'\u2002', '')
+        text = text.replace(u'\u3000', '')
+        text = text.replace(u'\ufeff', '')
+        # \x??
+        text = text.replace(u'\xa0', '')
+        text = text.replace(u'\x7f', '')
+        # &??
+        text = text.replace('&nbsp', ' ')
+        text = text.replace('&ldquo;', '"')
+        text = text.replace('&rdquo;', '"')
+        text = text.replace('&bull;', '•')
+        text = text.replace('&mdash;', '—')
+        text = text.replace('&lsquo;', "'")
+        text = text.replace('&rsquo;', "'")
+        text = text.replace('&hellip;', '…')
+        text = text.replace('&middot;', '·')
+        text = text.replace('&quot;', '"')
+        text = text.replace('&amp;', '&')
+        text = text.replace('&#39;', "'")
+        text = text.replace('&deg;', "°")
+        text = text.replace('&times;', "×")
+        text = text.replace('&beta;', "β")
+        text = text.replace('&ndash;', "–")
+        # \n, \r, \t
+        text = text.replace('\n', '')
+        text = text.replace('\r', '')
+        text = text.replace('\t', '')
+        # '  ?  '
+        text = text.strip()
+    return text
+
+
+class FileHelper(object):
+    @staticmethod
+    def loadResourceFile(filename):
+        if not os.path.isabs(filename):
+            dirpath = os.path.abspath(os.path.dirname(__file__))
+            path = os.path.join(dirpath, 'resources', filename)
+        else:
+            path = filename
+        try:
+            f = codecs.open(path, 'r', 'utf-8')
+            content = f.read()
+            f.close()
+            return content
+        except IOError:
+            raise IOError("Couldn't open file %s" % path)
+
+
+config = read_config()
```

### Comparing `xgne-0.0.8/xgne.egg-info/SOURCES.txt` & `xgne-0.0.9/xgne.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 xgne/dom/DomHandler.py
 xgne/dom/__init__.py
 xgne/extractor/ArticleBodyExtractor.py
 xgne/extractor/AuthorExtractor.py
 xgne/extractor/ContentExtractor.py
 xgne/extractor/HeadMetaExtractor.py
 xgne/extractor/ImageExtractor.py
+xgne/extractor/InformationExtractor.py
 xgne/extractor/LangExtractor.py
 xgne/extractor/ListExtractor.py
 xgne/extractor/TimeExtractor.py
 xgne/extractor/TitleExtractor.py
 xgne/extractor/__init__.py
```

