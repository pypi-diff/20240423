# Comparing `tmp/pyrpabrowserdemo-0.0.4.tar.gz` & `tmp/pyrpabrowserdemo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrpabrowserdemo-0.0.4.tar", last modified: Thu Apr 18 21:20:29 2024, max compression
+gzip compressed data, was "pyrpabrowserdemo-0.0.5.tar", last modified: Tue Apr 23 16:53:56 2024, max compression
```

## Comparing `pyrpabrowserdemo-0.0.4.tar` & `pyrpabrowserdemo-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 21:20:29.135607 pyrpabrowserdemo-0.0.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 pyrpabrowserdemo-0.0.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-18 21:20:29.135607 pyrpabrowserdemo-0.0.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1419 2024-04-16 19:14:12.000000 pyrpabrowserdemo-0.0.4/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 21:20:29.135607 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2024-04-16 19:10:47.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1803 2024-04-18 21:16:40.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/booking.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      950 2024-04-18 21:08:19.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/bot_sparebin.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5510 2024-04-18 20:56:02.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/browser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1314 2024-04-18 20:37:46.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/definition.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      162 2024-04-18 21:13:58.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/run_test_bot.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 21:20:29.135607 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-18 21:20:29.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      407 2024-04-18 21:20:29.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-18 21:20:29.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-04-18 21:20:29.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2024-04-18 21:20:29.000000 pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-18 21:20:29.135607 pyrpabrowserdemo-0.0.4/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1124 2024-04-18 21:20:10.000000 pyrpabrowserdemo-0.0.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 16:53:56.917699 pyrpabrowserdemo-0.0.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 pyrpabrowserdemo-0.0.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-23 16:53:56.917699 pyrpabrowserdemo-0.0.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1419 2024-04-16 19:14:12.000000 pyrpabrowserdemo-0.0.5/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 16:53:56.917699 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2024-04-19 18:58:36.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1806 2024-04-19 18:20:54.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/booking.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1778 2024-04-19 19:41:39.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/bot_sparebin.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5627 2024-04-19 19:38:58.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/browser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1314 2024-04-19 18:20:54.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/definition.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      166 2024-04-19 19:03:33.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/run_test_bot.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-23 16:53:56.917699 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-23 16:53:56.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      407 2024-04-23 16:53:56.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-23 16:53:56.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-04-23 16:53:56.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2024-04-23 16:53:56.000000 pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-23 16:53:56.917699 pyrpabrowserdemo-0.0.5/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1124 2024-04-23 16:53:49.000000 pyrpabrowserdemo-0.0.5/setup.py
```

### Comparing `pyrpabrowserdemo-0.0.4/LICENSE` & `pyrpabrowserdemo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrpabrowserdemo-0.0.4/PKG-INFO` & `pyrpabrowserdemo-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrpabrowserdemo
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplify RPA activities with a browser.
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrpabrowserdemo-0.0.4/README.md` & `pyrpabrowserdemo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/booking.py` & `pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/booking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from browser import Browser 
 from definition import Spreadsheet
 
 
 
-class BookinBot:
+class BookingBot:
     def __init__(self):
         self.bot = Browser()
         self.spreadsheet = Spreadsheet()
-
-    def run(self):
-
-        bot = Browser()
-        bot.open_browser('https://booking.com/')
-
-        def click_dissmiss_sign_in():
+        self.bot.open_browser('https://booking.com/')
+    
+    def click_dissmiss_sign_in(self):
             try:
-                bot.click_by_aria_label("Dismiss sign-in info.")
+                self.bot.click_by_aria_label("Dismiss sign-in info.")
             except Exception as e:
                 print(e)
+
+    def run(self):
                 
-        click_dissmiss_sign_in() 
-        bot.fill_by_id(':re:', 'Teresina')
-        bot.click_element_by_data_test_id("searchbox-dates-container")
-        bot.click_general_element("data-date", "2024-04-25")
-        bot.click_button_by_type("submit")
+        self.click_dissmiss_sign_in() 
+        self.bot.fill_by_id(':re:', 'Teresina')
+        self.bot.click_element_by_data_test_id("searchbox-dates-container")
+        self.bot.click_general_element("data-date", "2024-04-25")
+        self.bot.click_button_by_type("submit")
 
 
-        click_dissmiss_sign_in()
-        popular_filters = bot.get_webelements_by_id("filter_group_popular_:rj:")
+        self.click_dissmiss_sign_in()
+        popular_filters = self.bot.get_webelements_by_id("filter_group_popular_:rj:")
 
-        bot.click_by_text(popular_filters, "Breakfast Included")
-        elements = bot.get_elements_by_data_test_id("property-card-container")
+        self.bot.click_by_text(popular_filters, "Breakfast Included")
+        elements = self.bot.get_elements_by_data_test_id("property-card-container")
 
         list_to_df = []
         for i in elements:
             fields = i.text.split('\n')
             
             data_dict = {
                 'name': fields[0],
@@ -48,9 +46,8 @@
                 'availability_info': fields[8],
                 'price_per_night': fields[9],
                 'includes_taxes_and_fees': fields[10],
                 'see_availability_link': fields[11]
             }
             list_to_df.append(data_dict)
 
-        spreadsheet = Spreadsheet()
-        spreadsheet.convert_list_to_excel(list_to_df, 'data.xlsx')
+        self.spreadsheet.convert_list_to_excel(list_to_df, 'data.xlsx')
```

### Comparing `pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/browser.py` & `pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,26 +142,30 @@
         """
         Click on button by type.
         """
         #//*[button[@type="submit"]]
         self.browser.wait_until_element_is_enabled(f'//*[button[@type="{type}"]]')
         self.browser.click_element_when_clickable(f'//*[button[@type="{type}"]]')
 
-    def get_html_select_options(self, locator: str) -> None:
+    def click_select_option_index(self, locator: str, index: str) -> None:
+        
         """
-        Get html select options.
+        Get html selector and click on the index option.
+
+        Example: 
+            - selector: //*[@id="salestarget"]
+            - index: 1
+            - full selector: //*[@id="salestarget"]/option[1]
         """
-        self.browser.wait_until_element_is_visible(locator)
-        select = self.browser.find_element(locator)
-        return select
+        self.click(f"{locator}/option[{index}]")
 
     def click_by_text(self, web_elements, text: str) -> None:
         """
         Click on element by text.
         """
         for web_element in web_elements:
             if text in web_element.text:
                 web_element.click()
 
-
+    
 
     #Sign in or register
```

### Comparing `pyrpabrowserdemo-0.0.4/pyrpabrowserdemo/definition.py` & `pyrpabrowserdemo-0.0.5/pyrpabrowserdemo/definition.py`

 * *Files identical despite different names*

### Comparing `pyrpabrowserdemo-0.0.4/pyrpabrowserdemo.egg-info/PKG-INFO` & `pyrpabrowserdemo-0.0.5/pyrpabrowserdemo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrpabrowserdemo
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplify RPA activities with a browser.
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrpabrowserdemo-0.0.4/setup.py` & `pyrpabrowserdemo-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Simplify RPA activities with a browser.'
 LONG_DESCRIPTION = 'A package that allows to execute RPA activities without configuration'
 
 # Setting up
 setup(
     name="pyrpabrowserdemo",
     version=VERSION,
```

