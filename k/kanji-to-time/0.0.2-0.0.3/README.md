# Comparing `tmp/kanji_to_time-0.0.2.tar.gz` & `tmp/kanji_to_time-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanji_to_time-0.0.2.tar", last modified: Sat Mar 30 06:10:51 2024, max compression
+gzip compressed data, was "kanji_to_time-0.0.3.tar", last modified: Tue Apr 23 06:32:17 2024, max compression
```

## Comparing `kanji_to_time-0.0.2.tar` & `kanji_to_time-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.134785 kanji_to_time-0.0.2/
--rw-r--r--   0 operation   (501) staff       (20)     1065 2024-03-30 04:59:15.000000 kanji_to_time-0.0.2/LICENSE
--rw-r--r--   0 operation   (501) staff       (20)       53 2024-03-30 06:00:29.000000 kanji_to_time-0.0.2/MANIFEST.in
--rw-r--r--   0 operation   (501) staff       (20)     2343 2024-03-30 06:10:51.134711 kanji_to_time-0.0.2/PKG-INFO
--rw-r--r--   0 operation   (501) staff       (20)     1733 2024-03-30 05:47:40.000000 kanji_to_time-0.0.2/README.md
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.131398 kanji_to_time-0.0.2/kanji_to_time/
--rw-r--r--   0 operation   (501) staff       (20)     1294 2024-03-30 05:13:20.000000 kanji_to_time-0.0.2/kanji_to_time/__init__.py
--rw-r--r--   0 operation   (501) staff       (20)      664 2024-03-30 05:07:29.000000 kanji_to_time-0.0.2/kanji_to_time/convert_table.py
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.132540 kanji_to_time-0.0.2/kanji_to_time/grammer/
--rw-r--r--   0 operation   (501) staff       (20)     1452 2024-03-30 04:30:50.000000 kanji_to_time-0.0.2/kanji_to_time/grammer/kanji_to_time.lark
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.133540 kanji_to_time-0.0.2/kanji_to_time/transformer/
--rw-r--r--   0 operation   (501) staff       (20)     1213 2024-03-30 05:28:37.000000 kanji_to_time-0.0.2/kanji_to_time/transformer/BaseTransformer.py
--rw-r--r--   0 operation   (501) staff       (20)      925 2024-03-30 05:28:31.000000 kanji_to_time-0.0.2/kanji_to_time/transformer/DatetimeTransformer.py
--rw-r--r--   0 operation   (501) staff       (20)      774 2024-03-30 05:13:09.000000 kanji_to_time-0.0.2/kanji_to_time/transformer/TimedeltaTransformer.py
--rw-r--r--   0 operation   (501) staff       (20)        0 2024-03-30 05:14:23.000000 kanji_to_time-0.0.2/kanji_to_time/transformer/__init__.py
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.134459 kanji_to_time-0.0.2/kanji_to_time.egg-info/
--rw-r--r--   0 operation   (501) staff       (20)     2343 2024-03-30 06:10:51.000000 kanji_to_time-0.0.2/kanji_to_time.egg-info/PKG-INFO
--rw-r--r--   0 operation   (501) staff       (20)      592 2024-03-30 06:10:51.000000 kanji_to_time-0.0.2/kanji_to_time.egg-info/SOURCES.txt
--rw-r--r--   0 operation   (501) staff       (20)        1 2024-03-30 06:10:51.000000 kanji_to_time-0.0.2/kanji_to_time.egg-info/dependency_links.txt
--rw-r--r--   0 operation   (501) staff       (20)       12 2024-03-30 06:10:51.000000 kanji_to_time-0.0.2/kanji_to_time.egg-info/requires.txt
--rw-r--r--   0 operation   (501) staff       (20)       14 2024-03-30 06:10:51.000000 kanji_to_time-0.0.2/kanji_to_time.egg-info/top_level.txt
--rw-r--r--   0 operation   (501) staff       (20)       89 2024-03-30 04:39:58.000000 kanji_to_time-0.0.2/pyproject.toml
--rw-r--r--   0 operation   (501) staff       (20)      711 2024-03-30 06:10:51.135041 kanji_to_time-0.0.2/setup.cfg
-drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-03-30 06:10:51.134170 kanji_to_time-0.0.2/tests/
--rw-r--r--   0 operation   (501) staff       (20)     1312 2024-03-30 05:04:43.000000 kanji_to_time-0.0.2/tests/test_number.py
--rw-r--r--   0 operation   (501) staff       (20)     1116 2024-03-30 05:04:43.000000 kanji_to_time-0.0.2/tests/test_to_datetime.py
--rw-r--r--   0 operation   (501) staff       (20)     1934 2024-03-30 05:04:43.000000 kanji_to_time-0.0.2/tests/test_to_timedelta.py
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.988956 kanji_to_time-0.0.3/
+-rw-r--r--   0 operation   (501) staff       (20)     1065 2024-03-30 04:59:15.000000 kanji_to_time-0.0.3/LICENSE
+-rw-r--r--   0 operation   (501) staff       (20)       53 2024-03-30 06:00:29.000000 kanji_to_time-0.0.3/MANIFEST.in
+-rw-r--r--   0 operation   (501) staff       (20)     3497 2024-04-23 06:32:17.988900 kanji_to_time-0.0.3/PKG-INFO
+-rw-r--r--   0 operation   (501) staff       (20)     2893 2024-04-11 04:59:19.000000 kanji_to_time-0.0.3/README.md
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.985750 kanji_to_time-0.0.3/kanji_to_time/
+-rw-r--r--   0 operation   (501) staff       (20)     1291 2024-04-11 05:04:16.000000 kanji_to_time-0.0.3/kanji_to_time/__init__.py
+-rw-r--r--   0 operation   (501) staff       (20)      747 2024-04-11 04:56:30.000000 kanji_to_time-0.0.3/kanji_to_time/convert_table.py
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.986741 kanji_to_time-0.0.3/kanji_to_time/grammer/
+-rw-r--r--   0 operation   (501) staff       (20)     1530 2024-04-11 04:56:30.000000 kanji_to_time-0.0.3/kanji_to_time/grammer/kanji_to_time.lark
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.987756 kanji_to_time-0.0.3/kanji_to_time/transformer/
+-rw-r--r--   0 operation   (501) staff       (20)     1122 2024-04-11 05:01:05.000000 kanji_to_time-0.0.3/kanji_to_time/transformer/BaseTransformer.py
+-rw-r--r--   0 operation   (501) staff       (20)      925 2024-03-30 05:28:31.000000 kanji_to_time-0.0.3/kanji_to_time/transformer/DatetimeTransformer.py
+-rw-r--r--   0 operation   (501) staff       (20)      972 2024-04-11 04:56:30.000000 kanji_to_time-0.0.3/kanji_to_time/transformer/TimedeltaTransformer.py
+-rw-r--r--   0 operation   (501) staff       (20)        0 2024-03-30 05:14:23.000000 kanji_to_time-0.0.3/kanji_to_time/transformer/__init__.py
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.988677 kanji_to_time-0.0.3/kanji_to_time.egg-info/
+-rw-r--r--   0 operation   (501) staff       (20)     3497 2024-04-23 06:32:17.000000 kanji_to_time-0.0.3/kanji_to_time.egg-info/PKG-INFO
+-rw-r--r--   0 operation   (501) staff       (20)      595 2024-04-23 06:32:17.000000 kanji_to_time-0.0.3/kanji_to_time.egg-info/SOURCES.txt
+-rw-r--r--   0 operation   (501) staff       (20)        1 2024-04-23 06:32:17.000000 kanji_to_time-0.0.3/kanji_to_time.egg-info/dependency_links.txt
+-rw-r--r--   0 operation   (501) staff       (20)       12 2024-04-23 06:32:17.000000 kanji_to_time-0.0.3/kanji_to_time.egg-info/requires.txt
+-rw-r--r--   0 operation   (501) staff       (20)       14 2024-04-23 06:32:17.000000 kanji_to_time-0.0.3/kanji_to_time.egg-info/top_level.txt
+-rw-r--r--   0 operation   (501) staff       (20)       89 2024-03-30 04:39:58.000000 kanji_to_time-0.0.3/pyproject.toml
+-rw-r--r--   0 operation   (501) staff       (20)      705 2024-04-23 06:32:17.989203 kanji_to_time-0.0.3/setup.cfg
+drwxr-xr-x   0 operation   (501) staff       (20)        0 2024-04-23 06:32:17.988411 kanji_to_time-0.0.3/tests/
+-rw-r--r--   0 operation   (501) staff       (20)     1074 2024-04-01 10:41:33.000000 kanji_to_time-0.0.3/tests/test_to_datetime.py
+-rw-r--r--   0 operation   (501) staff       (20)     1580 2024-04-01 05:42:01.000000 kanji_to_time-0.0.3/tests/test_to_number.py
+-rw-r--r--   0 operation   (501) staff       (20)     2129 2024-04-11 04:56:30.000000 kanji_to_time-0.0.3/tests/test_to_timedelta.py
```

### Comparing `kanji_to_time-0.0.2/LICENSE` & `kanji_to_time-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kanji_to_time-0.0.2/PKG-INFO` & `kanji_to_time-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kanji_to_time
-Version: 0.0.2
-Summary: Convert Japanese kanji time expressions to datetime objects
+Version: 0.0.3
+Summary: Convert Japanese time expressions to datetime objects
 Home-page: https://github.com/corkborg/kanji_to_time
 Author: corkborg
 Author-email: ax4squil8@mozmail.com
 License: MIT
 Keywords: kanji,timedelta,datetime,japanese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,17 @@
 Classifier: Natural Language :: Japanese
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lark>=1.1.9
 
 # Kanji to time
 
