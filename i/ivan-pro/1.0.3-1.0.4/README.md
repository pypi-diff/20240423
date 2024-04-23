# Comparing `tmp/ivan_pro-1.0.3-py3-none-any.whl.zip` & `tmp/ivan_pro-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 17870 bytes, number of entries: 20
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-22 18:35 ivan/__init__.py
--rw-r--r--  2.0 unx      219 b- defN 24-Mar-22 18:35 ivan/cli.py
--rw-r--r--  2.0 unx      400 b- defN 24-Mar-22 18:35 ivan/plugins/__init__.py
--rw-r--r--  2.0 unx     4211 b- defN 24-Mar-22 18:35 ivan/plugins/database.py
--rw-r--r--  2.0 unx     8153 b- defN 24-Mar-22 18:35 ivan/plugins/dbconfig.py
--rw-r--r--  2.0 unx     3664 b- defN 24-Mar-22 18:35 ivan/plugins/display.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Mar-22 18:35 ivan/plugins/export.py
--rw-r--r--  2.0 unx     9092 b- defN 24-Mar-22 18:35 ivan/plugins/find.py
--rw-r--r--  2.0 unx     8853 b- defN 24-Mar-22 18:35 ivan/plugins/ip.py
--rw-r--r--  2.0 unx     1727 b- defN 24-Mar-22 18:35 ivan/plugins/keys.py
--rw-r--r--  2.0 unx     1131 b- defN 24-Mar-22 18:35 ivan/plugins/query_export.py
--rw-r--r--  2.0 unx     8734 b- defN 24-Mar-22 18:35 ivan/plugins/sc_vuln_export.py
--rw-r--r--  2.0 unx      573 b- defN 24-Mar-22 18:35 ivan/plugins/scan.py
--rw-r--r--  2.0 unx     6987 b- defN 24-Mar-22 18:35 ivan/plugins/scan_evaluation.py
--rw-r--r--  2.0 unx      240 b- defN 24-Mar-22 18:35 ivan/plugins/update.py
--rw-r--r--  2.0 unx     2338 b- defN 24-Mar-22 18:36 ivan_pro-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 18:36 ivan_pro-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 24-Mar-22 18:36 ivan_pro-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-22 18:36 ivan_pro-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1578 b- defN 24-Mar-22 18:36 ivan_pro-1.0.3.dist-info/RECORD
-20 files, 59338 bytes uncompressed, 15316 bytes compressed:  74.2%
+Zip file size: 17700 bytes, number of entries: 20
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 16:35 ivan/__init__.py
+-rw-r--r--  2.0 unx      219 b- defN 24-Apr-23 16:35 ivan/cli.py
+-rw-r--r--  2.0 unx      400 b- defN 24-Apr-23 16:35 ivan/plugins/__init__.py
+-rw-r--r--  2.0 unx     2766 b- defN 24-Apr-23 16:35 ivan/plugins/database.py
+-rw-r--r--  2.0 unx     8153 b- defN 24-Apr-23 16:35 ivan/plugins/dbconfig.py
+-rw-r--r--  2.0 unx     3664 b- defN 24-Apr-23 16:35 ivan/plugins/display.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-23 16:35 ivan/plugins/export.py
+-rw-r--r--  2.0 unx     9092 b- defN 24-Apr-23 16:35 ivan/plugins/find.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-Apr-23 16:35 ivan/plugins/ip.py
+-rw-r--r--  2.0 unx     1727 b- defN 24-Apr-23 16:35 ivan/plugins/keys.py
+-rw-r--r--  2.0 unx     1131 b- defN 24-Apr-23 16:35 ivan/plugins/query_export.py
+-rw-r--r--  2.0 unx     8734 b- defN 24-Apr-23 16:35 ivan/plugins/sc_vuln_export.py
+-rw-r--r--  2.0 unx      573 b- defN 24-Apr-23 16:35 ivan/plugins/scan.py
+-rw-r--r--  2.0 unx     7016 b- defN 24-Apr-23 16:35 ivan/plugins/scan_evaluation.py
+-rw-r--r--  2.0 unx      240 b- defN 24-Apr-23 16:35 ivan/plugins/update.py
+-rw-r--r--  2.0 unx     2338 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1578 b- defN 24-Apr-23 16:53 ivan_pro-1.0.4.dist-info/RECORD
+20 files, 57922 bytes uncompressed, 15146 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: ivan/plugins/scan_evaluation.py
 Comment: 
 
 Filename: ivan/plugins/update.py
 Comment: 
 
