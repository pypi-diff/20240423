# Comparing `tmp/dmk_packages-0.6.4.tar.gz` & `tmp/dmk_packages-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.4.tar", last modified: Fri Apr 19 05:39:02 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.5.tar", last modified: Tue Apr 23 05:17:44 2024, max compression
```

## Comparing `dmk_packages-0.6.4.tar` & `dmk_packages-0.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.925508 dmk_packages-0.6.4/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-19 05:39:02.924895 dmk_packages-0.6.4/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-04-19 05:35:31.000000 dmk_packages-0.6.4/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-04-19 05:39:02.925616 dmk_packages-0.6.4/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.913126 dmk_packages-0.6.4/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.915662 dmk_packages-0.6.4/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.922439 dmk_packages-0.6.4/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     6713 2024-04-19 04:48:18.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 layla      (501) staff       (20)     6383 2024-04-19 05:21:54.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 layla      (501) staff       (20)     6418 2024-04-19 04:48:18.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 layla      (501) staff       (20)     2743 2024-04-19 04:48:18.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/fnguide_pdf_update.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-15 02:00:30.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)    13362 2024-04-19 05:37:30.000000 dmk_packages-0.6.4/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.923376 dmk_packages-0.6.4/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.6.4/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.6.4/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-19 05:39:02.924430 dmk_packages-0.6.4/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-19 05:39:02.000000 dmk_packages-0.6.4/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      684 2024-04-19 05:39:02.000000 dmk_packages-0.6.4/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-04-19 05:39:02.000000 dmk_packages-0.6.4/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-04-19 05:39:02.000000 dmk_packages-0.6.4/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-04-19 05:39:02.000000 dmk_packages-0.6.4/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.569694 dmk_packages-0.6.5/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-23 05:17:44.569427 dmk_packages-0.6.5/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-23 05:15:23.000000 dmk_packages-0.6.5/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-23 05:17:44.569752 dmk_packages-0.6.5/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.563577 dmk_packages-0.6.5/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.564953 dmk_packages-0.6.5/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.568125 dmk_packages-0.6.5/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-23 05:13:00.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6578 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6600 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-23 05:13:33.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.5/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.568713 dmk_packages-0.6.5/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.5/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-23 05:17:44.569117 dmk_packages-0.6.5/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      677 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-23 05:17:44.000000 dmk_packages-0.6.5/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.4/LICENSE` & `dmk_packages-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/PKG-INFO` & `dmk_packages-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.4
+Version: 0.6.5
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.4/README.md` & `dmk_packages-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/pyproject.toml` & `dmk_packages-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.4"
+version = "0.6.5"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/fnguide.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,167 +1,172 @@
 import os
-import pandas as pd
-from datetime import datetime
-
-from playwright.async_api import async_playwright
 import asyncio
-
-from dmk_packages.database import database as dbs
+import pendulum
 from loguru import logger
+from playwright.async_api import (
+    async_playwright,
+    TimeoutError as PlaywrightTimeoutError,
+)
+from dotenv import load_dotenv, find_dotenv
 
