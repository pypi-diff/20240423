# Comparing `tmp/batou_ext-2.4.5.tar.gz` & `tmp/batou_ext-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou_ext-2.4.5.tar", last modified: Wed Apr 17 14:26:48 2024, max compression
+gzip compressed data, was "batou_ext-2.4.6.tar", last modified: Tue Apr 23 14:53:48 2024, max compression
```

## Comparing `batou_ext-2.4.5.tar` & `batou_ext-2.4.6.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680901 batou_ext-2.4.5/
--rw-r--r--   0 flanitz    (501) staff       (20)     1299 2024-04-17 14:26:48.000000 batou_ext-2.4.5/CHANGES.md
--rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-17 14:26:48.000000 batou_ext-2.4.5/LICENSE.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-17 14:26:48.000000 batou_ext-2.4.5/MANIFEST.in
--rw-r--r--   0 flanitz    (501) staff       (20)     2561 2024-04-17 14:26:48.680993 batou_ext-2.4.5/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)      660 2024-04-17 14:26:48.000000 batou_ext-2.4.5/README.md
--rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-17 14:26:48.000000 batou_ext-2.4.5/pyproject.toml
--rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-17 14:26:48.681283 batou_ext-2.4.5/setup.cfg
--rw-r--r--   0 flanitz    (501) staff       (20)     1616 2024-04-17 14:26:48.000000 batou_ext-2.4.5/setup.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.670287 batou_ext-2.4.5/src/
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.675694 batou_ext-2.4.5/src/batou_ext/
--rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/acl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/archive.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/config.py
--rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/cron.py
--rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/fcio.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4854 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/file.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/geoip.py
--rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/git.py
--rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/htpasswd.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/http.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/jenkins.py
--rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/journalbeat.py
--rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/keypair.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5641 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mail.py
--rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mailhog.py
--rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/memcached.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mirror.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/mysql.py
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nfs.py
--rw-r--r--   0 flanitz    (501) staff       (20)    24039 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nix.py
--rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/nixos.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5500 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/oci.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/php.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677082 batou_ext-2.4.5/src/batou_ext/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/__init__.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677311 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/
--rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/database.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/local.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot.py
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/goceptnet.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.677894 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/
--rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/local.cf
--rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
--rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
--rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
--rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
--rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.678024 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/
--rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/config.local.php
--rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postfixadmin/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/python.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/rabbitmq.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/redis.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.679768 batou_ext-2.4.5/src/batou_ext/resources/
--rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/cert.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/check_systemd_unit.py
--rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/cron-wrapper.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/geoip-update.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/journalbeat.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/loader.c
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.679910 batou_ext-2.4.5/src/batou_ext/resources/mailhog/
--rw-r--r--   0 flanitz    (501) staff       (20)     1371 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/mailhog/mailhog.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/mirror.conf
--rw-r--r--   0 flanitz    (501) staff       (20)     1635 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/oci-template.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680272 batou_ext-2.4.5/src/batou_ext/resources/php/
--rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.conf
--rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.sh
--rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/php/php.ini
--rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/python.nix
--rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/rediscleanup.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/setupEnv.sh
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680433 batou_ext-2.4.5/src/batou_ext/resources/ssl/
--rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/ssl/local_certificate_check.sh
--rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/systemd.service
--rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/resources/userenv.nix
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.680796 batou_ext-2.4.5/src/batou_ext/roundcube/
--rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/__init__.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/config.inc.php
--rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/roundcube/postgres.py
--rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/run.py
--rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/s3.py
--rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/ssh.py
--rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/ssl.py
--rw-r--r--   0 flanitz    (501) staff       (20)     5258 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext/versions.py
-drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-17 14:26:48.676500 batou_ext-2.4.5/src/batou_ext.egg-info/
--rw-r--r--   0 flanitz    (501) staff       (20)     2561 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/PKG-INFO
--rw-r--r--   0 flanitz    (501) staff       (20)     2579 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/SOURCES.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/dependency_links.txt
--rw-r--r--   0 flanitz    (501) staff       (20)      113 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/entry_points.txt
--rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/not-zip-safe
--rw-r--r--   0 flanitz    (501) staff       (20)      109 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/requires.txt
--rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-17 14:26:48.000000 batou_ext-2.4.5/src/batou_ext.egg-info/top_level.txt
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232453 batou_ext-2.4.6/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1832 2024-04-23 14:53:47.000000 batou_ext-2.4.6/CHANGES.md
+-rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-23 14:53:47.000000 batou_ext-2.4.6/LICENSE.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-23 14:53:47.000000 batou_ext-2.4.6/MANIFEST.in
+-rw-r--r--   0 flanitz    (501) staff       (20)     3626 2024-04-23 14:53:48.232549 batou_ext-2.4.6/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)     1163 2024-04-23 14:53:47.000000 batou_ext-2.4.6/README.md
+-rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-23 14:53:47.000000 batou_ext-2.4.6/pyproject.toml
+-rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-23 14:53:48.232816 batou_ext-2.4.6/setup.cfg
+-rw-r--r--   0 flanitz    (501) staff       (20)     1737 2024-04-23 14:53:47.000000 batou_ext-2.4.6/setup.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.222394 batou_ext-2.4.6/src/
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.227900 batou_ext-2.4.6/src/batou_ext/
+-rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/acl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/archive.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/config.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/cron.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/fcio.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4854 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/file.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/geoip.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/git.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/htpasswd.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/http.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/jenkins.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/journalbeat.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/keypair.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5641 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mail.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mailhog.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/memcached.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mirror.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/mysql.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nfs.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    24116 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nix.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/nixos.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     6111 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/oci.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/php.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.229229 batou_ext-2.4.6/src/batou_ext/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/__init__.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.229454 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/
+-rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/database.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/local.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/goceptnet.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.230018 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/
+-rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/local.cf
+-rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
+-rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
+-rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
+-rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
+-rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.230126 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/config.local.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postfixadmin/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/python.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/rabbitmq.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/redis.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231490 batou_ext-2.4.6/src/batou_ext/resources/
+-rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/cert.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/check_systemd_unit.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/cron-wrapper.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/geoip-update.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/journalbeat.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/loader.c
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231587 batou_ext-2.4.6/src/batou_ext/resources/mailhog/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1371 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/mailhog/mailhog.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/mirror.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)     1898 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/oci-template.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.231890 batou_ext-2.4.6/src/batou_ext/resources/php/
+-rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/php/php.ini
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/python.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/rediscleanup.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/setupEnv.sh
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232045 batou_ext-2.4.6/src/batou_ext/resources/ssl/
+-rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/ssl/local_certificate_check.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/systemd.service
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/resources/userenv.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.232361 batou_ext-2.4.6/src/batou_ext/roundcube/
+-rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/config.inc.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/roundcube/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/run.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/s3.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     9400 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/s3_bootstrap.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/ssh.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/ssl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5258 2024-04-23 14:53:47.000000 batou_ext-2.4.6/src/batou_ext/versions.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-23 14:53:48.228659 batou_ext-2.4.6/src/batou_ext.egg-info/
+-rw-r--r--   0 flanitz    (501) staff       (20)     3626 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)     2609 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      171 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/entry_points.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/not-zip-safe
+-rw-r--r--   0 flanitz    (501) staff       (20)      153 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/requires.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-23 14:53:48.000000 batou_ext-2.4.6/src/batou_ext.egg-info/top_level.txt
```

### Comparing `batou_ext-2.4.5/CHANGES.md` & `batou_ext-2.4.6/CHANGES.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 
+## 2.4.6 (2024-04-23)
+
+
+- OCI: Support registries where the docker login is different than the registry used in referencing containers.
+
+- OCI: Improve change detection of remote images (required for docker.io)
+
+- OCI: The nix file does not contain sensitive data, so don’t mark it as such.
+
+- OCI: add support for extraOptions
+
+* Added a script `s3_bootstrap` that interactively creates an S3 bucket (including a radosgw account & keys if needed). Will be installed with `batou_ext` if the `s3-bootstrap` extra is requested.
+
+
 ## 2.4.5 (2024-04-17)
 
 
 - add an option to move mailhog log output (`stdout` + `stderr`) to a different namespace, e.g. "mailhog". see systemd.exec(5) for more information
