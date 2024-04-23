# Comparing `tmp/dihlibs-0.0.8.tar.gz` & `tmp/dihlibs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dihlibs-0.0.8.tar", last modified: Fri Feb 16 13:02:06 2024, max compression
+gzip compressed data, was "dihlibs-0.0.9.tar", last modified: Mon Feb 19 05:43:54 2024, max compression
```

## Comparing `dihlibs-0.0.8.tar` & `dihlibs-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/
--rw-r--r--   0 e         (1000) e         (1000)     1189 2024-02-16 13:02:06.462047 dihlibs-0.0.8/PKG-INFO
--rw-r--r--   0 e         (1000) e         (1000)      784 2024-02-07 11:18:33.000000 dihlibs-0.0.8/README.md
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs/
--rw-r--r--   0 e         (1000) e         (1000)        0 2024-01-11 08:34:41.000000 dihlibs-0.0.8/dihlibs/__init__.py
--rw-r--r--   0 e         (1000) e         (1000)     1322 2024-02-15 13:21:34.000000 dihlibs-0.0.8/dihlibs/command.py
--rw-r--r--   0 e         (1000) e         (1000)     1538 2024-01-15 07:05:12.000000 dihlibs-0.0.8/dihlibs/cron_logger.py
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs/data/
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs/data/bash/
--rw-r--r--   0 e         (1000) e         (1000)     2995 2024-02-16 11:56:48.000000 dihlibs-0.0.8/dihlibs/data/bash/script.sh
--rw-r--r--   0 e         (1000) e         (1000)     1164 2024-02-10 17:57:58.000000 dihlibs-0.0.8/dihlibs/data/describe_table.sql
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs/data/docker/
--rw-r--r--   0 e         (1000) e         (1000)    19019 2024-02-16 12:55:02.000000 dihlibs-0.0.8/dihlibs/data/docker/backend.zip
--rw-r--r--   0 e         (1000) e         (1000)     4154 2024-02-16 12:55:02.000000 dihlibs-0.0.8/dihlibs/data/docker/cronies.zip
--rw-r--r--   0 e         (1000) e         (1000)     2492 2024-02-15 14:01:42.000000 dihlibs-0.0.8/dihlibs/db.py
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs/dhis/
--rw-r--r--   0 e         (1000) e         (1000)     9153 2024-02-15 15:12:27.000000 dihlibs-0.0.8/dihlibs/dhis/__init__.py
--rw-r--r--   0 e         (1000) e         (1000)     6440 2024-02-16 09:03:09.000000 dihlibs-0.0.8/dihlibs/dhis/configuration.py
--rw-r--r--   0 e         (1000) e         (1000)     2769 2024-02-07 12:03:02.000000 dihlibs-0.0.8/dihlibs/dhis/dhis_meta.py
--rw-r--r--   0 e         (1000) e         (1000)     4284 2024-02-07 12:03:02.000000 dihlibs-0.0.8/dihlibs/dhis/fill_new_element.py
--rw-r--r--   0 e         (1000) e         (1000)     4903 2024-02-15 14:00:14.000000 dihlibs-0.0.8/dihlibs/dhis/main.py
--rw-r--r--   0 e         (1000) e         (1000)     2984 2024-02-12 08:18:30.000000 dihlibs-0.0.8/dihlibs/drive.py
--rw-r--r--   0 e         (1000) e         (1000)     5719 2024-02-15 11:04:28.000000 dihlibs-0.0.8/dihlibs/functions.py
-drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-16 13:02:06.462047 dihlibs-0.0.8/dihlibs.egg-info/
--rw-r--r--   0 e         (1000) e         (1000)     1189 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/PKG-INFO
--rw-r--r--   0 e         (1000) e         (1000)      579 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/SOURCES.txt
--rw-r--r--   0 e         (1000) e         (1000)        1 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/dependency_links.txt
--rw-r--r--   0 e         (1000) e         (1000)       48 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/entry_points.txt
--rw-r--r--   0 e         (1000) e         (1000)      155 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/requires.txt
--rw-r--r--   0 e         (1000) e         (1000)        8 2024-02-16 13:02:06.000000 dihlibs-0.0.8/dihlibs.egg-info/top_level.txt
--rw-r--r--   0 e         (1000) e         (1000)       38 2024-02-16 13:02:06.462047 dihlibs-0.0.8/setup.cfg
--rw-r--r--   0 e         (1000) e         (1000)     1337 2024-02-16 13:00:03.000000 dihlibs-0.0.8/setup.py
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/
+-rw-r--r--   0 e         (1000) e         (1000)     1189 2024-02-19 05:43:54.262342 dihlibs-0.0.9/PKG-INFO
+-rw-r--r--   0 e         (1000) e         (1000)      784 2024-02-07 11:18:33.000000 dihlibs-0.0.9/README.md
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs/
+-rw-r--r--   0 e         (1000) e         (1000)        0 2024-01-11 08:34:41.000000 dihlibs-0.0.9/dihlibs/__init__.py
+-rw-r--r--   0 e         (1000) e         (1000)     1322 2024-02-15 13:21:34.000000 dihlibs-0.0.9/dihlibs/command.py
+-rw-r--r--   0 e         (1000) e         (1000)     1538 2024-01-15 07:05:12.000000 dihlibs-0.0.9/dihlibs/cron_logger.py
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs/data/
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs/data/bash/
+-rw-r--r--   0 e         (1000) e         (1000)     3364 2024-02-18 12:49:55.000000 dihlibs-0.0.9/dihlibs/data/bash/script.sh
+-rw-r--r--   0 e         (1000) e         (1000)     1164 2024-02-10 17:57:58.000000 dihlibs-0.0.9/dihlibs/data/describe_table.sql
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs/data/docker/
+-rw-r--r--   0 e         (1000) e         (1000)    22081 2024-02-19 04:51:20.000000 dihlibs-0.0.9/dihlibs/data/docker/backend.zip
+-rw-r--r--   0 e         (1000) e         (1000)     4155 2024-02-19 04:51:20.000000 dihlibs-0.0.9/dihlibs/data/docker/cronies.zip
+-rw-r--r--   0 e         (1000) e         (1000)     2492 2024-02-15 14:01:42.000000 dihlibs-0.0.9/dihlibs/db.py
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs/dhis/
+-rw-r--r--   0 e         (1000) e         (1000)     9153 2024-02-15 15:12:27.000000 dihlibs-0.0.9/dihlibs/dhis/__init__.py
+-rw-r--r--   0 e         (1000) e         (1000)     7014 2024-02-19 05:19:16.000000 dihlibs-0.0.9/dihlibs/dhis/configuration.py
+-rw-r--r--   0 e         (1000) e         (1000)     2769 2024-02-07 12:03:02.000000 dihlibs-0.0.9/dihlibs/dhis/dhis_meta.py
+-rw-r--r--   0 e         (1000) e         (1000)     4284 2024-02-07 12:03:02.000000 dihlibs-0.0.9/dihlibs/dhis/fill_new_element.py
+-rw-r--r--   0 e         (1000) e         (1000)     4903 2024-02-15 14:00:14.000000 dihlibs-0.0.9/dihlibs/dhis/main.py
+-rw-r--r--   0 e         (1000) e         (1000)     2984 2024-02-12 08:18:30.000000 dihlibs-0.0.9/dihlibs/drive.py
+-rw-r--r--   0 e         (1000) e         (1000)     5789 2024-02-18 15:10:48.000000 dihlibs-0.0.9/dihlibs/functions.py
+drwxr-xr-x   0 e         (1000) e         (1000)        0 2024-02-19 05:43:54.262342 dihlibs-0.0.9/dihlibs.egg-info/
+-rw-r--r--   0 e         (1000) e         (1000)     1189 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/PKG-INFO
+-rw-r--r--   0 e         (1000) e         (1000)      579 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 e         (1000) e         (1000)        1 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 e         (1000) e         (1000)       48 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/entry_points.txt
+-rw-r--r--   0 e         (1000) e         (1000)      155 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/requires.txt
+-rw-r--r--   0 e         (1000) e         (1000)        8 2024-02-19 05:43:54.000000 dihlibs-0.0.9/dihlibs.egg-info/top_level.txt
+-rw-r--r--   0 e         (1000) e         (1000)       38 2024-02-19 05:43:54.262342 dihlibs-0.0.9/setup.cfg
+-rw-r--r--   0 e         (1000) e         (1000)     1337 2024-02-19 05:36:40.000000 dihlibs-0.0.9/setup.py
```

### Comparing `dihlibs-0.0.8/PKG-INFO` & `dihlibs-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dihlibs
-Version: 0.0.8
+Version: 0.0.9
 Summary: A helper package for data integrations
 Home-page: https://github.com/nKataraia/dihlibs
 Author: Nitu
 Author-email: nkataraia@d-tree.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dihlibs-0.0.8/README.md` & `dihlibs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/command.py` & `dihlibs-0.0.9/dihlibs/command.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/cron_logger.py` & `dihlibs-0.0.9/dihlibs/cron_logger.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/data/bash/script.sh` & `dihlibs-0.0.9/dihlibs/data/bash/script.sh`

 * *Files 14% similar despite different names*

```diff
@@ -40,54 +40,67 @@
 function strong_password() {
     trim <<-CODE | python
     import dihlibs.functions as fn
     print(fn.strong_password($1))
 CODE
 }
 
