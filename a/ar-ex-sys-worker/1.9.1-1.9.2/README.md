# Comparing `tmp/ar_ex_sys_worker-1.9.1-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18174 bytes, number of entries: 11
+Zip file size: 18573 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    38977 b- defN 24-Feb-20 06:40 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    21874 b- defN 24-Feb-20 06:39 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    42716 b- defN 24-Apr-23 04:10 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    22142 b- defN 24-Feb-26 12:35 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
--rw-rw-rw-  2.0 fat    11569 b- defN 24-Feb-19 13:57 ar_external_sys_worker/tests/main_test.py
+-rw-rw-rw-  2.0 fat    11290 b- defN 24-Apr-18 06:58 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Feb-20 06:42 ar_ex_sys_worker-1.9.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      341 b- defN 24-Feb-20 06:42 ar_ex_sys_worker-1.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-20 06:42 ar_ex_sys_worker-1.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Feb-20 06:42 ar_ex_sys_worker-1.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      989 b- defN 24-Feb-20 06:42 ar_ex_sys_worker-1.9.1.dist-info/RECORD
-11 files, 76063 bytes uncompressed, 16468 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-23 10:59 ar_ex_sys_worker-1.9.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-23 10:59 ar_ex_sys_worker-1.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 10:59 ar_ex_sys_worker-1.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-23 10:59 ar_ex_sys_worker-1.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 24-Apr-23 10:59 ar_ex_sys_worker-1.9.2.dist-info/RECORD
+11 files, 79791 bytes uncompressed, 16867 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.1.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.1.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.9.2.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.1.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.1.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.1.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -758,14 +758,100 @@
             }}
         with open("a", "w") as fobj:
             fobj.write(str(data))
         act_json = json.dumps(data)
         return act_json
 
 
+class SignAllKPPLiftsWorkerToken(SignAllKPPWorkerToken, mixins.VideoWorkerDB):
+    def __init__(self, sql_shell, platform_id, test=False, mutex=None,
+                 auto_auth=False):
+        super().__init__(sql_shell, mutex=mutex,
+                         platform_id=platform_id, test=test)
+        self.send_kpp_arrival_url = self.get_full_endpoint(
+            "/v1/gravity/passes/incidents/create")
+        self.table_name = "kpp_lifts"
+        self.link_create_act = "/v1/gravity/passes/incidents/create"
+        self.table_id = self.get_table_id_by_name(self.sql_shell, "kpp_arrivals")
+
+    def get_local_id(self, data):
+        return data['id']
+
+    @wsqluse.wsqluse.getTableDictStripper
+    def get_photo_types(self, sql_shell):
+        return sql_shell.get_table_dict(
+            "SELECT id, name FROM photo_types "
+            "WHERE name in ('kpp_internal_lift_up', 'kpp_external_lift_up', "
+            "'kpp_internal_lift_down', 'kpp_external_lift_down')"
+        )
+
+   # def get_photo_path(self, record_id, photo_type):
+
+    @wsqluse.wsqluse.getTableDictStripper
+    def get_unsend_acts(self, record_id=None, limit=None):
+        command = "SELECT id, time_start, time_end, external_video, " \
+                  "internal_video, user_id, notes, alerts," \
+                  "photo_external_start," \
+                  "photo_external_end FROM kpp_lifts WHERE time_end is not null "
+        if record_id:
+            command += f" and id={record_id} "
+        command += "and id NOT IN (SELECT local_id FROM " \
+                   f"ex_sys_data_send_reports WHERE table_id={self.table_id} " \
+                   f"and ex_sys_id = {self.ex_sys_id} and not get is null) "
+        if limit:
+            command += f"and LIMIT {limit}"
+        return self.sql_shell.get_table_dict(command)
+
+    @wsqluse.wsqluse.getTableDictStripper
+    def get_photo_info_by_id(self, photo_id):
+        return self.sql_shell.get_table_dict(
+            f"SELECT * FROM photos WHERE id={photo_id}")
+
+    def format_send_data(self, source, *args, **kwargs):
+        photo_in = source["photo_external_start"]
+        if not photo_in:
+            photo_in = ""
+        else:
+            photo_in_path = self.get_photo_info_by_id(photo_in)[0]["path"]
+            photo_in = self.get_photo_data(photo_in_path)
+        photo_out = source["photo_external_end"]
+        if not photo_out:
+            photo_out = ""
+        else:
+            photo_out_path = self.get_photo_info_by_id(photo_out)[0]["path"]
+            photo_out = self.get_photo_data(photo_out_path)
+        data = {
+            "number": str(source["id"]),
+        "photos":
+            {"photo_in": photo_in,
+             "photo_out": photo_out},
+        "time_in": source["time_start"].strftime("%Y-%m-%d %H:%M:%S"),
+        "time_out": source["time_end"].strftime("%Y-%m-%d %H:%M:%S"),
+        "video": [],
+        }
+        if source["external_video"]:
+            external_video_info = self.get_video_info(source["external_video"])
+            #if external_video_info:
+            vid = external_video_info[0]
+            data["video"].append(
+                {"id": str(vid["id"]),
+                 "label": "external",
+                 "thumb": vid["thumb"]})
+        if source["internal_video"]:
+            internal_video_info = self.get_video_info(source["internal_video"])
+            #if external_video_info:
+            vid = internal_video_info[0]
+            data["video"].append(
+                {"id": str(vid["id"]),
+                 "label": "internal",
+                 "thumb": vid["thumb"]})
+        print(data)
+        data_json = json.dumps(data)
+        return data_json
+
 class ASURoutesWorker(mixins.AsuMixin, DataWorker):
     def __init__(self, sql_shell, asu_login, asu_password, **kwargs):
         self.sql_shell = sql_shell
         self.login = asu_login
         self.password = asu_password
         self.headers = self.get_headers()