-日本語の漢字などで書かれた年月日をPythonのdatetime型やtimedelta型に変換するライブラリ。<br/>
+日本語の漢字などで書かれた年月日をPythonのdatetime型やtimedelta型に変換するライブラリ。
+内部では正規表現ではなくパーサージェネレータを使用しているので複雑なルールに対応しやすいようになっています。
+
 漢数字、旧字漢数字、全角などに対応しています。
 
 ## 使い方
 
 ```bash
 pip install kanji_to_time
 ```
@@ -40,48 +42,71 @@
 ```
 
 ## 対応パターン例
 
 ### datetimeの変換
 
 ```python
-dt = to_datetime("2024年4月5日22時30分4秒")
+dt = ktt.to_datetime("2024年4月5日22時30分4秒")
 self.assertEqual(dt, datetime(year=2024, month=4, day=5, hour=22, minute=30, second=4))
 
-dt = to_datetime("２０２０年５月７日")
+dt = ktt.to_datetime("２０２０年５月７日")
 self.assertEqual(dt, datetime(year=2020, month=5, day=7))
 
-dt = to_datetime("二〇二五年十二月七日")
+dt = ktt.to_datetime("二〇二五年十二月七日")
 self.assertEqual(dt, datetime(year=2025, month=12, day=7))
 