+"""
+## fnguide 크롤러 ##
+- 사용 유의사항
+해당 크롤러는 가져올 데이터는 일정하지만 카테고리가 상당히 많기때문에(서브카테고리 포함) 필요한 카테고리 elements를 매개변수로 지정
+ex. click_cat = (f'//*[@id="resultDivTabs"]/ul/li/button[contains(text(), "{cat}")]')
 
-class BigkindsCrawler:
-    def __init__(self, headless=False, download_path=None, start_date=None, end_date=None):
-        # playwright
-        self.browser = None
-        self.headless = headless
-        # 다운로드 경로
-        self.download_path = download_path
-
-        # 날짜설정
-        self.start_date = start_date
-        self.end_date = end_date
-        self.crawl_date = datetime.now()
+download경로를 None으로 설정할시 pdf파일은 다운로드 하지 않음
 
-    async def set_browser(self):
-        """
-        playwright 설정
-        """
+- 사용 : run_fnguide_crawler(카테고리, clickelements, download_path, view)
+"""
+load_dotenv(dotenv_path=find_dotenv())
+
+
+class FnguideCrawler:
+    DEFAULT_DT = pendulum.yesterday(tz=pendulum.timezone("Asia/Seoul"))
+
+    def __init__(self, date_from=None, date_until=None, login=None):
+
+        _date_from = pendulum.parse(date_from) if date_from else self.DEFAULT_DT
+        _date_until = pendulum.parse(date_until) if date_until else self.DEFAULT_DT
+        self._date_from = _date_from.to_date_string()
+        self._date_until = _date_until.to_date_string()
+
+        self.login_id = os.environ.get(f"{login}_LOGIN_ID")
+        self.login_pw = os.environ.get(f"{login}_LOGIN_PW")
+        if None in (self.login_id, self.login_pw):
+            raise Exception("check your login in .env")
+
+        # 다운로드 에러가 가는 url 리스트
+        self.url_e = []
+
+    async def _start_playwright(self, view=True):
         self.playwright = await async_playwright().start()
         self.browser = await self.playwright.chromium.launch(
-            headless=True  # 창 띄울지 말지 결정
+            headless=view  # 창띄울지 말지 결정
         )
         self.context = await self.browser.new_context(accept_downloads=True)
         self.page = await self.context.new_page()
         return self
 
-    async def playwright_crawling(self, cat):
+    async def _stop_playwright(self):
+        await self.context.close()
+        await self.browser.close()
+        await self.playwright.stop()
+
+    async def _set_login_date(self):
         """
-        사이트 접속 및 로그인, 검색창에 들어가 기간설정 및 카테고리 설정
+        사이트 접속후 로그인 및 기간설정
         """
