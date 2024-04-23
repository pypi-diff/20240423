# Comparing `tmp/types-paramiko-3.4.0.20240205.tar.gz` & `tmp/types-paramiko-3.4.0.20240311.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-paramiko-3.4.0.20240205.tar", last modified: Mon Feb  5 02:21:13 2024, max compression
+gzip compressed data, was "types-paramiko-3.4.0.20240311.tar", last modified: Mon Mar 11 02:18:04 2024, max compression
```

## Comparing `types-paramiko-3.4.0.20240205.tar` & `types-paramiko-3.4.0.20240311.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:21:13.175131 types-paramiko-3.4.0.20240205/
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-02-05 02:21:12.000000 types-paramiko-3.4.0.20240205/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 02:21:12.000000 types-paramiko-3.4.0.20240205/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-05 02:21:13.175131 types-paramiko-3.4.0.20240205/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:21:13.175131 types-paramiko-3.4.0.20240205/paramiko-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-05 02:21:12.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/auth_strategy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/ber.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/buffered_pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/compress.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/dsskey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/ecdsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/ed25519key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/hostkeys.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_curve25519.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_ecdh_nist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_gex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_group1.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_group14.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_group16.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/kex_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/pkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/primes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 02:21:12.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/rsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_attr.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_file.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_handle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_server.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_si.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/ssh_exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/ssh_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/win_openssh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-05 02:20:13.000000 types-paramiko-3.4.0.20240205/paramiko-stubs/win_pageant.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 02:21:13.175131 types-paramiko-3.4.0.20240205/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-05 02:21:12.000000 types-paramiko-3.4.0.20240205/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:21:13.175131 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-05 02:21:13.000000 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-05 02:21:13.000000 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 02:21:13.000000 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 02:21:13.000000 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 02:21:13.000000 types-paramiko-3.4.0.20240205/types_paramiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:04.924980 types-paramiko-3.4.0.20240311/
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-11 02:18:04.924980 types-paramiko-3.4.0.20240311/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:04.924980 types-paramiko-3.4.0.20240311/paramiko-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/auth_strategy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/ber.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/buffered_pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/compress.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/dsskey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/ecdsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/ed25519key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/hostkeys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_curve25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_ecdh_nist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_gex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_group1.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_group14.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_group16.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/kex_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/pkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/primes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/rsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_handle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_si.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/ssh_exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/ssh_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/win_openssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-11 02:14:35.000000 types-paramiko-3.4.0.20240311/paramiko-stubs/win_pageant.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:18:04.924980 types-paramiko-3.4.0.20240311/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:18:04.924980 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-11 02:18:04.000000 types-paramiko-3.4.0.20240311/types_paramiko.egg-info/top_level.txt
```

### Comparing `types-paramiko-3.4.0.20240205/CHANGELOG.md` & `types-paramiko-3.4.0.20240311/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.4.0.20240311 (2024-03-11)
+
+Use PEP 570 syntax in third party stubs (#11554)
+
 ## 3.4.0.20240205 (2024-02-05)
 
 A new shade of Black (#11362)
 
 ## 3.4.0.20240120 (2024-01-20)
 
 Re-export ChannelFile from paramiko (#11290)
```

### Comparing `types-paramiko-3.4.0.20240205/PKG-INFO` & `types-paramiko-3.4.0.20240311/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.4.0.20240205
+Version: 3.4.0.20240311
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a2a6aee89213d87ed6f86cf723a7fc4ed3c219a2` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
+with mypy 1.9.0, pyright 1.1.350, and
+pytype 2024.2.27.
```

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/__init__.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/_winapi.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/agent.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/agent.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/auth_handler.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/auth_handler.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/auth_strategy.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/auth_strategy.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/ber.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/ber.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/channel.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/channel.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/client.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from paramiko.sftp_client import SFTPClient
 from paramiko.transport import Transport, _SocketLike
 from paramiko.util import ClosingContextManager
 
 class _TransportFactory(Protocol):
     def __call__(
         self,
-        __sock: _SocketLike,
+        sock: _SocketLike,
+        /,
         *,
         gss_kex: bool,
         gss_deleg_creds: bool,
         disabled_algorithms: Mapping[str, Iterable[str]] | None,
     ) -> Transport: ...
 
 class SSHClient(ClosingContextManager):
```

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/common.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/config.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/dsskey.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/dsskey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/ecdsakey.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/ecdsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/ed25519key.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/ed25519key.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/file.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/hostkeys.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/hostkeys.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/kex_curve25519.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/kex_curve25519.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/kex_ecdh_nist.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/kex_ecdh_nist.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/kex_gex.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/kex_gex.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/kex_group1.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/kex_group1.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/kex_gss.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/kex_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/message.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/message.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/packet.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/packet.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/pipe.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/pkey.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/pkey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/proxy.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/rsakey.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/rsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/server.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_attr.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_attr.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_client.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_client.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_file.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_server.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/sftp_si.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/sftp_si.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/ssh_exception.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/ssh_exception.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/ssh_gss.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/ssh_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/transport.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/transport.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/util.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/paramiko-stubs/win_pageant.pyi` & `types-paramiko-3.4.0.20240311/paramiko-stubs/win_pageant.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.4.0.20240205/setup.py` & `types-paramiko-3.4.0.20240311/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a2a6aee89213d87ed6f86cf723a7fc4ed3c219a2` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
+with mypy 1.9.0, pyright 1.1.350, and
+pytype 2024.2.27.
 '''.lstrip()
 
 setup(name=name,
-      version="3.4.0.20240205",
+      version="3.4.0.20240311",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md",
```

### Comparing `types-paramiko-3.4.0.20240205/types_paramiko.egg-info/PKG-INFO` & `types-paramiko-3.4.0.20240311/types_paramiko.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.4.0.20240205
+Version: 3.4.0.20240311
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a2a6aee89213d87ed6f86cf723a7fc4ed3c219a2` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2024.1.24.
+This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
+with mypy 1.9.0, pyright 1.1.350, and
+pytype 2024.2.27.
```

### Comparing `types-paramiko-3.4.0.20240205/types_paramiko.egg-info/SOURCES.txt` & `types-paramiko-3.4.0.20240311/types_paramiko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