-dt = to_datetime("二千年八月三日")
+dt = ktt.to_datetime("二千年八月三日")
 self.assertEqual(dt, datetime(year=2000, month=8, day=3))
 
-dt = to_datetime("弐零弐参年伍月肆日")
+dt = ktt.to_datetime("弐零弐参年伍月肆日")
 self.assertEqual(dt, datetime(year=2023, month=5, day=4))
 ```
 
 ### timedeltaの変換
 
 ```python
-td = to_timedelta("二時間三十秒")
+td = ktt.to_timedelta("二時間三十秒")
 self.assertEqual(td, timedelta(hours=2, seconds=30))
 
-td = to_timedelta("六日間二時間五分間三秒間")
+td = ktt.to_timedelta("六日間二時間五分間三秒間")
 self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-td = to_timedelta("六日二時五分三秒")
+td = ktt.to_timedelta("六日二時五分三秒")
 self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-td = to_timedelta("90秒")
+td = ktt.to_timedelta("90秒")
 self.assertEqual(td, timedelta(seconds=90))
 
-td = to_timedelta("マイナス七億分")
+td = ktt.to_timedelta("マイナス七億分")
 self.assertEqual(td, timedelta(minutes=-700_000_000))
 ```
 
+その他詳細なパターンはこちらのファイルを参照
+* [tests/test_to_datetime.py](tests/test_to_datetime.py)
+* [tests/test_to_timedelta.py](tests/test_to_timedelta.py)
+* [tests/test_to_number.py](tests/test_to_number.py)
+
+対応している文法の構造自体を確認したい場合はLark定義ファイルを参照
+* [kanji_to_time/grammer/kanji_to_time.lark](kanji_to_time/grammer/kanji_to_time.lark)
+
 ## ユニットテスト
 
-```
+```bash
 pip install -r requirements.txt
 python -m unittest discover -s tests
 ```