-        try:
-            # 사이트 접속
-            url = "https://www.bigkinds.or.kr/v2/news/index.do"
-            await self.page.goto(url, wait_until="load")
-            await asyncio.sleep(2)
-
-            # 로그인
-            login_id = "scarlett@datamarketing.co.kr"
-            login_pw = "dmk1234!"
-            await self.page.get_by_role("button", name="로그인").click()
-            await asyncio.sleep(0.5)
-            await self.page.get_by_placeholder("이메일(E-mail) 주소").fill(login_id)
-            await asyncio.sleep(0.3)
-            await self.page.get_by_placeholder("비밀번호를 입력하세요.").fill(login_pw)
-            await asyncio.sleep(0.3)
-            await self.page.click("#login-btn")
-            await asyncio.sleep(2)
-            await self.page.wait_for_selector(
-                ".ft-map > div > div > ul > li > a", state="visible"
-            )
-            await self.page.click(".ft-map > div > div > ul > li > a")
-            await asyncio.sleep(2)
-            await self.page.click(".tab-btn")
-            await asyncio.sleep(0.5)
-
-            # 기간설정하기
-            date_s = await self.page.query_selector("#search-begin-date")
-            date_e = await self.page.query_selector("#search-end-date")
-            await date_s.fill(self.start_date)
-            await asyncio.sleep(0.3)
-            await date_e.fill(self.end_date)
-            await asyncio.sleep(0.3)
-
-            # 해당되는 카테고리 설정
-            await self.page.click(".tab-btn.tab3")
-            await asyncio.sleep(0.3)
-            set_cat = await self.page.query_selector(
-                f"xpath=.//span[@data-role='display' and text()='{cat}']"
-            )
-            await set_cat.click()
-            await asyncio.sleep(0.3)
-            await self.page.get_by_role("button", name="적용하기").click()
-            await asyncio.sleep(2)
-
-            # STEP 03 버튼 누르기
-            await self.page.get_by_role("button", name="분석 결과 및 시각화").click()
-            await asyncio.sleep(1)
-
-        except Exception as e:
-            logger.error(f"playwright 크롤링오류 | error_comment : {e}")
-
-    async def download_save_data(self, cat):
-        """
-        카테고리에 맞는 엑셀 저장 후 데이터변환하여 디비 적재
-        """
-        try:
-            # 엑셀 저장
-            async with self.page.expect_download() as download_info:
-                await self.page.get_by_role("button", name="엑셀 다운로드").click()
-            download = await download_info.value
-            await download.save_as(self.download_path + download.suggested_filename)
-
-            # 파일이름 변경
-            old_filename = os.path.join(
-                self.download_path,
-                f"NewsResult_{self.start_date.replace('-', '')}-{self.end_date.replace('-', '')}.xlsx",
-            )
-            new_filename = os.path.join(
-                self.download_path,
-                f"NewsResult_{self.start_date.replace('-', '')}-{self.end_date.replace('-', '')}_{cat}.xlsx",
-            )
-            os.rename(old_filename, new_filename)
-
-            # 엑셀파일 data_list 변환
-            data_list = []
-            if new_filename:
-                df = pd.read_excel(new_filename)
-                df = df.fillna("")
-                for i in df.index:
-                    data = {
-                        "channel_name": "Big Kinds",
-                        "category_name": cat,
-                        "identifier": str(df["뉴스 식별자"][i]),
-                        "regist_date": str(df["일자"][i]),
-                        "press_name": df["언론사"][i],
-                        "writer": df["기고자"][i],
-                        "title": df["제목"][i],
-                        "category_1": df["통합 분류1"][i],
-                        "category_2": df["통합 분류2"][i],
-                        "category_3": df["통합 분류3"][i],
-                        "incident_1": df["사건/사고 분류1"][i],
-                        "incident_2": df["사건/사고 분류2"][i],
-                        "incident_3": df["사건/사고 분류3"][i],
-                        "person": df["인물"][i],
-                        "location": df["위치"][i],
-                        "organization": df["기관"][i],
-                        "keyword": df["키워드"][i],
-                        "top50_keyword": df["특성추출(가중치순 상위 50개)"][i],
-                        "contents": df["본문"][i],
-                        "url": df["URL"][i],
-                        "except": df["분석제외 여부"][i],
-                        "created_at": self.crawl_date,
-                    }
-                    data_list.append(data)
-            return data_list
-        except Exception as e:
-            logger.error(f"데이터 저장 or 변환 실패 | error_comment : {e}")
-
-    async def bigkinds_crawl(self, cat):
-        """
-        playwright 크롤러 전반적인 운영
-        """
-        # playwright 실행 및 크롤링
-        logger.info(f"[{cat}] 크롤링 시작")
-        await self.set_browser()
-        await self.playwright_crawling(cat)
-        await asyncio.sleep(1)
 
-        # 파일 저장 및 적재
-        data = await self.download_save_data(cat)
+        # 로그인
+        url_fnguide = "https://www.fnguide.com/"
+        await self.page.goto(url_fnguide, wait_until="load")
+        await asyncio.sleep(2)
+
+        await self.page.fill('input[name="MemberID"]', self.login_id)
+        await self.page.fill('input[name="PassWord"]', self.login_pw)
+        await self.page.click(".btn--login")
+        await asyncio.sleep(2)
+
+        # fnresearch 들어가서 기간설정 후 검색
+        await self.page.click(".gnb--1dep > .p1")
+        await asyncio.sleep(2)
+
+        await self.page.fill("#frDate", self._date_from)
+        await self.page.fill("#toDate", self._date_until)
+        await self.page.locator("#srchBtn").click()
         await asyncio.sleep(0.5)
 