```

## ar_external_sys_worker/mixins.py

```diff
@@ -338,19 +338,28 @@
                  operator_comments: dict, photo_in: str,
                  photo_out: str):
         data = locals()
         data.__delitem__('self')
         json_data = json.dumps(data)
         return json_data
 
+class VideoWorkerDB:
+    sql_shell = None
+
+    @wsqluse.wsqluse.getTableDictStripper
+    def get_video_info(self, video_id):
+        return self.sql_shell.get_table_dict(
+            f"SELECT * FROM videos WHERE id={video_id}")
+
 
 class PhotoEncoderMixin:
     def get_photo_data(self, photo_path):
         """ Извлечь из фото последовательность байтов в кодировке base-64 """
         try:
+            print(photo_path)
             with open(photo_path, 'rb') as fobj:
                 photo_data = base64.b64encode(fobj.read())
                 return photo_data
         except FileNotFoundError:
             pass
```

## ar_external_sys_worker/tests/main_test.py

```diff
@@ -20,19 +20,24 @@
     inst = main.SignallActWorker(login=pol_login,
                                  password=pol_pass,
                                  sql_shell=sql_shell,
                                  trash_cats_list=['ТКО', 'ПО', 'Прочее'],
                                  time_start='2021.01.01')
     inst.link_host = 'https://signalltestdev.qodex.tech'
 
+    def test_kpp_lift(self):
+        inst = main.SignAllKPPLiftsWorkerToken(self.sql_shell, 1, test=True)
+        inst.auth()
+        inst.send_unsend_acts(record_id=70)
+        #print(res)
 
+    @unittest.SkipTest
     def test_kpp(self):
         inst = main.SignAllKPPWorkerToken(self.sql_shell, 1, test=True)
         inst.auth()
-        #res = inst.get_unsend_acts()
         inst.send_unsend_acts()
         #print(res)
 
     @unittest.SkipTest
     def test_some(self):
         list_name = ['1', '2']
         command = "SELECT * FROM records WHERE trash_cat IN {} and time_in > '06.05.2022'"
@@ -198,40 +203,24 @@
                                          login='1@signal.com',
                                          password='d4GExhec')
         inst.get_region_operators()
 
     @unittest.SkipTest
     def test_get_platforms(self):
         car_nums = [
-            'О539КН102',
-            '2267УК01',
-            'В106ХУ02',
-            'В662СН702',
-            'Х237ТМ702',
-            'В292МР702',
-            'С496КВ02',
-            'В562УР102',
-            'С543КУ02',
-            'В812ЕА702',
-            'В466КЕ702',
-            'Е909КК702',
-            'С036АУ102',
-            'В417ОУ156',
-            'А069АР702',
-            'У222УУ702',
-            'У222УУ702',
+            'А560СК702',
         ]
         inst = main.ASUActsWorker(self.sql_shell,
                                   trash_cats_list=['ТКО'],
-                                  time_start='2022.04.07',
+                                  time_start='2024.04.07',
                                   login="api", password="qwer1234")
         for car_num in car_nums:
             print('\n')
             print(car_num)
-            res = inst.get_route_info('В292МР702', '05.12.2022')
+            res = inst.get_route_info('А560СК702', '03.04.2024')
             print(res)
 
     @unittest.SkipTest
     def test_mutex(self):
         inst = main.SignAllActsWorkerToken(self.sql_shell,
                                            '2023.04.24',
                                            1,
```

## Comparing `ar_ex_sys_worker-1.9.1.dist-info/LICENSE` & `ar_ex_sys_worker-1.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