+
+## 問い合わせ
+
+バグや機能要望についてはissueに報告をお願いします。<br/>
+https://github.com/corkborg/kanji_to_time/issues
+
+その他の問い合わせはメールまで（メール転送サービスを利用しています）<br/>
+ax4squil8&#064;mozmail.com
+
+## リリースノート
+
+### v0.0.3
+
+* to_timedeltaで接尾辞の「前」、「後」のサポート。 20秒後(seconds-20)、20秒前（seconds=-20 ）
+* to_timedeltaで「プラス」、「+」などのサポート。 +20分（minutes=20）
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time/__init__.py` & `kanji_to_time-0.0.3/kanji_to_time/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 from .transformer.DatetimeTransformer import DatetimeTransformer
 from .transformer.TimedeltaTransformer import TimeDeltaTransformer
 
 schema_path = Path(__file__).parent / 'grammer'/ 'kanji_to_time.lark'
 
 def to_datetime(text: str) -> datetime:
     """
-    文字列をdatetimeに変換する
+    日付文字列をdatetimeに変換する
     """
     parser = Lark.open(
         str(schema_path),
         start=['start_datetime'],
         parser='lalr',
         transformer=DatetimeTransformer()
     )
     return cast(datetime, parser.parse(text, start='start_datetime'))
 
 def to_timedelta(text: str) -> timedelta:
     """
-    文字列をtimedeltaに変換する
+    日付文字列をtimedeltaに変換する
     """
     parser = Lark.open(
         str(schema_path),
         start=['start_timedelta'],
         parser='lalr',
         transformer=TimeDeltaTransformer()
     )
     return cast(timedelta, parser.parse(text, start='start_timedelta'))
 
 def to_number(text: str) -> timedelta:
     """
-    数値に変換する。主にデバッグ用の関数
+    日付文字列を数値に変換する
     """
     parser = Lark.open(
         str(schema_path),
         start=['number'],
         parser='lalr',
         transformer=TimeDeltaTransformer()
     )
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time/convert_table.py` & `kanji_to_time-0.0.3/kanji_to_time/convert_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,20 +15,25 @@
     "零" : 0,
     "ゼロ": 0,
     "〇": 0,
     "○": 0,  # 誤りのゼロ
     "◯": 0, # 誤りのゼロ
 }
 