-        # 브라우저 종료
-        await self.context.close()
-        await self.browser.close()
-        await self.playwright.stop()
+    async def _crawling_fnguide(self, cat, click_cat, download_path):
+        """
+        해당 카테고리 클릭후 크롤링 및 PDF파일 다운로드
+        """
+        # 카테고리 클릭
+        await self.page.click(click_cat)
+        await asyncio.sleep(0.5)
+
+        data_list = []
+        while True:
+            # 검색결과가 없는 경우
+            table = await self.page.query_selector("#resultDivGrid")
+            if await table.query_selector(".nodata"):
+                break
+
+            rows = await table.query_selector_all("tbody > tr")
+            for row in rows:
+                tds = await row.query_selector_all("td")
+                regist_date = await tds[0].inner_text()
+                category_name = cat
+                title = await tds[1].inner_text()
+                provider = await tds[4].inner_text()
+                writer = await tds[3].inner_text()
+                url_tag = await tds[1].eval_on_selector(
+                    "a", 'element => element.getAttribute("href")'
+                )
+                url = f"https://www.fnguide.com{url_tag}"
+
+                # 찾은 데이터 list에 append
+                data = {
+                    "channel_name": "Fnguide",
+                    "category_name": category_name,
+                    "regist_date": regist_date,
+                    "title": title,
+                    "writer": writer,
+                    "provider": provider,
+                    "url": url,
+                }
+                data_list.append(data)
+
+                # pdf 다운로드
+                try:
+                    if download_path is None:
+                        continue
+
+                    # 이미 다운로드 되어있는 파일 목록
+                    url_idx = url.split("bulletkind=")[-1]
+                    filename = f"{url_idx}_{regist_date}.pdf"
+
+                    os.chdir(download_path)
+                    file_list = os.listdir()
+
+                    # 오류나는 파일과 이미 다운로드가 되어있다면 패스 아니라면 다운로드 진행
+                    if (url_tag not in self.url_e) and (filename not in file_list):
+                        async with self.page.expect_download(
+                            timeout=15000
+                        ) as download_info:
+                            pdf = await row.query_selector(".btn--get")
+                            await pdf.click()
+
+                        download = await download_info.value
+                        await download.save_as(download_path + filename)
+                        await asyncio.sleep(0.5)
+
+                except PlaywrightTimeoutError:
+                    # 오류난 파일의 url_tag 추가
+                    logger.error(f"[{cat}][{regist_date}][{title}] download error")
+                    self.url_e.append(url_tag)
+
+                    # 다시 실행
+                    logger.info(f"[{cat}] rerun")
+                    await self._stop_playwright
+                    await self.run_fnguide_crawler_async(cat, click_cat, download_path)
+
+            # 반목문 중단 or 다음 페이지
+            try:
+                await self.page.click(".paging > .btn--next", timeout=1000)
+                await asyncio.sleep(0.5)
+
+            except PlaywrightTimeoutError:
+                break
+
+        return data_list
+
+    async def run_fnguide_crawler_async(self, cat, click_cat, download_path, view=True):
+        """
+        fnguide 크롤러 전체적인 실행후 데이터 반환
+        """
+        await self._start_playwright(view)
+        await self._set_login_date()
+        data = await self._crawling_fnguide(cat, click_cat, download_path)
+        await self._stop_playwright()
         return data