+function turn_on_cron_container(){
+    echo turning on dhis containers
+    docker-compose -f .cache/docker/cronies/docker-compose.yml up -d 2>&1
+}
+
+function turn_on_dhis_containers(){
+    echo turning on dhis containers
+    docker-compose -f .cache/docker/backend/dhis/"$1"-compose.yml up -d 2>&1
+}
+
+
 function deploy_cron() {
     file="${1%/}"
+    temp=$(mktemp -d)
+    
+    loc="$(dirname $file)"
+    [[ $loc == "." ]] && loc=$PWD;
+    proj="${loc##*/}"
+    file=${file##*/}
     folder="${file%.zip.enc}"
+
+    cp -r $loc/.* $loc/*  $temp/
+    cd $temp
+
     [ -d "$file" ] || decrypt "$file" <.env
     user="$(yq .dih_user -r <"$folder"/config.yaml)"
     cron_time="$(yq .cronies.cron_time -r <"$folder"/config.yaml)"
+    sed -ri "s/(dhis_url.*)localhost([^@]*$)?/\1${folder}-dhis:8080\2/g" "$folder/config.yaml"
     encrypt "$folder" <.env
-    proj="${PWD##*/}"
-
-    for x in {.cache,sql,$file}; do
-        docker cp ./$n "dih-cronies:/dih/cronies/${proj}"
+    
+    echo "local ni $loc"
+    docker exec dih-cronies mkdir -p "/dih/cronies/${proj}"
+    for x in {.cache,sql,$file,.env}; do
+        docker cp ./$x "dih-cronies:/dih/cronies/${proj}"
     done
     docker exec -i dih-cronies bash <<-CMD
         id -u $user || useradd -m -s /bin/bash -g dih $user
         chown -R $user /dih/cronies/${proj}
         runuser -u $user -- bash -c "{ crontab -l; echo '$cron_time' run "${proj}" ${file} ; } | crontab - "
 CMD
 
+    rm -rf $temp
+
     echo done deployment of $proj
 }
 