+ascii_number = {
+    str(num): num for num in range(0, 10)
+}
+
 table = {
     "一": 1, "壱": 1,
     "二": 2, "弐": 2,
     "三": 3, "参": 3,
     "四": 4, "肆": 4,
     "五": 5, "伍": 5,
     "六": 6, "陸": 6,
     "七": 7, "漆": 7,
     "八": 8, "捌": 8,
     "九": 9, "玖": 9,
     **zenkaku_table,
-    **zero_table
+    **zero_table,
+    **ascii_number,
 }
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time/grammer/kanji_to_time.lark` & `kanji_to_time-0.0.3/kanji_to_time/grammer/kanji_to_time.lark`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-start_datetime: year? month? day? hour? minute? second?
-start_timedelta: duration_day? duration_hour? duration_minute? duration_second?
+start_datetime: year month day hour? minute? second?
+start_timedelta: duration_day? duration_hour? duration_minute? duration_second? (BEFORE_TIME | AFTER_TIME)?
 
 year: number "年"
 month: number "月"
 day: number "日"
 hour: number "時"
 minute: number "分"
 second: number "秒"
 
 duration_day: number "日" | number "日間"
 duration_hour: number "時" | number "時間"
 duration_minute: number "分" | number "分間"
 duration_second: number "秒" | number "秒間"
 
-number: signed? kanji_num_parser
-kanji_num_parser: unit_oku? unit_man? unit_sen? unit_juu? mixed_number?
+BEFORE_TIME: "前"
+AFTER_TIME: "後"
 
-signed: "-" | /ー/ | /マイナス/ | /ひく/ | /引く/
+number: (MINUS | PLUS)? mixed_number_with_unit
+mixed_number_with_unit: unit_oku? unit_man? unit_sen? unit_juu? mixed_number?
 
-unit_oku: mixed_number "億" // 億は単位だけで登場することがないと考えている
-unit_man: mixed_number? "万"
+MINUS: "-" | "ー" | "マイナス" | "ひく" | "引く"
+PLUS: "+" | "＋" | "プラス" | "たす" | "足す"
+
+unit_oku: mixed_number "億" // 億は数値が必須
+unit_man: mixed_number "万" // 万は数値が必須
 unit_sen: mixed_number? "千"
 unit_juu: mixed_number? "十"
 
-mixed_number: (zenkaku_digit | kanji_digit | DIGIT)+ // 漢字混合で小数点のサポートは行わない
-kanji_unit: "十" | "百" | "千" | "万" | "億"
-kanji_digit: /一/ | /壱/
-           | /二/ | /弐/
-           | /三/ | /参/
-           | /四/ | /肆/
-           | /五/ | /伍/
-           | /六/ | /陸/
-           | /七/ | /漆/
-           | /八/ | /捌/
-           | /九/ | /玖/
-           | /〇/ | /ゼロ/ | /零/
-           | /○/ | /◯/ // 一応丸もサポートしておく
-zenkaku_digit: /０/ | /１/ | /２/ | /３/ | /４/ | /５/ | /６/ | /７/ | /８/ | /９/
+mixed_number: (ZENKAKU_DIGIT | KANJI_DIGIT | DIGIT)+ // 漢字混合で小数点のサポートは行わない
+KANJI_DIGIT: "一" | "壱"
+           | "二" | "弐"
+           | "三" | "参"
+           | "四" | "肆"
+           | "五" | "伍"
+           | "六" | "陸"
+           | "七" | "漆"
+           | "八" | "捌"
+           | "九" | "玖"
+           | "〇" | "ゼロ" | "零"
+           | "○" | "◯" // 一応丸もサポートしておく
+ZENKAKU_DIGIT: "０" | "１" | "２" | "３" | "４" | "５" | "６" | "７" | "８" | "９"
 
 %import common.DIGIT
 %import common.WS
-%ignore WS
+%ignore WS
+%ignore ","
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time/transformer/BaseTransformer.py` & `kanji_to_time-0.0.3/kanji_to_time/transformer/BaseTransformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,34 +2,28 @@
 from .. import convert_table
 
 class BaseTransformer(Transformer):
     """
     timedelta, datetime共通の解析ルール
     """
 
-    def kanji_digit(self, args: list[Token]):
-        return convert_table.to_number(args[0].value)
-
-    def zenkaku_digit(self, args: list[Token]):
-        return convert_table.to_number(args[0].value)
-
     def number(self, args):
-       if args[0] == "-":
-            return args[1] * -1
-       return args[0]
-
-    def signed(self, args):
-        return "-"
+        if isinstance(args[0], Token):
+            if args[0].type == "MINUS":
+                return args[1] * -1
+            elif args[0].type == "PLUS":
+                return args[1]
+        return args[0]
 
     def mixed_number(self, args):
         # 桁をあわせて結合
-        strs = [str(arg) for arg in args]
+        strs = [str(convert_table.to_number(arg)) for arg in args]
         return int(''.join(strs))
 
-    def kanji_num_parser(self, args):
+    def mixed_number_with_unit(self, args):
         return sum(args)
 
     def unit_juu(self, args):
         if len(args) == 1:
             return int(args[0]) * 10
         return 10
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time/transformer/DatetimeTransformer.py` & `kanji_to_time-0.0.3/kanji_to_time/transformer/DatetimeTransformer.py`

 * *Files identical despite different names*

### Comparing `kanji_to_time-0.0.2/kanji_to_time.egg-info/PKG-INFO` & `kanji_to_time-0.0.3/kanji_to_time.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kanji_to_time
-Version: 0.0.2
-Summary: Convert Japanese kanji time expressions to datetime objects
+Version: 0.0.3
+Summary: Convert Japanese time expressions to datetime objects
 Home-page: https://github.com/corkborg/kanji_to_time
 Author: corkborg
 Author-email: ax4squil8@mozmail.com
 License: MIT
 Keywords: kanji,timedelta,datetime,japanese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,17 @@
 Classifier: Natural Language :: Japanese
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lark>=1.1.9
 
 # Kanji to time
 
