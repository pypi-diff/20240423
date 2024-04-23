# Comparing `tmp/jpholiday-0.1.8.tar.gz` & `tmp/jpholiday-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpholiday-0.1.8.tar", last modified: Mon Nov 22 11:38:38 2021, max compression
+gzip compressed data, was "jpholiday-0.1.9.tar", last modified: Tue Mar  5 11:20:50 2024, max compression
```

## Comparing `jpholiday-0.1.8.tar` & `jpholiday-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 11:38:38.841165 jpholiday-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-11-22 11:38:30.000000 jpholiday-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6350 2021-11-22 11:38:38.841165 jpholiday-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5420 2021-11-22 11:38:30.000000 jpholiday-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 11:38:38.837164 jpholiday-0.1.8/jpholiday/
--rwxr-xr-x   0 runner    (1001) docker     (121)      668 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/holiday.py
--rw-r--r--   0 runner    (1001) docker     (121)     2570 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/jpholiday.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-11-22 11:38:30.000000 jpholiday-0.1.8/jpholiday/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 11:38:38.837164 jpholiday-0.1.8/jpholiday.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6350 2021-11-22 11:38:38.000000 jpholiday-0.1.8/jpholiday.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-11-22 11:38:38.000000 jpholiday-0.1.8/jpholiday.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 11:38:38.000000 jpholiday-0.1.8/jpholiday.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-11-22 11:38:38.000000 jpholiday-0.1.8/jpholiday.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-22 11:38:38.841165 jpholiday-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2021-11-22 11:38:30.000000 jpholiday-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:20:50.251088 jpholiday-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-05 11:20:40.000000 jpholiday-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-05 11:20:50.251088 jpholiday-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-05 11:20:40.000000 jpholiday-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:20:50.243088 jpholiday-0.1.9/jpholiday/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      668 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/holiday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/jpholiday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-05 11:20:40.000000 jpholiday-0.1.9/jpholiday/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:20:50.251088 jpholiday-0.1.9/jpholiday.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-05 11:20:50.000000 jpholiday-0.1.9/jpholiday.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-05 11:20:50.000000 jpholiday-0.1.9/jpholiday.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 11:20:50.000000 jpholiday-0.1.9/jpholiday.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-05 11:20:50.000000 jpholiday-0.1.9/jpholiday.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 11:20:50.251088 jpholiday-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-05 11:20:40.000000 jpholiday-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 11:20:50.251088 jpholiday-0.1.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8262 2024-03-05 11:20:40.000000 jpholiday-0.1.9/tests/test_basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5541 2024-03-05 11:20:40.000000 jpholiday-0.1.9/tests/test_datetime.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1494 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_freezegun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_1971.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_1992.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_1997.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_1998.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2003.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2006.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2015.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2018.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2019.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2021.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-03-05 11:20:41.000000 jpholiday-0.1.9/tests/test_year_2025.py
```

### Comparing `jpholiday-0.1.8/LICENSE` & `jpholiday-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jpholiday-0.1.8/PKG-INFO` & `jpholiday-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpholiday
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pure-Python Japan Public Holiday Generate
 Home-page: https://github.com/Lalcs/jpholiday
 Author: Vatis
 Author-email: vatis@lalcs.com
 License: MIT License
 Keywords: Japan,Holiday
 Platform: POSIX