```

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/clien.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,30 +21,31 @@
                 keyword, category = target
 
 - 사용 순서
 check_borad_sn > start_beautifulsoup > crawling_posts > check_next_page > crawling_post_detail_list
 > 디비 적재 > 페이지가 더 있다면 처음부터 다시 시작(페이지 추가)
 
 """
-tz = pendulum.timezone("Asia/Seoul")
 
 
 class ClienCrawler:
-    def __init__(self, date_from, date_until):
-        DEFAULT_DT = pendulum.yesterday(tz=tz)
+    DEFAULT_DT = pendulum.yesterday(tz=pendulum.timezone("Asia/Seoul"))
+
+    def __init__(self, date_from=None, date_until=None):
 
         self._user_agent = UserAgent(min_percentage=1.1, os=["windows", "macos"])
         self._session = requests.session()
         self._max_board_sn = 0
         self._min_board_sn = 0
         self._base_url = "https://www.clien.net"
 
-        self._date_from = pendulum.parse(date_from) if date_from else DEFAULT_DT
-        _date_until = pendulum.parse(date_until) if date_until else DEFAULT_DT
-        self._date_until = _date_until.strftime("%Y-%m-%d 23:59:59")
+        self._date_from = pendulum.parse(date_from) if date_from else self.DEFAULT_DT
+        _date_until = pendulum.parse(date_until) if date_until else self.DEFAULT_DT
+        _date_until = _date_until.strftime("%Y-%m-%d 23:59:59")
+        self._date_until = pendulum.parse(_date_until)
 
     def check_board_sn(self, keyword, category, table, engine):
         """
         keyword 및 category에 해당하는 board_sn컬럼의 max, min 값을 가져오는 컬럼
         """
 
         metadata = MetaData()
@@ -88,48 +89,50 @@
         게시물들의 기본적인 내용 크롤링
         """
         items = soup.select(".list_item.symph_row.jirum")
         results = []
 
         for item in items:
             board_sn = int(item["data-board-sn"])
-            regist_date = pendulum.parse(item.select_one(".timestamp").text)
+            _regist_date = pendulum.parse(item.select_one(".timestamp").text)
+            regist_date = _regist_date.add(hours=9)
 
             title = item.select_one(".subject_fixed").text
             if "헤드라인 모음" in title:
                 continue
 
             if self._min_board_sn <= board_sn <= self._max_board_sn:
                 continue
 
-            if self._date_from < regist_date < pendulum.parse(self._date_until):
+            if self._date_from < regist_date < self._date_until:
                 comment = int(item["data-comment-count"])
                 url = self._base_url + item.select_one(".subject_fixed")["href"]
 
                 data = {
                     "category_name": category,
-                    "regist_date": regist_date,
+                    "regist_date": regist_date.to_iso8601_string(),
                     "comment": comment,
                     "url": url,
                     "keyword": keyword,
                     "board_sn": board_sn,
                 }
                 results.append(data)
         return results
 
     def check_next_page(self, soup: BeautifulSoup):
         pages = soup.select(".board-nav-page")
         if len(pages) <= 1:
             return None
         next_btn_exists = bool(soup.select_one(".board-nav-next"))
 
-        last_item = soup.select(".list_item")[-1]
-        last_item_timestamp = last_item.select_one(".timestamp").text
+        last_item = soup.select(".list_item.symph_row.jirum")[-1]
+        last_item_timestamp = pendulum.parse(last_item.select_one(".timestamp").text)
+        last_item_timestamp = last_item_timestamp.add(hours=9)
 
-        if self._date_from > pendulum.parse(last_item_timestamp):
+        if self._date_from > last_item_timestamp:
             return None
 
         for idx, page in enumerate(pages):
             if "active" in page.get("class", []):
                 if next_btn_exists or idx + 1 < len(pages):
                     return idx + 1
                 break
```

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/fnguide_pdf_update.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,48 @@
-import sys
 import os
-import shutil
+import pdftotext
 
-sys.path.append(os.path.dirname(os.path.abspath(os.path.dirname(__file__))))
+"""
+## PDF파일을 Text로 변환 ##
+- file_name, pdf_text, update_idx 딕셔너리들을 리스트로 반환
+디비 적재시 원하는 키값을 확인
+
+- update 쿼리 작성시 유의사항
+다운로드 파일 제일 앞에 where문으로 검색할 인덱스값을 붙어야함
+ex. (where문으로 컬럼에서 찾을 인덱스)_파일명.pdf
+"""
 