-日本語の漢字などで書かれた年月日をPythonのdatetime型やtimedelta型に変換するライブラリ。<br/>
+日本語の漢字などで書かれた年月日をPythonのdatetime型やtimedelta型に変換するライブラリ。
+内部では正規表現ではなくパーサージェネレータを使用しているので複雑なルールに対応しやすいようになっています。
+
 漢数字、旧字漢数字、全角などに対応しています。
 
 ## 使い方
 
 ```bash
 pip install kanji_to_time
 ```
@@ -40,48 +42,71 @@
 ```
 
 ## 対応パターン例
 
 ### datetimeの変換
 
 ```python
-dt = to_datetime("2024年4月5日22時30分4秒")
+dt = ktt.to_datetime("2024年4月5日22時30分4秒")
 self.assertEqual(dt, datetime(year=2024, month=4, day=5, hour=22, minute=30, second=4))
 
-dt = to_datetime("２０２０年５月７日")
+dt = ktt.to_datetime("２０２０年５月７日")
 self.assertEqual(dt, datetime(year=2020, month=5, day=7))
 
-dt = to_datetime("二〇二五年十二月七日")
+dt = ktt.to_datetime("二〇二五年十二月七日")
 self.assertEqual(dt, datetime(year=2025, month=12, day=7))
 
-dt = to_datetime("二千年八月三日")
+dt = ktt.to_datetime("二千年八月三日")
 self.assertEqual(dt, datetime(year=2000, month=8, day=3))
 
-dt = to_datetime("弐零弐参年伍月肆日")
+dt = ktt.to_datetime("弐零弐参年伍月肆日")
 self.assertEqual(dt, datetime(year=2023, month=5, day=4))
 ```
 
 ### timedeltaの変換
 
 ```python
-td = to_timedelta("二時間三十秒")
+td = ktt.to_timedelta("二時間三十秒")
 self.assertEqual(td, timedelta(hours=2, seconds=30))
 
-td = to_timedelta("六日間二時間五分間三秒間")
+td = ktt.to_timedelta("六日間二時間五分間三秒間")
 self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-td = to_timedelta("六日二時五分三秒")
+td = ktt.to_timedelta("六日二時五分三秒")
 self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-td = to_timedelta("90秒")
+td = ktt.to_timedelta("90秒")
 self.assertEqual(td, timedelta(seconds=90))
 
-td = to_timedelta("マイナス七億分")
+td = ktt.to_timedelta("マイナス七億分")
 self.assertEqual(td, timedelta(minutes=-700_000_000))
 ```
 
+その他詳細なパターンはこちらのファイルを参照
+* [tests/test_to_datetime.py](tests/test_to_datetime.py)
+* [tests/test_to_timedelta.py](tests/test_to_timedelta.py)
+* [tests/test_to_number.py](tests/test_to_number.py)
+
+対応している文法の構造自体を確認したい場合はLark定義ファイルを参照
+* [kanji_to_time/grammer/kanji_to_time.lark](kanji_to_time/grammer/kanji_to_time.lark)
+
 ## ユニットテスト
 
-```
+```bash
 pip install -r requirements.txt
 python -m unittest discover -s tests
 ```
+
+## 問い合わせ
+
+バグや機能要望についてはissueに報告をお願いします。<br/>
+https://github.com/corkborg/kanji_to_time/issues
+
+その他の問い合わせはメールまで（メール転送サービスを利用しています）<br/>
+ax4squil8&#064;mozmail.com
+
+## リリースノート
+
+### v0.0.3
+
+* to_timedeltaで接尾辞の「前」、「後」のサポート。 20秒後(seconds-20)、20秒前（seconds=-20 ）
+* to_timedeltaで「プラス」、「+」などのサポート。 +20分（minutes=20）
```

### Comparing `kanji_to_time-0.0.2/kanji_to_time.egg-info/SOURCES.txt` & `kanji_to_time-0.0.3/kanji_to_time.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 kanji_to_time.egg-info/requires.txt
 kanji_to_time.egg-info/top_level.txt
 kanji_to_time/grammer/kanji_to_time.lark
 kanji_to_time/transformer/BaseTransformer.py
 kanji_to_time/transformer/DatetimeTransformer.py
 kanji_to_time/transformer/TimedeltaTransformer.py
 kanji_to_time/transformer/__init__.py