-Filename: ivan_pro-1.0.3.dist-info/METADATA
+Filename: ivan_pro-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ivan_pro-1.0.3.dist-info/WHEEL
+Filename: ivan_pro-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ivan_pro-1.0.3.dist-info/entry_points.txt
+Filename: ivan_pro-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ivan_pro-1.0.3.dist-info/top_level.txt
+Filename: ivan_pro-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ivan_pro-1.0.3.dist-info/RECORD
+Filename: ivan_pro-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ivan/plugins/database.py

```diff
@@ -39,43 +39,14 @@
         # end = time.time()
         # total = end - start
     query_conn.close()
     # click.echo("Sql Query took: {} seconds".format(total))
     return data
 
 
-def insert_assets(conn, assets):
-    sql = '''INSERT or IGNORE into assets(
-                                          ip_address, 
-                                          hostname, 
-                                          fqdn, 
-                                          uuid, 
-                                          first_found, 
-                                          last_found, 
-                                          operating_system,
-                                          mac_address, 
-                                          agent_uuid, 
-                                          last_licensed_scan_date, 
-                                          network, 
-                                          acr, 
-                                          aes, 
-                                          aws_id,
-                                          aws_ec2_instance_state,
-                                          aws_ec2_name,
-                                          aws_ec2_region,
-                                          aws_availability_zone,
-                                          gcp_instance_id,
-                                          gcp_project_id,
-                                          gcp_zone,
-                                          url) VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)'''
-    cur = conn.cursor()
-    cur.execute('pragma journal_mode=wal;')
-    cur.execute(sql, assets)
-
-
 def drop_tables(conn, table):
     try:
         drop_table = '''DROP TABLE {}'''.format(table)
         cur = conn.cursor()
         cur.execute('pragma journal_mode=wal;')
         cur.execute(drop_table)
     except Error:
```

## ivan/plugins/scan_evaluation.py

```diff
@@ -16,26 +16,26 @@
 def evaluate_a_scan():
     # Since no scanid was provided we assume the user wants stats on all scans
     click.echo("*" * 100)
     click.echo("\nThis command uses the 19506 plugin data found in the navi.db\n"
                "Run a navi update command to refresh the database.\n")
     click.echo("*" * 100)
     # Pull all 19506 Plugins from the DB
-    plugin_data = db_query("select asset_uuid, output from vulns where plugin_id='19506';")
+    plugin_data = db_query("select asset_ip, asset_uuid, output from vulns where plugin_id='19506';")
 
     # Set some dicts for organizing Data
     scan_policy_dict = {}
     scanner_dict = {}
     scan_name_dict = {}
     scanner_list = []
     # Open a CSV for export
     with open('evaluate.csv', mode='w', encoding='utf-8', newline="") as csv_file:
         agent_writer = csv.writer(csv_file, delimiter=',', quotechar='"')
 
-        header_list = ["asset uuid", "Scan Name", "Scan Policy", "Scanner IP", "Scan Time", "Max Checks", "Max Hosts", "Minutes", "RTT", "Hop Count"]
+        header_list = ["Asset IP Address", "Asset UUID", "Scan Name", "Scan Policy", "Scanner IP", "Scan Time", "Max Checks", "Max Hosts", "Minutes", "RTT", "Hop Count"]
 
         # Write the header to the csv
         agent_writer.writerow(header_list)
 
         # This function is used to parse the data
         # Getting the length of the Category and using it to get the average
         def average_by_policy(name, scan_info):
@@ -65,16 +65,16 @@
 
             click.echo("-" * 150)
 
         # Loop through each plugin 19506 and Parse data from it
         for vulns in plugin_data:
             plugin_dict = {}
 
-            # Output is the second item in the tuple from the DB
-            plugin_output = vulns[1]
+            # Output is the third item in the tuple from the DB
+            plugin_output = vulns[2]
 
             # split the output by return
             parsed_output = plugin_output.split("\n")
 
             for info_line in parsed_output:
                 try:
                     new_split = info_line.split(" : ")
```