-import pandas as pd
-from datetime import datetime
-from tqdm import tqdm
-import pdftotext
-from loguru import logger
-from dmk_packages.database import database as dbs
-from sqlalchemy import MetaData, Table, update
-
-
-class UpdateFnGuidePdfData:
-    """
-    다운로드 한 PDF 파일 TEXT 변환 후 UPDATE
-    """
-
-    def __init__(self, download_path=None, backup_path=None, engine=None, table=None):
-        # 파일 다운로드 경로
-        self.download_path = download_path
-        if not os.path.exists(self.download_path):
-            os.makedirs(self.download_path)
-
-        # 파일 오류시 백업파일 이동 경로
-        self.backup_path = backup_path
-        if not os.path.exists(self.backup_path):
-            os.makedirs(self.backup_path)
-
-        # 데이터베이스
-        self.get_engine = engine
-        self.table_name = table
-
-    def update_pdf_data(self):
-        logger.info("## PDF 파일 변환 및 적재 시작 ##")
-        for file in tqdm(os.listdir(self.download_path)):
+
+class PdftoText:
+    def pdf_to_text(self, download_path):
+        pdf_list = []
+        for file in os.listdir(download_path):
             if not file.endswith(".pdf"):
                 continue
 
-            # size 0인 파일 삭제후 건너뛰기
-            pdf_path = os.path.join(self.download_path, file)
+            pdf_path = os.path.join(download_path, file)
             if os.path.getsize(pdf_path) == 0:
                 os.remove(pdf_path)
                 continue
 
-            url_idx = file.split("_")[0]
-            pdf_path = os.path.join(self.download_path, file)
-
             # pdf -> text 변환
             with open(pdf_path, "rb") as f:
                 pdf = pdftotext.PDF(f)
 
             pdf_text = ""
             for page in pdf:
                 pdf_text += page
-            try:
-                # db 적재
-                logger.info(f"{file} 변환 후 적재")
-                metadata = MetaData()
-                metadata.bind = self.get_engine
-                table = Table(self.table_name, metadata, autoload_with=self.get_engine)
-
-                stmt = (
-                    update(table)
-                    .where(table.c.url.like(f"%{url_idx}%"))
-                    .values(pdf_contents=pdf_text)
-                )
-
-                with self.get_engine.begin() as connection:
-                    result = connection.execute(stmt)
-                    affected_rows = result.rowcount
-                if affected_rows == 0:
-                    shutil.move(pdf_path, os.path.join(self.backup_path, file))
-                    logger.info(f"{file}은 적재할 데이터가 없어 백업폴더로 이동")
-                else:
-                    os.remove(pdf_path)
-            except Exception as error:
-                logger.error(f"{file} 적재 오류 : {error}")
+
+            if len(pdf_text) == 0:
+                os.remove(pdf_path)
+                continue
+
+            # 디비에 update시 where문으로 찾기위한 인덱스
+            update_idx = file.split("_")[0]
+
+            data = {
+                "file_name": str(file),
+                "pdf_text": pdf_text,
+                "update_idx": str(update_idx),
+            }
+            pdf_list.append(data)
+        return pdf_list
```

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.5/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/src/dmk_packages/database/database.py` & `dmk_packages-0.6.5/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.5/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.4/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.5/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.4
+Version: 0.6.5
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.4/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.5/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 src/dmk_packages.egg-info/dependency_links.txt
 src/dmk_packages.egg-info/requires.txt
 src/dmk_packages.egg-info/top_level.txt
 src/dmk_packages/crawler/__init__.py
 src/dmk_packages/crawler/bigkinds.py
 src/dmk_packages/crawler/clien.py
 src/dmk_packages/crawler/fnguide.py
-src/dmk_packages/crawler/fnguide_pdf_update.py
 src/dmk_packages/crawler/naver_blog.py
 src/dmk_packages/crawler/naver_search_volume.py
+src/dmk_packages/crawler/pdf_to_text.py
 src/dmk_packages/crawler/youtube.py
 src/dmk_packages/database/__init__.py
 src/dmk_packages/database/database.py
```