-tests/test_number.py
 tests/test_to_datetime.py
+tests/test_to_number.py
 tests/test_to_timedelta.py
```

### Comparing `kanji_to_time-0.0.2/setup.cfg` & `kanji_to_time-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = kanji_to_time
-description = Convert Japanese kanji time expressions to datetime objects
-version = 0.0.2
+description = Convert Japanese time expressions to datetime objects
+version = 0.0.3
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
 keywords = kanji, timedelta, datetime, japanese
 author = corkborg
 author_email = ax4squil8@mozmail.com
```

### Comparing `kanji_to_time-0.0.2/tests/test_number.py` & `kanji_to_time-0.0.3/tests/test_to_number.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from datetime import datetime, timedelta
 import unittest
 from unittest.mock import patch, MagicMock, Mock
-from kanji_to_time import to_number
+import kanji_to_time as ktt
 
 class TestClass(unittest.TestCase):
     def test01(self):
-        n = to_number('2024')
+        n = ktt.to_number('2024')
         self.assertEqual(n, 2024)
 
-        n = to_number('二四')
+        n = ktt.to_number('二四')
         self.assertEqual(n, 24)
 
-        n = to_number('２３')
+        n = ktt.to_number('２３')
         self.assertEqual(n, 23)
 
-        n = to_number('弐壱')
+        n = ktt.to_number('弐壱')
         self.assertEqual(n, 21)
 
-        n = to_number('マイナス四３2')
+        n = ktt.to_number('マイナス四３2')
         self.assertEqual(n, -432)
 
-        n = to_number('9')
+        n = ktt.to_number('ひく43')
+        self.assertEqual(n, -43)
+
+        n = ktt.to_number('+3')
+        self.assertEqual(n, 3)
+
+        n = ktt.to_number('プラス9')
+        self.assertEqual(n, 9)
+
+        n = ktt.to_number('9')
         self.assertEqual(n, 9)
 
-        n = to_number('四')
+        n = ktt.to_number('四')
         self.assertEqual(n, 4)
 
-        n = to_number('〇')
+        n = ktt.to_number('〇')
         self.assertEqual(n, 0)
 
-        n = to_number('○')
+        n = ktt.to_number('○')
         self.assertEqual(n, 0)
 
-        n = to_number('◯')
+        n = ktt.to_number('◯')
         self.assertEqual(n, 0)
 
-        n = to_number('３')
+        n = ktt.to_number('３')
         self.assertEqual(n, 3)
 
-        n = to_number('-３')
+        n = ktt.to_number('-３')
         self.assertEqual(n, -3)
 
-        n = to_number('九十九')
+        n = ktt.to_number('九十九')
         self.assertEqual(n, 99)
 
-        n = to_number('十九')
+        n = ktt.to_number('十九')
         self.assertEqual(n, 19)
 
-        n = to_number('千7')
+        n = ktt.to_number('千7')
         self.assertEqual(n, 1007)
 
-        n = to_number('２万千7')
+        n = ktt.to_number('２万千7')
         self.assertEqual(n, 21007)
 
-        n = to_number('2億千7')
+        n = ktt.to_number('2億千7')
         self.assertEqual(n, 200_001_007)
```

### Comparing `kanji_to_time-0.0.2/tests/test_to_datetime.py` & `kanji_to_time-0.0.3/tests/test_to_datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 
-from datetime import datetime, timedelta
+from datetime import datetime
 import unittest
-from unittest.mock import patch, MagicMock, Mock
-from kanji_to_time import to_datetime
+import kanji_to_time as ktt
 
 class TestClass(unittest.TestCase):
 
     def test_standard(self):
-        dt = to_datetime("2024年4月5日22時30分4秒")
+        dt = ktt.to_datetime("2024年4月5日22時30分4秒")
         self.assertEqual(dt, datetime(year=2024, month=4, day=5, hour=22, minute=30, second=4))
 
-        dt = to_datetime("２０２０年５月７日")
+        dt = ktt.to_datetime("２０２０年５月７日")
         self.assertEqual(dt, datetime(year=2020, month=5, day=7))
 
-        dt = to_datetime("二〇二五年十二月七日")
+        dt = ktt.to_datetime("二〇二五年十二月七日")
         self.assertEqual(dt, datetime(year=2025, month=12, day=7))
 