@@ -14,19 +14,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JPHoliday
 
 [![image](https://img.shields.io/pypi/v/jpholiday.svg)](https://pypi.org/project/jpholiday/)
 [![image](https://img.shields.io/pypi/l/jpholiday.svg)](https://pypi.org/project/jpholiday/)
@@ -209,9 +210,7 @@
 
 jpholiday.is_holiday(datetime.date(2021, 2, 22))
 > True
 
 jpholiday.is_holiday_name(datetime.date(2021, 2, 22))
 > 特別休暇1
 ```
-
-
```

### Comparing `jpholiday-0.1.8/README.md` & `jpholiday-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jpholiday-0.1.8/jpholiday/__init__.py` & `jpholiday-0.1.9/jpholiday/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 2019年 国民の祝日に関する法律の一部を改正する法律(昭和23年法律第178号)
 2020年 国民の祝日に関する法律の一部を改正する法律(平成30年法律第57号)
 2020年 国民の祝日に関する法律(昭和23年法律第178号)の特例
 2019年 天皇の即位の日及び即位礼正殿の儀の行われる日を休日とする法律
 2020年 五輪特別措置法改正案
 """
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
```

### Comparing `jpholiday-0.1.8/jpholiday/holiday.py` & `jpholiday-0.1.9/jpholiday/holiday.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         return math.floor(i + 0.242194 * (year - 1980) - math.floor((year - 1980) / 4))
 
 
 # みどりの日
 class GreeneryDay(registry.BaseHoliday):
     def _is_holiday(self, date):
-        if date.year >= 1989 and date.year <= 2006 and date.month == 4 and date.day == 29:
+        if date.year in range(1989, 2006 + 1) and date.month == 4 and date.day == 29:
             return True
         elif date.year >= 2007 and date.month == 5 and date.day == 4:
             return True
         return False
 
     def _is_holiday_name(self, date):
         return 'みどりの日'
@@ -156,15 +156,15 @@
         # 2021: 五輪特別措置法改正案
         if date.year == 2021:
             if date == datetime.date(2021, 7, 22):
                 return True
 
             return False
 
-        if date.year >= 1996 and date.month == 7 and date.year <= 2002 and date.day == 20:
+        if date.year in range(1996, 2002 + 1) and date.month == 7 and date.day == 20:
             return True
         # 2020: 国民の祝日に関する法律の一部を改正する法律(平成30年法律第57号)
         elif date.year >= 2003 and date.month == 7 and date.day == utils._week_day(date, 3,
                                                                                                          1).day:
             return True
 
 
@@ -201,15 +201,15 @@
     def _is_holiday_name(self, date):
         return '山の日'
 
 
 # 敬老の日
 class RespectForTheAgedDay(registry.BaseHoliday):
     def _is_holiday(self, date):
-        if date.year >= 1966 and date.year <= 2002 and date.month == 9 and date.day == 15:
+        if date.year in range(1966, 2002 + 1) and date.month == 9 and date.day == 15:
             return True
         elif date.year >= 2003 and date.month == 9 and date.day == utils._week_day(date, 3, 1).day:
             return True
         return False
 
     def _is_holiday_name(self, date):
         return '敬老の日'
@@ -250,18 +250,17 @@
 
         return math.floor(i + 0.242194 * (year - 1980) - math.floor((year - 1980) / 4))
 
 
 # 体育の日
 class HealthAndSportsDay(registry.BaseHoliday):
     def _is_holiday(self, date):
-        if date.year >= 1966 and date.year <= 1999 and date.month == 10 and date.day == 10:
+        if date.year in range(1966, 1999 + 1) and date.month == 10 and date.day == 10:
             return True
-        elif date.year >= 2000 and date.year <= 2019 and date.month == 10 and date.day == utils._week_day(date, 2,
-                                                                                                          1).day:
+        elif date.year in range(2000, 2019 + 1) and date.month == 10 and date.day == utils._week_day(date, 2, 1).day:
             return True
         return False
 
     def _is_holiday_name(self, date):
         return '体育の日'
 
 
@@ -354,75 +353,53 @@
         return self.__transfer_holiday_name(date)
 
     def __transfer_holiday_name(self, date):
         # 1973年(昭和48年)4月12日 - 改正・施行
         if date.year < 1973:
             return None
 
-        # GW
-        if date.year > 2006 and date.month == 5 and date.day == 6 and date.isoweekday() in (2, 3):
-            for holiday in registry.RegistryHolder.get_registry():
-                if holiday.__class__.__name__ == self.__class__.__name__:
-                    continue
-
-                if isinstance(holiday, NationalHoliday):
-                    continue
-
-                if isinstance(holiday, registry.OriginalHoliday):
-                    continue
+        # 日曜日に振替休日は存在しない
+        if date.isoweekday() == 7:
+            return None
 
-                if holiday.is_holiday((date + datetime.timedelta(days=-date.isoweekday()))):
-                    return '{} {}'.format(
-                        holiday.is_holiday_name((date + datetime.timedelta(days=-date.isoweekday()))),
-                        '振替休日')
+        filtered_registry = list(filter(lambda x: not isinstance(x, TransferHoliday) and not isinstance(x, NationalHoliday) and not isinstance(x, registry.OriginalHoliday), registry.RegistryHolder.get_registry()))
 
-        # 月曜日でない
-        if date.isoweekday() != 1:
+        # 祝日が存在する日に振替休日は存在しない
+        if len(list(filter(lambda x: x.is_holiday(date), filtered_registry))) != 0:
             return None
 
-        # GW以外
-        for holiday in registry.RegistryHolder.get_registry():
-            if holiday.__class__.__name__ == self.__class__.__name__:
-                continue
-
-            if isinstance(holiday, NationalHoliday):
-                continue
-
-            if isinstance(holiday, registry.OriginalHoliday):
-                continue
-
-            if holiday.is_holiday((date + datetime.timedelta(days=-1))):
-                return '{} {}'.format(holiday.is_holiday_name((date + datetime.timedelta(days=-1))),
-                                      '振替休日')
+        current_date = date - datetime.timedelta(days=1)
+        while(True):
+            current_registry = list(filter(lambda x: x.is_holiday(current_date), filtered_registry))
+            if len(current_registry) == 0:
+                return None
 
+            if current_date.isoweekday() == 7:
+                if len(current_registry) != 0:
+                    return '{} {}'.format(
+                        current_registry[0].is_holiday_name(current_date),
+                        '振替休日'
+                    )
+                else:
+                    return None
+
+            current_date = current_date - datetime.timedelta(days=1)
 
 # 国民の休日
 class NationalHoliday(registry.BaseHoliday):
     def _is_holiday(self, date):
 
         if date.isoweekday() == 7:
             return None
 
-        result = {
-            'old': False,
-            'new': False,
-        }
-
-        for holiday in registry.RegistryHolder.get_registry():
-            if holiday.__class__.__name__ == self.__class__.__name__:
-                continue
-
-            if isinstance(holiday, registry.OriginalHoliday):
-                continue
-
-            if holiday.is_holiday((date + datetime.timedelta(days=-1))):
-                result['old'] = True
-            if holiday.is_holiday((date + datetime.timedelta(days=1))):
-                result['new'] = True
+        filtered_registry = list(filter(lambda x: not isinstance(x, NationalHoliday) and not isinstance(x, registry.OriginalHoliday), registry.RegistryHolder.get_registry()))
 
-            if list(result.values()) == [True, True]:
-                return True
+        if len(list(filter(lambda x: x.is_holiday(date), filtered_registry))) != 0:
+            return None
+
+        if len(list(filter(lambda x: x.is_holiday(date + datetime.timedelta(days=1)), filtered_registry))) != 0 and len(list(filter(lambda x: x.is_holiday(date - datetime.timedelta(days=1)), filtered_registry))) != 0:
+            return True
 
         return False
 
     def _is_holiday_name(self, date):
         return '国民の休日'
```

### Comparing `jpholiday-0.1.8/jpholiday/jpholiday.py` & `jpholiday-0.1.9/jpholiday/jpholiday.py`

 * *Files identical despite different names*

### Comparing `jpholiday-0.1.8/jpholiday/registry.py` & `jpholiday-0.1.9/jpholiday/registry.py`

 * *Files identical despite different names*

### Comparing `jpholiday-0.1.8/jpholiday/utils.py` & `jpholiday-0.1.9/jpholiday/utils.py`

 * *Files identical despite different names*

### Comparing `jpholiday-0.1.8/jpholiday.egg-info/PKG-INFO` & `jpholiday-0.1.9/jpholiday.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpholiday
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pure-Python Japan Public Holiday Generate
 Home-page: https://github.com/Lalcs/jpholiday
 Author: Vatis
 Author-email: vatis@lalcs.com
 License: MIT License
 Keywords: Japan,Holiday
 Platform: POSIX
@@ -14,19 +14,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JPHoliday
 
 [![image](https://img.shields.io/pypi/v/jpholiday.svg)](https://pypi.org/project/jpholiday/)
 [![image](https://img.shields.io/pypi/l/jpholiday.svg)](https://pypi.org/project/jpholiday/)
@@ -209,9 +210,7 @@
 
 jpholiday.is_holiday(datetime.date(2021, 2, 22))
 > True
 
 jpholiday.is_holiday_name(datetime.date(2021, 2, 22))
 > 特別休暇1
 ```
-
-
```

### Comparing `jpholiday-0.1.8/setup.py` & `jpholiday-0.1.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # -*- coding: utf-8 -*-
-from codecs import open
 import os
 import re
+from codecs import open
 from setuptools import setup
 
 with open(os.path.join('jpholiday', '__init__.py'), 'r', encoding='utf8') as f:
-	version = re.compile(
-		r".*__version__ = '(.*?)'", re.S).match(f.read()).group(1)
+    version = re.compile(
+        r".*__version__ = '(.*?)'", re.S).match(f.read()).group(1)
 
 setup(
-	name='jpholiday',
-	packages=['jpholiday'],
-	version=version,
-	license='MIT License',
-	platforms=['POSIX', 'Windows', 'Unix', 'MacOS'],
-	description='Pure-Python Japan Public Holiday Generate',
-	author='Vatis',
-	author_email='vatis@lalcs.com',
-	url='https://github.com/Lalcs/jpholiday',
-	keywords=['Japan', 'Holiday'],
-	classifiers=[
-		'Intended Audience :: Developers',
-		'License :: OSI Approved :: MIT License',
-		'Natural Language :: Japanese',
-		'Operating System :: MacOS',
-		'Operating System :: Microsoft',
-		'Operating System :: POSIX',
-		'Programming Language :: Python :: 3 :: Only',
-		'Programming Language :: Python :: 3.6',
-		'Programming Language :: Python :: 3.7',
-		'Programming Language :: Python :: 3.8',
-		'Programming Language :: Python :: 3.9',
-		'Programming Language :: Python :: 3.10',
-	],
-	data_files=[('', ['README.md'])],
-	long_description='{}'.format((open('README.md', encoding='utf8').read())),
-	long_description_content_type="text/markdown",
+    name='jpholiday',
+    packages=['jpholiday'],
+    version=version,
+    license='MIT License',
+    platforms=['POSIX', 'Windows', 'Unix', 'MacOS'],
+    description='Pure-Python Japan Public Holiday Generate',
+    author='Vatis',
+    author_email='vatis@lalcs.com',
+    url='https://github.com/Lalcs/jpholiday',
+    keywords=['Japan', 'Holiday'],
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: Japanese',
+        'Operating System :: MacOS',
+        'Operating System :: Microsoft',
+        'Operating System :: POSIX',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+    ],
+    data_files=[('', ['README.md'])],
+    long_description='{}'.format((open('README.md', encoding='utf8').read())),
+    long_description_content_type="text/markdown",
 )
```