+
 - add an option to disable `stdout` logging for the mailhog service
 
 - improve dectection of a versions file for versions updates
 
 - fix the oci.Container verify method not throwing an updaterequired on changes to the docker container's environment file
 
-Add systemd-run async cleanup option for SymlinkAndCleanup removals
+- Add systemd-run async cleanup option for SymlinkAndCleanup removals
 
 
 ## 2.4.4 (2024-04-05)
 
 
 - Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `batou_ext-2.4.5/LICENSE.txt` & `batou_ext-2.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/PKG-INFO` & `batou_ext-2.4.6/src/batou_ext.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: batou_ext
-Version: 2.4.5
+Name: batou-ext
+Version: 2.4.6
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: version-select
+Provides-Extra: s3-bootstrap
 License-File: LICENSE.txt
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
@@ -28,27 +29,65 @@
 
 ## Development and release process
 
 * Changes should be accompanied with a changelog entry. Use `./changelog.sh` to create one.
 
 * Releasing will create a tag and publishes the package to pypi. Use `./release-this.sh` to create a release.
 
+## Bootstrapping of S3 buckets
+
+Only applicable for administrators of the Flying Circus.
+
+Install the `s3-bootstrap` feature:
+
+```
+batou_ext[s3-bootstrap]>=2.4.6
+```
+
+Then run
+
+```
+./appenv update-lockfile
+./appenv run s3_bootstrap
+```
+
+The script will interactively walk you through the creation of
+creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
+an access keypair and lifecycle rules.
+
+On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
+
+
+
+## 2.4.6 (2024-04-23)
+
+
+- OCI: Support registries where the docker login is different than the registry used in referencing containers.
+
+- OCI: Improve change detection of remote images (required for docker.io)
+
+- OCI: The nix file does not contain sensitive data, so don’t mark it as such.
+
+- OCI: add support for extraOptions
+
+* Added a script `s3_bootstrap` that interactively creates an S3 bucket (including a radosgw account & keys if needed). Will be installed with `batou_ext` if the `s3-bootstrap` extra is requested.
 
 
 ## 2.4.5 (2024-04-17)
 
 
 - add an option to move mailhog log output (`stdout` + `stderr`) to a different namespace, e.g. "mailhog". see systemd.exec(5) for more information
+
 - add an option to disable `stdout` logging for the mailhog service
 
 - improve dectection of a versions file for versions updates
 
 - fix the oci.Container verify method not throwing an updaterequired on changes to the docker container's environment file
 
-Add systemd-run async cleanup option for SymlinkAndCleanup removals
+- Add systemd-run async cleanup option for SymlinkAndCleanup removals
 
 
 ## 2.4.4 (2024-04-05)
 
 
 - Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `batou_ext-2.4.5/setup.py` & `batou_ext-2.4.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 
 def project_path(*names):
     return os.path.join(*names)
 
 
 setup(
     name="batou_ext",
-    version="2.4.5",
+    version="2.4.6",
     install_requires=[
         "batou >= 2.3b4",
         "pyaml",
         "setuptools",
         "six",
+        "InquirerPy",
     ],
     extras_require={
         "test": [
             "boto3",
             "passlib>=1.7",
             "pytest",
             "pytest-mock",
         ],
-        "version-select": [
-            "InquirerPy",
-        ],
+        "version-select": ["InquirerPy"],
+        "s3-bootstrap": ["boto3", "InquirerPy"],
     },
     author="Flying Circus <support@flyingcircus.io>",
     author_email="support@flyingcircus.io",
     license="BSD (2-clause)",
     url="https://github.com/flyingcircusio/batou_ext",
     keywords="deployment",
     classifiers="""\
@@ -60,11 +60,12 @@
     include_package_data=True,
     data_files=[("", glob.glob(project_path("*.txt")))],
     entry_points=dict(
         console_scripts=[
             "jenkins = batou_ext.jenkins:main",
             "fcio = batou_ext.fcio:main",
             "versions = batou_ext.versions:main",
+            "s3_bootstrap = batou_ext.s3_bootstrap:main [s3-bootstrap]",
         ]
     ),
     zip_safe=False,
 )
```

### Comparing `batou_ext-2.4.5/src/batou_ext/acl.py` & `batou_ext-2.4.6/src/batou_ext/acl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/archive.py` & `batou_ext-2.4.6/src/batou_ext/archive.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/config.py` & `batou_ext-2.4.6/src/batou_ext/config.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/cron.py` & `batou_ext-2.4.6/src/batou_ext/cron.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/fcio.py` & `batou_ext-2.4.6/src/batou_ext/fcio.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/file.py` & `batou_ext-2.4.6/src/batou_ext/file.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/geoip.py` & `batou_ext-2.4.6/src/batou_ext/geoip.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/git.py` & `batou_ext-2.4.6/src/batou_ext/git.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/htpasswd.py` & `batou_ext-2.4.6/src/batou_ext/htpasswd.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/http.py` & `batou_ext-2.4.6/src/batou_ext/http.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/jenkins.py` & `batou_ext-2.4.6/src/batou_ext/jenkins.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/journalbeat.py` & `batou_ext-2.4.6/src/batou_ext/journalbeat.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/keypair.py` & `batou_ext-2.4.6/src/batou_ext/keypair.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/mail.py` & `batou_ext-2.4.6/src/batou_ext/mail.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/memcached.py` & `batou_ext-2.4.6/src/batou_ext/memcached.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/mirror.py` & `batou_ext-2.4.6/src/batou_ext/mirror.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/mysql.py` & `batou_ext-2.4.6/src/batou_ext/mysql.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/nfs.py` & `batou_ext-2.4.6/src/batou_ext/nfs.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/nix.py` & `batou_ext-2.4.6/src/batou_ext/nix.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,14 +608,16 @@
         return component_to_nix(value)
     elif isinstance(value, Address):
         return nix_dict_to_nix(address_to_nix_dict(value))
     elif isinstance(value, Host):
         return nix_dict_to_nix(host_to_nix_dict(value))
     elif isinstance(value, Environment):
         return nix_dict_to_nix(environment_to_nix_dict(value))
+    elif isinstance(value, batou.utils.Timer):
+        return None  # ignore
     else:
         raise TypeError(f"unsupported type '{type(value)}'")
 
 
 def component_to_nix(component: Component):
     from batou_ext.nixos import NixOSModuleContext
```

### Comparing `batou_ext-2.4.5/src/batou_ext/nixos.py` & `batou_ext-2.4.6/src/batou_ext/nixos.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/oci.py` & `batou_ext-2.4.6/src/batou_ext/oci.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,108 @@
-import hashlib
 import os
-import re
 import shlex
+from textwrap import dedent
 from typing import Optional
 
 import batou
-import pkg_resources
 from batou import UpdateNeeded
 from batou.component import Attribute, Component
 from batou.lib.file import File
-from batou.lib.service import Service
+from batou.utils import CmdExecutionError
 
 import batou_ext.nix
 
 
 @batou_ext.nix.rebuild
 class Container(Component):
-    """
-    A OCI Container component.
-    With this component you can dynamically schedule docker containers to be run on the target host
+    """A OCI Container component.
+
+    With this component you can dynamically schedule docker containers to be
+    run on the target host.
 
     Note: Docker image specifiers do not follow a properly resolvable pattern.
-        Therefore, container registries have to be specified seperately if you need to log in before.
-        If you do not provide a container registry, docker will use the default one for authentication.
-        You can choose to also append the image attribute with the registry but this module will do so
-        automatically.
-
-        ```
-        # the following two call are identical:
-        self += batou_ext.oci.Container(
-            image="foo",
-            registry_address="test.registry",
-            registry_user="foo",
-            registry_password="bar")
-
-        self += batou_ext.oci.Container(
-            image="test.registry/foo",
-            registry_address="test.registry",
-            registry_user="foo",
-            registry_password="bar")
-
-        # However, this will fail since docker will try to log into the default container registry
-        # with the provided credentials and then pull the image from the registry specified in the image string
-        self += batou_ext.oci.Container(
-            image="test.registry/foo",
-            registry_user="foo",
-            registry_password="bar")
-
-
-        # if you don't need to authenticate, not explicitly specifying the registry is fine of course
-        # and it will pull the image from the correct registry
-        self += batou_ext.oci.Container(image="test.registry/foo")
-        ```
+    Therefore, container registries have to be specified seperately if you need
+    to log in before. If you do not provide a container registry, docker will
+    use the default one for authentication. You can choose to also append the
+    image attribute with the registry but this module will do so automatically.
+
+    ```
+    # the following two call are identical:
+    self += batou_ext.oci.Container(
+        image="foo",
+        registry_address="test.registry",
+        registry_user="foo",
+        registry_password="bar")
+
+    self += batou_ext.oci.Container(
+        image="test.registry/foo",
+        registry_address="test.registry",
+        registry_user="foo",
+        registry_password="bar")
+
+    # However, this will fail since docker will try to log into the default container registry
+    # with the provided credentials and then pull the image from the registry specified in the image string
+    self += batou_ext.oci.Container(
+        image="test.registry/foo",
+        registry_user="foo",
+        registry_password="bar")
+
+
+    # if you don't need to authenticate, not explicitly specifying the registry is fine of course
+    # and it will pull the image from the correct registry
+    self += batou_ext.oci.Container(image="test.registry/foo")
+    ```
 
     Example:
     ```
     self += batou_ext.oci.Container(image = "mysql", version = "8.0")
     ```
+
     """
 
     # general options
     image = Attribute(str)
     version: str = "latest"
     container_name: Optional[str] = None
 
     # specific options
     entrypoint: Optional[str] = None
     docker_cmd: Optional[str] = None
     envfile: Optional[File] = None
     mounts: dict = {}
     ports: dict = {}
     env: dict = {}
+    depends_on: list = None
+    extra_options: list = None
 
     # secrets
     registry_address = Attribute(Optional[str], None)
     registry_user = Attribute(Optional[str], None)
     registry_password = Attribute(Optional[str], None)
 
     _required_params_ = {
         "image": "mysql",
     }
 
     def configure(self):
         if (
             self.registry_user or self.registry_password
         ) and not self.registry_address:
-            batou.output.annotate(
-                "WARN: you might want to specify the registry explicitly unless you really intend to log into the default docker registry"
+            self.log(
+                "WARN: you might want to specify the registry explicitly"
+                " unless you really intend to log into the default"
+                " docker registry"
             )
 
-        if self.version:
-            self.image = f"{self.image}:{self.version}"
-
-        if self.registry_address and not self.image.startswith(
+        if (
             self.registry_address
+            # This is for the strange case of index.docker.io where you have
+            # to set the registry_address to `https://index.docker.io/v1/`
+            and not self.registry_address.startswith("https://")
+            and not self.image.startswith(self.registry_address)
         ):
             self.image = f"{self.registry_address}{'/' if not self.registry_address.endswith('/') else ''}{self.image}"
 
         if self.registry_password:
             self += File(
                 "registry-password", mode=0o600, content=self.registry_password
             )
@@ -112,51 +117,74 @@
 {% endfor %}""",
             )
             self.envfile = self._
 
         if self.docker_cmd:
             self._docker_cmd_list = shlex.split(self.docker_cmd)
 
+        if not self.depends_on:
+            self.depends_on = []
+
         self += File(
             f"/etc/local/nixos/docker_{self.container_name}.nix",
-            sensitive_data=True,
+            sensitive_data=False,
             source=os.path.join(
                 os.path.dirname(__file__), "resources/oci-template.nix"
             ),
         )
 
     def verify(self):
         self.assert_no_changes()
         self.envfile.assert_no_changes()
 
         if self.registry_address:
             logintxt, _ = self.cmd(
                 self.expand(
-                    """
-                    docker login \\
-                        {%- if component.registry_user and component.registry_password %}
-                        -u {{component.registry_user}} \\
-                        -p {{component.registry_password}} \\
-                        {%- endif %}
-                        {{component.registry_address}}
-                """
+                    dedent(
+                        """\
+        docker login \\
+            {%- if component.registry_user and component.registry_password %}
+            -u {{component.registry_user}} \\
+            -p {{component.registry_password}} \\
+            {%- endif %}
+            {{component.registry_address}}
+        """
+                    )
                 )
             )
 
         local_digest, stderr = self.cmd(
-            "docker image inspect {{component.image}} | jq -r 'first | .RepoDigests | first | split(\"@\") | last' || echo image not available locally"
-        )
-        remote_digest, stderr = self.cmd(
-            "docker manifest inspect {{component.image}} -v | jq -r 'if type ==\"array\" then (. | first) else . end | .Descriptor.digest'"
+            dedent(
+                """\
+            docker image inspect {{component.image}}:{{component.version}} \
+                | jq -r 'first | .RepoDigests | first | split("@") | last' \
+                || echo image not available locally
+                """
+            )
         )
+        try:
+            self.cmd(
+                "docker manifest inspect"
+                f" {self.image}:{self.version}@{local_digest}"
+            )
+        except CmdExecutionError as e:
+            valid = False
+            error = e.stderr
+            if error.startswith("unsupported manifest format"):  # gitlab
+                batou.output.annotate(error, debug=True)
+                error = error[:50]
+        else:
+            valid = True
 
-        # `docker manifest inspect` silently raises an error, returns code 0 when unathorized
+        # `docker manifest inspect` silently raises an error, returns code 0
+        # when unathorized
         if stderr == "unauthorized":
             raise RuntimeError(
                 "Wrong credentials for remote container registry"
             )
 
-        if local_digest != remote_digest:
+        if not valid:
+            self.log("Update due digest verification error: %r", error)
             raise UpdateNeeded()
 
     def update(self):
         self.cmd(f"sudo systemctl restart docker-{self.container_name}")
```

### Comparing `batou_ext-2.4.5/src/batou_ext/php.py` & `batou_ext-2.4.6/src/batou_ext/php.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/__init__.py` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot/database.conf` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot/database.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/dovecot.py` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/dovecot.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/goceptnet.py` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix/local.cf` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix/local.cf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfix.py` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/postfixadmin/config.local.php` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/postfixadmin/config.local.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postfixadmin/postgres.py` & `batou_ext-2.4.6/src/batou_ext/postfixadmin/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/postgres.py` & `batou_ext-2.4.6/src/batou_ext/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/python.py` & `batou_ext-2.4.6/src/batou_ext/python.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/rabbitmq.py` & `batou_ext-2.4.6/src/batou_ext/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/redis.py` & `batou_ext-2.4.6/src/batou_ext/redis.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/cert.sh` & `batou_ext-2.4.6/src/batou_ext/resources/cert.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/loader.c` & `batou_ext-2.4.6/src/batou_ext/resources/loader.c`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/mailhog/mailhog.nix` & `batou_ext-2.4.6/src/batou_ext/resources/mailhog/mailhog.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/mirror.conf` & `batou_ext-2.4.6/src/batou_ext/resources/mirror.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/oci-template.nix` & `batou_ext-2.4.6/src/batou_ext/resources/oci-template.nix`

 * *Files 11% similar despite different names*

```diff
@@ -32,26 +32,38 @@
 
         # {% if component.registry_user and component.registry_password %}
         username = "{{component.registry_user}}";
         passwordFile = "{{component.password_file.path}}";
         # {% endif %}
       };
 
-      extraOptions = [ "--pull=always" ];
+      extraOptions = [
+        "--pull=always"
+        # {% for option in (component.extra_options or []) %}
+        "{{option}}"
+        # {% endfor %}
+      ];
 
       volumes = [
       # {% for key, value in component.mounts.items() | sort  %}
         "{{key}}:{{value}}"
       # {% endfor %}
       ];
 
-      image = "{{component.image}}";
+      image = "{{component.image}}:{{component.version}}";
       environmentFiles = [ {{component.envfile.path}} ];
 
       ports = [
       # {% for key, value in component.ports.items() | sort  %}
         "{{key}}:{{value}}"
       # {% endfor %}
       ];
+
+      dependsOn = [
+      # {% for value in component.depends_on  %}
+        "{{value}}"
+      # {% endfor %}
+
+      ];
     };
   };
 }
```

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/php/php-fpm.conf` & `batou_ext-2.4.6/src/batou_ext/resources/php/php-fpm.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/php/php.ini` & `batou_ext-2.4.6/src/batou_ext/resources/php/php.ini`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/python.nix` & `batou_ext-2.4.6/src/batou_ext/resources/python.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/setupEnv.sh` & `batou_ext-2.4.6/src/batou_ext/resources/setupEnv.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/ssl/local_certificate_check.sh` & `batou_ext-2.4.6/src/batou_ext/resources/ssl/local_certificate_check.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/resources/userenv.nix` & `batou_ext-2.4.6/src/batou_ext/resources/userenv.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/roundcube/__init__.py` & `batou_ext-2.4.6/src/batou_ext/roundcube/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/roundcube/config.inc.php` & `batou_ext-2.4.6/src/batou_ext/roundcube/config.inc.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/roundcube/postgres.py` & `batou_ext-2.4.6/src/batou_ext/roundcube/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/run.py` & `batou_ext-2.4.6/src/batou_ext/run.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/s3.py` & `batou_ext-2.4.6/src/batou_ext/s3.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/ssh.py` & `batou_ext-2.4.6/src/batou_ext/ssh.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/ssl.py` & `batou_ext-2.4.6/src/batou_ext/ssl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext/versions.py` & `batou_ext-2.4.6/src/batou_ext/versions.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.5/src/batou_ext.egg-info/PKG-INFO` & `batou_ext-2.4.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: batou-ext
-Version: 2.4.5
+Name: batou_ext
+Version: 2.4.6
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: version-select
+Provides-Extra: s3-bootstrap
 License-File: LICENSE.txt
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
@@ -28,27 +29,65 @@
 
 ## Development and release process
 
 * Changes should be accompanied with a changelog entry. Use `./changelog.sh` to create one.
 
 * Releasing will create a tag and publishes the package to pypi. Use `./release-this.sh` to create a release.
 
+## Bootstrapping of S3 buckets
+
+Only applicable for administrators of the Flying Circus.
+
+Install the `s3-bootstrap` feature:
+
+```
+batou_ext[s3-bootstrap]>=2.4.6
+```
+
+Then run
+
+```
+./appenv update-lockfile
+./appenv run s3_bootstrap
+```
+
+The script will interactively walk you through the creation of
+creating an [S3 bucket](https://wiki.flyingcircus.io/S3) and - if needed -
+an access keypair and lifecycle rules.
+
+On an activated virtualenv this can be tested with `python -m batou_ext.s3_bootstrap`.
+
+
+
+## 2.4.6 (2024-04-23)
+
+
+- OCI: Support registries where the docker login is different than the registry used in referencing containers.
+
+- OCI: Improve change detection of remote images (required for docker.io)
+
+- OCI: The nix file does not contain sensitive data, so don’t mark it as such.
+
+- OCI: add support for extraOptions
+
+* Added a script `s3_bootstrap` that interactively creates an S3 bucket (including a radosgw account & keys if needed). Will be installed with `batou_ext` if the `s3-bootstrap` extra is requested.
 
 
 ## 2.4.5 (2024-04-17)
 
 
 - add an option to move mailhog log output (`stdout` + `stderr`) to a different namespace, e.g. "mailhog". see systemd.exec(5) for more information
+
 - add an option to disable `stdout` logging for the mailhog service
 
 - improve dectection of a versions file for versions updates
 
 - fix the oci.Container verify method not throwing an updaterequired on changes to the docker container's environment file
 
-Add systemd-run async cleanup option for SymlinkAndCleanup removals
+- Add systemd-run async cleanup option for SymlinkAndCleanup removals
 
 
 ## 2.4.4 (2024-04-05)
 
 
 - Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `batou_ext-2.4.5/src/batou_ext.egg-info/SOURCES.txt` & `batou_ext-2.4.6/src/batou_ext.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/batou_ext/php.py
 src/batou_ext/postgres.py
 src/batou_ext/python.py
 src/batou_ext/rabbitmq.py
 src/batou_ext/redis.py
 src/batou_ext/run.py
 src/batou_ext/s3.py
+src/batou_ext/s3_bootstrap.py
 src/batou_ext/ssh.py
 src/batou_ext/ssl.py
 src/batou_ext/versions.py
 src/batou_ext.egg-info/PKG-INFO
 src/batou_ext.egg-info/SOURCES.txt
 src/batou_ext.egg-info/dependency_links.txt
 src/batou_ext.egg-info/entry_points.txt
```