-# function remove_cron() {
-#     file="${1%/}"
-#     folder="${file%.zip.enc}"
-#      || decrypt "$file" <.env
-#     user="$(yq .user -r <"$folder"/config.yaml)"
-#     cron_time="$(yq .cron_time -r <"$folder"/config.yaml)"
-#     encrypt "$folder" <.env
-#     proj=$(dirname .env)
-
-#     docker exec -u "$user" dih-cronies bash -c 'crontab -l | grep -vE "\b'"$1"'\$" | crontab -' &&
-#         docker exec dih-cronies rm -r "$folder"
-# }
-
 function perform() {
     case $1 in
     deploy) deploy_cron $2 ;;
     encrypt) encrypt $2 ;;
     decrypt) decrypt $2 ;;
-    logs) docker-compose -f $2 logs -f & ;;
+    dhis-log*) docker-compose -f .cache/docker/backend/dhis/"${2%.zip.enc}"-compose.yml logs -f ;;
+    cron-log*) docker-compose -f .cache/docker/cronies/docker-compose.yml logs -f ;;
     down) docker-compose -f $2 down ;;
     stop) docker ps | grep "$2" | awk '{print $1}' | xargs docker stop ;;
     rm) docker container ls -a | awk '{print $1}' | xargs docker stop | xargs docker rm ;;
     esac
 }
 
 function create_shared_docker_resources() {
```

### Comparing `dihlibs-0.0.8/dihlibs/data/describe_table.sql` & `dihlibs-0.0.9/dihlibs/data/describe_table.sql`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/data/docker/backend.zip` & `dihlibs-0.0.9/dihlibs/data/docker/backend.zip`

 * *Files 16% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                     19019 (0000000000004A4Bh)
-  Actual end-cent-dir record offset:         18997 (0000000000004A35h)
-  Expected end-cent-dir record offset:       18997 (0000000000004A35h)
+  Zip archive file size:                     22081 (0000000000005641h)
+  Actual end-cent-dir record offset:         22059 (000000000000562Bh)
+  Expected end-cent-dir record offset:       22059 (000000000000562Bh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 18 entries.
-  The central directory is 1737 (00000000000006C9h) bytes long,
+  central directory contains 21 entries.
+  The central directory is 2034 (00000000000007F2h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 17260 (000000000000436Ch).
+  is 20025 (0000000000004E39h).
 
 
 Central directory entry #1:
 ---------------------------
 
   backend/
 
@@ -355,20 +355,20 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 16 11:35:06
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:35:05 local
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:35:05 UTC
-  32-bit CRC value (hex):                         c5b0c6d7
-  compressed size:                                357 bytes
-  uncompressed size:                              561 bytes
+  file last modified on (DOS date/time):          2024 Feb 18 13:29:12
+  file last modified on (UT extra field modtime): 2024 Feb 18 10:29:11 local
+  file last modified on (UT extra field modtime): 2024 Feb 18 10:29:11 UTC
+  32-bit CRC value (hex):                         375defcb
+  compressed size:                                359 bytes
+  uncompressed size:                              564 bytes
   length of filename:                             31 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -382,16 +382,16 @@
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
   backend/dhis/compose/example.env
 
-  offset of local header from start of archive:   11454
-                                                  (0000000000002CBEh) bytes
+  offset of local header from start of archive:   11456
+                                                  (0000000000002CC0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -419,30 +419,30 @@
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
   backend/dhis/compose/compose-template.yml
 
-  offset of local header from start of archive:   11737
-                                                  (0000000000002DD9h) bytes
+  offset of local header from start of archive:   11739
+                                                  (0000000000002DDBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 16 11:13:46
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:13:46 local
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:13:46 UTC
-  32-bit CRC value (hex):                         62ca22df
-  compressed size:                                395 bytes
-  uncompressed size:                              1410 bytes
+  file last modified on (DOS date/time):          2024 Feb 17 19:26:58
+  file last modified on (UT extra field modtime): 2024 Feb 17 16:26:58 local
+  file last modified on (UT extra field modtime): 2024 Feb 17 16:26:58 UTC
+  32-bit CRC value (hex):                         a2c6322e
+  compressed size:                                398 bytes
+  uncompressed size:                              1434 bytes
   length of filename:                             41 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -456,26 +456,26 @@
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
   backend/dhis/start/
 
-  offset of local header from start of archive:   12231
-                                                  (0000000000002FC7h) bytes
+  offset of local header from start of archive:   12236
+                                                  (0000000000002FCCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 15 04:12:04
-  file last modified on (UT extra field modtime): 2024 Feb 15 01:12:03 local
-  file last modified on (UT extra field modtime): 2024 Feb 15 01:12:03 UTC
+  file last modified on (DOS date/time):          2024 Feb 18 12:50:58
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:50:57 local
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:50:57 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             19 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -492,16 +492,16 @@
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
   backend/dhis/start/postgresql.sh
 
-  offset of local header from start of archive:   12308
-                                                  (0000000000003014h) bytes
+  offset of local header from start of archive:   12313
+                                                  (0000000000003019h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -527,32 +527,69 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
+  backend/dhis/start/before.json
+
+  offset of local header from start of archive:   13571
+                                                  (0000000000003503h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Feb 18 12:46:28
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:46:28 local
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:46:28 UTC
+  32-bit CRC value (hex):                         a89f0a7f
+  compressed size:                                587 bytes
+  uncompressed size:                              2171 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #16:
+---------------------------
+
   backend/dhis/start/dhis.sh
 
-  offset of local header from start of archive:   13566
-                                                  (00000000000034FEh) bytes
+  offset of local header from start of archive:   14246
+                                                  (00000000000037A6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 16 11:11:10
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:11:10 local
-  file last modified on (UT extra field modtime): 2024 Feb 16 08:11:10 UTC
-  32-bit CRC value (hex):                         5a3bb356
-  compressed size:                                1419 bytes
-  uncompressed size:                              3509 bytes
+  file last modified on (DOS date/time):          2024 Feb 19 07:50:46
+  file last modified on (UT extra field modtime): 2024 Feb 19 04:50:46 local
+  file last modified on (UT extra field modtime): 2024 Feb 19 04:50:46 UTC
+  32-bit CRC value (hex):                         e43d5dcc
+  compressed size:                                1699 bytes
+  uncompressed size:                              4515 bytes
   length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -561,21 +598,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #17:
 ---------------------------
 
   backend/dhis/start/nginx.sh
 
-  offset of local header from start of archive:   15069
-                                                  (0000000000003ADDh) bytes
+  offset of local header from start of archive:   16029
+                                                  (0000000000003E9Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -598,21 +635,58 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #18:
+---------------------------
+
+  backend/dhis/start/run.ipynb
+
+  offset of local header from start of archive:   16776
+                                                  (0000000000004188h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Feb 18 12:46:12
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:46:12 local
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:46:12 UTC
+  32-bit CRC value (hex):                         ee4a9a10
+  compressed size:                                1016 bytes
+  uncompressed size:                              3859 bytes
+  length of filename:                             28 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #19:
 ---------------------------
 
   backend/dhis/start/common.sh
 
-  offset of local header from start of archive:   15816
-                                                  (0000000000003DC8h) bytes
+  offset of local header from start of archive:   17878
+                                                  (00000000000045D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -635,43 +709,80 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #20:
 ---------------------------
 
   backend/dhis/start/letsencrypt.sh
 
-  offset of local header from start of archive:   16184
-                                                  (0000000000003F38h) bytes
+  offset of local header from start of archive:   18246
+                                                  (0000000000004746h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 15 22:18:50
-  file last modified on (UT extra field modtime): 2024 Feb 15 19:18:49 local
-  file last modified on (UT extra field modtime): 2024 Feb 15 19:18:49 UTC
-  32-bit CRC value (hex):                         b1a71f6c
-  compressed size:                                985 bytes
-  uncompressed size:                              2621 bytes
+  file last modified on (DOS date/time):          2024 Feb 17 19:02:00
+  file last modified on (UT extra field modtime): 2024 Feb 17 16:01:59 local
+  file last modified on (UT extra field modtime): 2024 Feb 17 16:01:59 UTC
+  32-bit CRC value (hex):                         dff18db1
+  compressed size:                                990 bytes
+  uncompressed size:                              2644 bytes
   length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #21:
+---------------------------
+
+  backend/dhis/start/after.json
+
+  offset of local header from start of archive:   19327
+                                                  (0000000000004B7Fh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Feb 18 12:50:58
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:50:57 local
+  file last modified on (UT extra field modtime): 2024 Feb 18 09:50:57 UTC
+  32-bit CRC value (hex):                         2e647a98
+  compressed size:                                611 bytes
+  uncompressed size:                              2294 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
```

#### zipnote {}

```diff
@@ -36,20 +36,29 @@
 
 Filename: backend/dhis/start/
 Comment: 
 
 Filename: backend/dhis/start/postgresql.sh
 Comment: 
 
+Filename: backend/dhis/start/before.json
+Comment: 
+
 Filename: backend/dhis/start/dhis.sh
 Comment: 
 
 Filename: backend/dhis/start/nginx.sh
 Comment: 
 
+Filename: backend/dhis/start/run.ipynb
+Comment: 
+
 Filename: backend/dhis/start/common.sh
 Comment: 
 
 Filename: backend/dhis/start/letsencrypt.sh
 Comment: 
 
+Filename: backend/dhis/start/after.json
+Comment: 
+
 Zip file comment:
```

#### backend/dhis/compose/Dockerfile

```diff
@@ -1,10 +1,10 @@
 FROM debian:bullseye
 
-RUN apt-get update && apt-get -y install apt-utils wget vim curl xz-utils cron procps  netcat libterm-readline-gnu-perl
+RUN apt-get update && apt-get -y install apt-utils wget vim curl xz-utils jq cron procps  netcat libterm-readline-gnu-perl
 
 #openjdk-11-jre-headless netcat nginx postgresql postgis postgresql-contrib --fix-missing;
 RUN ln -sf /usr/share/zoneinfo/Africa/Nairobi /etc/localtime
 RUN groupadd dih
 
 
 ENV PATH="${PATH}:/dih/bin:/dih/lib/python/bin"
```

#### backend/dhis/compose/compose-template.yml

```diff
@@ -8,15 +8,15 @@
     container_name: ${proj}-dhis-db
     env_file:
       - ${env_file}  
     volumes: 
       - ${proj}-db:/var/lib/postgresql/data
       - ${proj}-db:/var/run/postgresql
       - ${proj}-common:/${proj}/common/
-      - .cache:/data/.backup/:ro
+      - ../../../../.cache:/data/.backup/:ro
     entrypoint: bash postgresql.sh
     networks:
       - dih-network
 
   ${proj}-dhis-web:
     image: dhis-base
     container_name: ${proj}-dhis-web
@@ -43,15 +43,15 @@
     env_file:
       - ${env_file}  
     networks:
       - dih-network
     volumes:
       - ${proj}-db:/var/run/postgresql
       - ${proj}-common:/${proj}/common/
-      - .cache:/data/.backup/:ro
+      - ../../../../.cache:/data/.backup/:ro
 
 volumes:
   ${proj}-db:
     driver: local
     name: ${proj}-db-volume
 
   ${proj}-common:
```

#### backend/dhis/start/dhis.sh

```diff
@@ -2,15 +2,15 @@
 
 source common.sh
 
 setup_tomcat() {
 
     [ -d /opt/tomcat ] && return
 
-    apt-get install -y openjdk-11-jre-headless  --fix-missing
+    apt-get install -y openjdk-11-jre-headless --fix-missing
 
     echo 'setting up tomcat'
     mkdir -p /opt/tomcat/ && cd /opt/tomcat
     url="https://dlcdn.apache.org/tomcat/tomcat-${tomcat_version:-9}"
     version=$(curl "$url/" -L 2>/dev/null | grep -Po '>v\K[^></]+' | sort | tail -1)
     wget -O apache-tomcat.tar.gz --progress=dot:giga "$url/v$version/bin/apache-tomcat-$version.tar.gz"
     tar xfz apache*.tar.gz && mv apache-tomcat*/* /opt/tomcat/.
@@ -40,58 +40,84 @@
         sed -ri "s/connection.password.*/connection.password = $dhis_password/g" /home/dhis/config/dhis.conf
         unset dhis_password
     fi
     wget --progress=dot:giga -O ROOT.war ${dhis_war}
     mv ROOT.war /opt/tomcat/webapps/ROOT.war
 }
 
-admin_pass=$dhis_admin_password
-set_admin_password() {
-
-    [ -z $dhis_admin_password ] && return
-
-    echo "attempt to change the dhis admin password away from the default one"
-    auth="admin:district"
-    url='http://localhost:8080/api/users'
-    user_id=$(curl -s -u $auth $url?filter=code:eq:admin | grep -Po 'id\W+\K\w+')
-
-    [ -n $admin_pass ] &&
-        curl -s -u $auth $url/$user_id |
+fetch() {
+    endpoint="$1" filter="$2"
+    auth="admin:${3:-$dhis_admin_password}"
+    url='http://localhost:8080/api'
+    id=$(curl -s -u $auth "$url/$endpoint"?filter="$filter" | jq -r ".$endpoint[0].id")
+    curl -s -u $auth "$url/$endpoint/$id"
+}
+
+put() {
+    endpoint="$1"
+    read -r data
+    auth="admin:${2:-$dhis_admin_password}"
+    id=$(echo $data | jq .id -r)
+    url='http://localhost:8080/api'
+    echo $data | curl -s -u $auth -X PUT -H "Content-type: application/json" $url/$endpoint/$id -d @- | {
+        read results
+        echo "$results" | grep -qP '\bOK\b' || (echo "$results" && return 1)
+    }
+}
+
+change_admin_org() {
+    org_id=$(fetch 'organisationUnits' 'level:eq:1' | jq -r .id)
+    org_perms='{
+        "organisationUnits": [{ "id": "'"$org_id"'" }],
+        "dataViewOrganisationUnits": [{ "id": "'"$org_id"'" }],
+        "teiSearchOrganisationUnits": [{ "id": "'"$org_id"'" }]
+    }'
+    echo $(fetch 'users' 'code:eq:admin' | jq ".+=$org_perms") | put "users"
+    [ $? -eq 0 ] && echo 'successfully changed admin orgs' || echo ' could not change admin orgs'
+}
+
+change_admin_password() {
+    #anchoring password field to same parent as previousPasswords field so since the path changes accroding to DHIS2 instance
+    fetch users code:eq:admin "district" |
         sed -r "s/\"previousPasswords/\"password\":\"$dhis_admin_password\",\"previousPasswords/g" |
-            curl -u $auth -sX PUT -H "Content-type: application/json" $url/$user_id -d @- |
-            grep -qP '\bOK\b' && echo "successfully changed admin password" || echo "could not change password reusing the default"
-    unset dhis_admin_password
+        put "users" "district"
+    [ $? -eq 0 ] && echo 'successfully changed admin password' || echo ' could not change admin password'
 }
 
 ask_postgresql_to_change_admin_password() {
     echo change | nc -q 2 ${proj}-dhis_db 12345
 }
 
 import_metadata() {
-    [ ! -f /data/.backup/metadata.json ] && return
-    curl -H 'Content-Type: application/json' \
-        -u "admin:$admin_pass" \
-        -d @/data/.backup/metadata.json http://localhost:8080/api/metadata &&
-        curl -H 'Content-Type: application/json' \
-            -u "admin:$admin_pass" \
+    [ -f /data/.backup/metadata.json ] &&
+        echo 'uploading metadata from metadata.json' &&
+        curl -s -H 'Content-Type: application/json' \
+            -u "admin:$dhis_admin_password" \
+            -d @/data/.backup/metadata.json http://localhost:8080/api/metadata
+
+    [ $? -eq 0 ] && [ -f /data/.backup/data_set.json ] &&
+        echo 'uploading data_sets from data_set.json' &&
+        curl -s -H 'Content-Type: application/json' \
+            -u "admin:$dhis_admin_password" \
             -d @/data/.backup/data_set.json http://localhost:8080/api/metadata &&
         rm -rf /data.backup/metadata.json
 }
 
 on_war_deployed() {
     echo -e "\033[1;30m turning logs grayish till when war is released"
     while read -r line; do
-        if echo "$line" | grep -q 'Deployment of.*[/]ROOT.war.* has finished'; then
+        if echo "$line" | grep -qE 'Deployment of.*[/]ROOT.war.* has finished'; then
             echo "***** $line"
-            set_admin_password &&
+            change_admin_password &&
                 import_metadata
+            change_admin_org
             # && ask_postgresql_to_change_admin_password
             echo -e "\033[0m"
         else
-            echo $line
+            echo "$line"
         fi
     done < <(/opt/tomcat/bin/catalina.sh run 2>&1 &) && echo "War deployed"
 }
 
 wait_for_db_setup_first() {
     echo 'waiting for dhis2 database to be set'
     while read -r line && [[ $line != "dhis2_database_set" ]]; do echo "receive $line"; done < <(nc -l -p 12345)
```

#### backend/dhis/start/letsencrypt.sh

```diff
@@ -5,15 +5,16 @@
 function notify_nginx() {
     echo $1 | nc -q 2 localhost 12345
 }
 
 function setup_python() {
     quiet python --version && return
     echo setting up python
-    here=$(pwd) && cd /dih/lib
+    here=$(pwd) && mkdir -p /dih/lib;
+    cd /dih/lib
     url="https://storage.googleapis.com/py-binary/python-3.11.3.tar.xz"; 
     wget --no-check-certificate -O /dih/lib/python-3.11.3.tar.xz --progress=dot:giga "$url"
     quiet tar -xf python*xz
     ln -s /dih/lib/python/bin/pip3 /dih/bin/pip &&
         ln -s /dih/lib/python/bin/python3 /dih/bin/python
     echo setting up python $(pwd)
     cd $here
```

### Comparing `dihlibs-0.0.8/dihlibs/data/docker/cronies.zip` & `dihlibs-0.0.9/dihlibs/data/docker/cronies.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4154 bytes, number of entries: 8
+Zip file size: 4155 bytes, number of entries: 8
 drwxr-xr-x  3.0 unx        0 bx stor 24-Feb-15 15:26 cronies/
 drwxr-xr-x  3.0 unx        0 bx stor 24-Feb-16 12:44 cronies/bin/
 -rw-r--r--  3.0 unx      818 tx defN 24-Feb-15 01:41 cronies/bin/start.sh
 -rw-r--r--  3.0 unx     4678 tx defN 24-Feb-15 19:26 cronies/bin/functions.sh
 -rw-r--r--  3.0 unx      184 tx defN 24-Feb-16 12:20 cronies/bin/run.sh
 -rw-r--r--  3.0 unx       98 tx defN 24-Feb-15 01:41 cronies/.dockerignore
--rw-r--r--  3.0 unx      656 tx defN 24-Feb-16 12:48 cronies/Dockerfile
+-rw-r--r--  3.0 unx      660 tx defN 24-Feb-17 13:22 cronies/Dockerfile
 -rw-r--r--  3.0 unx      429 tx defN 24-Feb-16 12:47 cronies/docker-compose.yml
-8 files, 6863 bytes uncompressed, 2814 bytes compressed:  59.0%
+8 files, 6867 bytes uncompressed, 2815 bytes compressed:  59.0%
```

#### cronies/Dockerfile

```diff
@@ -7,12 +7,12 @@
 WORKDIR /dih
 ENV PATH="${PATH}:/dih/bin:/dih/lib/python/bin"
 COPY --chown=root:dih bin/*.sh bin/
 WORKDIR /dih/cronies
 RUN mkdir -p /dih/common /dih/lib \
     && chown :dih -R /dih \
     && chmod  770 -R /dih \
-    && mv  /dih/bin/start.sh /dih/bin/start
-    && mv  /dih/bin/run.sh /dih/bin/run
+    && mv  /dih/bin/start.sh /dih/bin/start \
+    && mv  /dih/bin/run.sh /dih/bin/run \
     && find /dih -type f -exec chmod  660 {} \; \
     && chmod +x /dih/bin/* 
 ENTRYPOINT  /dih/bin/start
```

### Comparing `dihlibs-0.0.8/dihlibs/db.py` & `dihlibs-0.0.9/dihlibs/db.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/dhis/__init__.py` & `dihlibs-0.0.9/dihlibs/dhis/__init__.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/dhis/configuration.py` & `dihlibs-0.0.9/dihlibs/dhis/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os, sys, re,json
+import os, sys, re, json
 import pandas as pd
 import sqlalchemy
 import requests, asyncio
 from functools import partial
 import argparse
 
 from dihlibs.dhis import DHIS, UploadSummary
 from dihlibs import functions as fn
 from dihlibs import cron_logger as logger
 from dihlibs import drive as gd
 import pkg_resources as pkr
-import shlex, shutil,tempfile,yaml
+import shlex, shutil, tempfile, yaml
 
 
 class Configuration:
     def __init__(self):
         self.conf = self._load()
         action = self.get("action")
         if action is None:
@@ -29,63 +29,66 @@
             self.create_cron_compose()
             exit(0)
 
         else:
             data = fn.read_non_blocking([sys.stdin.fileno(), sys.stderr.fileno()])
             data_input = f"<<<{shlex.quote(data)}" if data else ""
             command = f"perform {action} {self.get('config-file')} {data_input}"
-            print(command)
-            output = fn.cmd_wait(command)
-            print(output)
+            fn.cmd_wait(command,verbose=True)
             exit(0)
 
     def _load(self):
         args = self._get_commandline_args()
-        if args.get('action'):
+        if args.get("action"):
             return args
 
         file = args.get("config-file")
         folder = file.replace(".zip.enc", "")
-        self.conf=args
+        self.conf = args
         conf = self._get_conf(args)
         c = conf["cronies"]
         c["action"] = args.get("action")
         c["country"] = conf["country"]
-        # c["ssh"] = c.get("tunnel_ssh", "echo No ssh command") 
+        # c["ssh"] = c.get("tunnel_ssh", "echo No ssh command")
         c["month"] = fn.parse_month(args.get("month", fn.get_month(-1)))
         c["selection"] = args.get("selection")
         c["task_dir"] = os.path.basename(os.getcwd())
         c["config-file"] = args.get("config-file")
         c["config-folder"] = args.get("config-file").replace(".zip.enc", "")
         return c
 
+    def pick_config_file(self, args):
+        if args.get("config-file") is None:
+            file = next(filter(lambda x: "zip.enc" in x, os.listdir()), "no-file")
+        else:
+            file = args.get("config-file")
+        return file
+
     def _get_commandline_args(self):
         parser = argparse.ArgumentParser(
             description="For moving data from postgresql warehouse to dhis2"
         )
         parser.add_argument("-m", "--month", type=str, help="Date in format YYYY-MM")
         parser.add_argument("-s", "--selection", type=str, help="Element Selection")
+        parser.add_argument("-a", "--action", type=str, help="do various functions")
         parser.add_argument(
             "config-file",
             nargs="?",
-            default="secret.zip.enc",
+            # default="secret.zip.enc",
             help="Configuration File path",
         )
-        parser.add_argument(
-            "-a", "--action", type=str, help="Perform one of various functions "
-        )
         args = vars(parser.parse_args())  # Convert args to dictionary
-        file=args.get('config-file')
-        args['config-file'] = file[:-1] if file[-1] == "/" else file
+        args["config-file"] = self.pick_config_file(args)
+        args["config-folder"] = args.get("config-file").replace(".zip.enc", "")
         return {k: v for k, v in args.items() if v is not None}
 
     def _get_mappings(self, conf):
         log = logger.get_logger_task(conf.get("task_dir"))
         log.info("seeking mapping file from google drive ....")
-        drive = gd.Drive(json.loads(self.get_file('google.json')))
+        drive = gd.Drive(json.loads(self.get_file("google.json")))
         excel = drive.get_excel(conf.get("data_element_mapping"))
 
         emap = pd.read_excel(excel, "data_elements")
         emap.dropna(subset=["db_column", "element_id"], inplace=True)
         emap["map_key"] = emap.db_view + "_" + emap.db_column
         emap = emap.set_index("map_key")
         emap = self._apply_element_selection(conf, emap)
@@ -95,29 +98,30 @@
         to_skip = ["skip", "deleted", "deprecated", "false", "ruka", "ficha"]
         selection = conf.get("selection")
         if selection:
             return emap[(emap.selection.isin(selection.strip().split(" ")))]
         else:
             return emap[~emap.selection.isin(to_skip)]
 
-    def get(self, what: str,default=None):
-        return self.conf.get(what,default)
+    def get(self, what: str, default=None):
+        return self.conf.get(what, default)
 
     def _get_conf(self, args):
         file = args.get("config-file")
         folder = file.replace(".zip.enc", "")
         if os.path.isdir(folder):
             conf = fn.file_dict(f"{folder}/config.yaml")
-            if args.get('action') != 'encrypt':
-                print(fn.cmd_wait(f" strong_password 64 > .env && encrypt {folder} < .env "))
-                args['config-file']=f'{file}.zip.enc'
-                conf['config-file']=f'{file}.zip.enc'
-            return conf;
+            if args.get("action") != "encrypt":
+                command = f" strong_password 64 > .env && encrypt {folder} < .env "
+                print(fn.cmd_wait(command))
+                args["config-file"] = f"{file}.zip.enc"
+                conf["config-file"] = f"{file}.zip.enc"
+            return conf
         else:
-            return yaml.safe_load(self.get_file('config.yaml'))
+            return yaml.safe_load(self.get_file("config.yaml"))
 
     def get_backend_conf(self):
         args = self._get_commandline_args()
         dih_conf = self._get_conf(args)
         conf = fn.get(dih_conf, "backends.dhis")
         conf.update(
             {
@@ -126,35 +130,42 @@
                 "dih_user": dih_conf.get("dih_user"),
                 "env_file": f'compose/{self.get("config-folder")}.env',
             }
         )
         return {k.strip(): v.strip() for k, v in conf.items()}
 
     def create_cron_compose(self):
-        os.makedirs('docker/cronies', exist_ok=True)
+        os.makedirs(".cache/docker/cronies", exist_ok=True)
         cronies = pkr.resource_filename("dihlibs", "data/docker/cronies.zip")
-        fn.cmd_wait(f"cd docker && cp {cronies} . && unzip -o cronies.zip -d . && rm cronies.zip ")
-        fn.to_file('docker/cronies/.env',f'proj={self.get("config-folder")}')
+
+        command = f"cd .cache/docker && cp {cronies} . && unzip -o cronies.zip -d . && rm cronies.zip "
+        fn.cmd_wait(command)
+        fn.to_file(".cache/docker/cronies/.env", f'proj={self.get("config-folder")}')
+        fn.cmd_wait("turn_on_cron_container",verbose=True)
 
     def create_dhis_compose(self):
-        os.makedirs('docker/backend', exist_ok=True)
+        os.makedirs(".cache/docker/backend", exist_ok=True)
+        print('changes hapa')
         # create compose file
         backend = pkr.resource_filename("dihlibs", "data/docker/backend.zip")
-        fn.cmd_wait(f"cd docker && cp {backend}  . && unzip -o backend.zip -d . && rm backend.zip ")
-        comp = fn.file_text(f"docker/backend/dhis/compose/compose-template.yml")
+        command = f"cd .cache/docker && cp {backend}  . && unzip -o backend.zip -d . && rm backend.zip "
+        fn.cmd_wait(command)
+        comp = fn.file_text(f".cache/docker/backend/dhis/compose/compose-template.yml")
         conf = self.get_backend_conf()
         for key, value in conf.items():
             comp = comp.replace(f"${{{key}}}", value)
-        fn.to_file(f"docker/backend/dhis/{conf.get('proj')}-compose.yml", comp)
+        fn.to_file(f".cache/docker/backend/dhis/{conf.get('proj')}-compose.yml", comp)
         # create env file
         entries = [f"{k}={v}" for k, v in conf.items()]
-        fn.lines_to_file(f'docker/backend/dhis/{conf.get("env_file")}', entries)
+        fn.lines_to_file(f'.cache/docker/backend/dhis/{conf.get("env_file")}', entries)
+        #turn on containers right away
+        command=f'turn_on_dhis_containers {conf.get("proj")}'
+        fn.cmd_wait(command,verbose=True)
 
-    def get_file(self,filename):
+    def get_file(self, filename):
         file = self.get("config-file")
         with tempfile.TemporaryDirectory() as temp_dir:
             temp = os.path.join(temp_dir, file)
             shutil.copy(file, temp)
-            password=shlex.quote(fn.file_text('.env'));
+            password = shlex.quote(fn.file_text(".env"))
             print(fn.cmd_wait(f"cd {temp_dir} && decrypt {temp} <<<{password}"))
-            return fn.file_text(temp.replace(".zip.enc", "/"+filename))
-        
+            return fn.file_text(temp.replace(".zip.enc", "/" + filename))
```

### Comparing `dihlibs-0.0.8/dihlibs/dhis/dhis_meta.py` & `dihlibs-0.0.9/dihlibs/dhis/dhis_meta.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/dhis/fill_new_element.py` & `dihlibs-0.0.9/dihlibs/dhis/fill_new_element.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/dhis/main.py` & `dihlibs-0.0.9/dihlibs/dhis/main.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/drive.py` & `dihlibs-0.0.9/dihlibs/drive.py`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/dihlibs/functions.py` & `dihlibs-0.0.9/dihlibs/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 from dihlibs.command import _Command
 
 
 def run_cmd(cmd, bg=True):
     return _Command(cmd, bg)
 
 
-def cmd_wait(cmd, bg=True):
+def cmd_wait(cmd, bg=True,verbose=False):
     with _Command(cmd, bg) as proc:
         rs = []
         while (x := proc.wait()) is not None:
+            if verbose:
+                print(x)
             rs.append(x)
         return "\n".join(rs)
 
-
 def get(obj, field, defaultValue=None):
     """Retrieves a nested value with dot and array index support."""
     for part in field.split("."):
         try:
             obj = obj[part] if isinstance(obj, dict) else obj[int(part)]
         except (KeyError, IndexError, ValueError):
             return defaultValue
@@ -109,15 +110,14 @@
 def to_file(file_name, text, mode="w"):
     with open(file_name, mode=mode) as file:
         return file.write(text)
 
 
 def lines_to_file(file_name, lines: list, mode="w"):
     data = "\n".join(lines)
-    print(data)
     to_file(file_name, data)
 
 
 def parse_month(date: str):
     formats = ["%Y%m", "%Y%m%d", "%d%m%Y", "%m%Y"]
     for fmt in formats:
         try:
@@ -180,11 +180,11 @@
 
 
 def read_non_blocking(readables: list):
     max_bytes = 1024
     ready_to_read, _, _ = select.select(readables, [], [], 0)
     data = []
     for fd in ready_to_read:
-        data.append(os.read(fd, max_bytes).decode().strip())
+        data.append(os.read(fd, max_bytes).decode('utf-8', errors='ignore').strip())
     data = [x for x in data if x]
     if len(data) > 0:
         return "\n".join(data)
```

### Comparing `dihlibs-0.0.8/dihlibs.egg-info/PKG-INFO` & `dihlibs-0.0.9/dihlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dihlibs
-Version: 0.0.8
+Version: 0.0.9
 Summary: A helper package for data integrations
 Home-page: https://github.com/nKataraia/dihlibs
 Author: Nitu
 Author-email: nkataraia@d-tree.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dihlibs-0.0.8/dihlibs.egg-info/SOURCES.txt` & `dihlibs-0.0.9/dihlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dihlibs-0.0.8/setup.py` & `dihlibs-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dihlibs",
-    version="0.0.8",
+    version="0.0.9",
     author="Nitu",
     author_email="nkataraia@d-tree.org",
     description="A helper package for data integrations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nKataraia/dihlibs",
     packages=find_packages(),
```