## Comparing `ivan_pro-1.0.3.dist-info/METADATA` & `ivan_pro-1.0.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivan-pro
-Version: 1.0.3
+Version: 1.0.4
 Summary: A command-line interface to Tenable Security Center
 Home-page: https://github.com/packetchaos/ivan
 Author: Casey Reid
 Author-email: itprofguru@gmail.com
 License: GNUv3
 Keywords: tenable securitycenter ivan tsc,automation
 Platform: UNKNOWN
```

## Comparing `ivan_pro-1.0.3.dist-info/RECORD` & `ivan_pro-1.0.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ivan/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ivan/cli.py,sha256=3goU3FeQcu6Ux2ECWQiYc0LjDRllAtCwYy25mawaXaQ,219
 ivan/plugins/__init__.py,sha256=AVNOkBZT2BXi0sENXslXbZklM3XAZcB31wih8ssR80A,400
-ivan/plugins/database.py,sha256=I02nMQt0o-1T-4wreWlEv7PKGx6lvxUwO5qfIGIZ_D0,4211
+ivan/plugins/database.py,sha256=RSaabhChewmXYJtWf_DYGwpHi0UPCqzut1OoZLx9FqI,2766
 ivan/plugins/dbconfig.py,sha256=COp-FsyiSVyceCirZ46PwrXwLDK2xMEZzcwzUbFCI4U,8153
 ivan/plugins/display.py,sha256=WkkrXMSzmllpehbzJxEDSmQBmqv54rGOE8R1icLKjyM,3664
 ivan/plugins/export.py,sha256=23UUrM4SkR42NYVcIJYYlW6tm_fmIP3xe1hes1AiWcU,1302
 ivan/plugins/find.py,sha256=qnH1RuwsrNVVaQbXRSkbJiwPs2mjgQsg3bPlaqdqitQ,9092
 ivan/plugins/ip.py,sha256=HjOtoUl7kb1oCaGT_Nkua9kulwuQaATqxd-bzLQLS0s,8853
 ivan/plugins/keys.py,sha256=KC4OXT7Rq7DTR_IgvaoP2BtInyvLvsZQbpA-pb8z7iM,1727
 ivan/plugins/query_export.py,sha256=f4qYQjrQe9hrLHF5OFlX3t6DePiKKVV47XUI7L_QQRc,1131
 ivan/plugins/sc_vuln_export.py,sha256=FD1R0bA9A1ENzsELx3hmT_c-Asdx07hHVpn1bdZnpFA,8734
 ivan/plugins/scan.py,sha256=bNW5SEyvYALeQ-dC2Sc0h9tzotRWh82Pz5zXixdy0zM,573
-ivan/plugins/scan_evaluation.py,sha256=tr-Sv3FS1wbOveXxYRnN34HTrkYi8Vy0BxvTgHq3eTA,6987
+ivan/plugins/scan_evaluation.py,sha256=jxfck1HHbskHZ_vegi1uHYRMu02Sl6EKfW8HnADqTyk,7016
 ivan/plugins/update.py,sha256=3hb9koJrbfFQxbor2WTwD4OLKLa6YC5G_gAsKSvEcJA,240
-ivan_pro-1.0.3.dist-info/METADATA,sha256=2L5K1FBgrwbCvmAmRfmQ8pp2sgzaMloIgdWtiwzElaw,2338
-ivan_pro-1.0.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ivan_pro-1.0.3.dist-info/entry_points.txt,sha256=LL3GUB9cAPkceQ1yevSr2Tol0ti7LnyBI0PBqNjJ810,39
-ivan_pro-1.0.3.dist-info/top_level.txt,sha256=woTedJTvuGD9qW1qtH4DAwO60Ztsxx37Fep0ka6mS-M,5
-ivan_pro-1.0.3.dist-info/RECORD,,
+ivan_pro-1.0.4.dist-info/METADATA,sha256=rIhN30owiuwqYCjleSLGN-GUn-y2l7jq-DyvMJGUgNA,2338
+ivan_pro-1.0.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+ivan_pro-1.0.4.dist-info/entry_points.txt,sha256=LL3GUB9cAPkceQ1yevSr2Tol0ti7LnyBI0PBqNjJ810,39
+ivan_pro-1.0.4.dist-info/top_level.txt,sha256=woTedJTvuGD9qW1qtH4DAwO60Ztsxx37Fep0ka6mS-M,5
+ivan_pro-1.0.4.dist-info/RECORD,,
```