-        dt = to_datetime("二千年八月三日")
+        dt = ktt.to_datetime("二千年八月三日")
         self.assertEqual(dt, datetime(year=2000, month=8, day=3))
 
-        dt = to_datetime("弐零弐参年伍月肆日")
+        dt = ktt.to_datetime("弐零弐参年伍月肆日")
         self.assertEqual(dt, datetime(year=2023, month=5, day=4))
 
 
     def test_detail(self):
-        dt = to_datetime("2024年四月5日")
+        dt = ktt.to_datetime("2024年四月5日")
         self.assertEqual(dt, datetime(year=2024, month=4, day=5))
 
-        dt = to_datetime("２０２4年４月5日")
+        dt = ktt.to_datetime("２０２4年４月5日")
         self.assertEqual(dt, datetime(year=2024, month=4, day=5))
```

### Comparing `kanji_to_time-0.0.2/tests/test_to_timedelta.py` & `kanji_to_time-0.0.3/tests/test_to_timedelta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 
 from datetime import timedelta
 import unittest
-from unittest.mock import patch, MagicMock, Mock
-from kanji_to_time import to_timedelta
+import kanji_to_time as ktt
 
 class TestClass(unittest.TestCase):
     def test_standard(self):
-        td = to_timedelta("二時間三十秒")
+        td = ktt.to_timedelta("二時間三十秒")
         self.assertEqual(td, timedelta(hours=2, seconds=30))
 
-        td = to_timedelta("六日間二時間五分間三秒間")
+        td = ktt.to_timedelta("六日間二時間五分間三秒間")
         self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-        td = to_timedelta("六日二時五分三秒")
+        td = ktt.to_timedelta("六日二時五分三秒")
         self.assertEqual(td, timedelta(days=6, hours=2, minutes=5, seconds=3))
 
-        td = to_timedelta("90秒")
+        td = ktt.to_timedelta("90秒")
         self.assertEqual(td, timedelta(seconds=90))
 
-        td = to_timedelta("マイナス七億分")
+        td = ktt.to_timedelta("マイナス七億分")
         self.assertEqual(td, timedelta(minutes=-700_000_000))
 
+        td = ktt.to_timedelta("45秒前")
+        self.assertEqual(td, timedelta(seconds=-45))
+
+        td = ktt.to_timedelta("45秒後")
+        self.assertEqual(td, timedelta(seconds=45))
+
     def test_detail(self):
-        td = to_timedelta("二時３分")
+        td = ktt.to_timedelta("二時３分")
         self.assertEqual(td, timedelta(hours=2, minutes=3))
 
-        td = to_timedelta("二時三分四秒")
+        td = ktt.to_timedelta("二時三分四秒")
         self.assertEqual(td, timedelta(hours=2, minutes=3, seconds=4))
 
-        td = to_timedelta("二9３分")
+        td = ktt.to_timedelta("二9３分")
         self.assertEqual(td, timedelta(minutes=293))
 
-        td = to_timedelta("二十分")
+        td = ktt.to_timedelta("二十分")
         self.assertEqual(td, timedelta(minutes=20))
 
-        td = to_timedelta("千二十分")
+        td = ktt.to_timedelta("千二十分")
         self.assertEqual(td, timedelta(minutes=1020))
 
-        td = to_timedelta("１億千二十分")
+        td = ktt.to_timedelta("１億千二十分")
         self.assertEqual(td, timedelta(minutes=100_001_020))
 
-        td = to_timedelta("5万千二十分")
+        td = ktt.to_timedelta("5万千二十分")
         self.assertEqual(td, timedelta(minutes=51_020))
 
-        td = to_timedelta("六億二十分")
+        td = ktt.to_timedelta("六億二十分")
         self.assertEqual(td, timedelta(minutes=600_000_020))
 
-        td = to_timedelta("5千二十分")
+        td = ktt.to_timedelta("5千二十分")
         self.assertEqual(td, timedelta(minutes=5020))
 
-        td = to_timedelta("-二分")
+        td = ktt.to_timedelta("-二分")
         self.assertEqual(td, timedelta(minutes=-2))
 
-        td = to_timedelta("マイナス二分")
+        td = ktt.to_timedelta("マイナス二分")
         self.assertEqual(td, timedelta(minutes=-2))
```

