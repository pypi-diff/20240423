# Comparing `tmp/mkmavrykchain-6.25.5-py3-none-any.whl.zip` & `tmp/mkmavrykchain-6.25.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9476 bytes, number of entries: 9
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-04 10:03 mavrykchain/_version.py
--rw-r--r--  2.0 unx     1916 b- defN 24-Apr-04 10:03 mavrykchain/keys.py
--rw-r--r--  2.0 unx    12374 b- defN 24-Apr-04 10:03 mavrykchain/mkmavrykchain.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Apr-04 10:03 mavrykchain/parameters.yaml
--rw-r--r--  2.0 unx     5164 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      753 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/RECORD
-9 files, 23455 bytes uncompressed, 8170 bytes compressed:  65.2%
+Zip file size: 9478 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-23 09:48 mavrykchain/_version.py
+-rw-r--r--  2.0 unx     1916 b- defN 24-Apr-23 09:48 mavrykchain/keys.py
+-rw-r--r--  2.0 unx    12375 b- defN 24-Apr-23 09:48 mavrykchain/mkmavrykchain.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-23 09:48 mavrykchain/parameters.yaml
+-rw-r--r--  2.0 unx     5164 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/RECORD
+9 files, 23456 bytes uncompressed, 8172 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mavrykchain/mkmavrykchain.py
 Comment: 
 
 Filename: mavrykchain/parameters.yaml
 Comment: 
 
-Filename: mkmavrykchain-6.25.5.dist-info/METADATA
+Filename: mkmavrykchain-6.25.6.dist-info/METADATA
 Comment: 
 
-Filename: mkmavrykchain-6.25.5.dist-info/WHEEL
+Filename: mkmavrykchain-6.25.6.dist-info/WHEEL
 Comment: 
 
-Filename: mkmavrykchain-6.25.5.dist-info/entry_points.txt
+Filename: mkmavrykchain-6.25.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.5.dist-info/top_level.txt
+Filename: mkmavrykchain-6.25.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.5.dist-info/RECORD
+Filename: mkmavrykchain-6.25.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mavrykchain/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-04T11:52:15+0200",
+ "date": "2024-04-23T11:46:17+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "78188ae4e7ffb221b0b7f96b61635ea918c13c82",
- "version": "6.25.5"
+ "full-revisionid": "56a783955d53fd40500e5d1c1b618d0859cebed8",
+ "version": "6.25.6"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## mavrykchain/mkmavrykchain.py

```diff
@@ -180,15 +180,15 @@
             "zerotier_token": args.zerotier_token,
         },
         # Custom chains should not pull snapshots or tarballs
         "snapshot_source": None,
         "node_globals": {
             # Needs a quotedstring otherwise helm interprets "Y" as true and it does not work
             "env": {
-                "all": {"TEZOS_CLIENT_UNSAFE_DISABLE_DISCLAIMER": QuotedString("Y")}
+                "all": {"MAVRYK_CLIENT_UNSAFE_DISABLE_DISCLAIMER": QuotedString("Y")}
             }
         },
         "protocols": [
             {
                 "command": "PtNairob",
                 "vote": {"liquidity_baking_toggle_vote": "pass"},
             }
```

## Comparing `mkmavrykchain-6.25.5.dist-info/METADATA` & `mkmavrykchain-6.25.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkmavrykchain
-Version: 6.25.5
+Version: 6.25.6
 Summary: A utility to generate k8s configs for a Mavryk blockchain
 Home-page: https://github.com/mavryk-network/mavryk-k8s
 Author: MavrykDynamics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `mkmavrykchain-6.25.5.dist-info/RECORD` & `mkmavrykchain-6.25.6.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-mavrykchain/_version.py,sha256=vDyA_X5BqullEilFuLRyXKjOoDAzk4gXoQe29_o0NMI,498
+mavrykchain/_version.py,sha256=lHI4KbuOc46_KRsZaDtE_SDqr6k3RPlhfnj4-ZQxyFE,498
 mavrykchain/keys.py,sha256=i_WucWcLv2XoKd-z63Ki4BWis_64VsL-OVrj2hu-Gv0,1916
-mavrykchain/mkmavrykchain.py,sha256=TDBG5gKgusS_o43NV7cC0BDlfWkwakySefIq35P-YSM,12374
+mavrykchain/mkmavrykchain.py,sha256=JYh8EBqiCLJRFsuUywZXqU8tU2ZeprHiRfaU-heL08M,12375
 mavrykchain/parameters.yaml,sha256=7bLg5OtDeWjgTTijnNir2V-nGyFC2aaLJQpQCIRgK90,2580
-mkmavrykchain-6.25.5.dist-info/METADATA,sha256=OF5sLcLdWOUZBQ03VdEEN4vdAK22a4fapk9IUHnht6Y,5164
-mkmavrykchain-6.25.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mkmavrykchain-6.25.5.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
-mkmavrykchain-6.25.5.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
-mkmavrykchain-6.25.5.dist-info/RECORD,,
+mkmavrykchain-6.25.6.dist-info/METADATA,sha256=iBoOH5mC6IZcf0cAZMsLB-jWFYNUcUliS6_-whioRrQ,5164
+mkmavrykchain-6.25.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mkmavrykchain-6.25.6.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
+mkmavrykchain-6.25.6.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
+mkmavrykchain-6.25.6.dist-info/RECORD,,
```

