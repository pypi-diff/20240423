# Comparing `tmp/artistools-2024.2.22.2.tar.gz` & `tmp/artistools-2024.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistools-2024.2.22.2.tar", last modified: Thu Feb 22 11:08:47 2024, max compression
+gzip compressed data, was "artistools-2024.4.23.tar", last modified: Tue Apr 23 11:24:48 2024, max compression
```

## Comparing `artistools-2024.2.22.2.tar` & `artistools-2024.4.23.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.376366 artistools-2024.2.22.2/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-02-22 11:08:47.376366 artistools-2024.2.22.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.316366 artistools-2024.2.22.2/artistools/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.316366 artistools-2024.2.22.2/artistools/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/atomic/_atomic_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/codecomparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.316366 artistools-2024.2.22.2/artistools/data/
--rw-r--r--   0 runner    (1001) docker     (127)    70935 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/ElBiEn_2007.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/atomic_properties.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/betaminusdecays.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/binding_energies.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.324366 artistools-2024.2.22.2/artistools/data/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/400.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/520.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.324366 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/ASIAGO/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48059 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/FUV.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/H.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/H_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55262 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/J.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/J_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/K.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/K_ab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.324366 artistools-2024.2.22.2/artistools/data/filters/LCOGT/
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LCOGT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.324366 artistools-2024.2.22.2/artistools/data/filters/LSQ/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LSQ/rs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.328366 artistools-2024.2.22.2/artistools/data/filters/LT/
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24161 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/LT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.328366 artistools-2024.2.22.2/artistools/data/filters/NOT/
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NOT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.328366 artistools-2024.2.22.2/artistools/data/filters/NTT/
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/B.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/R.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NTT/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/NUV.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.328366 artistools-2024.2.22.2/artistools/data/filters/OGLE/
--rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/OGLE/I.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/OGLE/V.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.332366 artistools-2024.2.22.2/artistools/data/filters/PS1/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/PS1/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/PS1/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/PS1/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/PS1/ws.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/PS1/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)    84060 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/R.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.332366 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/zs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/U.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55259 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/V.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/gs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/is.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/rs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/us.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvm2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvm2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvw1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvw1_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvw2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/uvw2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/filters/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.340366 artistools-2024.2.22.2/artistools/data/lightcurves/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN1991T.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN1999by.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN1999dq.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2005cf.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2011fe.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2012cg.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2012dn.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2012fr.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2014J.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2015F.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/SN2018byg.dat.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.340366 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.364366 artistools-2024.2.22.2/artistools/data/refspectra/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    75182 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)    73950 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2010lp_20110928_fors2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   787320 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   713500 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   713176 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   664004 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   708656 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   712196 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   709200 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   552728 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   707384 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)   705880 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   257680 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   104189 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   210900 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/nero-nebspec.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)   103168 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/solar_r_abundance_pattern.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/data/splitmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.364366 artistools-2024.2.22.2/artistools/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18027 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/estimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/exportmassfractions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/plot3destimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47858 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/plotestimators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/estimators/test_estimators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26353 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/gsinetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/hesma_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.368366 artistools-2024.2.22.2/artistools/inputmodel/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6400 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/1dslicefrom3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3984 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/botyanski2017.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11110 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/describeinputmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/downscale3dgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/energyinputfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/from_alcar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.368366 artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10750 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2701 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/fullymixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    55905 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/inputmodel_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5146 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/makeartismodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/map_1d_to_3d_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17227 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/maptogrid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16460 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/modelfromhydro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/opacityinputfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3814 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/plotdensity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17375 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/plotinitialcomposition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8260 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/recombinationenergy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23819 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/rprocess_from_trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5542 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/rprocess_solar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2636 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/scalevelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3571 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/shen2018.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9578 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/slice1dfromconein3dmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/test_inputmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/inputmodel/to_tardis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.372366 artistools-2024.2.22.2/artistools/lightcurve/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22236 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)    65452 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/plotlightcurve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2953 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (127)    31883 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/viewingangleanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/lightcurve/writebollightcurvedata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38260 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/linefluxes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/logfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5914 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/macroatom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/make_vpkt_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    40271 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (127)    56450 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.372366 artistools-2024.2.22.2/artistools/nltepops/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nltepops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nltepops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nltepops/nltepops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32735 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nltepops/plotnltepops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.372366 artistools-2024.2.22.2/artistools/nonthermal/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58564 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/_nonthermal_core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5022 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/leptontransport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11742 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/plotnonthermal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14178 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/solvespencerfanocmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/nonthermal/test_nonthermal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.372366 artistools-2024.2.22.2/artistools/packets/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33695 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/packets/packets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/packets/packetsplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/packets/test_packets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15783 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/plotspherical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/plottools.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (127)    41607 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/radfield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.376366 artistools-2024.2.22.2/artistools/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55547 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/plotspectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/sampleblackbodyfrompacket_tr.py
--rw-r--r--   0 runner    (1001) docker     (127)    50936 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8501 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/test_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1338 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/test_vspectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/spectra/writespectra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4717 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/test_artistools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20585 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6857 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/viewing_angles_visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11321 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistools/writecomparisondata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 11:08:47.376366 artistools-2024.2.22.2/artistools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-02-22 11:08:47.000000 artistools-2024.2.22.2/artistools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/artistoolscompletions.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-22 11:08:26.000000 artistools-2024.2.22.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 11:08:47.376366 artistools-2024.2.22.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.174853 artistools-2024.4.23/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 11:24:42.000000 artistools-2024.4.23/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 11:24:42.000000 artistools-2024.4.23/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 11:24:42.000000 artistools-2024.4.23/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-23 11:24:42.000000 artistools-2024.4.23/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-23 11:24:42.000000 artistools-2024.4.23/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 11:24:42.000000 artistools-2024.4.23/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-23 11:24:42.000000 artistools-2024.4.23/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 11:24:42.000000 artistools-2024.4.23/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 11:24:42.000000 artistools-2024.4.23/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 11:24:42.000000 artistools-2024.4.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-23 11:24:48.170853 artistools-2024.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 11:24:42.000000 artistools-2024.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.110853 artistools-2024.4.23/artistools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.110853 artistools-2024.4.23/artistools/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/atomic/_atomic_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/codecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.114853 artistools-2024.4.23/artistools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    70935 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/ElBiEn_2007.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/atomic_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/betaminusdecays.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/binding_energies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.118853 artistools-2024.4.23/artistools/data/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/400.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/520.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.118853 artistools-2024.4.23/artistools/data/filters/ASIAGO/
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17947 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/ASIAGO/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48059 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/FUV.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/H.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/H_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55262 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/J.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/J_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/K.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/K_ab.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LCOGT/
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LCOGT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LSQ/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LSQ/rs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/LT/
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24161 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/LT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.122853 artistools-2024.4.23/artistools/data/filters/NOT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NOT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/NTT/
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22775 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NTT/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/NUV.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/OGLE/
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/OGLE/I.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/OGLE/V.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/PS1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/ws.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/PS1/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    84060 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/R.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.126853 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/SKYMAPPER/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/U.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55259 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/is.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/us.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvm2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvm2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw1_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/uvw2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/filters/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.134853 artistools-2024.4.23/artistools/data/lightcurves/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1991T.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1999by.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN1999dq.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2005cf.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2011fe.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012cg.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012dn.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2012fr.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2014J.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2015F.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/SN2018byg.dat.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.134853 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.158853 artistools-2024.4.23/artistools/data/refspectra/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    75182 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    73950 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   787320 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   713500 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   713176 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   664004 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   708656 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   712196 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   709200 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   552728 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   707384 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   705880 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   257680 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   104189 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   210930 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   210900 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/nero-nebspec.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   103168 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/solar_r_abundance_pattern.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/data/splitmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/deposition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.162853 artistools-2024.4.23/artistools/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17106 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/estimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/exportmassfractions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/plot3destimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48660 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/plotestimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/estimators/test_estimators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26288 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/gsinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/hesma_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/inputmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6406 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/1dslicefrom3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3984 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/botyanski2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11072 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/describeinputmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/downscale3dgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/energyinputfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/from_alcar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10699 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12645 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2701 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/fullymixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54779 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/inputmodel_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5146 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/makeartismodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/map_1d_to_3d_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17178 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/maptogrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16419 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/modelfromhydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/opacityinputfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3801 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/plotdensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17379 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/plotinitialcomposition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8257 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/recombinationenergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23731 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/rprocess_from_trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5325 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/rprocess_solar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2636 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/scalevelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3586 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/shen2018.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9548 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/slice1dfromconein3dmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/test_inputmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/inputmodel/to_tardis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/lightcurve/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23668 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65520 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/plotlightcurve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2953 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32172 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/viewingangleanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/lightcurve/writebollightcurvedata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38118 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/linefluxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/logfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5914 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/macroatom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/make_vpkt_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40374 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)    57242 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.166853 artistools-2024.4.23/artistools/nltepops/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/nltepops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32642 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nltepops/plotnltepops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/nonthermal/
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58560 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/_nonthermal_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5022 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/leptontransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11735 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/plotnonthermal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14149 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/solvespencerfanocmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/nonthermal/test_nonthermal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/packets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36685 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/packets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/packetsplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/packets/test_packets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17298 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/plotspherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/plottools.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41390 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/radfield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56091 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/plotspectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/sampleblackbodyfrompacket_tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55326 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8618 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/test_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3443 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/test_vspectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/spectra/writespectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4717 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/test_artistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23013 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6858 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/viewing_angles_visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11238 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistools/writecomparisondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:24:48.170853 artistools-2024.4.23/artistools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-23 11:24:48.000000 artistools-2024.4.23/artistools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-23 11:24:42.000000 artistools-2024.4.23/artistoolscompletions.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-23 11:24:42.000000 artistools-2024.4.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 11:24:42.000000 artistools-2024.4.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:24:48.174853 artistools-2024.4.23/setup.cfg
```

### Comparing `artistools-2024.2.22.2/.codecov.yml` & `artistools-2024.4.23/.codecov.yml`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/.gitignore` & `artistools-2024.4.23/.gitignore`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/.pre-commit-config.yaml` & `artistools-2024.4.23/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.5.0
+      rev: v4.6.0
       hooks:
           - id: check-added-large-files
             args: [--maxkb=800]
           - id: check-ast
           - id: check-case-conflict
           - id: check-builtin-literals
           - id: check-docstring-first
@@ -28,21 +28,21 @@
 
     # - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
     #   rev: 0.2.3
     #   hooks:
     #       - id: yamlfmt
 
     - repo: https://github.com/astral-sh/ruff-pre-commit
-      rev: v0.2.2
+      rev: v0.4.1
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
 
     - repo: https://github.com/astral-sh/ruff-pre-commit
-      rev: v0.2.2
+      rev: v0.4.1
       hooks:
           - id: ruff-format
 
     # - repo: https://github.com/pre-commit/mirrors-mypy
     #   rev: v1.6.1
     #   hooks:
     #       - id: mypy
```

### Comparing `artistools-2024.2.22.2/.sourcery.yaml` & `artistools-2024.4.23/.sourcery.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # or writing custom rules.
 
 # 📚 For a complete reference to this file, see the documentation at
 # https://docs.sourcery.ai/Configuration/Project-Settings/
 
 # This file was auto-generated by Sourcery on 2023-06-10 at 10:34.
 
-version: '1'  # The schema version of this config file
+version: '1' # The schema version of this config file
 
 ignore: # A list of paths or files which Sourcery will ignore.
     - .git
     - venv
     - .venv
     - env
     - .env
@@ -31,14 +31,15 @@
         - default
         - gpsg-standard-import-alias
     disable:
         - inline-variable
         - missing-dict-items
         - extract-method
         - extract-duplicate-method
+        - code_clarification
     rule_types:
         - refactoring
         - suggestion
         - comment
     python_version: '3.10' # A string specifying the lowest Python version your project supports. Sourcery will not suggest refactorings requiring a higher Python version.
 
 # rule_tags: {} # Additional rule tags.
@@ -53,12 +54,11 @@
 #   request_review: author
 #   sourcery_branch: sourcery/{base_branch}
 
 clone_detection:
     min_lines: 7
     min_duplicates: 2
     identical_clones_only: false
-
 # proxy:
 #   url:
 #   ssl_certs_file:
 #   no_ssl_verify: false
```

### Comparing `artistools-2024.2.22.2/CITATION.cff` & `artistools-2024.4.23/CITATION.cff`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/LICENSE.txt` & `artistools-2024.4.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/PKG-INFO` & `artistools-2024.4.23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2024.2.22.2
+Version: 2024.4.23
 Summary: Plotting and analysis tools for the ARTIS 3D radiative transfer code for supernovae and kilonovae.
 Author-email: "Luke J. Shingles" <luke.shingles@gmail.com>, "Christine E. Collins" <c.collins@gsi.de>, Alexander Holas <alexander.holas@h-its.org>, Fionntan Callan <fcallan02@qub.ac.uk>, Stuart Sim <s.sim@qub.ac.uk>
 License: MIT
-Project-URL: Repository, https://www.github.com/artis-mcrt/artistools/
+Project-URL: Repository, https://www.github.com/artis-mcrt/artistools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: argcomplete>=3.2.2
-Requires-Dist: astropy>=6.0.0
-Requires-Dist: coverage>=7.4.2
+Requires-Dist: argcomplete>=3.3.0
+Requires-Dist: astropy>=6.0.1
+Requires-Dist: coverage>=7.4.4
 Requires-Dist: extinction>=0.4.6
-Requires-Dist: imageio>=2.34.0
-Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: mypy>=1.8.0
+Requires-Dist: imageio>=2.34.1
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: mypy>=1.9.0
+Requires-Dist: numexpr>=2.10.0
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pandas[compression,consortium-standard,parquet,performance]>=2.2.0
-Requires-Dist: polars>=0.20.10
-Requires-Dist: pre-commit>=3.6.2
-Requires-Dist: pyarrow>=15.0.0
+Requires-Dist: pandas[compression,parquet,pyarrow]>=2.2.2
+Requires-Dist: polars>=0.20.22
+Requires-Dist: pre-commit>=3.7.0
+Requires-Dist: pyarrow>=16.0.0
 Requires-Dist: pynonthermal>=2024.2.17
 Requires-Dist: pypdf2>=3.0.1
-Requires-Dist: pytest>=8.0.1
-Requires-Dist: pytest-cov>=4.1.0
+Requires-Dist: pytest>=8.1.1
+Requires-Dist: pytest-cov>=5.0.0
 Requires-Dist: pytest-xdist[psutil]>=3.5.0
 Requires-Dist: python-xz>=0.5
-Requires-Dist: pyvista>=0.43.3
+Requires-Dist: pyvista>=0.43.5
 Requires-Dist: PyYAML>=6.0.1
-Requires-Dist: pyzstd>=0.15.9
-Requires-Dist: ruff>=0.2.2
-Requires-Dist: scipy>=1.12.0
+Requires-Dist: pyzstd>=0.15.10
+Requires-Dist: ruff>=0.4.1
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: setuptools_scm[toml]>=8.0.4
-Requires-Dist: typeguard>=4.1.5
-Requires-Dist: types-PyYAML>=6.0.12.12
-Requires-Dist: uv>=0.1.7
-Requires-Dist: wheel>=0.42.0
+Requires-Dist: tabulate>=0.9
+Requires-Dist: typeguard>=4.2.1
+Requires-Dist: types-PyYAML>=6.0.12.20240311
+Requires-Dist: types-tabulate>=0.9.0.20240106
+Requires-Dist: wheel>=0.43.0
 
 # Artistools
 
 > Artistools is collection of plotting, analysis, and file format conversion tools for the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code.
 
 [![DOI](https://zenodo.org/badge/53433932.svg)](https://zenodo.org/badge/latestdoi/53433932)
 [![Installation and pytest](https://github.com/artis-mcrt/artistools/actions/workflows/pytest.yml/badge.svg)](https://github.com/artis-mcrt/artistools/actions/workflows/pytest.yml)
@@ -83,8 +85,8 @@
 Distributed under the MIT license. See [LICENSE](https://github.com/artis-mcrt/artistools/blob/main/LICENSE.txt) for more information.
 
 [https://github.com/artis-mcrt/artistools](https://github.com/artis-mcrt/artistools)
 
 
 ## Citing Artistools
 
-If you make use of artistools please cite it. For details, see [https://zenodo.org/badge/latestdoi/53433932](https://zenodo.org/badge/latestdoi/53433932).
+If you artistools for a paper or presentation, please cite it. For details, see [https://zenodo.org/badge/latestdoi/53433932](https://zenodo.org/badge/latestdoi/53433932).
```

### Comparing `artistools-2024.2.22.2/README.md` & `artistools-2024.4.23/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 Distributed under the MIT license. See [LICENSE](https://github.com/artis-mcrt/artistools/blob/main/LICENSE.txt) for more information.
 
 [https://github.com/artis-mcrt/artistools](https://github.com/artis-mcrt/artistools)
 
 
 ## Citing Artistools
 
-If you make use of artistools please cite it. For details, see [https://zenodo.org/badge/latestdoi/53433932](https://zenodo.org/badge/latestdoi/53433932).
+If you artistools for a paper or presentation, please cite it. For details, see [https://zenodo.org/badge/latestdoi/53433932](https://zenodo.org/badge/latestdoi/53433932).
```

### Comparing `artistools-2024.2.22.2/artistools/__init__.py` & `artistools-2024.4.23/artistools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """artistools.
 
 A collection of plotting, analysis, and file format conversion tools
 for the ARTIS radiative transfer code.
 """
+
 import typing as t
 
 from artistools import atomic
 from artistools import codecomparison
 from artistools import commands
 from artistools import deposition
 from artistools import estimators
```

### Comparing `artistools-2024.2.22.2/artistools/__main__.py` & `artistools-2024.4.23/artistools/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # PYTHON_ARGCOMPLETE_OK
-
-
 import argparse
 import importlib
 import typing as t
 
 import argcomplete
 
 from artistools.commands import CommandType
```

### Comparing `artistools-2024.2.22.2/artistools/atomic/_atomic_core.py` & `artistools-2024.4.23/artistools/atomic/_atomic_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/codecomparison.py` & `artistools-2024.4.23/artistools/codecomparison.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/commands.py` & `artistools-2024.4.23/artistools/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # new subparser based list
 subcommandtree: CommandType = {
     "comparetogsinetwork": ("gsinetwork", "main"),
     "deposition": ("deposition", "main_analytical"),
     "describeinputmodel": ("inputmodel.describeinputmodel", "main"),
     "exportmassfractions": ("estimators.exportmassfractions", "main"),
     "getpath": ("", "get_path"),
+    "lc": ("lightcurve.plotlightcurve", "main"),
     "listtimesteps": ("", "showtimesteptimes"),
     "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
     "maptogrid": ("inputmodel.maptogrid", "main"),
     "plotestimators": ("estimators.plotestimators", "main"),
     "plotinitialcomposition": ("inputmodel.plotinitialcomposition", "main"),
     "plotlightcurves": ("lightcurve.plotlightcurve", "main"),
     "plotlinefluxes": ("linefluxes", "main"),
@@ -47,15 +48,16 @@
     "plotnltepops": ("nltepops.plotnltepops", "main"),
     "plotnonthermal": ("nonthermal.plotnonthermal", "main"),
     "plotradfield": ("radfield", "main"),
     "plotspectra": ("spectra.plotspectra", "main"),
     "plotspherical": ("plotspherical", "main"),
     "plottransitions": ("transitions", "main"),
     "plotviewingangles": ("viewing_angles_visualization", "main"),
-    "setupcompletions": ("commands", "setup_completions"),
+    "completions": ("commands", "setup_completions"),
+    "spec": ("spectra.plotspectra", "main"),
     "spencerfano": ("nonthermal.solvespencerfanocmd", "main"),
     "writecodecomparisondata": ("writecomparisondata", "main"),
     "writespectra": ("spectra.writespectra", "main"),
     "inputmodel": {
         "describe": ("inputmodel.describeinputmodel", "main"),
         "maptogrid": ("inputmodel.maptogrid", "main"),
         "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
```

### Comparing `artistools-2024.2.22.2/artistools/configuration.py` & `artistools-2024.4.23/artistools/configuration.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/ElBiEn_2007.txt` & `artistools-2024.4.23/artistools/data/ElBiEn_2007.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/atomic_properties.txt` & `artistools-2024.4.23/artistools/data/atomic_properties.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/betaminusdecays.txt` & `artistools-2024.4.23/artistools/data/betaminusdecays.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/binding_energies.txt` & `artistools-2024.4.23/artistools/data/binding_energies.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/collion-AR1985.txt` & `artistools-2024.4.23/artistools/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/collion-reference.txt` & `artistools-2024.4.23/artistools/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/collion.txt` & `artistools-2024.4.23/artistools/data/collion.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/elements.csv` & `artistools-2024.4.23/artistools/data/elements.csv`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/400.txt` & `artistools-2024.4.23/artistools/data/filters/400.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/520.txt` & `artistools-2024.4.23/artistools/data/filters/520.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/B.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/U.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/V.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/gs.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/is.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/rs.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/ASIAGO/zs.txt` & `artistools-2024.4.23/artistools/data/filters/ASIAGO/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/B.txt` & `artistools-2024.4.23/artistools/data/filters/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/FUV.txt` & `artistools-2024.4.23/artistools/data/filters/FUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/H.txt` & `artistools-2024.4.23/artistools/data/filters/H.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/H_ab.txt` & `artistools-2024.4.23/artistools/data/filters/H_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/I.txt` & `artistools-2024.4.23/artistools/data/filters/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/J.txt` & `artistools-2024.4.23/artistools/data/filters/J.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/J_ab.txt` & `artistools-2024.4.23/artistools/data/filters/J_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/K.txt` & `artistools-2024.4.23/artistools/data/filters/K.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/K_ab.txt` & `artistools-2024.4.23/artistools/data/filters/K_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/B.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/I.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/R.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/U.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/V.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/gs.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/is.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/rs.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/us.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LCOGT/zs.txt` & `artistools-2024.4.23/artistools/data/filters/LCOGT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LSQ/rs.txt` & `artistools-2024.4.23/artistools/data/filters/LSQ/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LT/gs.txt` & `artistools-2024.4.23/artistools/data/filters/LT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LT/is.txt` & `artistools-2024.4.23/artistools/data/filters/LT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LT/rs.txt` & `artistools-2024.4.23/artistools/data/filters/LT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LT/us.txt` & `artistools-2024.4.23/artistools/data/filters/LT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/LT/zs.txt` & `artistools-2024.4.23/artistools/data/filters/LT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/B.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/I.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/R.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/U.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/V.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/gs.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/is.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/rs.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/us.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NOT/zs.txt` & `artistools-2024.4.23/artistools/data/filters/NOT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/B.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/I.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/R.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/U.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/V.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/gs.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/rs.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NTT/zs.txt` & `artistools-2024.4.23/artistools/data/filters/NTT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/NUV.txt` & `artistools-2024.4.23/artistools/data/filters/NUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/OGLE/I.txt` & `artistools-2024.4.23/artistools/data/filters/OGLE/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/OGLE/V.txt` & `artistools-2024.4.23/artistools/data/filters/OGLE/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/PS1/gs.txt` & `artistools-2024.4.23/artistools/data/filters/PS1/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/PS1/is.txt` & `artistools-2024.4.23/artistools/data/filters/PS1/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/PS1/rs.txt` & `artistools-2024.4.23/artistools/data/filters/PS1/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/PS1/ws.txt` & `artistools-2024.4.23/artistools/data/filters/PS1/ws.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/PS1/zs.txt` & `artistools-2024.4.23/artistools/data/filters/PS1/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/R.txt` & `artistools-2024.4.23/artistools/data/filters/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/gs.txt` & `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/is.txt` & `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/rs.txt` & `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/us.txt` & `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/SKYMAPPER/zs.txt` & `artistools-2024.4.23/artistools/data/filters/SKYMAPPER/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/U.txt` & `artistools-2024.4.23/artistools/data/filters/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/V.txt` & `artistools-2024.4.23/artistools/data/filters/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/gs.txt` & `artistools-2024.4.23/artistools/data/filters/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/is.txt` & `artistools-2024.4.23/artistools/data/filters/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/rs.txt` & `artistools-2024.4.23/artistools/data/filters/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/us.txt` & `artistools-2024.4.23/artistools/data/filters/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvm2.txt` & `artistools-2024.4.23/artistools/data/filters/uvm2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvm2_ab.txt` & `artistools-2024.4.23/artistools/data/filters/uvm2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvw1.txt` & `artistools-2024.4.23/artistools/data/filters/uvw1.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvw1_ab.txt` & `artistools-2024.4.23/artistools/data/filters/uvw1_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvw2.txt` & `artistools-2024.4.23/artistools/data/filters/uvw2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/uvw2_ab.txt` & `artistools-2024.4.23/artistools/data/filters/uvw2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/filters/zs.txt` & `artistools-2024.4.23/artistools/data/filters/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt` & `artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt` & `artistools-2024.4.23/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt` & `artistools-2024.4.23/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/2010lp_20110928_fors2.txt` & `artistools-2024.4.23/artistools/data/refspectra/2010lp_20110928_fors2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz` & `artistools-2024.4.23/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt` & `artistools-2024.4.23/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt` & `artistools-2024.4.23/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt` & `artistools-2024.4.23/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt` & `artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt` & `artistools-2024.4.23/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt` & `artistools-2024.4.23/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt` & `artistools-2024.4.23/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt` & `artistools-2024.4.23/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt` & `artistools-2024.4.23/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/data/solar_r_abundance_pattern.txt` & `artistools-2024.4.23/artistools/data/solar_r_abundance_pattern.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/deposition.py` & `artistools-2024.4.23/artistools/deposition.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/estimators/__init__.py` & `artistools-2024.4.23/artistools/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/estimators/estimators.py` & `artistools-2024.4.23/artistools/estimators/estimators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 """Functions for reading and processing estimator files.
 
 Examples are temperatures, populations, and heating/cooling rates.
 """
+
 import argparse
 import contextlib
-import itertools
 import math
 import multiprocessing
+import multiprocessing.pool
 import sys
 import time
 import typing as t
 from collections import namedtuple
 from pathlib import Path
 
 import numpy as np
@@ -44,37 +45,35 @@
         **{f"vel_{ax}_mid_on_c": "c" for ax in ["x", "y", "z", "r", "rcyl"]},
     }
 
     return variableunits.get(key) or variableunits.get(key.split("_")[0])
 
 
 def get_variablelongunits(key: str) -> str | None:
-    variablelongunits = {
+    return {
         "heating_dep/total_dep": "",
         "TR": "Temperature [K]",
         "Te": "Temperature [K]",
         "TJ": "Temperature [K]",
-    }
-    return variablelongunits.get(key)
+    }.get(key)
 
 
 def get_varname_formatted(varname: str) -> str:
-    replacements = {
+    return {
         "nne": r"n$_{\rm e}$",
         "lognne": r"Log n$_{\rm e}$",
         "rho": r"$\rho$",
         "Te": r"T$_{\rm e}$",
         "TR": r"T$_{\rm R}$",
         "TJ": r"T$_{\rm J}$",
         "gamma_NT": r"$\Gamma_{\rm non-thermal}$ [s$^{-1}$]",
         "gamma_R_bfest": r"$\Gamma_{\rm phot}$ [s$^{-1}$]",
         "heating_dep/total_dep": "Heating fraction",
         **{f"vel_{ax}_mid_on_c": f"$v_{{{ax}}}$" for ax in ["x", "y", "z", "r", "rcyl"]},
-    }
-    return replacements.get(varname, varname)
+    }.get(varname, varname)
 
 
 def apply_filters(
     xlist: t.Sequence[float] | np.ndarray, ylist: t.Sequence[float] | np.ndarray, args: argparse.Namespace
 ) -> tuple[t.Any, t.Any]:
     if (filterfunc := at.get_filterfunc(args)) is not None:
         ylist = filterfunc(ylist)
@@ -109,15 +108,15 @@
         for line in filein:
             if row := line.split():
                 if len(row) != len(header_row):
                     print("Row contains wrong number of items for header:")
                     print(header_row)
                     print(row)
                     sys.exit()
-                records.append(recomb_tuple(*[float(row[index]) for index in [index_logt, index_low_n, index_tot]]))
+                records.append(recomb_tuple(*[float(row[index]) for index in (index_logt, index_low_n, index_tot)]))
 
     return pd.DataFrame.from_records(records, columns=recomb_tuple._fields)
 
 
 def get_units_string(variable: str) -> str:
     return f" [{units}]" if (units := get_variableunits(variable)) else ""
 
@@ -220,81 +219,61 @@
         estimblocklist.append(estimblock)
 
     return pl.DataFrame(estimblocklist).with_columns(
         pl.col(pl.Int64).cast(pl.Int32), pl.col(pl.Float64).cast(pl.Float32)
     )
 
 
-def batched(iterable, n):  # -> Generator[list, Any, None]:
-    """Batch data into iterators of length n. The last batch may be shorter."""
-    # batched('ABCDEFG', 3) --> ABC DEF G
-    if n < 1:
-        msg = "n must be at least one"
-        raise ValueError(msg)
-    it = iter(iterable)
-    while True:
-        chunk_it = itertools.islice(it, n)
-        try:
-            first_el = next(chunk_it)
-        except StopIteration:
-            return
-        yield list(itertools.chain((first_el,), chunk_it))
-
-
 def get_rankbatch_parquetfile(
     modelpath: Path,
     folderpath: Path,
     batch_mpiranks: t.Sequence[int],
     batchindex: int,
 ) -> Path:
     parquetfilepath = (
         folderpath / f"estimbatch{batchindex:02d}_{batch_mpiranks[0]:04d}_{batch_mpiranks[-1]:04d}.out.parquet.tmp"
     )
 
     if not parquetfilepath.exists():
-        print(f"{parquetfilepath.relative_to(modelpath.parent)} does not exist")
+        print(f"  generating {parquetfilepath.relative_to(modelpath.parent)}.")
         estfilepaths = []
         for mpirank in batch_mpiranks:
             # not worth printing an error, because ranks with no cells to update do not produce an estimator file
             with contextlib.suppress(FileNotFoundError):
                 estfilepath = at.firstexisting(f"estimators_{mpirank:04d}.out", folder=folderpath, tryzipped=True)
                 estfilepaths.append(estfilepath)
 
         print(
-            f"  reading {len(list(estfilepaths))} estimator files from {folderpath.relative_to(Path(folderpath).parent)}"
+            f"  reading {len(estfilepaths)} estimator files from {folderpath.relative_to(Path(folderpath).parent)}...",
+            end="",
+            flush=True,
         )
 
         time_start = time.perf_counter()
 
-        pldf_group = None
+        pldf_batch = None
         if at.get_config()["num_processes"] > 1:
-            with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
-                for pldf_file in pool.imap(read_estimators_from_file, estfilepaths):
-                    if pldf_group is None:
-                        pldf_group = pldf_file
-                    else:
-                        pldf_group = pl.concat([pldf_group, pldf_file], how="diagonal_relaxed")
+            with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+                pldf_batch = pl.concat(pool.imap(read_estimators_from_file, estfilepaths), how="diagonal_relaxed")
 
                 pool.close()
                 pool.join()
-                pool.terminate()
+
         else:
-            for pldf_file in (read_estimators_from_file(estfilepath) for estfilepath in estfilepaths):
-                pldf_group = (
-                    pldf_file if pldf_group is None else pl.concat([pldf_group, pldf_file], how="diagonal_relaxed")
-                )
-
-        print(f"    took {time.perf_counter() - time_start:.1f} s")
-
-        assert pldf_group is not None
-        print(f"  writing {parquetfilepath.relative_to(modelpath.parent)}")
-        pldf_group.write_parquet(parquetfilepath, compression="zstd", statistics=True, compression_level=8)
+            pldf_batch = pl.concat(map(read_estimators_from_file, estfilepaths), how="diagonal_relaxed")
+
+        print(
+            f"took {time.perf_counter() - time_start:.1f} s. Writing {parquetfilepath.relative_to(modelpath.parent)}..."
+        )
+
+        assert pldf_batch is not None
+        pldf_batch.write_parquet(parquetfilepath, compression="zstd", statistics=True, compression_level=8)
 
     filesize = parquetfilepath.stat().st_size / 1024 / 1024
-    print(f"Scanning {parquetfilepath.relative_to(modelpath.parent)} ({filesize:.2f} MiB)")
+    print(f"  scanning {parquetfilepath.relative_to(modelpath.parent)} ({filesize:.2f} MiB)")
 
     return parquetfilepath
 
 
 def scan_estimators(
     modelpath: Path | str = Path(),
     modelgridindex: None | int | t.Sequence[int] = None,
@@ -341,29 +320,31 @@
     mpiranks_matched = (
         {at.get_mpirankofcell(modelpath=modelpath, modelgridindex=mgi) for mgi in match_modelgridindex}
         if match_modelgridindex
         else set(mpiranklist)
     )
     mpirank_groups = [
         (batchindex, mpiranks)
-        for batchindex, mpiranks in enumerate(batched(mpiranklist, 100))
+        for batchindex, mpiranks in enumerate(at.misc.batched(mpiranklist, 100))
         if mpiranks_matched.intersection(mpiranks)
     ]
 
     runfolders = at.get_runfolders(modelpath, timesteps=match_timestep)
 
     parquetfiles = (
         get_rankbatch_parquetfile(modelpath, runfolder, mpiranks, batchindex=batchindex)
         for runfolder in runfolders
         for batchindex, mpiranks in mpirank_groups
     )
+
     assert bool(parquetfiles)
 
-    pldflazy = pl.concat([pl.scan_parquet(pfile) for pfile in parquetfiles], how="diagonal_relaxed")
-    pldflazy = pldflazy.unique(["timestep", "modelgridindex"], maintain_order=True, keep="first")
+    pldflazy = pl.concat([pl.scan_parquet(pfile) for pfile in parquetfiles], how="diagonal_relaxed").unique(
+        ["timestep", "modelgridindex"], maintain_order=True, keep="first"
+    )
 
     if match_modelgridindex is not None:
         pldflazy = pldflazy.filter(pl.col("modelgridindex").is_in(match_modelgridindex))
 
     if match_timestep is not None:
         pldflazy = pldflazy.filter(pl.col("timestep").is_in(match_timestep))
 
@@ -415,16 +396,16 @@
         estimators.lazy()
         .filter(pl.col("timestep").is_in(timesteps))
         .filter(pl.col("modelgridindex") == modelgridindex)
         .select({*keys, "timestep", "modelgridindex"})
         .collect()
     )
     for k in keys:
-        valuesum = 0
-        tdeltasum = 0
+        valuesum = 0.0
+        tdeltasum = 0.0
         for timestep, tdelta in zip(timesteps, tdeltas):
             value = (
                 estcollect.filter(pl.col("timestep") == timestep)
                 .filter(pl.col("modelgridindex") == modelgridindex)[k]
                 .item(0)
             )
             if value is None:
```

### Comparing `artistools-2024.2.22.2/artistools/estimators/estimators_classic.py` & `artistools-2024.4.23/artistools/estimators/estimators_classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import gzip
+import itertools
 import typing as t
 from pathlib import Path
 
 import pandas as pd
 
 import artistools as at
 
@@ -65,15 +66,17 @@
 
 def read_classic_estimators(
     modelpath: Path,
     modeldata: pd.DataFrame,
     readonly_mgi: list[int] | None = None,
     readonly_timestep: list[int] | None = None,
 ) -> dict[tuple[int, int], t.Any] | None:
-    estimfiles = list(Path(modelpath).glob("**/estimators_????.out"))
+    estimfiles = list(
+        itertools.chain(Path(modelpath).glob("estimators_????.out"), Path(modelpath).glob("*/estimators_????.out"))
+    )
     if not estimfiles:
         print("No estimator files found")
         return None
     print(f"Reading {len(estimfiles)} estimator files...")
 
     first_timesteps_in_dir = get_first_ts_in_run_directory(modelpath)
     atomic_composition = get_atomic_composition(modelpath)
@@ -90,15 +93,15 @@
         timestep = first_timesteps_in_dir[str(estfilepath).split("/")[0]]  # get the starting timestep for the estfile
         # timestep = first_timesteps_in_dir[str(estfile[:-20])]
         # timestep = 0  # if the first timestep in the file is 0 then this is fine
         with opener(estfilepath) as estfile:
             modelgridindex = -1
             for line in estfile:
                 row = line.split()
-                if int(row[0]) <= int(modelgridindex):
+                if int(row[0]) <= modelgridindex:
                     timestep += 1
                 modelgridindex = int(row[0])
 
                 if (not readonly_mgi or modelgridindex in readonly_mgi) and (
                     not readonly_timestep or timestep in readonly_timestep
                 ):
                     estimators[(timestep, modelgridindex)] = {}
```

### Comparing `artistools-2024.2.22.2/artistools/estimators/exportmassfractions.py` & `artistools-2024.4.23/artistools/estimators/exportmassfractions.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/estimators/plot3destimators_classic.py` & `artistools-2024.4.23/artistools/estimators/plot3destimators_classic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing as t
 from collections import namedtuple
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
-import pyvista as pv
 
 import artistools as at
 
 CLIGHT = 2.99792458e10
 
 
 def read_selected_mgi(
@@ -99,29 +98,31 @@
     for mgi in readonly_mgi:
         Te[assoc_cells[mgi][0] - 1] = estimators[(timestep, mgi)]["Te"]
 
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
     grid_Te = np.zeros((grid, grid, grid))  # needs 3D array
     xgrid = np.zeros(grid)
 
-    vmax = vmax / CLIGHT
+    vmax /= CLIGHT
     i = 0
     for z in range(grid):
         for y in range(grid):
             for x in range(grid):
                 grid_Te[x, y, z] = Te[i]
                 if modeldata["rho"][i] == 0.0:
                     grid_Te[x, y, z] = None
                 xgrid[x] = -vmax + 2 * x * vmax / grid
                 i += 1
 
     return grid_Te, xgrid
 
 
 def make_2d_plot(grid, grid_Te, vmax, modelpath, xgrid, time):
+    import pyvista as pv
+
     pyvista = False
     if pyvista:
         # PYVISTA
         x, y, z = np.meshgrid(xgrid, xgrid, xgrid)
         mesh = pv.StructuredGrid(x, y, z)
         mesh["Te [K]"] = grid_Te.ravel(order="F")
 
@@ -189,15 +190,14 @@
 def main() -> None:
     modelpath = Path()
     modeldata, _, vmax = at.inputmodel.get_modeldata_tuple(modelpath)
 
     # # Get mgi of grid cells along axis for 1D plot
     # # readonly_mgi = get_modelgridcells_along_axis(modelpath)
     readonly_mgi = get_modelgridcells_2D_slice(modeldata, modelpath)
-    #
     timestep = 82
     times = at.get_timestep_times(modelpath)
     time = times[timestep]
     estimators = read_selected_mgi(modelpath, readonly_mgi=readonly_mgi, readonly_timestep=[timestep])
     grid_Te, xgrid = get_Te_vs_velocity_2D(modelpath, modeldata, vmax, estimators, readonly_mgi, timestep)
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
     make_2d_plot(grid, grid_Te, vmax, modelpath, xgrid, time)
```

### Comparing `artistools-2024.2.22.2/artistools/estimators/plotestimators.py` & `artistools-2024.4.23/artistools/estimators/plotestimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 Examples are temperatures, populations, heating/cooling rates.
 """
 
 import argparse
 import contextlib
 import math
+import operator
+import string
 import typing as t
+from itertools import chain
 from pathlib import Path
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
 import polars as pl
 import polars.selectors as cs
@@ -66,15 +69,15 @@
 
     if startfromzero:
         xlist = xlist.copy()
         xlist.insert(0, 0.0)
 
     for speciesstr in specieslist:
         splitvariablename = speciesstr.split("_")
-        elsymbol = splitvariablename[0].strip("0123456789")
+        elsymbol = splitvariablename[0].strip(string.digits)
         atomic_number = at.get_atomic_number(elsymbol)
         if seriestype == "initabundances":
             ax.set_ylim(1e-20, 1.0)
             ax.set_ylabel("Initial mass fraction")
             valuetype = "X_"
         elif seriestype == "initmasses":
             ax.set_ylabel(r"Initial mass [M$_\odot$]")
@@ -279,16 +282,16 @@
         # level index query goes outside for caching granularity reasons
         dfnltepops = at.nltepops.read_files(
             modelpath, dfquery=f"Z=={atomic_number:.0f} and ion_stage=={ion_stage:.0f}"
         ).query("level==@levelindex")
 
         ylist = []
         for modelgridindex, timesteps in zip(mgilist, timestepslist):
-            valuesum = 0
-            tdeltasum = 0
+            valuesum = 0.0
+            tdeltasum = 0.0
             # print(f'modelgridindex {modelgridindex} timesteps {timesteps}')
 
             for timestep in timesteps:
                 levelpop = (
                     dfnltepops.query(
                         "modelgridindex==@modelgridindex and timestep==@timestep and Z==@atomic_number"
                         " and ion_stage==@ion_stage and level==@levelindex"
@@ -483,47 +486,56 @@
             if ymin > 0 and new_ymax > ymin and np.isfinite(new_ymax):
                 ax.set_ylim(top=new_ymax)
 
 
 def plot_series(
     ax: plt.Axes,
     startfromzero: bool,
-    variablename: str,
+    variable: str | pl.Expr,
     showlegend: bool,
     modelpath: str | Path,
     estimators: pl.LazyFrame | pl.DataFrame,
     args: argparse.Namespace,
     nounits: bool = False,
     **plotkwargs: t.Any,
 ) -> None:
     """Plot something like Te or TR."""
-    formattedvariablename = at.estimators.get_varname_formatted(variablename)
-    serieslabel = f"{formattedvariablename}"
+    if isinstance(variable, pl.Expr):
+        colexpr = variable
+    else:
+        assert variable in estimators.columns
+        colexpr = pl.col(variable)
+
+    variablename = colexpr.meta.output_name()
+
+    serieslabel = at.estimators.get_varname_formatted(variablename)
     units_string = at.estimators.get_units_string(variablename)
 
     if showlegend:
         linelabel = serieslabel
         if not nounits:
             linelabel += units_string
     else:
         ax.set_ylabel(serieslabel + units_string)
         linelabel = None
     print(f"Plotting {variablename}")
 
     series = (
         estimators.group_by("plotpointid", maintain_order=True)
-        .agg(pl.col(variablename).mean(), pl.col("xvalue").mean())
+        .agg(colexpr.mean(), pl.col("xvalue").mean())
         .lazy()
         .collect()
     )
+
     ylist = series[variablename].to_list()
     xlist = series["xvalue"].to_list()
 
-    if min(ylist) == 0 or math.log10(max(ylist) / min(ylist)) > 2:
-        ax.set_yscale("log")
+    with contextlib.suppress(ValueError):
+        if min(ylist) == 0 or math.log10(max(ylist) / min(ylist)) > 2:
+            ax.set_yscale("log")
 
     dictcolors = {
         "Te": "red",
         # 'heating_gamma': 'blue',
         # 'cooling_adiabatic': 'blue'
     }
 
@@ -544,15 +556,15 @@
     allnonemptymgilist: t.Sequence[int],
     estimators: pl.LazyFrame,
     timestepslist: t.Any,
     modelpath: str | Path,
     groupbyxvalue: bool,
     args: t.Any,
 ) -> tuple[list[float | int], list[int], list[list[int]], pl.LazyFrame]:
-    estimators = estimators.filter(pl.col("timestep").is_in([ts for tssublist in timestepslist for ts in tssublist]))
+    estimators = estimators.filter(pl.col("timestep").is_in(set(chain.from_iterable(timestepslist))))
 
     if xvariable in {"cellid", "modelgridindex"}:
         estimators = estimators.with_columns(xvalue=pl.col("modelgridindex"), plotpointid=pl.col("modelgridindex"))
     elif xvariable == "timestep":
         estimators = estimators.with_columns(xvalue=pl.col("timestep"), plotpointid=pl.col("timestep"))
     elif xvariable == "time":
         estimators = estimators.with_columns(xvalue=pl.col("time_mid"), plotpointid=pl.col("timestep"))
@@ -604,33 +616,39 @@
     estimators: pl.LazyFrame,
     args: argparse.Namespace,
     **plotkwargs: t.Any,
 ) -> None:
     """Make plot from ARTIS estimators."""
     # these three lists give the x value, modelgridex, and a list of timesteps (for averaging) for each plot of the plot
     showlegend = False
+    legend_kwargs = {}
     seriescount = 0
     ylabel = None
     sameylabel = True
-    for variablename in plotitems:
-        if isinstance(variablename, str):
-            seriescount += 1
-            if ylabel is None:
-                ylabel = get_ylabel(variablename)
-            elif ylabel != get_ylabel(variablename):
-                sameylabel = False
-                break
+    seriesvars = [var for var in plotitems if isinstance(var, str | pl.Expr)]
+    seriescount = len(seriesvars)
+
+    for variable in seriesvars:
+        variablename = variable.meta.output_name() if isinstance(variable, pl.Expr) else variable
+        if ylabel is None:
+            ylabel = get_ylabel(variablename)
+        elif ylabel != get_ylabel(variablename):
+            sameylabel = False
+            break
 
     for plotitem in plotitems:
-        if isinstance(plotitem, str):
-            showlegend = seriescount > 1 or len(plotitem) > 20 or not sameylabel
+        if isinstance(plotitem, str | pl.Expr):
+            variablename = plotitem.meta.output_name() if isinstance(plotitem, pl.Expr) else plotitem
+            assert isinstance(variablename, str)
+            showlegend = seriescount > 1 or len(variablename) > 35 or not sameylabel
+            print(f"Plotting {showlegend=} {len(variablename)=} {sameylabel=} {ylabel=}")
             plot_series(
                 ax=ax,
                 startfromzero=startfromzero,
-                variablename=plotitem,
+                variable=plotitem,
                 showlegend=showlegend,
                 modelpath=modelpath,
                 estimators=estimators,
                 args=args,
                 nounits=sameylabel,
                 **plotkwargs,
             )
@@ -690,14 +708,17 @@
 
             elif seriestype == "_yscale":
                 ax.set_yscale(params)
 
             else:
                 showlegend = True
                 seriestype, ionlist = plotitem
+                if seriestype == "populations" and len(ionlist) > 2 and args.yscale == "log":
+                    legend_kwargs["ncol"] = 2
+
                 plot_multi_ion_series(
                     ax=ax,
                     startfromzero=startfromzero,
                     seriestype=seriestype,
                     ionlist=ionlist,
                     estimators=estimators,
                     modelpath=modelpath,
@@ -708,19 +729,15 @@
     ax.tick_params(right=True)
     if showlegend and not args.nolegend:
         ax.legend(
             loc="upper right",
             handlelength=2,
             frameon=False,
             numpoints=1,
-            **(
-                {"ncol": math.ceil(len(plotitems[0][1]) / 2.0)}
-                if (plotitems[0][0] == "populations" and args.yscale == "log")
-                else {}
-            ),
+            **legend_kwargs,
             markerscale=3,
         )
 
 
 def make_plot(
     modelpath: Path | str,
     timestepslist_unfiltered: list[list[int]],
@@ -737,15 +754,16 @@
         nrows=len(plotlist),
         ncols=1,
         sharex=True,
         figsize=(
             args.figscale * at.get_config()["figwidth"] * args.scalefigwidth,
             args.figscale * at.get_config()["figwidth"] * 0.5 * len(plotlist),
         ),
-        tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
+        layout="constrained",
+        # tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
     )
     if len(plotlist) == 1:
         axes = [axes]
 
     # ax.xaxis.set_minor_locator(ticker.MultipleLocator(base=5))
     if not args.hidexlabel:
         axes[-1].set_xlabel(
@@ -817,15 +835,15 @@
         if Path(args.outputfile).is_dir():
             args.outputfile = str(Path(args.outputfile) / defaultoutputfile)
 
         assert isinstance(timestepslist[0], list)
         outfilename = str(args.outputfile).format(timestep=timestep, timedays=timedays, format=args.format)
 
     if not args.notitle:
-        axes[0].set_title(figure_title, fontsize=12)
+        axes[0].set_title(figure_title, fontsize=10)
 
     print(f"Saving {outfilename} ...")
     fig.savefig(outfilename, dpi=300)
 
     if args.show:
         plt.show()
     else:
@@ -861,15 +879,15 @@
                 list_rrc.append(dicttimestepmodelgrid["RRC_LTE_Nahar"][(atomic_number, ion_stage)])
                 list_rrc2.append(dicttimestepmodelgrid["Alpha_R"][(atomic_number, ion_stage)])
 
         if not list_rrc:
             continue
 
         # sort the pairs by temperature ascending
-        listT_e, list_rrc, list_rrc2 = zip(*sorted(zip(listT_e, list_rrc, list_rrc2), key=lambda x: x[0]))
+        listT_e, list_rrc, list_rrc2 = zip(*sorted(zip(listT_e, list_rrc, list_rrc2), key=operator.itemgetter(0)))
 
         ax.plot(listT_e, list_rrc, linewidth=2, label=f"{ionstr} ARTIS RRC_LTE_Nahar", **plotkwargs)
         ax.plot(listT_e, list_rrc2, linewidth=2, label=f"{ionstr} ARTIS Alpha_R", **plotkwargs)
 
         with contextlib.suppress(KeyError):
             dfrates = recombcalibrationdata[(atomic_number, ion_stage)].query(
                 "T_e > @T_e_min & T_e < @T_e_max", local_dict={"T_e_min": min(listT_e), "T_e_max": max(listT_e)}
@@ -898,15 +916,15 @@
         #     ax.plot(listT_e_Nahar, dfrecombrates['RRC_total'], linewidth=2,
         #             label=ionstr + " (Nahar)", markersize=6, marker='s', **plotkwargs)
 
         ax.legend(loc="best", handlelength=2, frameon=False, numpoints=1, prop={"size": 10})
 
     # modelname = at.get_model_name(".")
     # plotlabel = f'Timestep {timestep}'
-    # time_days = float(at.get_timestep_time('spec.out', timestep))
+    # time_days = at.get_timestep_time('spec.out', timestep)
     # if time_days >= 0:
     #     plotlabel += f' (t={time_days:.2f}d)'
     # fig.suptitle(plotlabel, fontsize=12)
     elsymbol = at.get_elsymbol(atomic_number)
     outfilename = f"plotestimators_recombrates_{elsymbol}.pdf"
     fig.savefig(outfilename)
     print(f"Saved {outfilename}")
@@ -1047,14 +1065,18 @@
 
     plotlist = args.plotlist or [
         # [["initabundances", ["Fe", "Ni_stable", "Ni_56"]]],
         # ['heating_dep', 'heating_coll', 'heating_bf', 'heating_ff',
         #  ['_yscale', 'linear']],
         # ['cooling_adiabatic', 'cooling_coll', 'cooling_fb', 'cooling_ff',
         #  ['_yscale', 'linear']],
+        # [
+        #     (pl.col("heating_coll") - pl.col("cooling_coll")).alias("collisional heating - cooling"),
+        #     ["_yscale", "linear"],
+        # ],
         # [['initmasses', ['Ni_56', 'He', 'C', 'Mg']]],
         # ['heating_gamma/gamma_dep'],
         # ["nne", ["_ymin", 1e5], ["_ymax", 1e10]],
         ["rho", ["_yscale", "log"], ["_ymin", 1e-16]],
         ["TR", ["_yscale", "linear"]],  # , ["_ymin", 1000], ["_ymax", 15000]
         # ["Te"],
         # ["Te", "TR"],
```

### Comparing `artistools-2024.2.22.2/artistools/estimators/test_estimators.py` & `artistools-2024.4.23/artistools/estimators/test_estimators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import mock
 
 import matplotlib.axes
 import numpy as np
+import polars as pl
 
 import artistools as at
 
 modelpath = at.get_config()["path_testdata"] / "testmodel"
 modelpath_classic_3d = at.get_config()["path_testdata"] / "test-classicmode_3d"
 outputpath = at.get_config()["path_testoutput"]
 
@@ -20,14 +21,15 @@
         [["averageionisation", ["Fe", "Ni"]]],
         [["averageexcitation", ["Fe II"]]],
         [["populations", ["Fe I", "Fe II", "Fe III", "Fe IV", "Fe V"]]],
         [["populations", ["Co II", "Co III", "Co IV"]]],
         [["gamma_NT", ["Fe I", "Fe II", "Fe III", "Fe IV"]]],
         ["heating_dep", "heating_coll", "heating_bf", "heating_ff", ["_yscale", "linear"]],
         ["cooling_adiabatic", "cooling_coll", "cooling_fb", "cooling_ff", ["_yscale", "linear"]],
+        [(pl.col("heating_coll") - pl.col("cooling_coll")).alias("collisional heating - cooling")],
     ]
 
     at.estimators.plot(argsraw=[], modelpath=modelpath, plotlist=plotlist, outputfile=outputpath, timedays=300)
     xarr = [0.0, 4000.0]
     for x in mockplot.call_args_list:
         assert xarr == x[0][1]
 
@@ -58,14 +60,15 @@
         "heating_coll": 2.37823e-09,
         "heating_bf": 1.27067e-13,
         "heating_ff": 1.86474e-16,
         "cooling_adiabatic": 9.72392e-13,
         "cooling_coll": 3.02786e-09,
         "cooling_fb": 4.82714e-12,
         "cooling_ff": 1.62999e-13,
+        "collisional heating - cooling": -6.4962990e-10,
     }
     assert len(expectedvals) == len(mockplot.call_args_list)
     yvals = {varname: callargs[0][2] for varname, callargs in zip(expectedvals.keys(), mockplot.call_args_list)}
 
     print({key: yarr[1] for key, yarr in yvals.items()})
 
     for varname, expectedval in expectedvals.items():
@@ -86,14 +89,15 @@
         [["averageionisation", ["Fe", "Ni"]]],
         [["averageexcitation", ["Fe II"]]],
         [["populations", ["Fe I", "Fe II", "Fe III", "Fe IV", "Fe V"]]],
         [["populations", ["Co II", "Co III", "Co IV"]]],
         [["gamma_NT", ["Fe I", "Fe II", "Fe III", "Fe IV"]]],
         ["heating_dep", "heating_coll", "heating_bf", "heating_ff", ["_yscale", "linear"]],
         ["cooling_adiabatic", "cooling_coll", "cooling_fb", "cooling_ff", ["_yscale", "linear"]],
+        [(pl.col("heating_coll") - pl.col("cooling_coll")).alias("collisional heating - cooling")],
     ]
 
     at.estimators.plot(argsraw=[], modelpath=modelpath, plotlist=plotlist, outputfile=outputpath, timestep="50-54")
     xarr = [0.0, 4000.0]
     for x in mockplot.call_args_list:
         assert xarr == x[0][1]
 
@@ -124,14 +128,15 @@
         "heating_coll": 2.4779998053503505e-09,
         "heating_bf": 1.2916119454357833e-13,
         "heating_ff": 2.1250019797070045e-16,
         "cooling_adiabatic": 1.000458830363593e-12,
         "cooling_coll": 3.1562059632506134e-09,
         "cooling_fb": 5.0357105638165756e-12,
         "cooling_ff": 1.7027620090835638e-13,
+        "collisional heating - cooling": -6.782059913668093e-10,
     }
     assert len(expectedvals) == len(mockplot.call_args_list)
     yvals = {varname: callargs[0][2] for varname, callargs in zip(expectedvals.keys(), mockplot.call_args_list)}
 
     print({key: yarr[1] for key, yarr in yvals.items()})
 
     for varname, expectedval in expectedvals.items():
@@ -183,15 +188,15 @@
 
     assert len(expectedvals) == len(mockplot.call_args_list)
     yvals = {
         varname: np.array(callargs[0][2]).mean()
         for varname, callargs in zip(expectedvals.keys(), mockplot.call_args_list)
     }
 
-    print(dict(yvals))
+    print(yvals)
 
     for varname, expectedval in expectedvals.items():
         assert np.allclose(expectedval, yvals[varname], rtol=0.001), (
             varname,
             expectedval,
             yvals[varname],
         )
```

### Comparing `artistools-2024.2.22.2/artistools/gsinetwork.py` & `artistools-2024.4.23/artistools/gsinetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # PYTHON_ARGCOMPLETE_OK
 
 
 import argparse
 import contextlib
 import math
 import multiprocessing
+import string
 import typing as t
 from functools import partial
 from pathlib import Path
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
@@ -17,15 +18,15 @@
 import polars as pl
 
 import artistools as at
 
 
 def strnuc_to_latex(strnuc: str):
     """Convert a string like sr89 to $^{89}$Sr."""
-    elsym = strnuc.rstrip("0123456789")
+    elsym = strnuc.rstrip(string.digits)
     massnum = strnuc.removeprefix(elsym)
 
     return rf"$^{{{massnum}}}${elsym.title()}"
 
 
 def plot_qdot(
     modelpath: Path,
@@ -441,15 +442,15 @@
         if direct_model_propgrid_map:
             print("  detected direct mapping of model cells to propagation grid")
     except FileNotFoundError:
         print("No grid mapping file found, assuming direct mapping of model cells to propagation grid")
         direct_model_propgrid_map = True
 
     if direct_model_propgrid_map:
-        correction_factors = {strnuc: 1.0 for strnuc in arr_strnuc}
+        correction_factors = dict.fromkeys(arr_strnuc, 1.0)
 
         lzdfmodel = lzdfmodel.with_columns(n_assoc_cells=pl.lit(1.0))
     else:
         ncoordgridx = math.ceil(np.cbrt(max(mgi_of_propcells.keys())))
         propcellcount = int(math.ceil(ncoordgridx ** (1 / 3.0)) ** 3)
         assert propcellcount**3 == ncoordgridx
         xmax_tmodel = modelmeta["vmax_cmps"] * modelmeta["t_model_init_days"] * 86400
@@ -542,15 +543,15 @@
 
             if mgi == first_mgi:
                 arr_time_artis_days.append(time_days)
 
             for strnuc, a in zip(arr_strnuc, arr_a):
                 abund = estimtsmgsi[f"nniso_{strnuc}"].item()
                 massfrac = abund * a * MH / estimtsmgsi["rho"].item()
-                massfrac = massfrac + estimtsmgsi[f"X_{strnuc}"].item() * (correction_factors[strnuc] - 1.0)
+                massfrac += estimtsmgsi[f"X_{strnuc}"].item() * (correction_factors[strnuc] - 1.0)
 
                 if mgi not in arr_abund_artis:
                     arr_abund_artis[mgi] = {}
 
                 if strnuc not in arr_abund_artis[mgi]:
                     arr_abund_artis[mgi][strnuc] = []
 
@@ -568,40 +569,41 @@
     mergertime_geomunits = at.inputmodel.modelfromhydro.get_merger_time_geomunits(griddata_root)
     t_mergertime_s = mergertime_geomunits * 4.926e-6
     arr_time_gsi_s_incpremerger = np.array(
         [modelmeta["t_model_init_days"] * 86400 + t_mergertime_s, *arr_time_artis_s_alltimesteps]
     )
     arr_time_gsi_days = list(arr_time_gsi_s / 86400)
 
-    dfpartcontrib = at.inputmodel.rprocess_from_trajectory.get_gridparticlecontributions(modelpath)
-    dfpartcontrib = dfpartcontrib.filter((pl.col("cellindex") <= npts_model) & (pl.col("frac_of_cellmass") > 0))
+    dfpartcontrib = at.inputmodel.rprocess_from_trajectory.get_gridparticlecontributions(modelpath).filter(
+        (pl.col("cellindex") <= npts_model) & (pl.col("frac_of_cellmass") > 0)
+    )
 
     mgiplotlistplus1 = [mgi + 1 for mgi in mgiplotlist]
     list_particleids_getabund = dfpartcontrib.filter(pl.col("cellindex").is_in(mgiplotlistplus1))["particleid"].unique()
     fworkerwithabund = partial(get_particledata, arr_time_gsi_s_incpremerger, arr_strnuc_z_n, traj_root, verbose=True)
 
     print(f"Reading trajectories from {traj_root}")
     print(f"Reading Qdot/thermo and abundance data for {len(list_particleids_getabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_withabund = pool.map(fworkerwithabund, list_particleids_getabund)
             pool.close()
             pool.join()
     else:
         list_particledata_withabund = [fworkerwithabund(particleid) for particleid in list_particleids_getabund]
 
     list_particleids_noabund = [
         pid for pid in dfpartcontrib["particleid"].unique() if pid not in list_particleids_getabund
     ]
     fworkernoabund = partial(get_particledata, arr_time_gsi_s_incpremerger, [], traj_root)
     print(f"Reading for Qdot/thermo data (no abundances needed) for {len(list_particleids_noabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_noabund = pool.map(fworkernoabund, list_particleids_noabund)
             pool.close()
             pool.join()
     else:
         list_particledata_noabund = [fworkernoabund(particleid) for particleid in list_particleids_noabund]
 
     allparticledata = dict(list_particledata_withabund + list_particledata_noabund)
```

### Comparing `artistools-2024.2.22.2/artistools/hesma_scripts.py` & `artistools-2024.4.23/artistools/hesma_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 def plot_hesma_spectrum(timeavg, axes):
     hesma_file = Path("/Users/ccollins/Downloads/hesma_files/M2a/hesma_specseq.dat")
     hesma_spec = pd.read_csv(hesma_file, comment="#", sep=r"\s+", dtype=float)
     # print(hesma_spec)
 
     def match_closest_time(reftime):
-        return str(f"{min((float(x) for x in hesma_spec.keys()[1:]), key=lambda x: abs(x - reftime))}")
+        return str(min((float(x) for x in hesma_spec.keys()[1:]), key=lambda x: abs(x - reftime)))
 
     closest_time = match_closest_time(timeavg)
     closest_time = f"{closest_time:.2f}"
     print(closest_time)
 
     # Scale distance to 1 Mpc
     dist_mpc = 1e-5  # HESMA specta at 10 pc
-    hesma_spec[closest_time] = hesma_spec[closest_time] * (dist_mpc) ** 2  # refspecditance Mpc / 1 Mpc ** 2
+    hesma_spec[closest_time] *= dist_mpc**2  # refspecditance Mpc / 1 Mpc ** 2
 
     for ax in axes:
         ax.plot(hesma_spec["0.00"], hesma_spec[closest_time], label="HESMA model")
 
 
 def plothesmaresspec(fig, ax):
     # specfiles = ["/Users/ccollins/Downloads/hesma_files/M2a_i55/hesma_specseq_theta.dat"]
@@ -78,15 +78,15 @@
         vspecdata = vspecdata_all["I"]
 
         timearray = vspecdata.columns.to_numpy()[1:]
         vspecdata = vspecdata.sort_values(by="nu", ascending=False)
         vspecdata = vspecdata.eval("lambda_angstroms = 2.99792458e+18 / nu")
         for time in timearray:
             vspecdata[time] = vspecdata[time] * vspecdata["nu"] / vspecdata["lambda_angstroms"]
-            vspecdata[time] = vspecdata[time] * (1e5) ** 2  # Scale to 10 pc (1 Mpc/10 pc) ** 2
+            vspecdata[time] *= 100000.0**2  # Scale to 10 pc (1 Mpc/10 pc) ** 2
 
         vspecdata = vspecdata.set_index("lambda_angstroms").reset_index()
         vspecdata = vspecdata.drop(["nu"], axis=1)
 
         vspecdata = vspecdata.rename(columns={"lambda_angstroms": "0"})
 
         outfilename = f"{modelname}_vspec_res.dat"
@@ -146,16 +146,15 @@
         "peakmag": dm15data["peakmag"],  # dm15 peak mag probably more accurate - shorter time window
         "dm15": dm15data["dm15"],
     }
     if dm40:
         outdata["dm40"] = dm40data["dm40"]
     outdata["angle_bin"] = angle_definition.values()
 
-    outdataframe = pd.DataFrame(outdata)
-    outdataframe = outdataframe.round(decimals=4)
+    outdataframe = pd.DataFrame(outdata).round(decimals=4)
     outdataframe.to_csv(outpath / f"{modelname}_width-luminosity.dat", sep=" ", index=False, header=True)
 
 
 def read_hesma_peakmag_dm15_dm40(pathtofiles):
     data = []
     for filename in os.listdir(pathtofiles):
         print(filename)
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/1dslicefrom3d.py` & `artistools-2024.4.23/artistools/inputmodel/1dslicefrom3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
 
             if len(blocksplit[1]) == 5:
                 (cell["ffe"], cell["f56ni"], cell["fco"], cell["f52fe"], cell["f48cr"]) = map(float, blocksplit[1])
             else:
                 print("Wrong line size")
                 sys.exit()
 
-            xmatch = cell["pos_x_min"] == "0.0000000" or chosenaxis == "x" and float(cell["pos_x_min"]) >= 0.0
-            ymatch = cell["pos_y_min"] == "0.0000000" or chosenaxis == "y" and float(cell["pos_y_min"]) >= 0.0
-            zmatch = cell["pos_z_min"] == "0.0000000" or chosenaxis == "z" and float(cell["pos_z_min"]) >= 0.0
+            xmatch = cell["pos_x_min"] == "0.0000000" or (chosenaxis == "x" and float(cell["pos_x_min"]) >= 0.0)
+            ymatch = cell["pos_y_min"] == "0.0000000" or (chosenaxis == "y" and float(cell["pos_y_min"]) >= 0.0)
+            zmatch = cell["pos_z_min"] == "0.0000000" or (chosenaxis == "z" and float(cell["pos_z_min"]) >= 0.0)
             if xmatch and ymatch and zmatch:
                 outcellid += 1
                 dict3dcellidto1dcellid[int(cell["cellid"])] = outcellid
                 append_cell_to_output(cell, outcellid, t_model, listout, xlist, ylists)
                 print(f"Cell {outcellid:4d} input1: {block[0].rstrip()}")
                 print(f"Cell {outcellid:4d} input2: {block[1].rstrip()}")
                 print(f"Cell {outcellid:4d} output: {listout[-1]}")
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/__init__.py` & `artistools-2024.4.23/artistools/inputmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/botyanski2017.py` & `artistools-2024.4.23/artistools/inputmodel/botyanski2017.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             radioabundances = [0.0, 0.0, 0.0, 0.0, 0.0]
             abundances[14] = 0.7
             abundances[16] = 0.29
             abundances[20] = 0.01
 
         dfmodel.loc[cellid] = [cellid + 1, v_outer, math.log10(rho), *radioabundances]
         dfelabundances.loc[cellid] = [cellid + 1, *abundances[1:31]]
-        r_inner, r_outer = ((v * u.km / u.s * t200 * 200 * u.day).to("cm").value for v in [v_inner, v_outer])
+        r_inner, r_outer = ((v * u.km / u.s * t200 * 200 * u.day).to("cm").value for v in (v_inner, v_outer))
 
         vol_shell = 4 * math.pi / 3 * (r_outer**3 - r_inner**3)
         m_shell = rho * vol_shell / u.solMass.to("g")
         m_tot += m_shell
 
         v_inner = v_outer
     print(f"M_tot = {m_tot:.3f} solMass")
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/describeinputmodel.py` & `artistools-2024.4.23/artistools/inputmodel/describeinputmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import math
 import os
+import string
 import typing as t
 from pathlib import Path
 
 import argcomplete
 import numpy as np
 import polars as pl
 import polars.selectors as cs
@@ -54,16 +55,17 @@
     dfmodel, modelmeta = at.inputmodel.get_modeldata_polars(
         args.inputfile,
         get_elemabundances=True,
         printwarningsonly=False,
         derived_cols=["mass_g", "vel_r_mid", "rho"],
     )
 
-    dfmodel = dfmodel.filter(pl.col("rho") > 0.0)
-    dfmodel = dfmodel.drop("X_n")  # don't confuse neutrons with Nitrogen
+    dfmodel = (
+        dfmodel.filter(pl.col("rho") > 0.0).drop("X_n")  # don't confuse neutrons with Nitrogen
+    )
 
     if args.noabund:
         dfmodel = dfmodel.drop(cs.starts_with("X_"))
 
     if not args.isotopes:
         dfmodel = dfmodel.drop(cs.matches("X_[A-z]+[0-9]"))
 
@@ -72,42 +74,42 @@
     t_model_init_days, vmax = modelmeta["t_model_init_days"], modelmeta["vmax_cmps"]
 
     t_model_init_seconds = t_model_init_days * 24 * 60 * 60
     msun_g = 1.989e33
     print(f"Model is defined at {t_model_init_days} days ({t_model_init_seconds:.4f} seconds)")
 
     if modelmeta["dimensions"] == 1:
-        vmax_kmps = dfmodel.select(pl.col("vel_r_max_kmps").max()).collect().item(0, 0)
+        vmax_kmps = dfmodel.select(pl.col("vel_r_max_kmps").max()).collect().item()
         vmax = vmax_kmps * 1e5
         print(
             f"Model contains {modelmeta['npts_model']} 1D spherical shells with vmax = {vmax / 1e5} km/s"
             f" ({vmax / 29979245800:.2f} * c)"
         )
     else:
-        nonemptycells = dfmodel.select([(pl.col("rho") > 0.0).count()]).collect().item(0, 0)
+        nonemptycells = dfmodel.filter(pl.col("rho") > 0.0).select(pl.len()).collect().item()
         print(
             f"Model contains {modelmeta['npts_model']} grid cells ({nonemptycells} nonempty) with "
             f"vmax = {vmax} cm/s ({vmax * 1e-5 / 299792.458:.2f} * c)"
         )
         vmax_corner_3d = math.sqrt(3 * vmax**2)
         print(f"  3D corner vmax: {vmax_corner_3d:.2e} cm/s ({vmax_corner_3d * 1e-5 / 299792.458:.2f} * c)")
         if modelmeta["dimensions"] == 2:
             vmax_corner_2d = math.sqrt(2 * vmax**2)
             print(f"  2D corner vmax: {vmax_corner_2d:.2e} cm/s ({vmax_corner_2d * 1e-5 / 299792.458:.2f} * c)")
 
-    minrho = dfmodel.select(pl.col("rho").min()).collect().item(0, 0)
+    minrho = dfmodel.select(pl.col("rho").min()).collect().item()
     minrho_cellcount = (
         dfmodel.filter(pl.col("rho") == minrho)
         .group_by("rho", maintain_order=False)
-        .agg(pl.count("inputcellid").alias("count_inputcellid"))
-        .select("count_inputcellid")
+        .agg(pl.len().alias("minrho_cellcount"))
+        .select("minrho_cellcount")
         .collect()
-        .item(0, 0)
+        .item()
     )
-    print(f"  min density: {minrho:.2e} g/cm^3. Cells with this density: {minrho_cellcount}")
+    print(f"  min density: {minrho:.2e} g/cm³. Cells with this density: {minrho_cellcount}")
 
     if args.cell is not None:
         mgi = int(args.cell)
         if mgi >= 0:
             print(f"Selected single cell mgi {mgi}:")
             dfmodel = dfmodel.filter(pl.col("inputcellid") == (mgi + 1))
 
@@ -117,21 +119,21 @@
         assoc_cells, mgi_of_propcells = at.get_grid_mapping(args.inputfile)
         print(f"  {len(assoc_cells)} model cells have associated prop cells")
     except FileNotFoundError:
         print("  no cell mapping file found")
         assoc_cells, mgi_of_propcells = None, None
 
     if "q" in dfmodel.columns:
-        initial_energy = dfmodel.select(pl.col("q").dot(pl.col("mass_g"))).collect().item(0, 0)
+        initial_energy = dfmodel.select(pl.col("q").dot(pl.col("mass_g"))).collect().item()
         assert initial_energy is not None
         print(f'  {"initial energy":19s} {initial_energy:.3e} erg')
     else:
         initial_energy = 0.0
 
-    mass_msun_rho = dfmodel.select(pl.col("mass_g").sum() / msun_g).collect().item(0, 0)
+    mass_msun_rho = dfmodel.select(pl.col("mass_g").sum() / msun_g).collect().item()
 
     if assoc_cells is not None and mgi_of_propcells is not None:
         direct_model_propgrid_map = all(
             len(propcells) == 1 and mgi == propcells[0] for mgi, propcells in assoc_cells.items()
         )
         if direct_model_propgrid_map:
             print("  detected direct mapping of model cells to propagation grid")
@@ -166,15 +168,15 @@
 
     if modelmeta["dimensions"] > 1:
         corner_mass = (
             dfmodel.select(["vel_r_mid", "mass_g"])
             .filter(pl.col("vel_r_mid") > vmax)
             .select(pl.col("mass_g").sum())
             .collect()
-            .item(0, 0)
+            .item()
         ) / msun_g
         print(
             f'  {"M_corners":19s} {corner_mass:8.5f} MSun ('
             f" {100 * corner_mass / mass_msun_rho:.2f}% of M_tot in cells with v_r_mid > vmax)"
         )
 
     if args.noabund:
@@ -185,26 +187,26 @@
     mass_msun_lanthanides = 0.0
     mass_msun_actinides = 0.0
     speciesmasses: dict[str, float] = {}
 
     for column in dfmodel.select(cs.starts_with("X_") - cs.by_name("X_Fegroup")).columns:
         species = column.replace("X_", "")
 
-        speciesabund_g = dfmodel.select(pl.col(column).dot(pl.col("mass_g"))).collect().item(0, 0)
+        speciesabund_g = dfmodel.select(pl.col(column).dot(pl.col("mass_g"))).collect().item()
 
         assert isinstance(speciesabund_g, float)
 
         species_mass_msun = speciesabund_g / msun_g
 
-        atomic_number = at.get_atomic_number(species.rstrip("0123456789"))
+        atomic_number = at.get_atomic_number(species.rstrip(string.digits))
 
         if species[-1].isdigit():
             # isotopic species
 
-            elname = species.rstrip("0123456789")
+            elname = species.rstrip(string.digits)
             strtotiso = f"{elname}_isosum"
             speciesmasses[strtotiso] = speciesmasses.get(strtotiso, 0.0) + speciesabund_g
             mass_msun_isotopes += species_mass_msun
 
             if args.isotopes and speciesabund_g > 0.0:
                 speciesmasses[species] = speciesabund_g
 
@@ -226,15 +228,15 @@
 
     if args.isotopes:
         print(
             f'  {"M_tot_iso":19s} {mass_msun_isotopes:8.5f} MSun ({mass_msun_isotopes / mass_msun_rho * 100:6.2f}% '
             "of M_tot_rho, but can be < 100% if stable isotopes not tracked)"
         )
 
-    mass_msun_fegroup = dfmodel.select(pl.col("X_Fegroup").dot(pl.col("mass_g"))).collect().item(0, 0) / msun_g
+    mass_msun_fegroup = dfmodel.select(pl.col("X_Fegroup").dot(pl.col("mass_g"))).collect().item() / msun_g
     print(
         f'  {"M_Fegroup":19s} {mass_msun_fegroup:8.5f} MSun'
         f" ({mass_msun_fegroup / mass_msun_rho * 100:6.2f}% of M_tot_rho)"
     )
 
     print(
         f'  {"M_lanthanide_isosum":19s} {mass_msun_lanthanides:8.5f} MSun'
@@ -276,15 +278,15 @@
                 # iso sum matches the element mass, so don't show it
                 continue
             strcomment += f"({mass_g / elem_mass * 100:6.2f}% of {elsymb} element mass from abundances.txt)"
 
             if mass_g > elem_mass * (1.0 + 1e-5):
                 strcomment += " ERROR! isotope sum is greater than element abundance"
 
-        zstr = f"{atomic_number}"
+        zstr = str(atomic_number)
         barstr = "-" * int(maxbarchars * (mass_g - mass_g_min) / (mass_g_max - mass_g_min))
         print(f"{zstr:>5} {species:11s} massfrac {massfrac:.3e}   {species_mass_msun:.3e} Msun  {barstr}")
         if strcomment:
             print(f"    {strcomment}")
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/downscale3dgrid.py` & `artistools-2024.4.23/artistools/inputmodel/downscale3dgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import itertools
 from pathlib import Path
 
 import numpy as np
+from typeguard import typechecked
 
 import artistools as at
 
 
+@typechecked
 def make_downscaled_3d_grid(
     modelpath: str | Path, outputgridsize: int = 50, plot: bool = False, outputfolder: Path | str | None = None
 ) -> Path:
     """Get a 3D model with smallgrid^3 cells from a 3D model with grid^3 cells.
     Should be same as downscale_3d_grid.pro.
     """
     modelpath = Path(modelpath)
@@ -17,15 +19,15 @@
     dfmodel, modelmeta = at.get_modeldata(modelpath)
     dfelemabund = at.inputmodel.get_initelemabundances(modelpath)
 
     inputgridsize = modelmeta["ncoordgridx"]
     grid = int(inputgridsize)
 
     assert inputgridsize % outputgridsize == 0
-    smallgrid = int(outputgridsize)
+    smallgrid = outputgridsize
 
     merge = grid / smallgrid
     merge = int(merge)
 
     outputfolder = Path(modelpath, f"downscale_{outputgridsize}^3") if outputfolder is None else Path(outputfolder)
     outputfolder.mkdir(exist_ok=True)
     smallmodelfile = outputfolder / "model.txt"
@@ -84,31 +86,31 @@
             rho_small[x, y, z] /= merge**3
 
     print("writing abundance file")
     i = 0
     with (modelpath / smallabundancefile).open("w") as newabundancefile:
         for z, y, x in itertools.product(range(smallgrid), range(smallgrid), range(smallgrid)):
             line = abund_small[x, y, z, :].tolist()  # index 1:30 are abundances
-            line[0] = int(i + 1)  # replace index 0 with index id
+            line[0] = i + 1  # replace index 0 with index id
             i += 1
             newabundancefile.writelines("%g " % item for item in line)
             newabundancefile.writelines("\n")
 
     print("writing model file")
     xmax = vmax * t_model_days * 3600 * 24
     cellindex = 0
     with (modelpath / smallmodelfile).open("w") as newmodelfile:
-        gridsize = int(smallgrid**3)
+        gridsize = smallgrid**3
         newmodelfile.write(f"{gridsize}\n")
         newmodelfile.write(f"{t_model_days}\n")
         newmodelfile.write(f"{vmax}\n")
 
         for z, y, x in itertools.product(range(smallgrid), range(smallgrid), range(smallgrid)):
             line1 = [
-                int(cellindex + 1),
+                cellindex + 1,
                 -xmax + 2 * x * xmax / smallgrid,
                 -xmax + 2 * y * xmax / smallgrid,
                 -xmax + 2 * z * xmax / smallgrid,
                 rho_small[x, y, z],
             ]
             line2 = radioabunds_small[x, y, z, :]
             newmodelfile.writelines("%g " % item for item in line1)
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/energyinputfiles.py` & `artistools-2024.4.23/artistools/inputmodel/energyinputfiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     dE = np.diff(times_and_rate["rate"] * E_tot)
     dt = np.diff(times * 24 * 60 * 60)
 
     intergrated_rate = dE / dt
     scale_factor_energy_diff = max(qdot[1:] / intergrated_rate)
     print(np.mean(scale_factor_energy_diff))
-    E_tot = E_tot * scale_factor_energy_diff
+    E_tot *= scale_factor_energy_diff
     # print(f"E_tot after integrated line scaled to match energy of power law: {E_tot}")
 
     dE = np.diff(times_and_rate["rate"] * E_tot)
     dt = np.diff(times * 24 * 60 * 60)
 
     # check energy rate is on top of power law line
     # plt.plot(times_and_rate["times"][1:], (dE / dt) * 0.01 * MSUN)
@@ -177,29 +177,28 @@
         interpolated_trajectories["mean"] = interpolated_trajectories.iloc[:, 1:].mean(axis=1)
 
         index_time_lessthan = interpolated_trajectories[interpolated_trajectories["time/s"] < 1.1e-1].index
         interpolated_trajectories = interpolated_trajectories.drop(index_time_lessthan)
 
         interpolated_trajectories.to_csv(path_to_rprocess_calculation / "interpolatedQdot.dat", sep=" ", index=False)
     print(f"sum etot {sum(trajectory_E_tot)}")
-    trajectory_energy = {"id": trajectory_ids, "E_tot": trajectory_E_tot}
-    trajectory_energy = pd.DataFrame.from_dict(trajectory_energy)
-    trajectory_energy = trajectory_energy.sort_values(by="id")
+    trajectory_energy = pd.DataFrame.from_dict({"id": trajectory_ids, "E_tot": trajectory_E_tot}).sort_values(by="id")
+
     print(trajectory_energy)
     trajectory_energy.to_csv(path_to_rprocess_calculation / "trajectoryQ.dat", sep=" ", index=False)
 
 
 def make_energydistribution_weightedbyrho(rho, E_tot_per_gram, Mtot_grams):
     print(f"energy distribution weighted by rho (E_tot per gram {E_tot_per_gram})")
     Etot = E_tot_per_gram * Mtot_grams
     print("Etot", Etot)
     numberofcells = len(rho)
 
     cellenergy = np.array([Etot] * numberofcells)
-    cellenergy = cellenergy * (rho / sum(rho))
+    cellenergy *= rho / sum(rho)
 
     energydistdata = {"cellid": np.arange(1, len(rho) + 1), "cell_energy": cellenergy}
 
     print(f"sum energy cells {sum(energydistdata['cell_energy'])} should equal Etot")
     return pd.DataFrame(data=energydistdata)
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/from_alcar.py` & `artistools-2024.4.23/artistools/inputmodel/from_alcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Prepare data for ARTIS KN calculation from end-to-end hydro models. Original script by Oliver Just with modifications by Gerrit Leck for abundance mapping."""
+
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import typing as t
 from pathlib import Path
 
 import argcomplete
 import numpy as np
@@ -161,15 +162,15 @@
     hsmooth = np.zeros(ntraj)
     for i in np.arange(ntraj):
         cont = True
         hl, hr = 0.00001 * cl * tsnap, 1.0 * cl * tsnap
         dist = np.sqrt((rcyltraj[i] - rcyltraj) ** 2 + (zcyltraj[i] - zcyltraj) ** 2)
         ic = 0
         while cont:
-            ic = ic + 1
+            ic += 1
             h1 = 0.5 * (hl + hr)
             wsph = sphkernel(dist, h1, nu)
             rhos = np.sum(wsph * mtraj)
             fun = (mtraj[i] / ((h1 / hsmeta) ** nu) - rhos) / rhos
             if fun > 0.0:
                 hl = h1
             else:
@@ -236,30 +237,29 @@
             for nr in np.arange(nvr):
                 cellid = nz * nvr + nr + 1
                 if dmgrid[nr, nz] > (1e-100 * mtot):
                     # print(
                     # f"{nr} {nz} {temint[nr, nz]} {q_ergperg[nr, nz]} {rhoint[nr, nz]} {dmgrid[nr, nz]} {xint[nr, nz]}"
                     # )
                     wloc = wall[nr, nz, :] * rho2dtraj / rho2dhat
-                    wloc = wloc / np.sum(wloc)
+                    wloc /= np.sum(wloc)
                     pids = np.where(wloc > 1.0e-20)[0]
                     for pid in pids:
                         fgridcontributions.write(
                             f"{pid:<10}  {cellid:<8} {wloc[pid]:25.15e} {wloc[pid]:25.15e}\n",
                         )
 
     return nvr, nvz, rgridc2d, zgridc2d, rhoint, xint, iso, q_ergperg
 
 
 def z_reflect(arr: np.ndarray) -> np.ndarray:
     """Flatten an array and add a reflection in z."""
     ngridrcyl, ngridz = arr.shape
     assert ngridz % 2 == 0
-    arr_ref = np.concatenate([np.flip(arr[:, ngridz // 2 :], axis=1), arr[:, ngridz // 2 :]], axis=1)
-    return arr_ref.flatten(order="F")
+    return np.concatenate([np.flip(arr[:, ngridz // 2 :], axis=1), arr[:, ngridz // 2 :]], axis=1).flatten(order="F")
 
 
 # function added by Luke and Gerrit to create the ARTIS model.txt
 def create_ARTIS_modelfile(
     ngridrcyl, ngridz, pos_t_s_grid_rad, pos_t_s_grid_z, rho_interpol, X_cells, isot_table, q_ergperg, outpath
 ):
     assert pos_t_s_grid_rad.shape == (ngridrcyl, ngridz)
@@ -303,16 +303,15 @@
             dictelabunds[elem_str] = (
                 dictelabunds[elem_str] + flat_isoabund if elem_str in dictelabunds else flat_isoabund
             )
 
     print(f"Number of non-zero nuclides {len(dictabunds)}")
     dfmodel = pd.concat([dfmodel, pd.DataFrame(dictabunds)], axis=1)
 
-    dfabundances = pd.DataFrame(dictelabunds)
-    dfabundances = dfabundances.fillna(0.0)
+    dfabundances = pd.DataFrame(dictelabunds).fillna(0.0)
 
     # create init abundance file
     at.inputmodel.save_initelemabundances(dfelabundances=dfabundances, outpath=outpath)
 
     # create modelmeta dictionary
     modelmeta = {
         "dimensions": 2,
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py` & `artistools-2024.4.23/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """Convert a CMFGEN model file to ARTIS format. Original script possibly by Markus Kromer?."""
+
 # from rd_cmfgen import rd_nuc_decay_data
 from math import exp
 from pathlib import Path
 
 import numpy as np
 
 from artistools.inputmodel.fromcmfgen.rd_cmfgen import rd_sn_hydro_data
@@ -216,17 +217,15 @@
             vel = rout[i] / a["time"] / 3600 / 24 / 1e5  # a['vel'][i]
             rho = np.log10(a["dens"][i])
             igefrac = a["specfrac"][i, ige_index].sum()
             ni56frac = a["isofrac"][i, 96]
             co56frac = a["isofrac"][i, 89]
             cr48frac = a["isofrac"][i, 75]
             v48frac = a["isofrac"][i, 49]
-            strout = "{:4d} {:1.7e} {:1.7e} {:1.7e} {:1.7e} {:1.7e} {:1.7e} {:1.7e}\n".format(
-                i + 1, vel, rho, igefrac, ni56frac, co56frac, cr48frac, v48frac
-            )
+            strout = f"{i + 1:4d} {vel:1.7e} {rho:1.7e} {igefrac:1.7e} {ni56frac:1.7e} {co56frac:1.7e} {cr48frac:1.7e} {v48frac:1.7e}\n"
             f.write(strout)
 
     # Create an array of size n_radial_cells*31 (31=running index + 30 ARTIS species)
     abund = np.zeros((a["nd"], 31))
 
     # Fill the array with availble mass fractions and the running index
     for i in range(a["nspec"] - 1):
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py` & `artistools-2024.4.23/artistools/inputmodel/fromcmfgen/rd_cmfgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ruff: noqa
 """various functions to read/write CMFGEN input/output files:
 
 rd_nuc_decay_data
 rd_sn_hydro_data
 """
+
 import sys
 
 import numpy as np
 
 # constants
 DAY2SEC = 86400.0
 MEV2ERG = 1.60217733e-6
@@ -85,15 +86,15 @@
             thalf[i] = float(linearr[2]) * DAY2SEC  # convert to seconds
             decay_const[i] = np.log(2) / thalf[i]
             isospec_daughter.append(linearr[3])
             amu_daughter[i] = float(linearr[4])
             aiso_daughter[i] = np.rint(amu_daughter[i])
             edec[i] = float(linearr[5]) * MEV2ERG  # convert to ergs
             seqnum.append(linearr[6])
-            if seqnum[-1] in ["F", "E"]:
+            if seqnum[-1] in ("F", "E"):
                 nchains = nchains + 1
             nlines[i] = int(linearr[7])
         if not quiet:
             print("INFO - Read in decay chains")
 
     # output
     out = {}
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/fullymixed.py` & `artistools-2024.4.23/artistools/inputmodel/fullymixed.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/inputmodel_misc.py` & `artistools-2024.4.23/artistools/inputmodel/inputmodel_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,42 +422,41 @@
         "ncoordgrid": ncoordgrid,
         "ncoordgridx": ncoordgrid,
         "ncoordgridy": ncoordgrid,
         "ncoordgridz": ncoordgrid,
         "headercommentlines": [],
     }
 
-    dfmodel = pl.DataFrame(
-        {"modelgridindex": range(ncoordgrid**3), "inputcellid": range(1, 1 + ncoordgrid**3)},
-        schema={"modelgridindex": pl.Int32, "inputcellid": pl.Int32},
-    ).lazy()
-
-    dfmodel = dfmodel.with_columns(
-        [
-            pl.col("modelgridindex").mod(ncoordgrid).alias("n_x"),
-            (pl.col("modelgridindex") // ncoordgrid).mod(ncoordgrid).alias("n_y"),
-            (pl.col("modelgridindex") // (ncoordgrid**2)).mod(ncoordgrid).alias("n_z"),
-        ]
-    )
-
-    dfmodel = dfmodel.with_columns(
-        [
-            (-xmax + 2 * pl.col("n_x") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_x_min"),
-            (-xmax + 2 * pl.col("n_y") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_y_min"),
-            (-xmax + 2 * pl.col("n_z") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_z_min"),
-        ]
+    dfmodel = (
+        pl.DataFrame(
+            {"modelgridindex": range(ncoordgrid**3), "inputcellid": range(1, 1 + ncoordgrid**3)},
+            schema={"modelgridindex": pl.Int32, "inputcellid": pl.Int32},
+        )
+        .lazy()
+        .with_columns(
+            [
+                pl.col("modelgridindex").mod(ncoordgrid).alias("n_x"),
+                (pl.col("modelgridindex") // ncoordgrid).mod(ncoordgrid).alias("n_y"),
+                (pl.col("modelgridindex") // (ncoordgrid**2)).mod(ncoordgrid).alias("n_z"),
+            ]
+        )
+        .with_columns(
+            [
+                (-xmax + 2 * pl.col("n_x") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_x_min"),
+                (-xmax + 2 * pl.col("n_y") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_y_min"),
+                (-xmax + 2 * pl.col("n_z") * xmax / ncoordgrid).cast(pl.Float32).alias("pos_z_min"),
+            ]
+        )
     )
 
     standardcols = get_standard_columns(3, includenico57=includenico57)
 
     dfmodel = dfmodel.with_columns(
         [pl.lit(0.0, dtype=pl.Float32).alias(colname) for colname in standardcols if colname not in dfmodel.columns]
-    )
-
-    dfmodel = dfmodel.select([*standardcols, "modelgridindex"])
+    ).select([*standardcols, "modelgridindex"])
 
     return dfmodel, modelmeta
 
 
 def get_modeldata(
     modelpath: Path | str = Path(),
     get_elemabundances: bool = False,
@@ -495,163 +494,117 @@
     keep_all = "ALL" in derived_cols
 
     dimensions = modelmeta["dimensions"]
     match dimensions:
         case 1:
             axes = ["r"]
 
-            dfmodel = dfmodel.with_columns(pl.col("vel_r_max_kmps").shift(n=1, fill_value=0.0).alias("vel_r_min_kmps"))
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (pl.col("vel_r_min_kmps") * 1e5).alias("vel_r_min"),
-                    (pl.col("vel_r_max_kmps") * 1e5).alias("vel_r_max"),
-                ]
-            )
-
-            dfmodel = dfmodel.with_columns(((pl.col("vel_r_max") + pl.col("vel_r_min")) / 2).alias("vel_r_mid"))
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (
+            dfmodel = (
+                dfmodel.with_columns(vel_r_min_kmps=pl.col("vel_r_max_kmps").shift(n=1, fill_value=0.0))
+                .with_columns(
+                    vel_r_min=(pl.col("vel_r_min_kmps") * 1e5),
+                    vel_r_max=(pl.col("vel_r_max_kmps") * 1e5),
+                )
+                .with_columns(vel_r_mid=((pl.col("vel_r_max") + pl.col("vel_r_min")) / 2))
+                .with_columns(
+                    volume=(
                         (4.0 / 3.0)
                         * math.pi
                         * (
                             pl.col("vel_r_max_kmps").cast(pl.Float64).pow(3)
                             - pl.col("vel_r_min_kmps").cast(pl.Float64).pow(3)
                         )
                         * pl.lit(1e5 * t_model_init_seconds).pow(3)
-                    ).alias("volume")
-                ]
+                    )
+                )
             )
 
         case 2:
             axes = ["rcyl", "z"]
 
             assert t_model_init_seconds is not None
             # pos_mid is defined in the input file
             # TODO: get wid_init from modelmeta
             dfmodel = dfmodel.with_columns(
                 [(pl.col(f"pos_{ax}_mid") - modelmeta[f"wid_init_{ax}"] / 2.0).alias(f"pos_{ax}_min") for ax in axes]
-            )
-
-            dfmodel = dfmodel.with_columns(
+            ).with_columns(
                 [(pl.col(f"pos_{ax}_mid") + modelmeta[f"wid_init_{ax}"] / 2.0).alias(f"pos_{ax}_max") for ax in axes]
             )
 
             # add a 3D radius column
             axes.append("r")
             dfmodel = dfmodel.with_columns(
-                [
-                    (
-                        pl.col("pos_rcyl_min").pow(2)
-                        + pl.min_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
-                    )
-                    .sqrt()
-                    .alias("pos_r_min")
-                ]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [(pl.col("pos_rcyl_mid").pow(2) + pl.col("pos_z_mid").pow(2)).sqrt().alias("pos_r_mid")]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (
-                        pl.col("pos_rcyl_max").pow(2)
-                        + pl.max_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
-                    )
-                    .sqrt()
-                    .alias("pos_r_max"),
-                ]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (
-                        math.pi
-                        * (
-                            pl.col("pos_rcyl_max").cast(pl.Float64).pow(2)
-                            - pl.col("pos_rcyl_min").cast(pl.Float64).pow(2)
-                        )
-                        * modelmeta["wid_init_z"]
-                    ).alias("volume")
-                ]
+                pos_r_min=(
+                    pl.col("pos_rcyl_min").pow(2)
+                    + pl.min_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
+                ).sqrt(),
+                pos_r_mid=(pl.col("pos_rcyl_mid").pow(2) + pl.col("pos_z_mid").pow(2)).sqrt(),
+                pos_r_max=(
+                    pl.col("pos_rcyl_max").pow(2)
+                    + pl.max_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
+                ).sqrt(),
+                volume=(
+                    math.pi
+                    * (pl.col("pos_rcyl_max").cast(pl.Float64).pow(2) - pl.col("pos_rcyl_min").cast(pl.Float64).pow(2))
+                    * modelmeta["wid_init_z"]
+                ),
             )
 
         case 3:
             axes = ["x", "y", "z"]
             for ax in axes:
                 if f"wid_init_{ax}" not in modelmeta:
                     modelmeta[f"wid_init_{ax}"] = modelmeta["wid_init"]
 
-            dfmodel = dfmodel.with_columns(
-                [pl.lit(modelmeta["wid_init_x"] * modelmeta["wid_init_y"] * modelmeta["wid_init_z"]).alias("volume")]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [(pl.col(f"pos_{ax}_min") + 0.5 * modelmeta[f"wid_init_{ax}"]).alias(f"pos_{ax}_mid") for ax in axes]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [(pl.col(f"pos_{ax}_min") + modelmeta[f"wid_init_{ax}"]).alias(f"pos_{ax}_max") for ax in axes]
+            dfmodel = (
+                dfmodel.with_columns(
+                    volume=pl.lit(modelmeta["wid_init_x"] * modelmeta["wid_init_y"] * modelmeta["wid_init_z"])
+                )
+                .with_columns(
+                    [
+                        (pl.col(f"pos_{ax}_min") + 0.5 * modelmeta[f"wid_init_{ax}"]).alias(f"pos_{ax}_mid")
+                        for ax in axes
+                    ]
+                )
+                .with_columns(
+                    [(pl.col(f"pos_{ax}_min") + modelmeta[f"wid_init_{ax}"]).alias(f"pos_{ax}_max") for ax in axes]
+                )
             )
 
             # add a 3D radius column
             axes.append("r")
 
             # xyz positions can be negative, so the min xyz side of the cube can have a larger radius than the max side
             dfmodel = dfmodel.with_columns(
-                [
-                    (
-                        pl.min_horizontal(pl.col("pos_x_min").abs(), pl.col("pos_x_max").abs()).pow(2)
-                        + pl.min_horizontal(pl.col("pos_y_min").abs(), pl.col("pos_y_max").abs()).pow(2)
-                        + pl.min_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
-                    )
-                    .sqrt()
-                    .alias("pos_r_min")
-                ]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (pl.col("pos_x_mid").pow(2) + pl.col("pos_y_mid").pow(2) + pl.col("pos_z_mid").pow(2))
-                    .sqrt()
-                    .alias("pos_r_mid")
-                ]
-            )
-
-            dfmodel = dfmodel.with_columns(
-                [
-                    (
-                        pl.max_horizontal(pl.col("pos_x_min").abs(), pl.col("pos_x_max").abs()).pow(2)
-                        + pl.max_horizontal(pl.col("pos_y_min").abs(), pl.col("pos_y_max").abs()).pow(2)
-                        + pl.max_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
-                    )
-                    .sqrt()
-                    .alias("pos_r_max")
-                ]
+                pos_r_min=(
+                    pl.min_horizontal(pl.col("pos_x_min").abs(), pl.col("pos_x_max").abs()).pow(2)
+                    + pl.min_horizontal(pl.col("pos_y_min").abs(), pl.col("pos_y_max").abs()).pow(2)
+                    + pl.min_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
+                ).sqrt(),
+                pos_r_mid=(pl.col("pos_x_mid").pow(2) + pl.col("pos_y_mid").pow(2) + pl.col("pos_z_mid").pow(2)).sqrt(),
+                pos_r_max=(
+                    pl.max_horizontal(pl.col("pos_x_min").abs(), pl.col("pos_x_max").abs()).pow(2)
+                    + pl.max_horizontal(pl.col("pos_y_min").abs(), pl.col("pos_y_max").abs()).pow(2)
+                    + pl.max_horizontal(pl.col("pos_z_min").abs(), pl.col("pos_z_max").abs()).pow(2)
+                ).sqrt(),
             )
 
     for col in dfmodel.columns:
         if col.startswith("pos_"):
             dfmodel = dfmodel.with_columns((pl.col(col) / t_model_init_seconds).alias(col.replace("pos_", "vel_")))
 
     if "logrho" not in dfmodel.columns:
-        dfmodel = dfmodel.with_columns(pl.col("rho").log10().alias("logrho"))
+        dfmodel = dfmodel.with_columns(logrho=pl.col("rho").log10())
 
     if "rho" not in dfmodel.columns:
         dfmodel = dfmodel.with_columns(
-            (pl.when(pl.col("logrho") > -98).then(10 ** pl.col("logrho")).otherwise(0.0)).alias("rho")
+            rho=(pl.when(pl.col("logrho") > -98).then(10 ** pl.col("logrho")).otherwise(0.0))
         )
 
-    dfmodel = dfmodel.with_columns([(pl.col("rho") * pl.col("volume")).alias("mass_g")])
-
-    dfmodel = dfmodel.with_columns(
+    dfmodel = dfmodel.with_columns(mass_g=(pl.col("rho") * pl.col("volume"))).with_columns(
         [(pl.col(colname) / 29979245800.0).alias(f"{colname}_on_c") for colname in dfmodel.columns]
     )
 
     if unknown_cols := [
         col
         for col in derived_cols
         if col not in dfmodel.columns and col not in {"pos_min", "pos_max", "ALL", "velocity"}
@@ -951,16 +904,14 @@
 def get_mgi_of_velocity_kms(modelpath: Path, velocity: float, mgilist: t.Sequence[int] | None = None) -> int | float:
     """Return the modelgridindex of the cell whose outer velocity is closest to velocity.
 
     If mgilist is given, then chose from these cells only.
     """
     modeldata, _, _ = get_modeldata_tuple(modelpath)
 
-    velocity = float(velocity)
-
     if not mgilist:
         mgilist = list(modeldata.index)
         arr_vouter = modeldata["vel_r_max_kmps"].to_numpy()
     else:
         arr_vouter = np.array([modeldata["vel_r_max_kmps"][mgi] for mgi in mgilist])
 
     index_closestvouter = int(np.abs(arr_vouter - velocity).argmin())
@@ -1063,17 +1014,15 @@
         abundancefilename = Path(outpath) / "abundances.txt"
     else:
         abundancefilename = Path(outpath)
 
     if isinstance(dfelabundances, pd.DataFrame):
         dfelabundances = pl.from_pandas(dfelabundances)
 
-    dfelabundances = dfelabundances.clone().lazy().collect()
-
-    dfelabundances = dfelabundances.with_columns([pl.col("inputcellid").cast(pl.Int32)])
+    dfelabundances = dfelabundances.clone().lazy().collect().with_columns([pl.col("inputcellid").cast(pl.Int32)])
 
     atomic_numbers = {
         at.get_atomic_number(colname[2:]) for colname in dfelabundances.select(pl.selectors.starts_with("X_")).columns
     }
     max_atomic_number = max([30, *atomic_numbers])
     elcolnames = [f"X_{at.get_elsymbol(Z)}" for Z in range(1, 1 + max_atomic_number)]
     for colname in elcolnames:
@@ -1142,15 +1091,15 @@
         ncoordgridz = 0
 
     dfmodel = dfmodel.lazy().collect()
 
     if modelmeta is None:
         modelmeta = {}
 
-    modelmeta_out = {k: v for k, v in modelmeta.items() if not k.startswith("ncoord") and not k.startswith("wid_init")}
+    modelmeta_out = {k: v for k, v in modelmeta.items() if not k.startswith(("ncoord", "wid_init"))}
 
     assert all(
         key not in modelmeta_out or modelmeta_out[key] == kwargs[key] for key in kwargs
     )  # can't define the same thing twice unless the values are the same
 
     modelmeta_out |= kwargs  # add any extra keyword arguments to modelmeta
 
@@ -1363,15 +1312,15 @@
             dfmodel["rho"] *= timefactor**-3
         elif col == "logrho":
             dfmodel["logrho"] += math.log10(timefactor**-3)
 
     if modelmeta is not None:
         modelmeta["t_model_days"] = targetmodeltime_days
         modelmeta.get("headercommentlines", []).append(
-            "scaled from {t_model_days} to {targetmodeltime_days} (no abund change from decays)"
+            f"scaled from {t_model_days} to {targetmodeltime_days} (no abund change from decays)"
         )
 
     return dfmodel, modelmeta
 
 
 def savetologfile(outputfolderpath, logfilename="modellog.txt"):
     # save the printed output to a log file
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/makeartismodel.py` & `artistools-2024.4.23/artistools/inputmodel/makeartismodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/map_1d_to_3d_grid.py` & `artistools-2024.4.23/artistools/inputmodel/map_1d_to_3d_grid.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/maptogrid.py` & `artistools-2024.4.23/artistools/inputmodel/maptogrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,36 +167,35 @@
     assert len(dfsnapshot.columns) == len(snapshot_columns_used)
 
     npart = len(dfsnapshot)
 
     # Propagate particles to dtextra using velocities
     logprint(f"Propagating particles for dtextra_seconds={dtextra_seconds}")
     dtextra = dtextra_seconds / 4.926e-6  # convert to geom units.
-    dfsnapshot = dfsnapshot.with_columns(dis_orig=(pl.col("x") ** 2 + pl.col("y") ** 2 + pl.col("z") ** 2).sqrt())
-
-    dfsnapshot = dfsnapshot.with_columns(
-        x_orig=pl.col("x"),
-        y_orig=pl.col("y"),
-        z_orig=pl.col("z"),
-        x=pl.col("x") + pl.col("vx") * dtextra,
-        y=pl.col("y") + pl.col("vy") * dtextra,
-        z=pl.col("z") + pl.col("vz") * dtextra,
-    )
-
-    dfsnapshot = dfsnapshot.with_columns(dis=(pl.col("x") ** 2 + pl.col("y") ** 2 + pl.col("z") ** 2).sqrt())
-
-    dfsnapshot = dfsnapshot.with_columns(
-        h=pl.col("h") / pl.col("dis_orig") * pl.col("dis"),
-        vrad=(pl.col("vx") * pl.col("x") + pl.col("vy") * pl.col("y") + pl.col("vz") * pl.col("z")) / pl.col("dis"),
-        vtot=(pl.col("vx") ** 2 + pl.col("vy") ** 2 + pl.col("vz") ** 2).sqrt(),
-    )
-    dfsnapshot = dfsnapshot.with_columns(
-        vperp=pl.when(pl.col("vtot") > pl.col("vrad"))
-        .then((pl.col("vtot") ** 2 - pl.col("vrad") ** 2).sqrt())
-        .otherwise(0.0),
+    dfsnapshot = (
+        dfsnapshot.with_columns(
+            dis_orig=(pl.col("x") ** 2 + pl.col("y") ** 2 + pl.col("z") ** 2).sqrt(),
+            x_orig=pl.col("x"),
+            y_orig=pl.col("y"),
+            z_orig=pl.col("z"),
+            x=pl.col("x") + pl.col("vx") * dtextra,
+            y=pl.col("y") + pl.col("vy") * dtextra,
+            z=pl.col("z") + pl.col("vz") * dtextra,
+        )
+        .with_columns(dis=(pl.col("x") ** 2 + pl.col("y") ** 2 + pl.col("z") ** 2).sqrt())
+        .with_columns(
+            h=pl.col("h") / pl.col("dis_orig") * pl.col("dis"),
+            vrad=(pl.col("vx") * pl.col("x") + pl.col("vy") * pl.col("y") + pl.col("vz") * pl.col("z")) / pl.col("dis"),
+            vtot=(pl.col("vx") ** 2 + pl.col("vy") ** 2 + pl.col("vz") ** 2).sqrt(),
+        )
+        .with_columns(
+            vperp=pl.when(pl.col("vtot") > pl.col("vrad"))
+            .then((pl.col("vtot") ** 2 - pl.col("vrad") ** 2).sqrt())
+            .otherwise(0.0),
+        )
     )
 
     particleid = dfsnapshot["id"].to_numpy()
     x = dfsnapshot["x"].to_numpy()
     y = dfsnapshot["y"].to_numpy()
     z = dfsnapshot["z"].to_numpy()
     h = dfsnapshot["h"].to_numpy().copy()
@@ -206,18 +205,18 @@
     Ye = dfsnapshot["ye"].to_numpy()
 
     totmass = dfsnapshot["pmass"].sum()
     rmean = dfsnapshot["dis"].mean()
     hmean = dfsnapshot["h"].mean()
     rmax = dfsnapshot["dis"].max()
     with Path(outputfolderpath, "ejectapartanalysis.dat").open(mode="w", encoding="utf-8") as fpartanalysis:
-        for part in dfsnapshot.select(["dis", "h", "vrad", "vperp", "vtot"]).iter_rows(named=True):
-            fpartanalysis.write(
-                f"{part['dis']} {part['h']} {part['h'] / part['dis']} {part['vrad']} {part['vperp']} {part['vtot']}\n"
-            )
+        fpartanalysis.writelines(
+            f'{part["dis"]} {part["h"]} {part["h"] / part["dis"]} {part["vrad"]} {part["vperp"]} {part["vtot"]}\n'
+            for part in dfsnapshot.select(["dis", "h", "vrad", "vperp", "vtot"]).iter_rows(named=True)
+        )
 
     logprint(f"saved {outputfolderpath / 'ejectapartanalysis.dat'}")
 
     logprint(f"total mass of sph particle {totmass} max dist {rmax} mean dist {rmean}")
     logprint(f"smoothing length min {dfsnapshot['h'].min()} mean {hmean}")
     logprint("ratio between vrad and vperp mean", dfsnapshot.select(pl.col("vperp") - pl.col("vrad")).mean().item(0, 0))
 
@@ -371,22 +370,22 @@
         gx = x0 + dx * i
         for j in range(ncoordgrid):
             gy = y0 + dy * j
             for k in range(1, ncoordgrid):
                 # how many cells with rho=0?
 
                 if grho[i, j, k] < 1.0e-20:
-                    nzero = nzero + 1
+                    nzero += 1
 
                 gz = z0 + dz * k
 
                 dis = math.sqrt(gx * gx + gy * gy + gz * gz)
 
                 if grho[i, j, k] < 1.0e-20 and dis < rmean:
-                    nzerocentral = nzerocentral + 1
+                    nzerocentral += 1
 
     logprint(f"fraction of total mass on grid {gmass / totmass}")
 
     logprint(
         f"{'WARNING!' if gmass / totmass < 0.9 else ''} mass on grid from rho*V: {gmass} mass of particles: {totmass} "
     )
 
@@ -416,15 +415,15 @@
                 gy = y0 + dy * j
                 for i in range(ncoordgrid):
                     fgrid.write(
                         f"{gridindex:8d} {x0 + dx * i} {gy} {gz} {grho[i, j, k]} {gye[i, j, k]} {gparticlecounter[i, j, k]}\n"
                     )
                     # gridindex2 = ((k - 1) * ncoordgrid + (j - 1)) * ncoordgrid + (i - 1) + 1
 
-                    gridindex = gridindex + 1
+                    gridindex += 1
 
     logprint(f"saved {outputfolderpath / 'grid.dat'}")
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-inputpath", "-i", default=".", help="Path to ejectasnapshot")
     parser.add_argument(
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/modelfromhydro.py` & `artistools-2024.4.23/artistools/inputmodel/modelfromhydro.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,15 @@
     pathtogriddata: str | Path, targetmodeltime_days: None | float = None
 ) -> tuple[pd.DataFrame, float, float, float, dict[str, t.Any]]:
     griddatfilepath = Path(pathtogriddata) / "grid.dat"
 
     # Get simulation time for ejecta snapshot
     simulation_end_time_geomunits, mergertime_geomunits = get_snapshot_time_geomunits(pathtogriddata)
 
-    griddata = pd.read_csv(griddatfilepath, sep=r"\s+", comment="#", skiprows=3, dtype_backend="pyarrow")
-    griddata = griddata.rename(
+    griddata = pd.read_csv(griddatfilepath, sep=r"\s+", comment="#", skiprows=3, dtype_backend="pyarrow").rename(
         columns={
             "gridindex": "inputcellid",
             "pos_x": "pos_x_min",
             "pos_y": "pos_y_min",
             "pos_z": "pos_z_min",
             "posx": "pos_x_min",  # for compatibility with fortran maptogrid script
             "posy": "pos_y_min",
@@ -142,15 +141,15 @@
 
     factor_position = 1.478  # in km
     km_to_cm = 1e5
     griddata["pos_x_min"] = griddata["pos_x_min"] * factor_position * km_to_cm
     griddata["pos_y_min"] = griddata["pos_y_min"] * factor_position * km_to_cm
     griddata["pos_z_min"] = griddata["pos_z_min"] * factor_position * km_to_cm
 
-    griddata["rho"] = griddata["rho"] * 6.176e17  # convert to g/cm3
+    griddata["rho"] *= 6.176e17  # convert to g/cm3
 
     with griddatfilepath.open(encoding="utf-8") as gridfile:
         ngrid = int(gridfile.readline().split()[0])
         if ngrid != len(griddata["inputcellid"]):
             print("length of file and ngrid don't match")
             sys.exit(1)
         extratime_geomunits = float(gridfile.readline().split()[0])
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/opacityinputfile.py` & `artistools-2024.4.23/artistools/inputmodel/opacityinputfile.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/plotdensity.py` & `artistools-2024.4.23/artistools/inputmodel/plotdensity.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     axes[-1].set_xlim(left=0.0)
     axes[0].set_ylim(bottom=0.0)
     axes[1].set_ylim(bottom=0.0)
 
     outfilepath = Path(args.outputpath)
     if outfilepath.is_dir():
-        outfilepath = outfilepath / "densityprofile.pdf"
+        outfilepath /= "densityprofile.pdf"
 
     plt.savefig(outfilepath)
     print(f"Saved {outfilepath}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/plotinitialcomposition.py` & `artistools-2024.4.23/artistools/inputmodel/plotinitialcomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 
 
 import argparse
 import math
+import string
 import typing as t
 from pathlib import Path
 
 import argcomplete
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
@@ -119,15 +120,15 @@
         )
 
     return im, scaledmap
 
 
 def plot_2d_initial_abundances(modelpath, args=None) -> None:
     # if the species ends in a number then we need to also get the nuclear mass fractions (not just element abundances)
-    get_elemabundances = any(plotvar[-1] not in "0123456789" for plotvar in args.plotvars)
+    get_elemabundances = any(plotvar[-1] not in string.digits for plotvar in args.plotvars)
     dfmodel, modelmeta = at.get_modeldata(
         modelpath,
         get_elemabundances=get_elemabundances,
         derived_cols=["pos_min", "pos_max"],
     )
     assert modelmeta["dimensions"] > 1
 
@@ -185,16 +186,16 @@
     for plotvar, ax in zip(args.plotvars, axes):
         colname = plotvar if plotvar in df2dslice.columns else f"X_{plotvar}"
 
         im, scaledmap = plot_slice_modelcolumn(
             ax, df2dslice, modelmeta, colname, plotaxis1, plotaxis2, modelmeta["t_model_init_days"], args
         )
 
-    xlabel = r"v$_{" + f"{plotaxis1}" + r"}$ [$c$]"
-    ylabel = r"v$_{" + f"{plotaxis2}" + r"}$ [$c$]"
+    xlabel = r"v$_{" + str(plotaxis1) + r"}$ [$c$]"
+    ylabel = r"v$_{" + str(plotaxis2) + r"}$ [$c$]"
 
     cbar = fig.colorbar(im, cax=axcbar, location="top", use_gridspec=True)
     axes[0].set_xlabel(xlabel)
     axes[0].set_ylabel(ylabel)
 
     if "cellYe" not in args.plotvars and "tracercount" not in args.plotvars:
         cbar.set_label(r"log10($\rho$ [g/cm3])" if args.logcolorscale else r"$\rho$ [g/cm3]")
@@ -291,15 +292,15 @@
 
     # generate grid from data
     grid = round(len(model["rho"]) ** (1.0 / 3.0))
     surfacecolorscale = np.zeros((grid, grid, grid))  # needs 3D array
     xgrid = np.zeros(grid)
 
     surfacearr = np.array(model[coloursurfaceby])
-    vmax = vmax / 2.99792458e10
+    vmax /= 29979245800.0
     i = 0
     for z in range(grid):
         for y in range(grid):
             for x in range(grid):
                 surfacecolorscale[x, y, z] = surfacearr[i]
                 xgrid[x] = -vmax + 2 * x * vmax / grid
                 i += 1
@@ -410,15 +411,15 @@
     z = heatmap
     phis = yedges
 
     cmap = "coolwarm_r" if weightby == "Ye" else "coolwarm"
     im = ax.pcolormesh(phis, radii, z, cmap=cmap)
     cbar = fig.colorbar(im)
 
-    cbar.set_label(f"{weightby}", rotation=90)
+    cbar.set_label(weightby, rotation=90)
     plt.xlabel(r"azimuthal angle")
     plt.ylabel("Radial velocity [c]")
     ax.yaxis.set_label_coords(-0.15, 0.5)
 
     outfilename = f"model{weightby}phi.pdf"
     plt.savefig(Path(modelpath) / outfilename, format="pdf")
     print(f"Saved {outfilename}")
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/recombinationenergy.py` & `artistools-2024.4.23/artistools/inputmodel/recombinationenergy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 import argparse
+import string
 import typing as t
 from pathlib import Path
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -38,15 +39,15 @@
             speciesabund_g = np.dot(dfmodel[column], dfmodel["mass_g"])
 
             species_mass_msun = speciesabund_g / msun_g
 
             if species[-1].isdigit():  # isotopic species
                 atomic_number = at.get_atomic_number(species)
                 elsymb = at.get_elsymbol(atomic_number)
-                massnumber = int(species.lstrip("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"))
+                massnumber = int(species.lstrip(string.ascii_letters))
                 matchrows = dfbinding.query("Z == @atomic_number")
 
                 binding_en_ev = 0.0 if matchrows.empty else matchrows.iloc[0]["TotBEn"]
 
                 # print(species, atomic_number, massnumber, el_binding_en_ev)
                 contrib_binding_en_ev = speciesabund_g / (massnumber * amu_g) * binding_en_ev
 
@@ -108,18 +109,18 @@
         dfthermo = dfthermo.query("time_s >= @tmin_s")
         dfthermo = dfthermo.query("time_s <= @time_s_end")
         return np.trapz(y=dfthermo["Qdot"], x=dfthermo["time_s"]) * erg_to_ev
         # print(dfthermo)
 
 
 def get_particles_recomb_nuc_energy(traj_root, dfbinding):
+    # sourcery skip: use-contextlib-suppress
     dfsnapshot = at.inputmodel.modelfromhydro.read_ejectasnapshot(
         "/Users/luke/Library/Mobile Documents/com~apple~CloudDocs/Archive/Astronomy/Mergers/SFHo_snapshot"
-    )
-    dfsnapshot = dfsnapshot.sort_values("ye")
+    ).sort_values("ye")
 
     dictbinding = dict(dfbinding[["Z", "TotBEn"]].itertuples(index=False))
 
     tmin_s = 10
     time_s = 6 * 3600
 
     ye_list = []
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/rprocess_from_trajectory.py` & `artistools-2024.4.23/artistools/inputmodel/rprocess_from_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import gc
 import io
 import math
 import multiprocessing
+import string
 import tarfile
 import time
 import typing as t
 from functools import lru_cache
 from functools import partial
+from itertools import chain
 from pathlib import Path
 
 import argcomplete
 import numpy as np
 import pandas as pd
 import polars as pl
 
@@ -35,15 +37,15 @@
     elemisotopes: dict[int, list[str]] = {}
     nuclidesincluded = 0
 
     for colname in sorted(dfnucabundances.columns):
         if not colname.startswith("X_"):
             continue
         nuclidesincluded += 1
-        atomic_number = at.get_atomic_number(colname[2:].rstrip("0123456789"))
+        atomic_number = at.get_atomic_number(colname[2:].rstrip(string.digits))
         if atomic_number in elemisotopes:
             elemisotopes[atomic_number].append(colname)
         else:
             elemisotopes[atomic_number] = [colname]
 
     elementsincluded = len(elemisotopes)
 
@@ -58,19 +60,19 @@
                 )
                 for atomic_number in range(1, max(elemisotopes.keys()) + 1)
             },
         },
     )
 
     # ensure cells with no traj contributions are included
-    dfelabundances = pl.DataFrame(pl.Series(name="inputcellid", values=dfmodel["inputcellid"], dtype=pl.Int32))
-
-    dfelabundances = dfelabundances.join(
-        dfelabundances_partial, how="left", left_on="inputcellid", right_on="inputcellid"
-    ).fill_null(0.0)
+    dfelabundances = (
+        pl.DataFrame(pl.Series(name="inputcellid", values=dfmodel["inputcellid"], dtype=pl.Int32))
+        .join(dfelabundances_partial, how="left", left_on="inputcellid", right_on="inputcellid")
+        .fill_null(0.0)
+    )
 
     print(f" took {time.perf_counter() - timestart:.1f} seconds")
     print(f" there are {nuclidesincluded} nuclides from {elementsincluded} elements included")
 
     return dfelabundances
 
 
@@ -80,20 +82,20 @@
     which are much faster to access.
 
     memberfilename: file path within the trajectory tarfile, eg. ./Run_rprocess/evol.dat
     """
     path_extracted_file = Path(traj_root, str(particleid), memberfilename)
     tarfilepaths = [
         Path(traj_root, filename)
-        for filename in [
+        for filename in (
             f"{particleid}.tar",
             f"{particleid:05d}.tar",
             f"{particleid}.tar.xz",
             f"{particleid:05d}.tar.xz",
-        ]
+        )
     ]
     tarfilepath = next((tarfilepath for tarfilepath in tarfilepaths if tarfilepath.is_file()), None)
 
     # and memberfilename.endswith(".dat")
     if not path_extracted_file.is_file() and tarfilepath is not None:
         try:
             tarfile.open(tarfilepath, "r:*").extract(path=Path(traj_root, str(particleid)), member=memberfilename)
@@ -309,20 +311,20 @@
         },
     )
 
 
 def particlenetworkdatafound(traj_root: Path, particleid: int) -> bool:
     tarfilepaths = [
         Path(traj_root, filename)
-        for filename in [
+        for filename in (
             f"{particleid}.tar",
             f"{particleid:05d}.tar",
             f"{particleid}.tar.xz",
             f"{particleid:05d}.tar.xz",
-        ]
+        )
     ]
     return any(tarfilepath.is_file() for tarfilepath in tarfilepaths)
 
 
 def filtermissinggridparticlecontributions(traj_root: Path, dfcontribs: pl.DataFrame) -> pl.DataFrame:
     missing_particleids = [
         particleid
@@ -332,20 +334,18 @@
     print(
         f"Adding gridcontributions column that excludes {len(missing_particleids)} "
         "particles without abundance data and renormalising...",
         end="",
     )
     # after filtering, frac_of_cellmass_includemissing will still include particles with rho but no abundance data
     # frac_of_cellmass will exclude particles with no abundances
-    dfcontribs = dfcontribs.with_columns(pl.col("frac_of_cellmass").alias("frac_of_cellmass_includemissing"))
-    dfcontribs = dfcontribs.with_columns(
-        pl.when(pl.col("particleid").is_in(missing_particleids))
+    dfcontribs = dfcontribs.with_columns(frac_of_cellmass_includemissing=pl.col("frac_of_cellmass")).with_columns(
+        frac_of_cellmass=pl.when(pl.col("particleid").is_in(missing_particleids))
         .then(0.0)
         .otherwise(pl.col("frac_of_cellmass"))
-        .alias("frac_of_cellmass")
     )
 
     cell_frac_sum: dict[int, float] = {}
     cell_frac_includemissing_sum: dict[int, float] = {}
     for (cellindex,), dfparticlecontribs in dfcontribs.group_by(["cellindex"]):  # type: ignore[misc]
         assert isinstance(cellindex, int)
         cell_frac_sum[cellindex] = dfparticlecontribs["frac_of_cellmass"].sum()
@@ -389,15 +389,15 @@
 
     return dfcontribs
 
 
 def save_gridparticlecontributions(dfcontribs: pd.DataFrame | pl.DataFrame, gridcontribpath: Path | str) -> None:
     gridcontribpath = Path(gridcontribpath)
     if gridcontribpath.is_dir():
-        gridcontribpath = gridcontribpath / "gridcontributions.txt"
+        gridcontribpath /= "gridcontributions.txt"
     if gridcontribpath.is_file():
         oldfile = gridcontribpath.rename(gridcontribpath.with_suffix(".bak"))
         print(f"{gridcontribpath} already exists. Renaming existing file to {oldfile}")
 
     if isinstance(dfcontribs, pl.DataFrame):
         dfcontribs = dfcontribs.to_pandas(use_pyarrow_extension_array=True)
 
@@ -430,27 +430,28 @@
     )
 
     print("Reading trajectory abundances...")
     timestart = time.perf_counter()
     trajworker = partial(get_trajectory_abund_q, t_model_s=t_model_s, traj_root=traj_root, getqdotintegral=True)
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
             list_traj_nuc_abund = pool.map(trajworker, particleids)
             pool.close()
             pool.join()
+            pool.terminate()
     else:
         list_traj_nuc_abund = [trajworker(particleid) for particleid in particleids]
 
     n_missing_particles = len([d for d in list_traj_nuc_abund if not d])
     print(f"  {n_missing_particles} particles are missing network abundance data out of {len(particleids)}")
 
     assert len(particleids) > n_missing_particles
 
-    allkeys = list({k for abund in list_traj_nuc_abund for k in abund})
+    allkeys = list(set(chain.from_iterable(list_traj_nuc_abund)))
 
     dfnucabundances = pl.DataFrame(
         {
             f"particle_{particleid}": [traj_nuc_abund.get(k, 0.0) for k in allkeys]
             for particleid, traj_nuc_abund in zip(particleids, list_traj_nuc_abund)
         }
     ).with_columns(pl.all().cast(pl.Float64))
@@ -468,22 +469,20 @@
             pl.sum_horizontal(
                 [
                     pl.col(f"particle_{particleid}") * pl.lit(frac_of_cellmass)
                     for particleid, frac_of_cellmass in dfthiscellcontribs[
                         ["particleid", "frac_of_cellmass"]
                     ].iter_rows()
                 ]
-            ).alias(f"{cellindex}")
+            ).alias(str(cellindex))
             for (cellindex,), dfthiscellcontribs in dfcontribs.group_by(["cellindex"])
         ]
     )
 
-    colnames = [
-        key if isinstance(key, str) else f"X_{at.get_elsymbol(int(key[0]))}{int(key[0] + key[1])}" for key in allkeys
-    ]
+    colnames = [key if isinstance(key, str) else f"X_{at.get_elsymbol(key[0])}{key[0] + key[1]}" for key in allkeys]
 
     dfnucabundances = (
         dfnucabundanceslz.drop([col for col in dfnucabundances.columns if col.startswith("particle_")])
         .collect()
         .transpose(include_header=True, column_names=colnames, header_name="inputcellid")
         .with_columns(pl.col("inputcellid").cast(pl.Int32))
     )
@@ -539,15 +538,15 @@
         dfdensities = pd.DataFrame({"rho": rho, "vel_r_max_kmps": 6.0e4}, index=[0])
 
     # print(dfdensities)
 
     # write abundances.txt
     dictelemabund = get_elemabund_from_nucabund(dfnucabund)
 
-    dfelabundances = pd.DataFrame([dict(inputcellid=mgi + 1, **dictelemabund) for mgi in range(len(dfdensities))])
+    dfelabundances = pd.DataFrame([dictelemabund | {"inputcellid": mgi + 1} for mgi in range(len(dfdensities))])
     # print(dfelabundances)
     at.inputmodel.save_initelemabundances(dfelabundances=dfelabundances, outpath=args.outputpath)
 
     # write model.txt
 
     rowdict = {
         # 'inputcellid': 1,
@@ -563,20 +562,20 @@
     }
 
     for _, row in dfnucabund.query("radioactive == True").iterrows():
         A = row.N + row.Z
         rowdict[f"X_{at.get_elsymbol(row.Z)}{A}"] = row.massfrac
 
     modeldata = [
-        dict(
-            inputcellid=mgi + 1,
-            vel_r_max_kmps=densityrow["vel_r_max_kmps"],
-            logrho=math.log10(densityrow["rho"]),
-            **rowdict,
-        )
+        {
+            "inputcellid": mgi + 1,
+            "vel_r_max_kmps": densityrow["vel_r_max_kmps"],
+            "logrho": math.log10(densityrow["rho"]),
+        }
+        | rowdict
         for mgi, densityrow in dfdensities.iterrows()
     ]
     # print(modeldata)
 
     dfmodel = pd.DataFrame(modeldata)
     # print(dfmodel)
     at.inputmodel.save_modeldata(dfmodel=dfmodel, t_model_init_days=t_model_init_days, filepath=Path(args.outputpath))
@@ -596,22 +595,19 @@
         skiprows=1,
         names=["cellid", "vel_r_max_kmps", "rho"],
     )
     result["cellid"] = result["cellid"].astype(int)
     result["vel_r_min_kmps"] = np.concatenate(([0.0], result["vel_r_max_kmps"].to_numpy()[:-1]))
 
     t_model_init_seconds_in = t_model_init_days_in * 24 * 60 * 60  # noqa: F841
-    result = result.eval(
+    return result.eval(
         "mass_g = rho * 4. / 3. * @math.pi * (vel_r_max_kmps ** 3 - vel_r_min_kmps ** 3)"
         "* (1e5 * @t_model_init_seconds_in) ** 3"
-    )
-
-    # now replace the density at the input time with the density at required time
-
-    return result.eval(
+    ).eval(
+        # now replace the density at the input time with the density at required time
         "rho = mass_g / ("
         "4. / 3. * @math.pi * (vel_r_max_kmps ** 3 - vel_r_min_kmps ** 3)"
         " * (1e5 * @t_model_init_seconds) ** 3)"
     )
 
 
 if __name__ == "__main__":
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/rprocess_solar.py` & `artistools-2024.4.23/artistools/inputmodel/rprocess_solar.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,30 +42,26 @@
         dfmasschain = dfbetaminus.query("A == @row.A", inplace=False)
         return int(row.Z) if dfmasschain.empty else int(dfmasschain.Z.min())
 
     dfsolarabund_undecayed = dfsolarabund.copy()
     dfsolarabund_undecayed["Z"] = dfsolarabund_undecayed.apply(undecayed_z, axis=1)
 
     # Andreas uses 90% Fe and the rest solar
-    dfsolarabund_undecayed = dfsolarabund_undecayed.append(
-        {"Z": 26, "A": 56, "numberfrac": 0.005, "radioactive": False}, ignore_index=True
-    )
-    dfsolarabund_undecayed = dfsolarabund_undecayed.append(
-        {"Z": 27, "A": 59, "numberfrac": 0.005, "radioactive": False}, ignore_index=True
-    )
-    dfsolarabund_undecayed = dfsolarabund_undecayed.append(
-        {"Z": 28, "A": 58, "numberfrac": 0.005, "radioactive": False}, ignore_index=True
+    dfsolarabund_undecayed = (
+        dfsolarabund_undecayed.append({"Z": 26, "A": 56, "numberfrac": 0.005, "radioactive": False}, ignore_index=True)
+        .append({"Z": 27, "A": 59, "numberfrac": 0.005, "radioactive": False}, ignore_index=True)
+        .append({"Z": 28, "A": 58, "numberfrac": 0.005, "radioactive": False}, ignore_index=True)
     )
 
     normfactor = (  # noqa: F841
         dfsolarabund_undecayed.numberfrac.sum()
     )  # convert number fractions in solar to fractions of r-process
-    dfsolarabund_undecayed = dfsolarabund_undecayed.eval("numberfrac = numberfrac / @normfactor")
-
-    dfsolarabund_undecayed = dfsolarabund_undecayed.eval("massfrac = numberfrac * A")
+    dfsolarabund_undecayed = dfsolarabund_undecayed.eval("numberfrac = numberfrac / @normfactor").eval(
+        "massfrac = numberfrac * A"
+    )
     massfracnormfactor = dfsolarabund_undecayed.massfrac.sum()  # noqa: F841
     dfsolarabund_undecayed = dfsolarabund_undecayed.eval("massfrac = massfrac / @massfracnormfactor")
 
     # print(dfsolarabund_undecayed)
 
     t_model_init_days = 0.000231481
     t_model_init_seconds = t_model_init_days * 24 * 60 * 60  # noqa: F841
@@ -102,15 +98,15 @@
 
     dictelemabund = {}
     for atomic_number in range(1, dfsolarabund_undecayed.Z.max() + 1):
         dictelemabund[f"X_{at.get_elsymbol(atomic_number)}"] = dfsolarabund_undecayed.query(
             "Z == @atomic_number", inplace=False
         ).massfrac.sum()
 
-    dfelabundances = pd.DataFrame([dict(inputcellid=mgi + 1, **dictelemabund) for mgi in range(cellcount)])
+    dfelabundances = pd.DataFrame([{"inputcellid": mgi + 1} | dictelemabund for mgi in range(cellcount)])
     # print(dfelabundances)
     at.inputmodel.save_initelemabundances(dfelabundances=dfelabundances, outpath=Path(args.outputpath))
 
     # write model.txt
 
     rowdict = {
         # 'inputcellid': 1,
@@ -124,26 +120,25 @@
         "X_Ni57": 0.0,
         "X_Co57": 0.0,
     }
 
     for _, row in dfsolarabund_undecayed.query("radioactive == True").iterrows():
         rowdict[f"X_{at.get_elsymbol(int(row.Z))}{int(row.A)}"] = row.massfrac
 
-    modeldata = []
-    for mgi, densityrow in dfdensities.iterrows():
-        # print(mgi, densityrow)
-        modeldata.append(
-            dict(
-                inputcellid=mgi + 1,
-                vel_r_max_kmps=densityrow["vel_r_max_kmps"],
-                logrho=math.log10(densityrow["rho"]),
-                **rowdict,
-            )
+    modeldata = [
+        (
+            {
+                "inputcellid": mgi + 1,
+                "vel_r_max_kmps": densityrow["vel_r_max_kmps"],
+                "logrho": math.log10(densityrow["rho"]),
+            }
+            | rowdict
         )
-    # print(modeldata)
+        for mgi, densityrow in dfdensities.iterrows()
+    ]
 
     dfmodel = pd.DataFrame(modeldata)
     # print(dfmodel)
     at.inputmodel.save_modeldata(dfmodel=dfmodel, t_model_init_days=t_model_init_days, outpath=args.outputpath)
 
 
 if __name__ == "__main__":
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/scalevelocity.py` & `artistools-2024.4.23/artistools/inputmodel/scalevelocity.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/shen2018.py` & `artistools-2024.4.23/artistools/inputmodel/shen2018.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 import argparse
 import math
+import string
 import typing as t
 from pathlib import Path
 
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
@@ -26,15 +27,15 @@
 
     with Path(args.inputpath).open() as infile:
         columns = infile.readline().split()
 
     atomicnumberofspecies = {}
     isotopesofelem: dict[int, list[str]] = {}
     for species in columns[5:]:
-        atomic_number = at.get_atomic_number(species.rstrip("0123456789"))
+        atomic_number = at.get_atomic_number(species.rstrip(string.digits))
         atomicnumberofspecies[species] = atomic_number
         isotopesofelem.setdefault(atomic_number, []).append(species)
 
     datain = pd.read_csv(args.inputpath, sep=r"\s+", skiprows=0, header=[0]).dropna()
 
     dfmodel = pd.DataFrame(
         columns=[
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/slice1dfromconein3dmodel.py` & `artistools-2024.4.23/artistools/inputmodel/slice1dfromconein3dmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     slice1d = slice1d.drop(
         ["inputcellid", f"pos_{args.other_axis1}_min", f"pos_{args.other_axis2}_min"], axis=1
     )  # Remove columns we don't need
 
     if args.rhoscale:
         logprint("Scaling density by a factor of:", args.rhoscale)
-        slice1d["rho"] = slice1d["rho"] * args.rhoscale
+        slice1d["rho"] *= args.rhoscale
 
     slice1d["rho"] = slice1d["rho"].apply(lambda x: np.log10(x) if x != 0 else -100)
     # slice1d = slice1d[slice1d['rho_model'] != -100]  # Remove empty cells
     # TODO: fix this, -100 probably breaks things if it's not one of the outer cells that gets chopped
     slice1d = slice1d.rename(columns={"rho": "logrho"})
 
     slice1d.index += 1
@@ -174,16 +174,15 @@
 # cone = cone.loc[cone['rho_model'] > 0.0]
 
 
 def make_plot(args):
     cone = make_cone(args)
 
     cone = cone.loc[cone["rho_model"] > 0.0002]  # cut low densities (empty cells?) from plot
-    fig = plt.figure()
-    ax = fig.gca(projection="3d")
+    ax = plt.figure().gca(projection="3d")
 
     # print(cone['rho_model'])
 
     # set up for big model. For scaled down artis input model switch x and z
     x = cone["pos_z_min"].apply(lambda x: x / args.t_model * (u.cm / u.day).to("km/s")) / 1e3
     y = cone["pos_y_min"].apply(lambda x: x / args.t_model * (u.cm / u.day).to("km/s")) / 1e3
     z = cone["pos_x_min"].apply(lambda x: x / args.t_model * (u.cm / u.day).to("km/s")) / 1e3
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/test_inputmodel.py` & `artistools-2024.4.23/artistools/inputmodel/test_inputmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
 
 def test_describeinputmodel_3d() -> None:
     at.inputmodel.describeinputmodel.main(argsraw=[], inputfile=modelpath_3d, isotopes=True)
 
 
 def test_get_modeldata_1d() -> None:
-    for getheadersonly in [False, True]:
+    for getheadersonly in (False, True):
         dfmodel, modelmeta = at.get_modeldata(modelpath=modelpath, getheadersonly=getheadersonly)
         assert np.isclose(modelmeta["vmax_cmps"], 800000000.0)
         assert modelmeta["dimensions"] == 1
         assert modelmeta["npts_model"] == 1
 
     dfmodel, modelmeta = at.get_modeldata(modelpath=modelpath, derived_cols=["mass_g"])
     assert np.isclose(dfmodel.mass_g.sum(), 1.416963e33)
 
 
 def test_get_modeldata_3d() -> None:
-    for getheadersonly in [False, True]:
+    for getheadersonly in (False, True):
         dfmodel, modelmeta = at.get_modeldata(modelpath=modelpath_3d, getheadersonly=getheadersonly)
         assert np.isclose(modelmeta["vmax_cmps"], 2892020000.0)
         assert modelmeta["dimensions"] == 3
         assert modelmeta["npts_model"] == 1000
         assert modelmeta["ncoordgridx"] == 10
 
     dfmodel, modelmeta = at.get_modeldata(modelpath=modelpath_3d, derived_cols=["mass_g"])
@@ -84,15 +84,15 @@
     for filename, checksum_expected in checksums_expected.items():
         fullpath = Path(folder) / filename
         m = hashlib.new(digest)
         with Path(fullpath).open("rb") as f:
             for chunk in f:
                 m.update(chunk)
 
-        checksums_actual[fullpath] = str(m.hexdigest())
+        checksums_actual[fullpath] = m.hexdigest()
         strpassfail = "pass" if checksums_actual[fullpath] == checksum_expected else "FAILED"
         print(f"{filename}: {strpassfail} if actual {checksums_actual[fullpath]} expected {checksum_expected}")
 
     for filename, checksum_expected in checksums_expected.items():
         fullpath = Path(folder) / filename
         assert (
             checksums_actual[fullpath] == checksum_expected
@@ -109,28 +109,28 @@
                 "ejectapartanalysis.dat": "e8694a679515c54c2b4867122122263a375d9ffa144a77310873ea053bb5a8b4",
                 "grid.dat": "ea930d0decca79d2e65ac1df1aaaa1eb427fdf45af965a623ed38240dce89954",
                 "gridcontributions.txt": "a2c09b96d32608db2376f9df61980c2ad1423066b579fbbe744f07e536f2891e",
             },
             "makeartismodel_sums": {
                 "gridcontributions.txt": "12f006c43c0c8d1f84c3927b3c80959c1b2cecc01598be92c2f24a130892bc60",
                 "abundances.txt": "5f782005ce879a8c81c43d0a7a791ad9b177eee8630b4771586949bf7fbca28e",
-                "model.txt": "9b1d2b39af397ab24f84e9b3304eee5e8c1c699aae7bb850b4dc7ecfb563f8ba",
+                "model.txt": "547426e194741e4ab58a65848f165dcd3ef9275de711ba4870b11f32bf7b06d5",
             },
         },
         {
             "maptogridargs": {"ncoordgrid": 16},
             "maptogrid_sums": {
                 "ejectapartanalysis.dat": "e8694a679515c54c2b4867122122263a375d9ffa144a77310873ea053bb5a8b4",
                 "grid.dat": "b179427dc76e3b465d83fb303c866812fa9cb775114d1b8c45411dd36bf295b2",
                 "gridcontributions.txt": "63e6331666c4928bdc6b7d0f59165e96d6555736243ea8998a779519052a425f",
             },
             "makeartismodel_sums": {
                 "gridcontributions.txt": "6c8186b992e8037f27c249feb19557705dc11db86dc47fa0d1e7257e420fce23",
                 "abundances.txt": "5f782005ce879a8c81c43d0a7a791ad9b177eee8630b4771586949bf7fbca28e",
-                "model.txt": "5700128f7aaefa18a71d58cc47e3df6b125991b72eae3f3bdd3245f9bd3100dc",
+                "model.txt": "01c5870c321fa25f07ab080a2c11705b340c7b810748ee2500fc3746479f6286",
             },
         },
     ]
 
     for config in config_checksums_3d:
         shutil.copytree(
             testdatapath / "kilonova", gridfolderpath, dirs_exist_ok=True, ignore=shutil.ignore_patterns("trajectories")
@@ -143,15 +143,15 @@
         verify_file_checksums(
             config["maptogrid_sums"],
             digest="sha256",
             folder=gridfolderpath,
         )
 
         dfcontribs = {}
-        for dimensions in [3, 2, 1, 0]:
+        for dimensions in (3, 2, 1, 0):
             outpath_kn = outputpath / f"kilonova_{dimensions:d}d"
             outpath_kn.mkdir(exist_ok=True, parents=True)
 
             shutil.copyfile(gridfolderpath / "gridcontributions.txt", outpath_kn / "gridcontributions.txt")
 
             at.inputmodel.modelfromhydro.main(
                 argsraw=[],
@@ -295,15 +295,15 @@
     dfmodel3d_pl[mgi2, "rho"] = 1
     dfmodel3d_pl[mgi1, "X_Ni56"] = 0.75
 
     dfmodel3d_pl = at.inputmodel.add_derived_cols_to_modeldata(
         dfmodel=dfmodel3d_pl, modelmeta=modelmeta_3d, derived_cols=["mass_g"]
     ).collect()
 
-    outpath = outputpath / "test_dimension_reduce_3d_{outputdimensions:d}d"
+    outpath = outputpath / f"test_dimension_reduce_3d_{outputdimensions:d}d"
     outpath.mkdir(exist_ok=True, parents=True)
     (
         dfmodel_lowerd,
         dfabundances_lowerd,
         dfgridcontributions_lowerd,
         modelmeta_lowerd,
     ) = at.inputmodel.dimension_reduce_3d_model(
```

### Comparing `artistools-2024.2.22.2/artistools/inputmodel/to_tardis.py` & `artistools-2024.4.23/artistools/inputmodel/to_tardis.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/__init__.py` & `artistools-2024.4.23/artistools/lightcurve/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/lightcurve.py` & `artistools-2024.4.23/artistools/lightcurve/lightcurve.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     modelpath: str | Path,
     escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
     maxpacketfiles: int | None = None,
     directionbins: t.Collection[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     get_cmf_column: bool = True,
+    directionbins_are_vpkt_observers: bool = False,
 ) -> dict[int, pl.DataFrame]:
     """Get ARTIS luminosity vs time from packets files."""
     if directionbins is None:
         directionbins = [-1]
     tmidarray = at.get_timestep_times(modelpath=modelpath, loc="mid")
     timearray = at.get_timestep_times(modelpath=modelpath, loc="start")
     arr_timedelta = at.get_timestep_times(modelpath=modelpath, loc="delta")
@@ -79,85 +80,112 @@
 
     timearrayplusend = np.concatenate([timearray, [timearray[-1] + arr_timedelta[-1]]])
 
     nphibins = at.get_viewingdirection_phibincount()
     ncosthetabins = at.get_viewingdirection_costhetabincount()
     ndirbins = at.get_viewingdirectionbincount()
 
-    nprocs_read, dfpackets = at.packets.get_packets_pl(
-        modelpath, maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type=escape_type
-    )
+    if directionbins_are_vpkt_observers:
+        vpkt_config = at.get_vpkt_config(modelpath)
+        nprocs_read, dfpackets = at.packets.get_virtual_packets_pl(modelpath, maxpacketfiles=maxpacketfiles)
+    else:
+        nprocs_read, dfpackets = at.packets.get_packets_pl(
+            modelpath, maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type=escape_type
+        )
 
     if get_cmf_column:
         dfpackets = dfpackets.with_columns(
             [
                 (pl.col("escape_time") * escapesurfacegamma / 86400.0).alias("t_arrive_cmf_d"),
             ]
         )
 
-    getcols = ["t_arrive_d", "e_rf"]
-    if get_cmf_column:
-        getcols += ["e_cmf", "t_arrive_cmf_d"]
-    if directionbins != [-1]:
-        if average_over_phi:
-            getcols.append("costhetabin")
-        elif average_over_theta:
-            getcols.append("phibin")
-        else:
-            getcols.append("dirbin")
+    getcols = set()
+    if directionbins_are_vpkt_observers:
+        vpkt_config = at.get_vpkt_config(modelpath)
+        for dirbin in directionbins:
+            obsdirindex = dirbin // vpkt_config["nspectraperobs"]
+            opacchoiceindex = dirbin % vpkt_config["nspectraperobs"]
+            getcols |= {
+                f"dir{obsdirindex}_nu_rf",
+                f"dir{obsdirindex}_t_arrive_d",
+                f"dir{obsdirindex}_e_rf_{opacchoiceindex}",
+            }
+    else:
+        getcols |= {"t_arrive_d", "e_rf"}
+        if get_cmf_column:
+            getcols |= {"e_cmf", "t_arrive_cmf_d"}
+        if directionbins != [-1]:
+            if average_over_phi:
+                getcols.add("costhetabin")
+            elif average_over_theta:
+                getcols.add("phibin")
+            else:
+                getcols.add("dirbin")
 
     dfpackets = dfpackets.select(getcols).collect(streaming=True).lazy()
 
     lcdata = {}
     for dirbin in directionbins:
-        if dirbin == -1:
+        if directionbins_are_vpkt_observers:
+            obsdirindex = dirbin // vpkt_config["nspectraperobs"]
+            opacchoiceindex = dirbin % vpkt_config["nspectraperobs"]
+            pldfpackets_dirbin = dfpackets.with_columns(
+                e_rf=pl.col(f"dir{obsdirindex}_e_rf_{opacchoiceindex}"),
+                t_arrive_d=pl.col(f"dir{obsdirindex}_t_arrive_d"),
+            )
+            solidanglefactor = 4 * math.pi
+        elif dirbin == -1:
             solidanglefactor = 1.0
             pldfpackets_dirbin = dfpackets
         elif average_over_phi:
             assert not average_over_theta
             solidanglefactor = ncosthetabins
-            pldfpackets_dirbin = dfpackets.filter(pl.col("costhetabin") * 10 == dirbin)
+            pldfpackets_dirbin = dfpackets.filter(pl.col("costhetabin") * nphibins == dirbin)
         elif average_over_theta:
             solidanglefactor = nphibins
             pldfpackets_dirbin = dfpackets.filter(pl.col("phibin") == dirbin)
         else:
             solidanglefactor = ndirbins
             pldfpackets_dirbin = dfpackets.filter(pl.col("dirbin") == dirbin)
 
         dftimebinned = at.packets.bin_and_sum(
             pldfpackets_dirbin,
             bincol="t_arrive_d",
             bins=list(timearrayplusend),
             sumcols=["e_rf"],
         )
 
+        npkts_selected = pldfpackets_dirbin.select(pl.count("e_rf")).collect().item(0, 0)
+        print(f"    dirbin {dirbin} contains {npkts_selected:.2e} packets")
+
         unitfactor = float((u.erg / u.day).to("solLum"))
         dftimebinned = dftimebinned.with_columns(
             [
                 pl.Series(name="time", values=tmidarray),
                 ((pl.col("e_rf_sum") / nprocs_read * solidanglefactor * unitfactor) / pl.Series(arr_timedelta)).alias(
                     "lum"
                 ),
             ]
         ).drop(["e_rf_sum", "t_arrive_d_bin"])
 
-        lcdata[dirbin] = dftimebinned
+        lcdata[dirbin] = dftimebinned.collect()
 
         if get_cmf_column:
             dftimebinned_cmf = at.packets.bin_and_sum(
                 pldfpackets_dirbin,
                 bincol="t_arrive_cmf_d",
                 bins=list(timearrayplusend),
                 sumcols=["e_cmf"],
-            )
+            ).collect()
 
             assert escapesurfacegamma is not None
             lcdata[dirbin] = lcdata[dirbin].with_columns(
                 (
-                    dftimebinned_cmf["e_cmf_sum"]
+                    dftimebinned_cmf.get_column("e_cmf_sum").to_numpy()
                     / nprocs_read
                     * solidanglefactor
                     / escapesurfacegamma
                     * (u.erg / u.day).to("solLum")
                     / arr_timedelta
                 ).alias("lum_cmf")
             )
@@ -264,34 +292,33 @@
                     wavelength_from_spectrum = np.linspace(wavefilter_min, wavefilter_max, len(wavefilter))
                     flux = interpolate_fn(wavelength_from_spectrum)
 
                 phot_filtobs_sn = evaluate_magnitudes(flux, transmission, wavelength_from_spectrum, zeropointenergyflux)
 
                 # print(time, phot_filtobs_sn)
                 if phot_filtobs_sn != 0.0:
-                    phot_filtobs_sn = phot_filtobs_sn - 25  # Absolute magnitude
+                    phot_filtobs_sn -= 25  # Absolute magnitude
                 filters_dict[filter_name].append((time, phot_filtobs_sn))
 
     return filters_dict
 
 
 def bolometric_magnitude(
     modelpath: Path,
-    timearray: t.Collection[float],
+    timearray: t.Collection[float | str],
     args: argparse.Namespace,
     angle: int = -1,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
 ) -> tuple[list[float], list[float]]:
     magnitudes = []
     times = []
 
     for timestep, time in enumerate(timearray):
         time = float(time)
-
         if (args.timemin is None or args.timemin <= time) and (args.timemax is None or args.timemax >= time):
             if angle == -1:
                 spectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[-1]
 
             elif args.plotvspecpol:
                 spectrum = at.spectra.get_vspecpol_spectrum(modelpath, time, angle, args)
             else:
```

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/plotlightcurve.py` & `artistools-2024.4.23/artistools/lightcurve/plotlightcurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     modelname = at.get_model_name(modelpath) if label is None else label
     if lcfilename is not None:
         modelname += f" {lcfilename}"
     if not modelname:
         print("====> (no series label)")
     else:
         print(f"====> {modelname}")
-    print(f" folder: {modelpath.resolve().parts[-1]}")
+    print(f" modelpath: {modelpath.resolve().parts[-1]}")
 
     if args is not None and args.title:
         axis.set_title(modelname)
 
     if directionbins is None:
         directionbins = [-1]
 
@@ -314,14 +314,15 @@
             modelpath,
             escape_type=escape_type,
             maxpacketfiles=maxpacketfiles,
             directionbins=directionbins,
             average_over_phi=average_over_phi,
             average_over_theta=average_over_theta,
             get_cmf_column=args.plotcmf,
+            directionbins_are_vpkt_observers=args.plotvspecpol is not None,
         )
     else:
         if lcfilename is None:
             lcfilename = (
                 "light_curve_res.out"
                 if directionbins != [-1]
                 else "gamma_light_curve.out"
@@ -502,15 +503,15 @@
             sharex=True,
             figsize=(args.figscale * conffigwidth, args.figscale * conffigwidth / 1.6),
             tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
         )
     else:
         axistherm = None
 
-    # take any assigned colours our of the cycle
+    # take any specified colours our of the cycle
     colors = [
         color for i, color in enumerate(plt.rcParams["axes.prop_cycle"].by_key()["color"]) if f"C{i}" not in args.color
     ]
     axis.set_prop_cycle(color=colors)
     reflightcurveindex = 0
 
     plottedsomething = False
@@ -537,24 +538,25 @@
                 )
             else:
                 axis.scatter(dflightcurve["time_days"], dflightcurve["luminosity_erg/s"], **plotkwargs)
             print(f"====> {lightcurvelabel}")
             reflightcurveindex += 1
             plottedsomething = True
         else:
+            dirbin = args.plotviewingangle or (args.plotvspecpol or [-1])
             lcdataframes = plot_artis_lightcurve(
                 modelpath=modelpath,
                 lcindex=lcindex,
                 label=args.label[lcindex],
                 axis=axis,
                 escape_type=escape_type,
                 frompackets=frompackets,
                 maxpacketfiles=maxpacketfiles,
                 axistherm=axistherm,
-                directionbins=args.plotviewingangle if args.plotviewingangle is not None else [-1],
+                directionbins=dirbin,
                 average_over_phi=args.average_over_phi_angle,
                 average_over_theta=args.average_over_theta_angle,
                 usedegrees=args.usedegrees,
                 args=args,
             )
             plottedsomething = plottedsomething or (lcdataframes is not None)
 
@@ -642,15 +644,15 @@
         if args.xmax is not None:
             axistherm.set_xlim(right=args.xmax)
         axistherm.set_ylim(bottom=0.0)
         # axistherm.set_ylim(top=1.05)
 
         # filenameout2 = "plotthermalisation.pdf"
         filenameout2 = str(filenameout).replace(".pdf", "_thermalisation.pdf")
-        figtherm.savefig(str(filenameout2), format="pdf")
+        figtherm.savefig(filenameout2, format="pdf")
         print(f"Saved {filenameout2}")
 
     plt.close()
 
 
 def create_axes(args):
     if "labelfontsize" in args:
@@ -697,26 +699,26 @@
     modelnumber: int,
     angle: int | None,
     angle_definition: dict[int, str] | None,
     args,
 ) -> str:
     if angle is not None and angle != -1:
         assert angle_definition is not None
-        linelabel = f"{angle_definition[angle]}" if args.nomodelname else f"{modelname} {angle_definition[angle]}"
+        linelabel = angle_definition[angle] if args.nomodelname else f"{modelname} {angle_definition[angle]}"
         # linelabel = None
         # linelabel = fr"{modelname} $\theta$ = {angle_names[index]}$^\circ$"
         # plt.plot(time, magnitude, label=linelabel, linewidth=3)
     elif args.label:
-        linelabel = rf"{args.label[modelnumber]}"
+        linelabel = str(args.label[modelnumber])
     else:
-        linelabel = f"{modelname}"
+        linelabel = modelname
         # linelabel = 'Angle averaged'
 
     if linelabel == "None" or linelabel is None:
-        linelabel = f"{modelname}"
+        linelabel = modelname
 
     return linelabel
 
 
 def set_lightcurveplot_legend(ax, args):
     if not args.nolegend:
         if args.subplots:
@@ -1378,15 +1380,15 @@
 
     parser.add_argument(
         "-plotviewingangle",
         type=int,
         nargs="+",
         help=(
             "Plot viewing angles. Expects int for angle number in specpol_res.out"
-            "use args = -1 to select all the viewing angles"
+            "use args = -2 to select all the viewing angles"
         ),
     )
     parser.add_argument(
         "--usedegrees",
         action="store_true",
         help="Use degrees instead of radians for viewing angles. Only works with -plotviewingangle",
     )
@@ -1453,28 +1455,28 @@
         "--save_viewing_angle_peakmag_risetime_delta_m15_to_file",
         action="store_true",
         help=(
             "Save the band risetime, peak mag and delta m15 values for "
             "all viewing angles specified for plotting at a later time "
             "as these values take a long time to calculate for all "
             "viewing angles. Need to run this command first alongside "
-            "--plotviewingangles in order to save the data for the "
+            "-plotviewingangle in order to save the data for the "
             "viewing angles you want to use before making the scatter"
             "plots"
         ),
     )
 
     parser.add_argument(
         "--test_viewing_angle_fit",
         action="store_true",
         help=(
             "Plots the lightcurves for each  viewing angle along with"
             "the polynomial fit for each viewing angle specified"
             "to check the fit is working properly: use alongside"
-            "--plotviewingangle "
+            "-plotviewingangle "
         ),
     )
 
     parser.add_argument(
         "--make_viewing_angle_peakmag_risetime_scatter_plot",
         action="store_true",
         help=(
```

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/test_lightcurve.py` & `artistools-2024.4.23/artistools/lightcurve/test_lightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/viewingangleanalysis.py` & `artistools-2024.4.23/artistools/lightcurve/viewingangleanalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,22 +141,26 @@
     "sandybrown",
     "teal",
 ]
 
 
 def parse_directionbin_args(modelpath: Path | str, args: argparse.Namespace) -> tuple[t.Sequence[int], dict[int, str]]:
     modelpath = Path(modelpath)
-    viewing_angle_data_exists = bool(list(modelpath.glob("*_res.out*")))
+    viewing_angle_data_exists = args.frompackets or bool(list(modelpath.glob("*_res.out*")))
     if isinstance(args.plotviewingangle, int):
         args.plotviewingangle = [args.plotviewingangle]
     dirbins = []
     if args.plotvspecpol and (modelpath / "vpkt.txt").is_file():
         dirbins = args.plotvspecpol
     elif args.plotviewingangle and args.plotviewingangle[0] == -2 and viewing_angle_data_exists:
         dirbins = np.arange(0, 100, 1, dtype=int).tolist()
+        if args.average_over_phi_angle:
+            dirbins = [d for d in dirbins if d % at.get_viewingdirection_phibincount() == 0]
+        if args.average_over_theta_angle:
+            dirbins = [d for d in dirbins if d < at.get_viewingdirection_costhetabincount()]
     elif args.plotviewingangle and viewing_angle_data_exists:
         dirbins = args.plotviewingangle
     elif (
         args.calculate_costheta_phi_from_viewing_angle_numbers
         and args.calculate_costheta_phi_from_viewing_angle_numbers[0] == -2
     ):
         dirbins = np.arange(0, 100, 1, dtype=int).tolist()
@@ -165,15 +169,15 @@
         assert dirbins is not None
     else:
         dirbins = [-1]
 
     dirbin_definition: dict[int, str] = {}
 
     if args.plotvspecpol:
-        dirbin_definition = at.get_vspec_dir_labels(modelpath=modelpath)
+        dirbin_definition = at.get_vspec_dir_labels(modelpath=modelpath, usedegrees=args.usedegrees)
     else:
         dirbin_definition = at.get_dirbin_labels(
             dirbins=dirbins,
             modelpath=modelpath,
             average_over_phi=args.average_over_phi_angle,
             average_over_theta=args.average_over_theta_angle,
             usedegrees=args.usedegrees,
@@ -204,15 +208,15 @@
                 ],
                 delimiter=" ",
                 header="peak_mag_polyfit risetime_polyfit deltam15_polyfit deltam40_polyfit",
                 comments="",
             )
         else:
             np.savetxt(
-                outputfolder / band_name + "band_" + f"{modelname}" + "_viewing_angle_data.txt",
+                outputfolder / f"{band_name}band_{modelname}_viewing_angle_data.txt",
                 np.c_[args.band_peakmag_polyfit, args.band_risetime_polyfit, args.band_deltam15_polyfit],
                 delimiter=" ",
                 header="peak_mag_polyfit risetime_polyfit deltam15_polyfit",
                 comments="",
             )
 
     elif (
@@ -241,15 +245,15 @@
 def write_viewing_angle_data(band_name, modelnames, args):
     if (
         args.save_angle_averaged_peakmag_risetime_delta_m15_to_file
         or args.make_viewing_angle_peakmag_risetime_scatter_plot
         or args.make_viewing_angle_peakmag_delta_m15_scatter_plot
     ):
         np.savetxt(
-            band_name + "band_" + f"{modelnames[0]}" + "_angle_averaged_all_models_data.txt",
+            f"{band_name}band_{modelnames[0]}_angle_averaged_all_models_data.txt",
             np.c_[
                 modelnames,
                 args.band_risetime_angle_averaged_polyfit,
                 args.band_peakmag_angle_averaged_polyfit,
                 args.band_delta_m15_angle_averaged_polyfit,
             ],
             delimiter=" ",
@@ -281,15 +285,15 @@
         "The --test_viewing_angle_fit flag will allow you to check the fitting is "
         "behaving as expected. In general fitting over a smaller region of the    "
         "light curve tends to produce better fits."
     )
     fxfit, xfit = lightcurve_polyfit(time, magnitude, args)
 
     def match_closest_time_polyfit(reftime_polyfit):
-        return str(f"{min((float(x) for x in xfit), key=lambda x: abs(x - reftime_polyfit))}")
+        return str(min((float(x) for x in xfit), key=lambda x: abs(x - reftime_polyfit)))
 
     index_min = np.argmin(fxfit)
     tmax_polyfit = xfit[index_min]
     time_after15days_polyfit = match_closest_time_polyfit(tmax_polyfit + 15)
     if args.include_delta_m40:
         time_after40days_polyfit = match_closest_time_polyfit(tmax_polyfit + 40)
     for ii, xfits in enumerate(xfit):
@@ -525,15 +529,15 @@
 
 def make_viewing_angle_risetime_peakmag_delta_m15_scatter_plot(modelnames, key, args):
     fig, ax = plt.subplots(
         nrows=1, ncols=1, sharex=True, figsize=(8, 6), tight_layout={"pad": 0.5, "w_pad": 1.5, "h_pad": 0.3}
     )
 
     for ii, modelname in enumerate(modelnames):
-        viewing_angle_plot_data = pd.read_csv(key + "band_" + f"{modelname}" + "_viewing_angle_data.txt", delimiter=" ")
+        viewing_angle_plot_data = pd.read_csv(key + "band_" + str(modelname) + "_viewing_angle_data.txt", delimiter=" ")
 
         band_peak_mag_viewing_angles = viewing_angle_plot_data["peak_mag_polyfit"].to_numpy()
         band_delta_m15_viewing_angles = viewing_angle_plot_data["deltam15_polyfit"].to_numpy()
         band_risetime_viewing_angles = viewing_angle_plot_data["risetime_polyfit"].to_numpy()
 
         plotkwargsviewingangles, plotkwargsangleaveraged = set_scatterplot_plotkwargs(ii, args)
 
@@ -614,15 +618,15 @@
     )
 
     for modelnumber, modelpath in enumerate(args.modelpath):
         modelname = at.get_model_name(modelpath)
 
         bands = [args.filter[0], args.filter[1]]
 
-        datafilename = bands[0] + "band_" + f"{modelname}" + "_viewing_angle_data.txt"
+        datafilename = bands[0] + "band_" + str(modelname) + "_viewing_angle_data.txt"
         viewing_angle_plot_data = pd.read_csv(datafilename, delimiter=" ")
         data = {f"{bands[0]}max": viewing_angle_plot_data["peak_mag_polyfit"].to_numpy()}
         data[f"time_{bands[0]}max"] = viewing_angle_plot_data["risetime_polyfit"].to_numpy()
 
         # Get brightness in second band at time of peak in first band
         if len(data[f"time_{bands[0]}max"]) != 100:
             print(f"All 100 angles are not in file {datafilename}. Quitting")
```

### Comparing `artistools-2024.2.22.2/artistools/lightcurve/writebollightcurvedata.py` & `artistools-2024.4.23/artistools/lightcurve/writebollightcurvedata.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/linefluxes.py` & `artistools-2024.4.23/artistools/linefluxes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """Artistools - spectra related functions."""
 
-
 import argparse
 import contextlib
 import json
 import math
 import multiprocessing
 import typing as t
 from collections import namedtuple
@@ -62,24 +61,24 @@
 
     return dfpackets.query(f"{emtypecolumn} in @lineindices", inplace=False).copy()
 
 
 def get_packets_with_emtype(
     modelpath: Path | str, emtypecolumn: str, lineindices: t.Sequence[int], maxpacketfiles: int | None = None
 ):
-    packetsfiles = at.packets.get_packetsfilepaths(modelpath, maxpacketfiles=maxpacketfiles)
+    packetsfiles = at.packets.get_packets_text_paths(modelpath, maxpacketfiles=maxpacketfiles)
     nprocs_read = len(packetsfiles)
     assert nprocs_read > 0
 
     model, _ = at.inputmodel.get_modeldata(modelpath)
     # vmax = model.iloc[-1].vel_r_max_kmps * u.km / u.s
     processfile = partial(get_packets_with_emtype_onefile, emtypecolumn, lineindices)
     if at.get_config()["num_processes"] > 1:
         print(f"Reading packets files with {at.get_config()['num_processes']} processes")
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
             arr_dfmatchingpackets = pool.map(processfile, packetsfiles)
             pool.close()
             pool.join()
             # pool.terminate()
     else:
         arr_dfmatchingpackets = [processfile(f) for f in packetsfiles]
 
@@ -228,16 +227,17 @@
     ion_stage: int,
     approxlambdalabel: str | int,
     lambdamin: float | None = None,
     lambdamax: float | None = None,
     lowerlevelindex: int | None = None,
     upperlevelindex: int | None = None,
 ):
-    dflinelist = at.get_linelist_dataframe(modelpath)
-    dflinelistclosematches = dflinelist.query("atomic_number == @atomic_number and ion_stage == @ion_stage").copy()
+    dflinelistclosematches = (
+        at.get_linelist_dataframe(modelpath).query("atomic_number == @atomic_number and ion_stage == @ion_stage").copy()
+    )
     if lambdamin is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamin < lambda_angstroms")
     if lambdamax is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamax > lambda_angstroms")
     if lowerlevelindex is not None:
         dflinelistclosematches = dflinelistclosematches.query("lowerlevelindex==@lowerlevelindex")
     if upperlevelindex is not None:
@@ -435,15 +435,15 @@
         if not args.nolegend:
             ax.legend(loc="upper right", frameon=False, handlelength=1, ncol=2, numpoints=1, prop={"size": 9})
 
     defaultoutputfile = "linefluxes.pdf"
     if not args.outputfile:
         args.outputfile = defaultoutputfile
     elif not Path(args.outputfile).suffixes:
-        args.outputfile = args.outputfile / defaultoutputfile
+        args.outputfile /= defaultoutputfile
 
     fig.savefig(args.outputfile, format="pdf")
     # plt.show()
     print(f"Saved {args.outputfile}")
     plt.close()
 
 
@@ -608,15 +608,15 @@
     Tedata_all = {}
 
     # data is collected, now make plots
     defaultoutputfile = "emittingregions.pdf"
     if not args.outputfile:
         args.outputfile = defaultoutputfile
     elif not Path(args.outputfile).suffixes:
-        args.outputfile = args.outputfile / defaultoutputfile
+        args.outputfile /= defaultoutputfile
 
     args.modelpath.append(None)
     args.label.append(f"All models: {args.label}")
     args.modeltag.append("all")
     for modelindex, (modelpath, modellabel, modeltag) in enumerate(zip(args.modelpath, args.label, args.modeltag)):
         print(f"ARTIS model: '{modellabel}'")
 
@@ -710,17 +710,15 @@
                         refdatapoints[refdataindex][timeindexb]["temp"],
                         color="0.4",
                         lw=2,
                         label=f"{refdatalabels[refdataindex]} +{refdatakeys[refdataindex][timeindexb]}d",
                     )
 
             if modeltag == "all":
-                for bars in [
-                    False,
-                ]:  # [False, True]
+                for bars in (False,):  # (False, True)
                     for truemodelindex in range(modelindex):
                         emfeatures = get_labelandlineindices(args.modelpath[truemodelindex], args.emfeaturesearch)
 
                         em_log10nne = np.concatenate(
                             [
                                 emdata_all[truemodelindex][(tmid, feature.colname)]["em_log10nne"]
                                 for feature in emfeatures
@@ -758,17 +756,15 @@
                     marker="o",
                     color="0.4",
                     lw=0,
                     edgecolors="none",
                     label="All cells",
                 )
 
-                for bars in [
-                    False,
-                ]:  # [False, True]
+                for bars in (False,):  # (False, True)
                     for featureindex, feature in enumerate(emfeatures):
                         emdata = emdata_all[modelindex][(tmid, feature.colname)]
 
                         if not bars:
                             print(f'   {len(emdata["em_log10nne"])} points plotted for {feature.featurelabel}')
 
                         serieslabel = (
```

### Comparing `artistools-2024.2.22.2/artistools/logfiles.py` & `artistools-2024.4.23/artistools/logfiles.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/macroatom.py` & `artistools-2024.4.23/artistools/macroatom.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/make_vpkt_input.py` & `artistools-2024.4.23/artistools/make_vpkt_input.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,22 +28,28 @@
 tmax_vgrid_in_days = 1.5
 
 # Specify wavelength range for velocity grid map: number of intervals (Nrange_grid) and limits (dum10,dum11)
 Nrange_grid = 1
 vgrid_lambda_min = 3500
 vgrid_lambda_max = 6000  # can have multiple ranges -- not implemented
 
+str_custom_lambda_ranges = (
+    (f" {len(custom_lambda_ranges)}" + " ".join(f"{lmin} {lmax}" for lmin, lmax in custom_lambda_ranges))
+    if custom_lambda_ranges
+    else ""
+)
+
 new_vpktfile = Path() / "vpkt.txt"
 with new_vpktfile.open("w") as vpktfile:
     vpktfile.write(
         f"{len(directions_costheta_phi)}\n"
         f"{' '.join(str(costheta) for costheta, _ in directions_costheta_phi)}\n"
         f"{' '.join(str(phi) for _, phi in directions_costheta_phi)}\n"
         f"{bool(opacityexclusions):d} {f'{len(opacityexclusions)} ' + ' '.join(str(x) for x in opacityexclusions) if opacityexclusions else ''}\n"
         f"{override_tminmax} {vspec_tmin_in_days} {vspec_tmax_in_days}\n"
-        f"{bool(custom_lambda_ranges):d} {(f'{len(custom_lambda_ranges)}' + ' '.join(f'{lmin} {lmax}' for lmin, lmax in custom_lambda_ranges)) if custom_lambda_ranges else ''}\n"  # this can have multiple wavelength ranges. May need changed.
+        f"{bool(custom_lambda_ranges):d}{str_custom_lambda_ranges}\n"
         f"{overrride_thickcell_tau:d} {cell_is_optically_thick_vpkt}\n"
         f"{tau_max_vpkt}\n"
         f"{vgrid_on:d}\n"
         f"{tmin_vgrid_in_days} {tmax_vgrid_in_days}\n"
         f"{Nrange_grid} {vgrid_lambda_min} {vgrid_lambda_max}"  # this can have multiple wavelength ranges. May need changed.
     )
```

### Comparing `artistools-2024.2.22.2/artistools/matplotlibrc` & `artistools-2024.4.23/artistools/matplotlibrc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pdf.fonttype: 42
 font.family: sans-serif
-font.sans-serif: Tahoma, 'DejaVu Sans', 'Lucida Grande', Verdana
+font.sans-serif: Tahoma, DejaVu Sans, Bitstream Vera Sans, Computer Modern Sans Serif, Lucida Grande, Verdana, Geneva, Lucid, Arial, Helvetica, Avant Garde, sans-serif
 #figure.constrained_layout.use: True
 # figure.figsize: 4.5, 4.
 
 savefig.format:    pdf
 
 
 #axes.formatter.useoffset: False
```

### Comparing `artistools-2024.2.22.2/artistools/misc.py` & `artistools-2024.4.23/artistools/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import argparse
+import functools
 import gzip
 import io
+import itertools
 import math
+import string
 import typing as t
 from collections import namedtuple
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import polars as pl
 import pyzstd
 import xz
+from typeguard import typechecked
 
 import artistools as at
 
 roman_numerals = (
     "",
     "I",
     "II",
@@ -47,16 +51,15 @@
         kwargs["max_help_position"] = 39
         super().__init__(*args, **kwargs)
 
     def add_arguments(self, actions: t.Iterable[argparse.Action]) -> None:
         getinvocation = super()._format_action_invocation
 
         def my_sort(action: argparse.Action) -> str:
-            opstr = getinvocation(action)
-            return opstr.upper().replace("-", "z")  # push dash chars below alphabet
+            return getinvocation(action).upper().replace("-", "z")  # push dash chars below alphabet
 
         actions = sorted(actions, key=my_sort)
         super().add_arguments(actions)
 
 
 class AppendPath(argparse.Action):
     def __call__(self, parser, args, values, option_string=None) -> None:  # type: ignore[no-untyped-def] # noqa: ARG002
@@ -211,15 +214,15 @@
         print(f"bin number {start_bin} = the average of bins {[start_bin, *list(contribbins)]}")
 
     return dirbindataframesout
 
 
 def match_closest_time(reftime: float, searchtimes: list[t.Any]) -> str:
     """Get time closest to reftime in list of times (searchtimes)."""
-    return str(f"{min((float(x) for x in searchtimes), key=lambda x: abs(x - reftime))}")
+    return str(min((float(x) for x in searchtimes), key=lambda x: abs(x - reftime)))
 
 
 def get_vpkt_config(modelpath: Path | str) -> dict[str, t.Any]:
     filename = Path(modelpath, "vpkt.txt")
 
     with filename.open() as vpkt_txt:
         vpkt_config: dict[str, t.Any] = {
@@ -423,14 +426,15 @@
         if tstart <= timedays_float < tend:
             return ts
 
     msg = f"Could not find timestep bracketing time {timedays_float}"
     raise ValueError(msg)
 
 
+@typechecked
 def get_time_range(
     modelpath: Path,
     timestep_range_str: str | None = None,
     timemin: float | None = None,
     timemax: float | None = None,
     timedays_range_str: None | str | float = None,
 ) -> tuple[int, int, float | None, float | None]:
@@ -574,18 +578,18 @@
 
 
 def get_z_a_nucname(nucname: str) -> tuple[int, int]:
     """Return atomic number and mass number from a string like 'Pb208', 'X_Pb208', or "nniso_Pb208' (returns 92, 208)."""
     if "_" in nucname:
         nucname = nucname.split("_")[1]
 
-    z = get_atomic_number(nucname.rstrip("0123456789"))
+    z = get_atomic_number(nucname.rstrip(string.digits))
     assert z > 0
 
-    a = int(nucname.lower().lstrip("abcdefghijklmnopqrstuvwxyz"))
+    a = int(nucname.lower().lstrip(string.ascii_lowercase))
 
     return z, a
 
 
 @lru_cache(maxsize=1)
 def get_elsymbolslist() -> list[str]:
     """Return a list of element symbols.
@@ -620,15 +624,15 @@
     )
 
 
 def get_atomic_number(elsymbol: str) -> int:
     """Return the atomic number of an element symbol."""
     assert elsymbol is not None
     elsymbol = elsymbol.removeprefix("X_")
-    elsymbol = elsymbol.split("_")[0].split("-")[0].rstrip("0123456789")
+    elsymbol = elsymbol.split("_")[0].split("-")[0].rstrip(string.digits)
 
     if elsymbol.title() in get_elsymbolslist():
         return get_elsymbolslist().index(elsymbol.title())
 
     return -1
 
 
@@ -696,30 +700,30 @@
     atomic_number: int | np.int64,
     ion_stage: None | int | np.int64 | t.Literal["ALL"],
     style: t.Literal["spectral", "chargelatex", "charge"] = "spectral",
     sep: str = " ",
 ) -> str:
     """Return a string with the element symbol and ionisation stage."""
     if ion_stage is None or ion_stage == "ALL":
-        return f"{get_elsymbol(atomic_number)}"
+        return get_elsymbol(atomic_number)
 
     if isinstance(ion_stage, str) and ion_stage.startswith(at.get_elsymbol(atomic_number)):
         # nuclides like Sr89 get passed in as atomic_number=38, ion_stage='Sr89'
         return ion_stage
 
     assert not isinstance(ion_stage, str)
 
     if style == "spectral":
         return f"{get_elsymbol(atomic_number)}{sep}{roman_numerals[ion_stage]}"
 
     strcharge = ""
     if style == "chargelatex":
         # ion notion e.g. Co+, Fe2+
         if ion_stage > 2:
-            strcharge = r"$^{" + f"{ion_stage - 1}" + r"{+}}$"
+            strcharge = r"$^{" + str(ion_stage - 1) + r"{+}}$"
         elif ion_stage == 2:
             strcharge = r"$^{+}$"
     elif ion_stage > 2:
         strcharge = f"{ion_stage - 1}+"
     elif ion_stage == 2:
         strcharge = "+"
 
@@ -800,81 +804,109 @@
             listout.extend(elem)
         else:
             listout.append(elem)
     return listout
 
 
 def zopen(filename: Path | str, mode: str = "rt", encoding: str | None = None) -> t.Any:
-    """Open filename, filename.ztd, filename.gz or filename.xz."""
+    """Open filename, filename.zst, filename.gz or filename.xz."""
     ext_fopen: dict[str, t.Callable] = {".zst": pyzstd.open, ".gz": gzip.open, ".xz": xz.open}
 
     for ext, fopen in ext_fopen.items():
         file_withext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
         if Path(file_withext).exists():
             return fopen(file_withext, mode=mode, encoding=encoding)
 
     # open() can raise file not found if this file doesn't exist
     return Path(filename).open(mode=mode, encoding=encoding)  # noqa: SIM115
 
 
 def zopenpl(filename: Path | str, mode: str = "rt", encoding: str | None = None) -> t.Any | Path:
-    """Open filename, filename.ztd, filename.gz or filename.xz. If polars.read_csv can read the file directly, return a Path object instead of a file object."""
+    """Open filename, filename.zst, filename.gz or filename.xz. If polars.read_csv can read the file directly, return a Path object instead of a file object."""
     mode = "r"
-    ext_fopen: dict[str, t.Callable] = {".zst": pyzstd.open, ".gz": gzip.open, ".xz": xz.open}
+    ext_fopen: dict[str, t.Callable | None] = {".zst": None, ".gz": None, ".xz": xz.open}
 
     for ext, fopen in ext_fopen.items():
         file_withext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
         if Path(file_withext).exists():
-            if ext in {".gz", ".zst"}:
-                return Path(file_withext)
-            return fopen(file_withext, mode=mode, encoding=encoding)
+            return Path(file_withext) if fopen is None else fopen(file_withext, mode=mode, encoding=encoding)
+
     return Path(filename)
 
 
 def firstexisting(
     filelist: t.Sequence[str | Path] | str | Path,
     folder: Path | str = Path(),
     tryzipped: bool = True,
+    search_subfolders: bool = True,
 ) -> Path:
     """Return the first existing file in file list. If none exist, raise exception."""
     if isinstance(filelist, str | Path):
         filelist = [filelist]
+
     folder = Path(folder)
+    folders = [folder]
 
     fullpaths = []
     for filename in filelist:
-        fullpaths.append(Path(folder) / filename)
+        if search_subfolders:
+            folders += [
+                p.parent for filename in filelist for p in folder.glob(f"*/{filename}*") if p.parent not in folders
+            ]
+
+        for folder in folders:
+            fullpaths.append(Path(folder) / filename)
 
-        if tryzipped:
-            for ext in [".zst", ".gz", ".xz"]:
-                filenameext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
-                if filenameext not in filelist:
-                    fullpaths.append(folder / filenameext)
+            if tryzipped:
+                for ext in (".zst", ".gz", ".xz"):
+                    filenameext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
+                    if filenameext not in filelist:
+                        fullpaths.append(folder / filenameext)
 
     for fullpath in fullpaths:
         if fullpath.exists():
             return fullpath
 
-    filelist = "\n  ".join([str(x.relative_to(folder)) for x in fullpaths])
-    msg = f"None of these files exist in {folder}: \n  {filelist}"
+    strfilelist = "\n  ".join([str(x.relative_to(folder)) for x in fullpaths])
+    orsub = " or subfolders" if search_subfolders else ""
+    msg = f"None of these files exist in {folder}{orsub}: \n  {strfilelist}"
     raise FileNotFoundError(msg)
 
 
 def anyexist(
     filelist: t.Sequence[str | Path],
     folder: Path | str = Path(),
     tryzipped: bool = True,
-) -> bool:
+    search_subfolders: bool = True,
+) -> Path | None:
     """Return true if any files in file list exist."""
     try:
-        firstexisting(filelist=filelist, folder=folder, tryzipped=tryzipped)
+        filepath = firstexisting(
+            filelist=filelist, folder=folder, tryzipped=tryzipped, search_subfolders=search_subfolders
+        )
     except FileNotFoundError:
-        return False
+        return None
 
-    return True
+    return filepath
+
+
+def batched(iterable: t.Iterable[t.Any], n: int) -> t.Generator[list, t.Any, None]:
+    """Batch data into iterators of length n. The last batch may be shorter."""
+    # batched('ABCDEFG', 3) --> ABC DEF G
+    if n < 1:
+        msg = "n must be at least one"
+        raise ValueError(msg)
+    it = iter(iterable)
+    while True:
+        chunk_it = itertools.islice(it, n)
+        try:
+            first_el = next(chunk_it)
+        except StopIteration:
+            return
+        yield list(itertools.chain((first_el,), chunk_it))
 
 
 def stripallsuffixes(f: Path) -> Path:
     """Take a file path (e.g. packets00_0000.out.gz) and return the Path with no suffixes (e.g. packets)."""
     f_nosuffixes = Path(f)
     for _ in f.suffixes:
         f_nosuffixes = f_nosuffixes.with_suffix("")  # each call removes only one suffix
@@ -882,15 +914,15 @@
     return f_nosuffixes
 
 
 def readnoncommentline(file: io.TextIOBase) -> str:
     """Read a line from the text file, skipping blank and comment lines that begin with #."""
     line = ""
 
-    while not line.strip() or line.strip().lstrip().startswith("#"):
+    while not line.strip() or line.lstrip().startswith("#"):
         line = file.readline()
 
     return line
 
 
 @lru_cache(maxsize=24)
 def get_file_metadata(filepath: Path | str) -> dict[str, t.Any]:
@@ -947,21 +979,20 @@
 
         assert filterfunc is None
         filterfunc = movavgfilterfunc
 
     if dictargs.get("filtersavgol", False):
         import scipy.signal
 
-        window_length, poly_order = (int(x) for x in args.filtersavgol)
-
-        def savgolfilterfunc(ylist: t.Any) -> t.Any:
-            return scipy.signal.savgol_filter(ylist, window_length, poly_order, mode=mode)
+        window_length, polyorder = (int(x) for x in args.filtersavgol)
 
         assert filterfunc is None
-        filterfunc = savgolfilterfunc
+        filterfunc = functools.partial(
+            scipy.signal.savgol_filter, window_length=window_length, polyorder=polyorder, mode=mode
+        )
 
         print("Applying Savitzky-Golay filter")
 
     return filterfunc
 
 
 def merge_pdf_files(pdf_files: list[str]) -> None:
@@ -1383,15 +1414,15 @@
     costhetabins_lower = np.arange(-1.0, 1.0, 2.0 / ncosthetabins)
     costhetabins_upper = costhetabins_lower + 2.0 / ncosthetabins
     if usedegrees:
         if usepiminustheta:
             piminusthetabins_upper = (np.pi - np.arccos(costhetabins_upper)) / np.pi * 180
             piminusthetabins_lower = (np.pi - np.arccos(costhetabins_lower)) / np.pi * 180
             binlabels = [
-                rf"{lower:.0f}° < $\pi$-$\theta$ < {upper:.0f}°"
+                rf"{lower:.0f}° < π-θ < {upper:.0f}°"
                 for lower, upper in zip(piminusthetabins_lower, piminusthetabins_upper)
             ]
         else:
             thetabins_upper = np.arccos(costhetabins_lower) / np.pi * 180
             thetabins_lower = np.arccos(costhetabins_upper) / np.pi * 180
 
             binlabels = [f"{lower:.0f}° < θ < {upper:.0f}°" for lower, upper in zip(thetabins_lower, thetabins_upper)]
@@ -1415,32 +1446,28 @@
     if z_exclude == -1:
         return "no-bb"
     if z_exclude == -2:
         return "no-bf"
     return "no-es" if z_exclude == -3 else f"no-{at.get_elsymbol(z_exclude)}"
 
 
-def get_vspec_dir_labels(modelpath: str | Path, viewinganglelabelunits: str = "rad") -> dict[int, str]:
+def get_vspec_dir_labels(modelpath: str | Path, usedegrees: bool = False) -> dict[int, str]:
     vpkt_config = at.get_vpkt_config(modelpath)
     dirlabels = {}
     for dirindex in range(vpkt_config["nobsdirections"]):
         phi_angle = round(vpkt_config["phi"][dirindex])
         for specindex in range(vpkt_config["nspectraperobs"]):
             opacity_condition_label = get_opacity_condition_label(int(vpkt_config["z_excludelist"][specindex]))
             ind_comb = vpkt_config["nspectraperobs"] * dirindex + specindex
             cos_theta = vpkt_config["cos_theta"][dirindex]
-            if viewinganglelabelunits == "deg":
+            if usedegrees:
                 theta_degrees = round(math.degrees(math.acos(cos_theta)))
-                dirlabels[
-                    ind_comb
-                ] = rf"v$\theta$ = {theta_degrees}$^\circ$, $\phi$ = {phi_angle}$^\circ$ {specindex} {opacity_condition_label}"
-            elif viewinganglelabelunits == "rad":
-                dirlabels[
-                    ind_comb
-                ] = rf"cos $\theta$ = {cos_theta}, $\phi$ = {phi_angle}$^\circ$ {opacity_condition_label}"
+                dirlabels[ind_comb] = rf"θ = {theta_degrees}°, ϕ = {phi_angle}° {specindex} {opacity_condition_label}"
+            else:
+                dirlabels[ind_comb] = rf"cos θ = {cos_theta}, ϕ = {phi_angle}° {opacity_condition_label}"
 
     return dirlabels
 
 
 def get_dirbin_labels(
     dirbins: npt.NDArray[np.int32] | t.Sequence[int] | None = None,
     modelpath: Path | str | None = None,
@@ -1480,17 +1507,17 @@
             angle_definitions[dirbin] = ""
             continue
 
         costheta_index = dirbin // nphibins
         phi_index = dirbin % nphibins
 
         if average_over_phi:
-            angle_definitions[dirbin] = f"{costhetabinlabels[costheta_index]}"
+            angle_definitions[dirbin] = costhetabinlabels[costheta_index]
             assert phi_index == 0
             assert not average_over_theta
         elif average_over_theta:
-            angle_definitions[dirbin] = f"{phibinlabels[phi_index]}"
+            angle_definitions[dirbin] = phibinlabels[phi_index]
             assert costheta_index == 0
         else:
             angle_definitions[dirbin] = f"{costhetabinlabels[costheta_index]}, {phibinlabels[phi_index]}"
 
     return angle_definitions
```

### Comparing `artistools-2024.2.22.2/artistools/nltepops/nltepops.py` & `artistools-2024.4.23/artistools/nltepops/nltepops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Artistools - NLTE population related functions."""
 
 import math
 import multiprocessing
 import re
+import string
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
 
 import pandas as pd
 from astropy import constants as const
 
@@ -28,15 +29,15 @@
             passed_term_Lchar = True
         elif re.match("[eo]", termpiece) is not None and passed_term_Lchar:
             # odd flag, but don't want to confuse it with the energy index (e.g. o4Fo[2])
             if termpiece != "e":  # even is assumed by default (and looks neater with all the 'e's)
                 strtermtex += r"$^{\rm " + termpiece + r"}$"
         elif re.match(r"[0-9]?.*\]", termpiece) is not None:
             # J value
-            strtermtex += termpiece.split("[")[0] + r"$_{" + termpiece.lstrip("0123456789").strip("[]") + r"}$"
+            strtermtex += termpiece.split("[")[0] + r"$_{" + termpiece.lstrip(string.digits).strip("[]") + r"}$"
         elif re.match("[0-9]", termpiece) is not None and passed_term_Lchar:
             # extra number after S char
             strtermtex += termpiece
 
     return strtermtex.replace("$$", "")
 
 
@@ -53,16 +54,15 @@
 
     for parentterm in re.findall(r"\([0-9][A-Z][^)]?\)", strout):
         parentermtex = f'({texifyterm(parentterm.strip("()"))})'
         strout = strout.replace(parentterm, parentermtex)
     strterm = levelname.split("_")[-1]
     strout += " " + texifyterm(strterm)
 
-    strout = strout.replace("#", "")
-    return strout.replace("$$", "")
+    return strout.replace("#", "").replace("$$", "")
 
 
 def add_lte_pops(modelpath, dfpop, columntemperature_tuples, noprint=False, maxlevel=-1):
     """Add columns to dfpop with LTE populations.
 
     columntemperature_tuples is a sequence of tuples of column name and temperature, e.g., ('mycolumn', 3000)
     """
@@ -206,15 +206,15 @@
 
     if dfquery:
         if dfquery_full:
             dfquery_full = f"({dfquery_full}) and "
         dfquery_full += f"({dfquery})"
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
             arr_dfnltepop = pool.map(
                 partial(read_file_filtered, strquery=dfquery_full, dfqueryvars=dfqueryvars), nltefilepaths
             )
             pool.close()
             pool.join()
             pool.terminate()
     else:
```

### Comparing `artistools-2024.2.22.2/artistools/nltepops/plotnltepops.py` & `artistools-2024.4.23/artistools/nltepops/plotnltepops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """Artistools - NLTE population related functions."""
 
-
 import argparse
 import contextlib
 import math
 import sys
 import typing as t
 from pathlib import Path
 
@@ -37,15 +36,15 @@
         size=10,
         va="bottom",
         ha="center",
     )
 
 
 def plot_reference_data(ax, atomic_number: int, ion_stage: int, estimators_celltimestep, dfpopthision, annotatelines):
-    nne, Te, TR, W = (estimators_celltimestep[s] for s in ["nne", "Te", "TR", "W"])
+    nne, Te, TR, W = (estimators_celltimestep[s] for s in ("nne", "Te", "TR", "W"))
     # comparison to Chianti file
     elsym = at.get_elsymbol(atomic_number)
     elsymlower = elsym.lower()
     if Path("data", f"{elsymlower}_{ion_stage}-levelmap.txt").exists():
         # ax.set_ylim(bottom=2e-3)
         # ax.set_ylim(top=4)
         with Path("data", f"{elsymlower}_{ion_stage}-levelmap.txt").open("r") as levelmapfile:
@@ -245,17 +244,17 @@
         # scale to match the ground state populations
         float(dfpopthision["n_NLTE"].iloc[0] / dfpopthision["n_LTE_T_e"].iloc[0])
         if args.departuremode
         # else scale to match the ion population
         else float(ionpopulation / dfpopthision["n_LTE_T_e"].sum())
     )
 
-    dfpopthision = dfpopthision.eval("n_LTE_T_e_normed = n_LTE_T_e * @x", local_dict={"x": lte_scalefactor})
-
-    dfpopthision = dfpopthision.eval("departure_coeff = n_NLTE / n_LTE_T_e_normed")
+    dfpopthision = dfpopthision.eval("n_LTE_T_e_normed = n_LTE_T_e * @x", local_dict={"x": lte_scalefactor}).eval(
+        "departure_coeff = n_NLTE / n_LTE_T_e_normed"
+    )
 
     pd.set_option("display.max_columns", 150)
     if len(dfpopthision) < 30:
         # print(dfpopthision[
         #     ['Z', 'ion_stage', 'level', 'config', 'departure_coeff', 'texname']].to_string(index=False))
         print(
             dfpopthision.loc[
@@ -376,15 +375,15 @@
 
 def make_plot_populations_with_time_or_velocity(modelpaths, args):
     font = {"size": 18}
     mpl.rc("font", **font)
 
     ionlevels = args.levels
 
-    Z = int(at.get_atomic_number(args.elements[0]))
+    Z = at.get_atomic_number(args.elements[0])
     ion_stage = int(args.ion_stages[0])
 
     adata = at.atomic.get_levels(args.modelpath[0], get_transitions=True)
     ion_data = adata.query("Z == @Z and ion_stage == @ion_stage").iloc[0]
     levelconfignames = ion_data["levels"]["levelname"]
     # levelconfignames = [at.nltepops.texifyconfiguration(name) for name in levelconfignames]
 
@@ -434,17 +433,17 @@
     else:
         ax.legend(loc="best", frameon=True, fontsize="x-small", ncol=1)
         ax.set_yscale("log")
 
     if not args.notitle:
         title = f"Z={Z}, ion_stage={ion_stage}"
         if args.x == "time":
-            title = title + f", mgi = {args.modelgridindex[0]}"
+            title += f", mgi = {args.modelgridindex[0]}"
         elif args.x == "velocity":
-            title = title + f", {args.timedays} days"
+            title += f", {args.timedays} days"
         plt.title(title)
 
     at.plottools.set_axis_properties(ax, args)
 
     figname = f"plotnltelevelpopsZ{Z}.pdf"
     plt.savefig(modelpaths[0] / figname, format="pdf")
     print(f"Saved {figname}")
@@ -455,23 +454,23 @@
         timesteps = list(range(args.timestepmin, args.timestepmax))
 
         if not args.modelgridindex:
             print("Please specify modelgridindex")
             sys.exit(1)
 
         modelgridindex_list = np.ones_like(timesteps)
-        modelgridindex_list = modelgridindex_list * int(args.modelgridindex[0])
+        modelgridindex_list *= int(args.modelgridindex[0])
 
     if args.x == "velocity":
         modeldata, _ = at.inputmodel.get_modeldata(modelpaths[0])  # TODO: move into modelpath loop
         velocity = modeldata["vel_r_max_kmps"]
         modelgridindex_list = [mgi for mgi, _ in enumerate(velocity)]
 
         timesteps = np.ones_like(modelgridindex_list)
-        timesteps = timesteps * at.get_timestep_of_timedays(modelpaths[0], timedays)
+        timesteps *= at.get_timestep_of_timedays(modelpaths[0], timedays)
 
     markers = ["o", "x", "^", "s", "8"]
     for modelnumber, modelpath in enumerate(modelpaths):
         # modelname = at.get_model_name(modelpath)
 
         populations = {}
         # populationsLTE = {}
@@ -487,21 +486,21 @@
                     "n_NLTE"
                 ].to_numpy()[0]
                 # populationsLTE[(timestep, ionlevel)] = (timesteppops.loc[timesteppops['level']
                 #                                                          == ionlevel]['n_LTE'].values[0])
 
         for ionlevel in ionlevels:
             plottimesteps = np.array([int(ts) for ts, level, mgi in populations if level == ionlevel])
-            timedays = [float(at.get_timestep_time(modelpath, ts)) for ts in plottimesteps]
+            timedays = [at.get_timestep_time(modelpath, ts) for ts in plottimesteps]
             plotpopulations = np.array(
                 [float(populations[ts, level, mgi]) for ts, level, mgi in populations if level == ionlevel]
             )
             # plotpopulationsLTE = np.array([float(populationsLTE[ts, level]) for ts, level in populationsLTE.keys()
             #                             if level == ionlevel])
-            linelabel = rf"{levelconfignames[ionlevel]}"
+            linelabel = str(levelconfignames[ionlevel])
             # linelabel = f'level {ionlevel} {modelname}'
 
             if args.x == "time":
                 ax.plot(timedays, plotpopulations, marker=markers[modelnumber], label=linelabel)
             elif args.x == "velocity":
                 ax.plot(velocity, plotpopulations, marker=markers[modelnumber], label=linelabel)
             # plt.plot(timedays, plotpopulationsLTE, marker=markers[modelnumber+1],
@@ -509,15 +508,15 @@
 
 
 def make_plot(modelpath, atomic_number, ion_stages_displayed, mgilist, timestep, args):
     """Plot level populations for chosens ions of an element in a cell and timestep of an ARTIS model."""
     modelname = at.get_model_name(modelpath)
     adata = at.atomic.get_levels(modelpath, get_transitions=args.gettransitions)
 
-    time_days = float(at.get_timestep_time(modelpath, timestep))
+    time_days = at.get_timestep_time(modelpath, timestep)
     modelname = at.get_model_name(modelpath)
 
     dfpop = at.nltepops.read_files(modelpath, timestep=timestep, modelgridindex=mgilist[0]).copy()
 
     if dfpop.empty:
         print(f"No NLTE population data for modelgrid cell {mgilist[0]} timestep {timestep}")
         return
@@ -593,22 +592,22 @@
         if len(dfpop.query("ion_stage == @max_ion_stage")) == 1:  # single-level ion, so skip it
             max_ion_stage -= 1
 
         # timearray = at.get_timestep_times(modelpath)
         nne = estimators[(timestep, modelgridindex)]["nne"]
         W = estimators[(timestep, modelgridindex)]["W"]
 
-        subplot_title = f"{modelname}"
+        subplot_title = str(modelname)
         if len(modelname) > 10:
             subplot_title += "\n"
         velocity = at.inputmodel.get_modeldata_tuple(modelpath)[0]["vel_r_max_kmps"][modelgridindex]
         subplot_title += f" {velocity:.0f} km/s at"
 
         try:
-            time_days = float(at.get_timestep_time(modelpath, timestep))
+            time_days = at.get_timestep_time(modelpath, timestep)
         except FileNotFoundError:
             time_days = 0
             subplot_title += f" timestep {timestep:d}"
         else:
             subplot_title += f" {time_days:.0f}d"
         subplot_title += rf" (Te={T_e:.0f} K, nne={nne:.1e} cm$^{{-3}}$, T$_R$={T_R:.0f} K, W={W:.1e})"
```

### Comparing `artistools-2024.2.22.2/artistools/nonthermal/__init__.py` & `artistools-2024.4.23/artistools/nonthermal/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/nonthermal/_nonthermal_core.py` & `artistools-2024.4.23/artistools/nonthermal/_nonthermal_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,15 +967,15 @@
         binding = get_mean_binding_energy(Z, ion_stage, electron_binding, ionpot_ev=ionpot_valence)  # binding in erg
         oneoverW = Aconst * binding / Zbar / (2 * math.pi * pow(QE, 4))  # per erg
         deposition_density_erg = deposition_density_ev * EV
 
         # to get the non-thermal ionization rate we need to divide the energy deposited
         # per unit volume per unit time in the grid cell (sum of terms above)
         # by the total ion number density and the "work per ion pair"
-        print(f"       work function: {1. / oneoverW / EV:.2f} [eV]")
+        print(f"       work function: {1.0 / oneoverW / EV:.2f} [eV]")
         print(f"   work fn ratecoeff: {deposition_density_erg / nntot * oneoverW:.2e}")
         # Axelrod 1980 Eq 3.225 with E0 = E = E_max
         # xs = lossfunction(engrid[-1], nne) * EV * oneoverW / nntot
         # print(f"         WFApprox xs: {xs:.2e} cm^2")
 
         print()
 
@@ -1482,9 +1482,9 @@
     # axes[-1].set_ylabel(r'Ionisation fraction of deposited energy')
     axes[-1].set_yscale("log")
     # axes[-1].set_ylabel(r'log y(E) [s$^{-1}$ cm$^{-2}$ eV$^{-1}$]', fontsize=fs)
     # axes[-1].yaxis.set_minor_locator(ticker.MultipleLocator(base=5))
     axes[-1].legend(frameon=False, loc="upper right")
     outputfilename = "plot.pdf"
     print(f"Saving '{outputfilename}'")
-    fig.savefig(str(outputfilename), format="pdf")
+    fig.savefig(outputfilename, format="pdf")
     plt.close()
```

### Comparing `artistools-2024.2.22.2/artistools/nonthermal/leptontransport.py` & `artistools-2024.4.23/artistools/nonthermal/leptontransport.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/nonthermal/plotnonthermal.py` & `artistools-2024.4.23/artistools/nonthermal/plotnonthermal.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             continue
 
         if index < len(args.modellabels):
             model_label = args.modellabels[index]
         else:
             model_label = f"{modelname} cell {modelgridindex} at timestep {timestep}"
             try:
-                time_days = float(at.get_timestep_time(Path(), timestep))
+                time_days = at.get_timestep_time(Path(), timestep)
             except FileNotFoundError:
                 time_days = 0
             else:
                 model_label += f" ({time_days:.2f}d)"
 
         outputfile = str(args.outputfile).format(modelgridindex, timestep)
         print(f"Plotting timestep {timestep:d}")
```

### Comparing `artistools-2024.2.22.2/artistools/nonthermal/solvespencerfanocmd.py` & `artistools-2024.4.23/artistools/nonthermal/solvespencerfanocmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 
 
 def make_ntstats_plot(ntstatfile: str | Path) -> None:
     fig, ax = plt.subplots(
         nrows=1, ncols=1, sharex=True, figsize=(4, 3), tight_layout={"pad": 0.5, "w_pad": 0.3, "h_pad": 0.3}
     )
 
-    dfstats = pd.read_csv(ntstatfile, sep=r"\s+", escapechar="#")
-    dfstats = dfstats.fillna(0)
+    dfstats = pd.read_csv(ntstatfile, sep=r"\s+", escapechar="#").fillna(0)
 
     norm_frac_sum = False
     if norm_frac_sum:
         # scale up (or down) ionisation, excitation, and heating to force frac_sum = 1.0
         dfstats = dfstats.eval("frac_sum = frac_ionization + frac_excitation + frac_heating")
         norm_factors = 1.0 / dfstats["frac_sum"]
     else:
@@ -191,15 +190,15 @@
         # nne = estim["nne"]
         T_e = estim["Te"]
         print("WARNING: Use LTE pops at Te for now")
         deposition_density_ev = estim["heating_dep"] / 1.6021772e-12  # convert erg to eV
         ionpopdict = {at.get_ion_tuple(k): v for k, v in estim.items() if k.startswith(("nnion_", "nnelement_"))}
 
         velocity = modeldata["vel_r_max_kmps"][args.modelgridindex]
-        args.timedays = float(at.get_timestep_time(modelpath, args.timestep))
+        args.timedays = at.get_timestep_time(modelpath, args.timestep)
         print(f"timestep {args.timestep} cell {args.modelgridindex} (v={velocity} km/s at {args.timedays:.1f}d)")
 
     # ionpopdict = {}
     # deposition_density_ev = 327
     # nne = 6.7e5
     #
     # ionpopdict[(26, 1)] = ionpopdict[26] * 1e-4
```

### Comparing `artistools-2024.2.22.2/artistools/packets/__init__.py` & `artistools-2024.4.23/artistools/packets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from artistools.packets.packets import add_derived_columns_lazy
 from artistools.packets.packets import add_packet_directions_lazypolars
 from artistools.packets.packets import bin_and_sum
 from artistools.packets.packets import bin_packet_directions
 from artistools.packets.packets import bin_packet_directions_lazypolars
 from artistools.packets.packets import get_directionbin
 from artistools.packets.packets import get_mean_packet_emission_velocity_per_ts
+from artistools.packets.packets import get_packets_batch_parquet_paths
 from artistools.packets.packets import get_packets_pl
-from artistools.packets.packets import get_packetsfilepaths
+from artistools.packets.packets import get_packets_text_paths
+from artistools.packets.packets import get_virtual_packets_pl
 from artistools.packets.packets import make_3d_grid
 from artistools.packets.packets import make_3d_histogram_from_packets
 from artistools.packets.packets import readfile
 from artistools.packets.packets import readfile_text
 from artistools.packets.packets import type_ids
```

### Comparing `artistools-2024.2.22.2/artistools/packets/packets.py` & `artistools-2024.4.23/artistools/packets/packets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import calendar
-import gzip
 import math
-import multiprocessing
+import time
 import typing as t
 from functools import lru_cache
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import polars as pl
 
 import artistools as at
 
-# for the parquet files
-time_parquetschemachange = (2024, 2, 16, 11, 0, 0)
-
 CLIGHT = 2.99792458e10
 DAY = 86400
 
 types = {
     10: "TYPE_GAMMA",
     11: "TYPE_RPKT",
     20: "TYPE_NTLEPTON",
@@ -190,15 +186,15 @@
 
     if "emtrue_timestep" in colnames:
         dfpackets["emtrue_timestep"] = dfpackets.apply(emtrue_timestep, axis=1)
 
     if "em_timestep" in colnames:
         dfpackets["em_timestep"] = dfpackets.apply(em_timestep, axis=1)
 
-    if any(x in colnames for x in ["angle_bin", "dirbin", "costhetabin", "phibin"]):
+    if any(x in colnames for x in ("angle_bin", "dirbin", "costhetabin", "phibin")):
         dfpackets = bin_packet_directions(modelpath, dfpackets)
 
     return dfpackets
 
 
 def add_derived_columns_lazy(
     dfpackets: pl.LazyFrame | pl.DataFrame,
@@ -206,129 +202,129 @@
     dfmodel: pd.DataFrame | pl.LazyFrame | None = None,
 ) -> pl.LazyFrame:
     """Add columns to a packets DataFrame that are derived from the values that are stored in the packets files.
 
     We might as well add everything, since the columns only get calculated when they are actually used (polars LazyFrame).
     """
     dfpackets = dfpackets.lazy().with_columns(
-        [
+        emission_velocity=(
+            (pl.col("em_posx") ** 2 + pl.col("em_posy") ** 2 + pl.col("em_posz") ** 2).sqrt() / pl.col("em_time")
+        ),
+        emission_velocity_lineofsight=(
             (
-                (pl.col("em_posx") ** 2 + pl.col("em_posy") ** 2 + pl.col("em_posz") ** 2).sqrt() / pl.col("em_time")
-            ).alias("emission_velocity")
-        ]
-    )
-
-    dfpackets = dfpackets.with_columns(
-        [
-            (
-                (
-                    (pl.col("em_posx") * pl.col("dirx")) ** 2
-                    + (pl.col("em_posy") * pl.col("diry")) ** 2
-                    + (pl.col("em_posz") * pl.col("dirz")) ** 2
-                ).sqrt()
-                / pl.col("em_time")
-            ).alias("emission_velocity_lineofsight")
-        ]
+                (pl.col("em_posx") * pl.col("dirx")) ** 2
+                + (pl.col("em_posy") * pl.col("diry")) ** 2
+                + (pl.col("em_posz") * pl.col("dirz")) ** 2
+            ).sqrt()
+            / pl.col("em_time")
+        ),
     )
 
     if modelmeta is None:
         return dfpackets
 
     if modelmeta["dimensions"] > 1:
         t_model_s = modelmeta["t_model_init_days"] * 86400.0
         vmax = modelmeta["vmax_cmps"]
 
         if modelmeta["dimensions"] == 2:
             vwidthrcyl = modelmeta["wid_init_rcyl"] / t_model_s
             vwidthz = modelmeta["wid_init_z"] / t_model_s
             dfpackets = dfpackets.with_columns(
-                [
-                    ((pl.col("em_posx").pow(2) + pl.col("em_posy").pow(2)).sqrt() / pl.col("em_time") / vwidthrcyl)
-                    .cast(pl.Int32)
-                    .alias("coordpointnumrcyl"),
-                    ((pl.col("em_posz") / pl.col("em_time") + vmax) / vwidthz).cast(pl.Int32).alias("coordpointnumz"),
-                ]
-            )
-            dfpackets = dfpackets.with_columns(
-                [
-                    (pl.col("coordpointnumz") * modelmeta["ncoordgridrcyl"] + pl.col("coordpointnumrcyl")).alias(
-                        "em_modelgridindex"
-                    )
-                ]
+                coordpointnumrcyl=(
+                    (pl.col("em_posx").pow(2) + pl.col("em_posy").pow(2)).sqrt() / pl.col("em_time") / vwidthrcyl
+                ).cast(pl.Int32),
+                coordpointnumz=((pl.col("em_posz") / pl.col("em_time") + vmax) / vwidthz).cast(pl.Int32),
+            ).with_columns(
+                em_modelgridindex=(pl.col("coordpointnumz") * modelmeta["ncoordgridrcyl"] + pl.col("coordpointnumrcyl"))
             )
 
         elif modelmeta["dimensions"] == 3:
             vwidth = modelmeta["wid_init"] / t_model_s
             dfpackets = dfpackets.with_columns(
                 [
                     ((pl.col(f"em_pos{ax}") / pl.col("em_time") + vmax) / vwidth)
                     .cast(pl.Int32)
                     .alias(f"coordpointnum{ax}")
-                    for ax in ["x", "y", "z"]
-                ]
-            )
-            dfpackets = dfpackets.with_columns(
-                [
-                    (
-                        pl.col("coordpointnumz") * modelmeta["ncoordgridy"] * modelmeta["ncoordgridx"]
-                        + pl.col("coordpointnumy") * modelmeta["ncoordgridx"]
-                        + pl.col("coordpointnumx")
-                    ).alias("em_modelgridindex")
+                    for ax in ("x", "y", "z")
                 ]
+            ).with_columns(
+                em_modelgridindex=(
+                    pl.col("coordpointnumz") * modelmeta["ncoordgridy"] * modelmeta["ncoordgridx"]
+                    + pl.col("coordpointnumy") * modelmeta["ncoordgridx"]
+                    + pl.col("coordpointnumx")
+                )
             )
+
     elif modelmeta["dimensions"] == 1:
         assert dfmodel is not None, "dfmodel must be provided for 1D models to set em_modelgridindex"
         velbins = (dfmodel.select("vel_r_max_kmps").lazy().collect()["vel_r_max_kmps"] * 1000.0).to_list()
         dfpackets = dfpackets.with_columns(
-            (
+            em_modelgridindex=(
                 pl.col("emission_velocity")
                 .cut(breaks=list(velbins), labels=[str(x) for x in range(-1, len(velbins))])
                 .cast(str)
                 .cast(pl.Int32)
-            ).alias("em_modelgridindex")
+            )
         )
 
     return dfpackets
 
 
-def readfile_text(packetsfile: Path | str, modelpath: Path = Path()) -> pl.DataFrame:
-    """Read a packets*.out(.xz/.zstd) space-separated text file into a polars DataFrame."""
-    print(f"Reading {packetsfile}")
-    column_names: list[str] | None = None
-    try:
-        fpackets = at.zopen(packetsfile, mode="rt", encoding="utf-8")
-
-        datastartpos = fpackets.tell()  # will be updated if this was actually the start of a header
+def get_packets_text_columns(packetsfile: Path | str, modelpath: Path = Path()) -> list[str]:
+    with at.zopen(packetsfile, mode="rt", encoding="utf-8") as fpackets:
         firstline = fpackets.readline()
 
         if firstline.lstrip().startswith("#"):
             column_names = firstline.lstrip("#").split()
             assert column_names is not None
 
             # get the column count from the first data line to check header matched
-            datastartpos = fpackets.tell()
             dataline = fpackets.readline()
             inputcolumncount = len(dataline.split())
             assert inputcolumncount == len(column_names)
         else:
             inputcolumncount = len(firstline.split())
             column_names = get_column_names_artiscode(modelpath)
             if column_names:  # found them in the artis code files
                 assert len(column_names) == inputcolumncount
 
             else:  # infer from column positions
                 assert len(columns_full) >= inputcolumncount
                 column_names = columns_full[:inputcolumncount]
 
-        fpackets.seek(datastartpos)  # go to first data line
+    return column_names
 
-    except gzip.BadGzipFile:
-        print(f"\nBad Gzip File: {packetsfile}")
-        raise
 
+def readfile(
+    packetsfile: Path | str,
+    packet_type: str | None = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
+) -> pd.DataFrame:
+    """Read a packet file into a Pandas DataFrame."""
+    dfpackets = readfile_text(packetsfile, column_names=get_packets_text_columns(packetsfile))
+
+    if escape_type is not None:
+        assert packet_type is None or packet_type == "TYPE_ESCAPE"
+        dfpackets = dfpackets.filter(
+            (pl.col("type_id") == type_ids["TYPE_ESCAPE"]) & (pl.col("escape_type_id") == type_ids[escape_type])
+        )
+    elif packet_type is not None and packet_type:
+        dfpackets = dfpackets.filter(pl.col("type_id") == type_ids[packet_type])
+
+    return dfpackets.to_pandas(use_pyarrow_extension_array=True)
+
+
+def readfile_text(
+    packetsfiletext: Path | str,
+    column_names: list[str],
+) -> pl.DataFrame:
+    """Read a packets*.out(.xz/.zstd) space-separated text file into a polars DataFrame."""
+    packetsfiletext = Path(packetsfiletext)
+    print(f"  reading {packetsfiletext}")
     dtype_overrides = {
         "absorption_freq": pl.Float32,
         "absorption_type": pl.Int32,
         "absorptiondirx": pl.Float32,
         "absorptiondiry": pl.Float32,
         "absorptiondirz": pl.Float32,
         "e_cmf": pl.Float64,
@@ -360,193 +356,257 @@
         "trueem_time": pl.Float32,
         "trueemissiontype": pl.Int32,
         "type_id": pl.Int32,
     }
 
     try:
         dfpackets = pl.read_csv(
-            at.zopenpl(packetsfile),
+            at.zopenpl(packetsfiletext),
             separator=" ",
             has_header=False,
             comment_prefix="#",
             new_columns=column_names,
             infer_schema_length=20000,
             dtypes=dtype_overrides,
         )
 
     except Exception:
-        print(f"Error occured in file {packetsfile}")
+        print(f"Error occured in file {packetsfiletext}")
         raise
 
-    dfpackets = dfpackets.drop(["next_trans", "last_cross"])
+    mpirank = int(packetsfiletext.name.split("_")[-1].split(".")[0])
+    dfpackets = dfpackets.drop(["next_trans", "last_cross"]).with_columns(mpirank=pl.lit(mpirank, dtype=pl.Int32))
 
     # drop last column of nulls (caused by trailing space on each line)
     if dfpackets[dfpackets.columns[-1]].is_null().all():
         dfpackets = dfpackets.drop(dfpackets.columns[-1])
 
-    if "true_emission_velocity" in dfpackets.columns:
-        # some packets don't have this set, which confused read_csv to mark it as str
-        dfpackets = dfpackets.with_columns([pl.col("true_emission_velocity").cast(pl.Float32)])
-
     if "originated_from_positron" in dfpackets.columns:
         dfpackets = dfpackets.with_columns([pl.col("originated_from_positron").cast(pl.Boolean)])
 
     # Luke: packet energies in ergs can be huge (>1e39) which is too large for Float32
     return dfpackets.with_columns(
         [pl.col(pl.Int64).cast(pl.Int32), pl.col(pl.Float64).exclude(["e_rf", "e_cmf"]).cast(pl.Float32)]
     )
 
 
-def readfile(
-    packetsfile: Path | str,
-    packet_type: str | None = None,
-    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
-    use_pyarrow_extension_array=True,
-) -> pd.DataFrame:
-    """Read a packet file into a Pandas DataFrame."""
-    dfpackets = pl.read_parquet(packetsfile)
+def read_virtual_packets_text_file(vpacketsfiletext: Path | str, column_names: list[str]) -> pl.DataFrame:
+    vpacketsfiletext = Path(vpacketsfiletext)
+    mpirank = int(vpacketsfiletext.name.split("_")[-1].split(".")[0])
+
+    return pl.read_csv(
+        vpacketsfiletext,
+        separator=" ",
+        has_header=False,
+        comment_prefix="#",
+        new_columns=column_names,
+        dtypes={
+            "emissiontype": pl.Int32,
+            "trueemissiontype": pl.Int32,
+            "absorption_type": pl.Int32,
+            "absorption_freq": pl.Float64,
+        }
+        | {col: pl.Float64 for col in column_names if col.endswith("_nu_rf") or "_e_rf" in col}
+        | {col: pl.Float32 for col in column_names if col.endswith("_t_arrive_d")},
+    ).with_columns(mpirank=pl.lit(mpirank, dtype=pl.Int32))
 
-    if escape_type is not None:
-        assert packet_type is None or packet_type == "TYPE_ESCAPE"
-        dfpackets = dfpackets.filter(
-            (pl.col("type_id") == type_ids["TYPE_ESCAPE"]) & (pl.col("escape_type_id") == type_ids[escape_type])
+
+def get_packets_text_paths(modelpath: str | Path, maxpacketfiles: int | None = None) -> list[Path]:
+    """Get a list of Paths to packets*.out files."""
+    modelpath = Path(modelpath)
+    nprocs_read = at.get_nprocs(modelpath)
+    if maxpacketfiles is not None:
+        nprocs_read = min(nprocs_read, maxpacketfiles)
+
+    return [
+        at.firstexisting(
+            f"packets00_{rank:04d}.out",
+            folder=modelpath,
+            tryzipped=True,
+            search_subfolders=True,
         )
-    elif packet_type is not None and packet_type:
-        dfpackets = dfpackets.filter(pl.col("type_id") == type_ids[packet_type])
+        for rank in range(nprocs_read)
+    ]
 
-    return dfpackets.to_pandas(use_pyarrow_extension_array=use_pyarrow_extension_array)
 
+def get_vpackets_text_columns(vpacketsfiletext: Path) -> list[str]:
+    firstline = at.zopen(vpacketsfiletext, mode="rt", encoding="utf-8").readline()
 
-def convert_text_to_parquet(
-    packetsfiletext: Path | str,
+    assert firstline.lstrip().startswith("#")
+    return firstline.lstrip("#").split()
+
+
+def get_rankbatch_parquetfile(
+    modelpath: Path | str, batch_mpiranks: t.Sequence[int], batchindex: int, virtual: bool
 ) -> Path:
-    packetsfiletext = Path(packetsfiletext)
-    packetsfileparquet = at.stripallsuffixes(packetsfiletext).with_suffix(".out.parquet")
+    """Get the path to a parquet file containing packets for a specific batch of MPI ranks. If the file does not exists or is outdated, generate it first from the text files."""
+    modelpath = Path(modelpath)
+    strpacket = "vpackets" if virtual else "packets"
+    packetdir = Path(modelpath, strpacket)
+    packetdir.mkdir(exist_ok=True, parents=True)
 
-    dfpackets = readfile_text(packetsfiletext).lazy()
-    dfpackets = dfpackets.with_columns(
-        [
-            (
-                (
-                    pl.col("escape_time")
-                    - (
-                        pl.col("posx") * pl.col("dirx")
-                        + pl.col("posy") * pl.col("diry")
-                        + pl.col("posz") * pl.col("dirz")
-                    )
-                    / 29979245800.0
-                )
-                / 86400.0
-            )
-            .cast(pl.Float32)
-            .alias("t_arrive_d"),
-        ]
+    parquetfilepath = (
+        packetdir / f"{strpacket}batch{batchindex:02d}_{batch_mpiranks[0]:04d}_{batch_mpiranks[-1]:04d}.out.parquet.tmp"
     )
 
-    syn_dir = next(
-        (at.get_syn_dir(p) for p in packetsfiletext.parents if Path(p, "syn_dir.txt").is_file()),
-        (0.0, 0.0, 1.0),
-    )
-    dfpackets = add_packet_directions_lazypolars(dfpackets, syn_dir)
-    dfpackets = bin_packet_directions_lazypolars(dfpackets)
+    # time when the schema for the parquet files last change (e.g. new computed columns added or data types changed)
+    time_parquetschemachange = (2024, 4, 23, 9, 0, 0)
+    t_lastschemachange = calendar.timegm(time_parquetschemachange)
 
-    # print(f"Saving {packetsfileparquet}")
-    dfpackets = dfpackets.sort(by=["type_id", "escape_type_id", "t_arrive_d"])
-    dfpackets.collect().write_parquet(packetsfileparquet, compression="zstd", statistics=True, compression_level=6)
+    text_filenames = [
+        (f"vpackets_{rank:04d}.out" if virtual else f"packets00_{rank:04d}.out") for rank in batch_mpiranks
+    ]
+
+    conversion_needed = True
+    if parquetfilepath.is_file():
+        parquet_mtime = parquetfilepath.stat().st_mtime
+        last_textfile_mtime = (
+            at.firstexisting(text_filenames[-1], folder=modelpath, tryzipped=True, search_subfolders=True)
+            .stat()
+            .st_mtime
+        )
 
-    return packetsfileparquet
+        if parquet_mtime > last_textfile_mtime and parquet_mtime > t_lastschemachange:
+            conversion_needed = False
+        else:
+            print(f"  outdated file: {parquetfilepath}. Will overwrite")
 
+    if conversion_needed:
+        time_start_load = time.perf_counter()
+        print(
+            f"  generating {parquetfilepath.relative_to(modelpath.parent)}. Reading text files...", end="", flush=True
+        )
 
-def get_packetsfilepaths(
-    modelpath: str | Path, maxpacketfiles: int | None = None, printwarningsonly: bool = False
-) -> list[Path]:
-    """Get a list of Paths to parquet-formatted packets files, (which are generated from text files if needed)."""
-    nprocs = at.get_nprocs(modelpath)
+        text_file_paths = [
+            at.firstexisting(filename, folder=modelpath, tryzipped=True, search_subfolders=True)
+            for filename in text_filenames
+        ]
 
-    searchfolders = [Path(modelpath, "packets"), Path(modelpath)]
-    # in descending priority (based on speed of reading)
-    suffix_priority = [".out.zst", ".out.zst", ".out", ".out.gz", ".out.xz"]
-    t_lastschemachange = calendar.timegm(time_parquetschemachange)
+        column_names = (
+            get_vpackets_text_columns(text_file_paths[0])
+            if virtual
+            else get_packets_text_columns(text_file_paths[0], modelpath=modelpath)
+        )
+
+        ftextreader = read_virtual_packets_text_file if virtual else readfile_text
+
+        pldf_batch = pl.concat(
+            (ftextreader(text_file_path, column_names=column_names).lazy() for text_file_path in text_file_paths),
+            how="vertical",
+        )
 
-    parquetpacketsfiles = []
-    parquetrequiredfiles = []
+        assert pldf_batch is not None
 
-    for rank in range(nprocs + 1):
-        name_nosuffix = f"packets00_{rank:04d}"
-        found_rank = False
-
-        for folderpath in searchfolders:
-            filepath = (folderpath / name_nosuffix).with_suffix(".out.parquet")
-            if filepath.is_file():
-                if filepath.stat().st_mtime < t_lastschemachange:
-                    filepath.unlink(missing_ok=True)
-                    print(f"{filepath} is out of date.")
-                else:
-                    if rank < nprocs:
-                        parquetpacketsfiles.append(filepath)
-                    found_rank = True
-
-        if not found_rank:
-            for suffix in suffix_priority:
-                for folderpath in searchfolders:
-                    filepath = (folderpath / name_nosuffix).with_suffix(suffix)
-                    if filepath.is_file():
-                        if rank < nprocs:
-                            parquetrequiredfiles.append(filepath)
-                        found_rank = True
-                        break
-
-                if found_rank:
-                    break
-
-        if found_rank and rank >= nprocs:
-            print(f"WARNING: nprocs is {nprocs} but file {filepath} exists")
-        elif not found_rank and rank < nprocs:
-            print(f"WARNING: packets file for rank {rank} was not found.")
-
-        if maxpacketfiles is not None and (len(parquetpacketsfiles) + len(parquetrequiredfiles)) >= maxpacketfiles:
-            break
-
-    if len(parquetrequiredfiles) >= 20 and at.get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
-            convertedparquetpacketsfiles = pool.map(convert_text_to_parquet, parquetrequiredfiles)
-            pool.close()
-            pool.join()
+        if virtual:
+            pldf_batch = pldf_batch.sort(by=["dir0_t_arrive_d"])
+        else:
+            pldf_batch = pldf_batch.with_columns(
+                t_arrive_d=(
+                    (
+                        pl.col("escape_time")
+                        - (
+                            pl.col("posx") * pl.col("dirx")
+                            + pl.col("posy") * pl.col("diry")
+                            + pl.col("posz") * pl.col("dirz")
+                        )
+                        / 29979245800.0
+                    )
+                    / 86400.0
+                ).cast(pl.Float32),
+            ).sort(by=["type_id", "escape_type_id", "t_arrive_d"])
+
+            syn_dir = at.get_syn_dir(modelpath)
+
+            pldf_batch = add_packet_directions_lazypolars(pldf_batch, syn_dir)
+            pldf_batch = bin_packet_directions_lazypolars(pldf_batch)
+
+        print(f"took {time.perf_counter() - time_start_load:.1f} seconds. Writing parquet file...", end="", flush=True)
+        time_start_write = time.perf_counter()
+        pldf_batch.sink_parquet(parquetfilepath, compression="zstd", statistics=True, compression_level=8)
+        print(f"took {time.perf_counter() - time_start_write:.1f} seconds")
     else:
-        convertedparquetpacketsfiles = [convert_text_to_parquet(p) for p in parquetrequiredfiles]
+        print(f"  scanning {parquetfilepath.relative_to(modelpath)}")
+
+    return parquetfilepath
+
+
+def get_packets_batch_parquet_paths(
+    modelpath: str | Path, maxpacketfiles: int | None = None, printwarningsonly: bool = False, virtual: bool = False
+) -> tuple[int, list[Path]]:
+    """Get a list of Paths to parquet-formatted packets files, (which are generated from text files if needed)."""
+    nprocs = at.get_nprocs(modelpath)
 
-    parquetpacketsfiles += list(convertedparquetpacketsfiles)
+    mpirank_groups_all = list(enumerate(at.misc.batched(range(nprocs), 100)))
+    mpirank_groups = [
+        (batchindex, batch_mpiranks)
+        for batchindex, batch_mpiranks in mpirank_groups_all
+        if maxpacketfiles is None or batch_mpiranks[-1] < maxpacketfiles
+    ]
+
+    if not mpirank_groups:
+        msg = f"No packets batches selected. Set maxpacketfiles to at least {mpirank_groups_all[0][1][-1] + 1}"
+        raise ValueError(msg)
 
     if not printwarningsonly:
         if maxpacketfiles is not None and nprocs > maxpacketfiles:
-            print(f"Reading from the first {maxpacketfiles} of {nprocs} packets files")
+            nprocs_read = mpirank_groups[-1][1][-1] + 1
+            print(f"Reading packets from the first {nprocs_read} of {nprocs} ranks")
         else:
-            print(f"Reading from {len(parquetpacketsfiles)} packets files")
+            print(f"Reading packets from {nprocs} ranks")
+
+    parquetpacketsfiles = [
+        get_rankbatch_parquetfile(modelpath, batch_mpiranks=batch_mpiranks, batchindex=batchindex, virtual=virtual)
+        for batchindex, batch_mpiranks in mpirank_groups
+    ]
+    assert bool(parquetpacketsfiles)
+    nprocs_read = sum(len(batch_mpiranks) for _, batch_mpiranks in mpirank_groups)
+    return nprocs_read, parquetpacketsfiles
+
+
+def get_virtual_packets_pl(modelpath: str | Path, maxpacketfiles: int | None = None) -> tuple[int, pl.LazyFrame]:
+    nprocs_read, vpacketparquetfiles = get_packets_batch_parquet_paths(
+        modelpath, maxpacketfiles=maxpacketfiles, virtual=True
+    )
+
+    nbatches_read = len(vpacketparquetfiles)
+    packetsdatasize_gb = nbatches_read * Path(vpacketparquetfiles[0]).stat().st_size / 1024 / 1024 / 1024
+    print(f"  data size is {packetsdatasize_gb:.1f} GB ({nbatches_read} * size of {vpacketparquetfiles[0].parts[-1]})")
+
+    # add some extra columns to imitate the real packets
+    dfpackets = pl.scan_parquet(vpacketparquetfiles).with_columns(
+        type_id=type_ids["TYPE_ESCAPE"], escape_type_id=type_ids["TYPE_RPKT"]
+    )
+
+    npkts_total = dfpackets.select(pl.count("dir0_t_arrive_d")).collect().item(0, 0)
+    print(f"  files contain {npkts_total:.2e} virtual packet events (shared among directions and opacity choices)")
 
-    return parquetpacketsfiles
+    return nprocs_read, dfpackets
 
 
 def get_packets_pl(
     modelpath: str | Path,
     maxpacketfiles: int | None = None,
     packet_type: str | None = None,
     escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
 ) -> tuple[int, pl.LazyFrame]:
     if escape_type is not None:
         assert packet_type in {None, "TYPE_ESCAPE"}
         if packet_type is None:
             packet_type = "TYPE_ESCAPE"
 
-    packetsfiles = get_packetsfilepaths(modelpath, maxpacketfiles)
+    nprocs_read, packetsparquetfiles = get_packets_batch_parquet_paths(modelpath, maxpacketfiles)
 
-    nprocs_read = len(packetsfiles)
-    packetsdatasize_gb = nprocs_read * Path(packetsfiles[0]).stat().st_size / 1024 / 1024 / 1024
-    print(f" data size is {packetsdatasize_gb:.1f} GB ({nprocs_read} * size of {packetsfiles[0].parts[-1]})")
+    nbatches_read = len(packetsparquetfiles)
+    packetsdatasize_gb = nbatches_read * Path(packetsparquetfiles[0]).stat().st_size / 1024 / 1024 / 1024
+    print(f"  data size is {packetsdatasize_gb:.1f} GB ({nbatches_read} * size of {packetsparquetfiles[0].parts[-1]})")
 
-    pldfpackets = pl.scan_parquet(packetsfiles)
+    pldfpackets = pl.scan_parquet(packetsparquetfiles)
+
+    npkts_total = pldfpackets.select(pl.count("e_rf")).collect().item(0, 0)
+    print(f"  files contain {npkts_total:.2e} packets")
 
     if escape_type is not None:
         assert packet_type is None or packet_type == "TYPE_ESCAPE"
         pldfpackets = pldfpackets.filter(
             (pl.col("type_id") == type_ids["TYPE_ESCAPE"]) & (pl.col("escape_type_id") == type_ids[escape_type])
         )
     elif packet_type is not None and packet_type:
@@ -735,15 +795,15 @@
     # timestep = 63 # 82 73 #63 #54 46 #27
     # print([(ts, time) for ts, time in enumerate(timeminarray)])
     if em_time:
         print("Binning by packet emission time")
     else:
         print("Binning by packet arrival time")
 
-    packetsfiles = at.packets.get_packetsfilepaths(modelpath)
+    packetsfiles = at.packets.get_packets_batch_parquet_paths(modelpath)
 
     emission_position3d = [[], [], []]
     e_rf = []
     e_cmf = []
 
     only_packets_0_scatters = False
     for packetsfile in packetsfiles:
@@ -827,16 +887,15 @@
     # print(grid_Te.shape)
     return grid_3d, x, y, z
 
 
 def get_mean_packet_emission_velocity_per_ts(
     modelpath, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT", maxpacketfiles=None, escape_angles=None
 ) -> pd.DataFrame:
-    packetsfiles = at.packets.get_packetsfilepaths(modelpath, maxpacketfiles=maxpacketfiles)
-    nprocs_read = len(packetsfiles)
+    nprocs_read, packetsfiles = at.packets.get_packets_batch_parquet_paths(modelpath, maxpacketfiles=maxpacketfiles)
     assert nprocs_read > 0
 
     timearray = at.get_timestep_times(modelpath=modelpath, loc="mid")
     arr_timedelta = at.get_timestep_times(modelpath=modelpath, loc="delta")
     timearrayplusend = np.concatenate([timearray, [timearray[-1] + arr_timedelta[-1]]])
 
     dfpackets_escape_velocity_and_arrive_time = pd.DataFrame()
@@ -876,30 +935,30 @@
 
 def bin_and_sum(
     df: pl.DataFrame | pl.LazyFrame,
     bincol: str,
     bins: list[float | int],
     sumcols: list[str] | None = None,
     getcounts: bool = False,
-) -> pl.DataFrame:
+) -> pl.LazyFrame:
     """Bins is a list of lower edges, and the final upper edge."""
     # Polars method
 
-    df = df.with_columns(
-        (
-            pl.col(bincol)
-            .cut(breaks=list(bins), labels=[str(x) for x in range(-1, len(bins))])
-            .cast(str)
-            .cast(pl.Int32)
-        ).alias(f"{bincol}_bin")
+    df = df.lazy().with_columns(
+        (pl.col(bincol).cut(breaks=bins, labels=[str(x) for x in range(-1, len(bins))])).alias(f"{bincol}_bin")
     )
 
     aggs = [pl.col(col).sum().alias(col + "_sum") for col in sumcols] if sumcols is not None else []
 
     if getcounts:
         aggs.append(pl.col(bincol).count().alias("count"))
 
-    wlbins = df.group_by(f"{bincol}_bin").agg(aggs).lazy().collect()
+    wlbins = df.group_by(f"{bincol}_bin").agg(aggs).with_columns(pl.col(f"{bincol}_bin").cast(pl.Int32))
 
     # now we will include the empty bins
-    dfout = pl.DataFrame(pl.Series(name=f"{bincol}_bin", values=np.arange(0, len(bins) - 1), dtype=pl.Int32))
-    return dfout.join(wlbins, how="left", on=f"{bincol}_bin").fill_null(0)
+    return (
+        pl.DataFrame({f"{bincol}_bin": range(len(bins) - 1)}, schema={f"{bincol}_bin": pl.Int32})
+        .lazy()
+        .join(wlbins, how="left", on=f"{bincol}_bin")
+        .fill_null(0)
+        .sort(by=f"{bincol}_bin")
+    )
```

### Comparing `artistools-2024.2.22.2/artistools/packets/packetsplots.py` & `artistools-2024.4.23/artistools/packets/packetsplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     em_time = True  # False for arrive time
 
     hist = at.packets.make_3d_histogram_from_packets(
         modelpath, timestep_min=timestep_min, timestep_max=timestep_max, em_time=em_time
     )
 
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
-    vmax_cms = vmax_cms / CLIGHT
+    vmax_cms /= CLIGHT
 
     # # Don't plot empty cells
     # i = 0
     # for z in range(0, grid):
     #     for y in range(0, grid):
     #         for x in range(0, grid):
     #             if modeldata["rho"][i] == 0.0:
@@ -169,16 +169,16 @@
     hist, bin_edges = np.histogram(
         dfpackets_selected.select("emission_velocity").collect() / 2.99792458e10,
         range=(0.0, 0.7),
         bins=28,
         weights=weights,
     )
     hist = hist / nprocs_read / (timemaxarray[timestep_max] - timeminarray[timestep_min])  # erg/day
-    hist = hist * (u.erg / u.day).to("erg/s")
-    hist = hist / 1e40
+    hist *= (u.erg / u.day).to("erg/s")
+    hist /= 1e40
     width = np.diff(bin_edges)
     center = (bin_edges[:-1] + bin_edges[1:]) / 2
 
     ax.bar(center, hist, align="center", width=width, linewidth=2, fill=True)
 
     ax.set_xticks(bin_edges[::4])
     ax.set_xlabel("Velocity [c]")
```

### Comparing `artistools-2024.2.22.2/artistools/packets/test_packets.py` & `artistools-2024.4.23/artistools/packets/test_packets.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,7 +60,16 @@
     )
 
     for row in pddfpackets.itertuples(index=True):
         assert np.isclose(row.costheta_defined, row.costheta, rtol=1e-4, atol=1e-4)
         assert np.isclose(row.phi_defined, row.phi, rtol=1e-4, atol=1e-4)
 
         assert np.isclose(testdirections.item(row[0], "dirbin"), row.dirbin, rtol=1e-4, atol=1e-4)
+
+
+def test_get_virtual_packets_pl():
+    nprocs, dfvpkt = at.packets.get_virtual_packets_pl(
+        modelpath=at.get_config()["path_testdata"] / "vpktcontrib", maxpacketfiles=2
+    )
+
+    npkts_total = dfvpkt.select(pl.count("dir0_t_arrive_d")).collect().item(0, 0)
+    assert npkts_total == 13783
```

### Comparing `artistools-2024.2.22.2/artistools/plotspherical.py` & `artistools-2024.4.23/artistools/plotspherical.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,24 @@
     maxpacketfiles: int | None = None,
     atomic_number: int | None = None,
     ion_stage: int | None = None,
     gaussian_sigma: int | None = None,
     plotvars: list[str] | None = None,
     figscale: float = 1.0,
     cmap: str | None = None,
-) -> tuple[plt.Figure, t.Any, float, float]:
+) -> tuple[plt.Figure, t.Any, float, float, str]:
+    condition = ""
     if plotvars is None:
         plotvars = ["luminosity", "emvelocityoverc", "emlosvelocityoverc"]
 
     _, tmin_d_valid, tmax_d_valid = at.get_escaped_arrivalrange(modelpath)
     if tmin_d_valid is None or tmax_d_valid is None:
         print("WARNING! The observer never gets light from the entire ejecta. Plotting all packets anyway")
         timemindays, timemaxdays = (
-            dfpackets.select(pl.col("t_arrive_d").min().alias("tmin"), pl.col("t_arrive_d").max().alias("tmax"))
-            .collect()
-            .to_numpy()[0]
+            dfpackets.select(tmin=pl.col("t_arrive_d").min(), tmax=pl.col("t_arrive_d").max()).collect().to_numpy()[0]
         )
     else:
         if timemindays is None:
             print(f"setting timemindays to start of valid observable range {tmin_d_valid:.2f} d")
             timemindays = tmin_d_valid
         elif timemindays < tmin_d_valid:
             print(
@@ -78,22 +77,30 @@
         dfpackets=dfpackets, nphibins=nphibins, ncosthetabins=ncosthetabins, phibintype="phiascending"
     )
 
     # for figuring out where the axes are on the plot, make a cut
     # dfpackets = dfpackets.filter(pl.col("dirz") > 0.9)
 
     aggs = []
+    if nnelement_vars := [var for var in plotvars if var.startswith("nnelement_")]:
+        aggs += [
+            ((pl.col(var) * pl.col("e_rf")).mean() / pl.col("e_rf").mean() / 29979245800).alias(var)
+            for var in nnelement_vars
+        ]
 
     if "emvelocityoverc" in plotvars:
         aggs.append(
             ((pl.col("emission_velocity") * pl.col("e_rf")).mean() / pl.col("e_rf").mean() / 29979245800).alias(
                 "emvelocityoverc"
             )
         )
 
+    if "emvelocityoverc_sigma" in plotvars:
+        aggs.append(((pl.col("emission_velocity") / 29979245800).std()).alias("emvelocityoverc_sigma"))
+
     if "emlosvelocityoverc" in plotvars:
         aggs.append(
             (
                 (pl.col("emission_velocity_lineofsight") * pl.col("e_rf")).mean() / pl.col("e_rf").mean() / 29979245800
             ).alias("emlosvelocityoverc")
         )
 
@@ -101,66 +108,81 @@
         solidanglefactor = nphibins * ncosthetabins
         aggs.append(
             (pl.col("e_rf").sum() / nprocs_read * solidanglefactor / (timemaxdays - timemindays) / 86400).alias(
                 "luminosity"
             )
         )
 
-    if "temperature" in plotvars:
+    if "temperature" in plotvars or "temperature_sigma" in plotvars or nnelement_vars:
         timebins = [
             *at.get_timestep_times(modelpath, loc="start") * 86400.0,
             at.get_timestep_times(modelpath, loc="end")[-1] * 86400.0,
         ]
         dfpackets = dfpackets.with_columns(
             (
                 pl.col("em_time")
-                .cut(breaks=list(timebins), labels=[str(x) for x in range(-1, len(timebins))])
+                .cut(breaks=timebins, labels=[str(x) for x in range(-1, len(timebins))])
                 .cast(str)
                 .cast(pl.Int32)
             ).alias("em_timestep")
         )
 
         assert dfestimators is not None
         dfestimators = (
-            dfestimators.select(["timestep", "modelgridindex", "TR"])
+            dfestimators.select(["timestep", "modelgridindex", "TR", *nnelement_vars])
             .drop_nulls()
-            .rename({"timestep": "em_timestep", "modelgridindex": "em_modelgridindex", "TR": "em_TR"})
+            .rename({"timestep": "em_timestep", "modelgridindex": "em_modelgridindex"})
         )
         dfpackets = dfpackets.join(dfestimators, on=["em_timestep", "em_modelgridindex"], how="left")
-        aggs.append(((pl.col("em_TR") * pl.col("e_rf")).mean() / pl.col("e_rf").mean()).alias("temperature"))
+
+    if "temperature" in plotvars:
+        aggs.append(((pl.col("TR") * pl.col("e_rf")).mean() / pl.col("e_rf").mean()).alias("temperature"))
+
+    if "temperature_sigma" in plotvars:
+        aggs.append((pl.col("TR").std()).alias("temperature_sigma"))
 
     if atomic_number is not None or ion_stage is not None:
         dflinelist = at.get_linelist_pldf(modelpath)
+        elem_cond = f"Z={atomic_number} {at.get_elsymbol(atomic_number)}" if atomic_number is not None else ""
+        ion_stage_cond = f"ion stage {ion_stage}" if ion_stage is not None else ""
+        condition = f"last emitted/absorbed by {elem_cond} {ion_stage_cond}"
+        print(f"Including only packets {condition}")
         if atomic_number is not None:
-            print(f"Including only packets emitted by Z={atomic_number} {at.get_elsymbol(atomic_number)}")
             dflinelist = dflinelist.filter(pl.col("atomic_number") == atomic_number)
         if ion_stage is not None:
-            print(f"Including only packets emitted by ionisation stage {ion_stage}")
             dflinelist = dflinelist.filter(pl.col("ion_stage") == ion_stage)
 
         selected_emtypes = dflinelist.select("lineindex").collect().get_column("lineindex")
-        dfpackets = dfpackets.filter(pl.col("emissiontype").is_in(selected_emtypes))
+        dfpackets = dfpackets.filter(
+            pl.col("emissiontype").is_in(selected_emtypes) | pl.col("absorption_type").is_in(selected_emtypes)
+        )
 
     aggs.append(pl.len().alias("count"))
-    dfpackets = dfpackets.group_by(["costhetabin", "phibin"]).agg(aggs)
-    dfpackets = dfpackets.select(["costhetabin", "phibin", "count", *plotvars])
+    dfpackets = (
+        dfpackets.group_by(["costhetabin", "phibin"]).agg(aggs).select(["costhetabin", "phibin", "count", *plotvars])
+    )
 
     ndirbins = nphibins * ncosthetabins
-    alldirbins = pl.DataFrame(
-        {"phibin": (d % nphibins for d in range(ndirbins)), "costhetabin": (d // nphibins for d in range(ndirbins))}
-    ).with_columns(pl.all().cast(pl.Int32))
     alldirbins = (
-        alldirbins.join(
-            dfpackets.collect(),
+        pl.DataFrame(
+            {
+                "phibin": (d % nphibins for d in range(ndirbins)),
+                "costhetabin": (d // nphibins for d in range(ndirbins)),
+            },
+            schema={"phibin": pl.Int32, "costhetabin": pl.Int32},
+        )
+        .lazy()
+        .join(
+            dfpackets,
             how="left",
             on=["costhetabin", "phibin"],
         )
         .fill_null(0)
         .sort(["costhetabin", "phibin"])
-    )
+    ).collect()
 
     print(f'packets plotted: {alldirbins.select("count").sum().item(0, 0):.1e}')
 
     # these phi and theta angle ranges are defined differently to artis
     phigrid = np.linspace(-np.pi, np.pi, nphibins + 1, endpoint=True, dtype=np.float64)
 
     # costhetabin zero is (0,0,-1) so theta angle
@@ -169,23 +191,24 @@
     thetagrid = np.pi / 2 - np.arccos(costhetagrid)
 
     meshgrid_phi, meshgrid_theta = np.meshgrid(phigrid, thetagrid)
 
     fig, axes = plt.subplots(
         len(plotvars),
         1,
-        figsize=(figscale * at.get_config()["figwidth"], 3.2 * len(plotvars)),
+        figsize=(figscale * at.get_config()["figwidth"], 3.5 * len(plotvars)),
         subplot_kw={"projection": "mollweide"},
-        # tight_layout={"pad": 0, "w_pad": 0, "h_pad": 5.0},
+        layout="constrained",
         gridspec_kw={"wspace": 0.0, "hspace": 0.0},
     )
 
     if len(plotvars) == 1:
         axes = (axes,)
 
+    # for ax, axcbar, plotvar in zip(axes[::2], axes[1::2], plotvars):
     for ax, plotvar in zip(axes, plotvars):
         data = alldirbins.get_column(plotvar).to_numpy().reshape((ncosthetabins, nphibins))
 
         if gaussian_sigma is not None and gaussian_sigma > 0:
             import scipy.ndimage
 
             sigma_bins = gaussian_sigma / 360 * nphibins
@@ -194,22 +217,30 @@
         colormesh = ax.pcolormesh(meshgrid_phi, meshgrid_theta, data, rasterized=True, cmap=cmap)
 
         match plotvar:
             case "emlosvelocityoverc":
                 colorbartitle = r"Mean line of sight velocity [c]"
             case "emvelocityoverc":
                 colorbartitle = r"Last interaction ejecta velocity [c]"
+            case "emvelocityoverc_sigma":
+                colorbartitle = r"Last interaction ejecta velocity standard deviation [c]"
             case "luminosity":
                 colorbartitle = r"Radiant intensity $\cdot\,4π$ [{}erg/s]"
             case "temperature":
                 colorbartitle = r"Temperature [{}K]"
+            case "temperature_sigma":
+                colorbartitle = r"Temperature standard deviation [{}K]"
+            case s if s.startswith("nnelement_"):
+                elemsymbol = s.split("_", maxsplit=1)[1]
+                colorbartitle = f"Number density of {elemsymbol} " + r"[{}/cm³]"
             case _:
-                raise AssertionError
+                msg = f"Unknown plotvar {plotvar}"
+                raise AssertionError(msg)
 
-        cbar = fig.colorbar(colormesh, ax=ax, location="bottom", pad=0.2)
+        cbar = fig.colorbar(colormesh, location="bottom", pad=0.03, ax=ax, shrink=0.95)
         cbar.outline.set_linewidth(0)  # type: ignore[operator]
         cbar.ax.tick_params(axis="both", direction="out")
         cbar.ax.xaxis.set_ticks_position("top")
         # cbar.ax.set_title(colorbartitle)
         cbar.ax.set_xlabel(colorbartitle)
         cbar.ax.xaxis.set_label_position("top")
         if r"{}" in colorbartitle:
@@ -227,15 +258,15 @@
         # ax.set_xticks(ticks=xticks_deg / 180 * np.pi - np.pi, labels=[rf"${deg:.0f}\degree$" for deg in xticks_deg])
 
         # yticks_deg = np.linspace(0, 180, 7)
         # ax.set_yticks(
         #     ticks=-yticks_deg / 180 * np.pi + np.pi / 2.0, labels=[rf"${deg:.0f}\degree$" for deg in yticks_deg]
         # )
 
-    return fig, axes, timemindays, timemaxdays
+    return fig, axes, timemindays, timemaxdays, condition
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "-modelpath",
         type=Path,
         default=Path(),
@@ -325,15 +356,15 @@
         outformat = args.format or "pdf"
 
     outputfilenames = []
     for tstart, tend, label in time_ranges:
         if tstart is not None and tend is not None:
             print(f"Plotting spherical map for {tstart:.2f}-{tend:.2f} days {label}")
         # tstart and tend are requested, but the actual plotted time range may be different
-        fig, axes, timemindays, timemaxdays = plot_spherical(
+        fig, axes, timemindays, timemaxdays, condition = plot_spherical(
             modelpath=args.modelpath,
             dfpackets=dfpackets,
             dfestimators=dfestimators,
             dfmodel=dfmodel,
             modelmeta=modelmeta,
             nprocs_read=nprocs_read,
             timemindays=tstart,
@@ -345,24 +376,27 @@
             atomic_number=args.atomic_number,
             ion_stage=args.ion_stage,
             plotvars=args.plotvars,
             cmap=args.cmap,
             figscale=args.figscale,
         )
 
-        axes[0].set_title(f"{timemindays:.2f}-{timemaxdays:.2f} days")
+        axes[0].set_title(
+            f"{timemindays:.2f}-{timemaxdays:.2f} days{f' ({condition})' if condition else ''}",
+            loc="left",
+        )
 
         defaultfilename = "plotspherical_{timemindays:.2f}-{timemaxdays:.2f}d.{outformat}"
         outfilename = str(
             args.outputfile
             if (args.outputfile and not Path(args.outputfile).is_dir() and not args.makegif)
             else Path(args.outputfile) / defaultfilename
         ).format(timemindays=timemindays, timemaxdays=timemaxdays, outformat=outformat)
 
-        fig.savefig(outfilename, format=outformat, dpi=300)
+        fig.savefig(outfilename, format=outformat, dpi=300, pad_inches=0.0)
         print(f"Saved {outfilename}")
         plt.close()
         plt.clf()
 
         outputfilenames.append(outfilename)
 
     if args.makegif:
```

### Comparing `artistools-2024.2.22.2/artistools/plottools.py` & `artistools-2024.4.23/artistools/plottools.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,10 +223,10 @@
             lim = ax.get_ylim()
             fixed, dependent = y, x
 
         low, high = calculate_new_limit(fixed, dependent, lim)
         newlow = min(newlow, low)
         newhigh = max(newhigh, high)
 
-    margin = margin * (newhigh - newlow)
+    margin *= newhigh - newlow
 
     setlim(newlow - margin, newhigh + margin)
```

### Comparing `artistools-2024.2.22.2/artistools/radfield.py` & `artistools-2024.4.23/artistools/radfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,22 +219,23 @@
     return arr_lambda, j_lambda_fitted
 
 
 def plot_line_estimators(axis, radfielddata, xmin, xmax, modelgridindex=None, timestep=None, **plotkwargs):
     """Plot the Jblue_lu values from the detailed line estimators on a spectrum."""
     ymax = -1
 
-    radfielddataselected = radfielddata.query(
-        "bin_num < -1"
-        + (" & modelgridindex==@modelgridindex" if modelgridindex else "")
-        + (" & timestep==@timestep" if timestep else "")
-    )[["nu_upper", "J_nu_avg"]]
-
-    radfielddataselected = radfielddataselected.eval("lambda_angstroms = 2.99792458e18 / nu_upper")
-    radfielddataselected = radfielddataselected.eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
+    radfielddataselected = (
+        radfielddata.query(
+            "bin_num < -1"
+            + (" & modelgridindex==@modelgridindex" if modelgridindex else "")
+            + (" & timestep==@timestep" if timestep else "")
+        )[["nu_upper", "J_nu_avg"]]
+        .eval("lambda_angstroms = 2.99792458e18 / nu_upper")
+        .eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
+    )
 
     ymax = radfielddataselected["Jb_lambda"].max()
 
     if not radfielddataselected.empty:
         axis.scatter(
             radfielddataselected["lambda_angstroms"],
             radfielddataselected["Jb_lambda"],
@@ -259,19 +260,19 @@
 
     specfilename = Path(specfilename)
     if specfilename.is_dir():
         modelpath = specfilename
     elif specfilename.is_file():
         modelpath = Path(specfilename).parent
 
-    dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep)[-1]
+    dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep)[-1].to_pandas()
     label = "Emergent spectrum"
     if scale_factor is not None:
         label += " (scaled)"
-        dfspectrum["f_lambda"] = dfspectrum["f_lambda"] * scale_factor
+        dfspectrum["f_lambda"] *= scale_factor
 
     if peak_value is not None:
         label += " (normalised)"
         dfspectrum["f_lambda"] = dfspectrum["f_lambda"] / dfspectrum["f_lambda"].max() * peak_value
 
     dfspectrum.plot(x="lambda_angstroms", y="f_lambda", ax=axis, label=label, **plotkwargs)
 
@@ -829,23 +830,24 @@
     )
 
 
 def plot_line_estimator_evolution(
     axis, radfielddata, bin_num, modelgridindex=None, timestep_min=None, timestep_max=None, **plotkwargs
 ):
     """Plot the Jblue_lu values over time for a detailed line estimators."""
-    radfielddataselected = radfielddata.query(
-        "bin_num == @bin_num"
-        + (" & modelgridindex == @modelgridindex" if modelgridindex else "")
-        + (" & timestep >= @timestep_min" if timestep_min else "")
-        + (" & timestep <= @timestep_max" if timestep_max else "")
-    )[["timestep", "nu_upper", "J_nu_avg"]]
-
-    radfielddataselected = radfielddataselected.eval("lambda_angstroms = 2.99792458e18 / nu_upper")
-    radfielddataselected = radfielddataselected.eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
+    radfielddataselected = (
+        radfielddata.query(
+            "bin_num == @bin_num"
+            + (" & modelgridindex == @modelgridindex" if modelgridindex else "")
+            + (" & timestep >= @timestep_min" if timestep_min else "")
+            + (" & timestep <= @timestep_max" if timestep_max else "")
+        )[["timestep", "nu_upper", "J_nu_avg"]]
+        .eval("lambda_angstroms = 2.99792458e18 / nu_upper")
+        .eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
+    )
 
     axis.plot(
         radfielddataselected["timestep"],
         radfielddataselected["Jb_lambda"],
         label=f"Jb_lu bin_num {bin_num}",
         **plotkwargs,
     )
@@ -867,21 +869,24 @@
             args.figscale * at.get_config()["figwidth"],
             args.figscale * at.get_config()["figwidth"] * (0.25 + nlinesplotted * 0.35),
         ),
         tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
     )
 
     timestep = at.get_timestep_of_timedays(modelpath, 330)
-    time_days = float(at.get_timestep_time(modelpath, timestep))
+    time_days = at.get_timestep_time(modelpath, timestep)
 
-    dftopestimators = radfielddataselected.query("timestep==@timestep and bin_num < -1").copy()
-    dftopestimators = dftopestimators.eval("lambda_angstroms = 2.99792458e18 / nu_upper")
-    dftopestimators = dftopestimators.eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
-    dftopestimators = dftopestimators.sort_values(by="Jb_lambda", ascending=False)
-    dftopestimators = dftopestimators.iloc[:nlinesplotted]
+    dftopestimators = (
+        radfielddataselected.query("timestep==@timestep and bin_num < -1")
+        .copy()
+        .eval("lambda_angstroms = 2.99792458e18 / nu_upper")
+        .eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
+        .sort_values(by="Jb_lambda", ascending=False)
+        .iloc[:nlinesplotted]
+    )
 
     print(f"Top estimators at timestep {timestep} t={time_days:.1f}")
     print(dftopestimators)
 
     for ax, bin_num_estimator, nu_line in zip(
         axes, dftopestimators.bin_num.to_numpy(), dftopestimators.nu_upper.to_numpy()
     ):
@@ -970,15 +975,15 @@
         if args.xaxis == "lambda"
         else Path("plotradfield_cell{modelgridindex:03d}_evolution.pdf")
     )
 
     if not args.outputfile:
         args.outputfile = defaultoutputfile
     elif args.outputfile.is_dir():
-        args.outputfile = args.outputfile / defaultoutputfile
+        args.outputfile /= defaultoutputfile
 
     modelpath = args.modelpath
 
     pdf_list = []
     modelgridindexlist = []
 
     if args.velocity >= 0.0:
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/__init__.py` & `artistools-2024.4.23/artistools/spectra/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Artistools - spectra related functions."""
+
 from artistools.spectra import plotspectra
 from artistools.spectra import writespectra
 from artistools.spectra.plotspectra import main as plot
 from artistools.spectra.spectra import get_exspec_bins
 from artistools.spectra.spectra import get_flux_contributions
 from artistools.spectra.spectra import get_flux_contributions_from_packets
 from artistools.spectra.spectra import get_from_packets
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/plotspectra.py` & `artistools-2024.4.23/artistools/spectra/plotspectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 """Artistools - spectra plotting functions."""
 
-
 import argparse
 import math
 import sys
 import typing as t
 from pathlib import Path
 
 import argcomplete
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import polars as pl
 from matplotlib import ticker
 from matplotlib.artist import Artist
 
 import artistools as at
 
 hatches = ["", "x", "-", "\\", "+", "O", ".", "", "x", "*", "\\", "+", "O", "."]  # ,
 
 
+def path_is_artis_model(filepath: str | Path) -> bool:
+    if Path(filepath).name.endswith(".out.zst"):
+        return True
+    if Path(filepath).suffix == ".out":
+        return True
+    return Path(filepath).is_dir()
+
+
 def plot_polarisation(modelpath: Path, args) -> None:
     angle = args.plotviewingangle[0]
     stokes_params = at.spectra.get_specpol_data(angle=angle, modelpath=modelpath)
     stokes_params[args.stokesparam] = stokes_params[args.stokesparam].eval("lambda_angstroms = 2.99792458e18 / nu")
 
     timearray = stokes_params[args.stokesparam].keys()[1:-1]
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
     assert args.timemin is not None
     assert args.timemax is not None
     timeavg = (args.timemin + args.timemax) / 2.0
 
     def match_closest_time(reftime):
-        return str(f"{min((float(x) for x in timearray), key=lambda x: abs(x - reftime)):.4f}")
+        return f"{min((float(x) for x in timearray), key=lambda x: abs(x - reftime)):.4f}"
 
     timeavg = match_closest_time(timeavg)
 
     filterfunc = at.get_filterfunc(args)
     if filterfunc is not None:
         print("Applying filter to ARTIS spectrum")
         stokes_params[args.stokesparam][timeavg] = filterfunc(stokes_params[args.stokesparam][timeavg])
@@ -82,15 +90,15 @@
         args.xmin = 0
     assert args.xmin < args.xmax
     assert args.ymin < args.ymax
 
     plt.ylim(args.ymin, args.ymax)
     plt.xlim(args.xmin, args.xmax)
 
-    plt.ylabel(f"{args.stokesparam}")
+    plt.ylabel(str(args.stokesparam))
     plt.xlabel(r"Wavelength ($\mathrm{{\AA}}$)")
     figname = f"plotpol_{timeavg}_days_{args.stokesparam.split('/')[0]}_{args.stokesparam.split('/')[1]}.pdf"
     plt.savefig(modelpath / figname, format="pdf")
     print(f"Saved {figname}")
 
 
 def plot_reference_spectrum(
@@ -111,26 +119,28 @@
     """
     specdata, metadata = at.spectra.get_reference_spectrum(filename)
 
     # scale to flux at required distance
     if scale_to_dist_mpc:
         print(f"Scale to {scale_to_dist_mpc} Mpc")
         assert metadata["dist_mpc"] > 0  # we must know the true distance in order to scale to some other distance
-        specdata["f_lambda"] = specdata["f_lambda"] * (metadata["dist_mpc"] / scale_to_dist_mpc) ** 2
+        specdata["f_lambda"] *= (metadata["dist_mpc"] / scale_to_dist_mpc) ** 2
 
     if "label" not in plotkwargs:
         plotkwargs["label"] = metadata.get("label", filename)
 
     if scaletoreftime is not None:
         timefactor = at.spectra.timeshift_fluxscale_co56law(scaletoreftime, float(metadata["t"]))
         print(f" Scale from time {metadata['t']} to {scaletoreftime}, factor {timefactor} using Co56 decay law")
         specdata["f_lambda"] *= timefactor
         plotkwargs["label"] += f" * {timefactor:.2f}"
+
     if "scale_factor" in metadata:
         specdata["f_lambda"] *= metadata["scale_factor"]
+
     if metadata.get("mask_telluric", False):
         print("Masking telluric regions")
         z = metadata["z"]
         bands = [(1.35e4, 1.44e4), (1.8e4, 1.94e4)]  # [Angstroms]
         for band_low_rest, band_high_rest in bands:
             band_low = band_low_rest / (1 + z)
             band_high = band_high_rest / (1 + z)
@@ -155,14 +165,15 @@
     #     print(f" downsampling to {len(specdata)} points")
     #     specdata = specdata.query("index % 3 == 0")
 
     # clamp negative values to zero
     # specdata['f_lambda'] = specdata['f_lambda'].apply(lambda x: max(0, x))
 
     if flambdafilterfunc:
+        print(" applying filter to reference spectrum")
         specdata.loc[:, "f_lambda"] = flambdafilterfunc(specdata["f_lambda"])
 
     if scale_to_peak:
         specdata["f_lambda_scaled"] = specdata["f_lambda"] / specdata["f_lambda"].max() * scale_to_peak
         ycolumnname = "f_lambda_scaled"
     else:
         ycolumnname = "f_lambda"
@@ -202,15 +213,15 @@
     plotpacketcount: bool = False,
     directionbins: list[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     usedegrees: bool = False,
     maxpacketfiles: int | None = None,
     **plotkwargs,
-) -> pd.DataFrame | None:
+) -> pl.DataFrame | None:
     """Plot an ARTIS output spectrum. The data plotted are also returned as a DataFrame."""
     modelpath = Path(modelpath)
     if Path(modelpath).is_file():  # handle e.g. modelpath = 'modelpath/spec.out'
         specfilename = Path(modelpath).parts[-1]
         print(f"WARNING: ignoring filename of {specfilename}")
         modelpath = Path(modelpath).parent
 
@@ -250,85 +261,80 @@
 
         assert args.timemin is not None
         assert args.timemax is not None
         timeavg = (args.timemin + args.timemax) / 2.0
         timedelta = (args.timemax - args.timemin) / 2
         linelabel_is_custom = linelabel is not None
         if linelabel is None:
-            linelabel = f"{modelname}" if len(modelname) < 70 else f"...{modelname[-67:]}"
+            linelabel = modelname if len(modelname) < 70 else f"...{modelname[-67:]}"
 
             if not args.hidemodeltime and not args.multispecplot:
                 # TODO: fix this for multispecplot - use args.showtime for now
                 linelabel += f" +{timeavg:.1f}d"
-            if not args.hidemodeltimerange and not args.multispecplot:
+            if not args.hidemodeltimerange and not args.multispecplot and timedelta >= 0.1:
                 linelabel += rf" ($\pm$ {timedelta:.1f}d)"
         # Luke: disabled below because line label has already been formatted with e.g. timeavg values
         # formatting for a second time makes it impossible to use curly braces in line labels (needed for LaTeX math)
         # else:
         #     linelabel = linelabel.format(**locals())
         print(
             f"====> '{linelabel}' timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d)"
         )
         print(f" modelpath {modelpath}")
 
-        viewinganglespectra: dict[int, pd.DataFrame] = {}
-
-        # have to get the spherical average "bin" if directionbins is None
-        dbins_get = list(directionbins).copy()
-        if -1 not in dbins_get:
-            dbins_get.append(-1)
+        viewinganglespectra = {}
 
         supxmin, supxmax = axis.get_xlim()
         if from_packets:
-            assert args.plotvspecpol is None
             viewinganglespectra = at.spectra.get_from_packets(
                 modelpath,
                 args.timemin,
                 args.timemax,
                 lambda_min=supxmin * 0.9,
                 lambda_max=supxmax * 1.1,
                 use_time=use_time,
                 maxpacketfiles=maxpacketfiles,
                 delta_lambda=args.deltalambda,
-                getpacketcount=plotpacketcount,
-                directionbins=dbins_get,
+                directionbins=directionbins,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
-                fnufilterfunc=filterfunc,
+                fluxfilterfunc=filterfunc,
+                directionbins_are_vpkt_observers=args.plotvspecpol is not None,
             )
+
         elif args.plotvspecpol is not None:
             # read virtual packet files (after running plotartisspectrum --makevspecpol)
             vpkt_config = at.get_vpkt_config(modelpath)
             if vpkt_config["time_limits_enabled"] and (
                 args.timemin < vpkt_config["initial_time"] or args.timemax > vpkt_config["final_time"]
             ):
                 print(
                     f"Timestep out of range of virtual packets: start time {vpkt_config['initial_time']} days "
                     f"end time {vpkt_config['final_time']} days"
                 )
                 sys.exit(1)
 
             viewinganglespectra = {
-                dirbin: at.spectra.get_vspecpol_spectrum(modelpath, timeavg, dirbin, args, fnufilterfunc=filterfunc)
-                for dirbin in dbins_get
+                dirbin: at.spectra.get_vspecpol_spectrum(modelpath, timeavg, dirbin, args, fluxfilterfunc=filterfunc)
+                for dirbin in directionbins
                 if dirbin >= 0
             }
         else:
             viewinganglespectra = at.spectra.get_spectrum(
                 modelpath=modelpath,
-                directionbins=dbins_get,
+                directionbins=directionbins,
                 timestepmin=timestepmin,
                 timestepmax=timestepmax,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
-                fnufilterfunc=filterfunc,
+                fluxfilterfunc=filterfunc,
             )
 
         dirbin_definitions = (
-            at.get_vspec_dir_labels(modelpath=modelpath, viewinganglelabelunits=args.viewinganglelabelunits)
+            at.get_vspec_dir_labels(modelpath=modelpath, usedegrees=usedegrees)
             if args.plotvspecpol
             else at.get_dirbin_labels(
                 dirbins=directionbins,
                 modelpath=modelpath,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
                 usedegrees=usedegrees,
@@ -351,37 +357,33 @@
         for dirbin in directionbins:
             if len(directionbins) > 1 and dirbin != directionbins[0]:
                 # only one colour was specified, but we have multiple direction bins
                 # to zero out all but the first one
                 plotkwargs = plotkwargs.copy()
                 plotkwargs["color"] = None
 
-            dfspectrum_fullrange = viewinganglespectra[dirbin]
-            dfspectrum = dfspectrum_fullrange[
-                (supxmin * 0.9 <= dfspectrum_fullrange["lambda_angstroms"])
-                & (dfspectrum_fullrange["lambda_angstroms"] <= supxmax * 1.1)
-            ].copy()
+            dfspectrum = (
+                pl.from_pandas(viewinganglespectra[dirbin])
+                if isinstance(viewinganglespectra[dirbin], pd.DataFrame)
+                else viewinganglespectra[dirbin].lazy().collect()
+            )
+            dfspectrum = dfspectrum.filter(pl.col("lambda_angstroms").is_between(supxmin * 0.9, supxmax * 1.1))
 
             linelabel_withdirbin = linelabel
             if dirbin != -1:
                 print(f" direction {dirbin:4d}  {dirbin_definitions[dirbin]}")
                 if len(directionbins) > 1 or not linelabel_is_custom:
                     linelabel_withdirbin = linelabel + " " + dirbin_definitions[dirbin]
 
             at.spectra.print_integrated_flux(dfspectrum["f_lambda"], dfspectrum["lambda_angstroms"])
 
             if scale_to_peak:
-                dfspectrum["f_lambda_scaled"] = dfspectrum["f_lambda"] / dfspectrum["f_lambda"].max() * scale_to_peak
-                if args.plotvspecpol is not None:
-                    for angle in args.plotvspecpol:
-                        viewinganglespectra[angle]["f_lambda_scaled"] = (
-                            viewinganglespectra[angle]["f_lambda"]
-                            / viewinganglespectra[angle]["f_lambda"].max()
-                            * scale_to_peak
-                        )
+                dfspectrum = dfspectrum.with_columns(
+                    f_lambda_scaled=pl.col("f_lambda") / pl.col("f_lambda").max() * scale_to_peak
+                )
 
                 ycolumnname = "f_lambda_scaled"
             else:
                 ycolumnname = "f_lambda"
 
             if plotpacketcount:
                 ycolumnname = "packetcount"
@@ -391,19 +393,22 @@
                 binned_flux = []
 
                 wavelengths = dfspectrum["lambda_angstroms"]
                 fluxes = dfspectrum[ycolumnname]
                 nbins = 5
 
                 for i in np.arange(0, len(wavelengths - nbins), nbins):
-                    new_lambda_angstroms.append(wavelengths[i + nbins // 2])
-                    sum_flux = sum(fluxes[j] for j in range(i, i + nbins))
-                    binned_flux.append(sum_flux / nbins)
+                    i_max = min(i + nbins, len(wavelengths))
+                    ncontribs = i_max - i
+                    sum_lambda = sum(wavelengths[j] for j in range(i, i_max))
+                    new_lambda_angstroms.append(sum_lambda / ncontribs)
+                    sum_flux = sum(fluxes[j] for j in range(i, i_max))
+                    binned_flux.append(sum_flux / ncontribs)
 
-                dfspectrum = pd.DataFrame({"lambda_angstroms": new_lambda_angstroms, ycolumnname: binned_flux})
+                dfspectrum = pl.DataFrame({"lambda_angstroms": new_lambda_angstroms, ycolumnname: binned_flux})
 
             axis.plot(
                 dfspectrum["lambda_angstroms"],
                 dfspectrum[ycolumnname],
                 label=linelabel_withdirbin if axindex == 0 else None,
                 **plotkwargs,
             )
@@ -420,32 +425,40 @@
 ) -> pd.DataFrame:
     """Plot reference spectra and ARTIS spectra."""
     dfalldata = pd.DataFrame()
     artisindex = 0
     refspecindex = 0
     seriesindex = 0
 
+    # take any specified colours our of the cycle
+    colors = [
+        color for i, color in enumerate(plt.rcParams["axes.prop_cycle"].by_key()["color"]) if f"C{i}" not in args.color
+    ]
+    for ax in axes:
+        ax.set_prop_cycle(color=colors)
+
     for seriesindex, specpath in enumerate(speclist):
         specpath = Path(specpath)
         plotkwargs: dict[str, t.Any] = {
             "alpha": args.linealpha[seriesindex],
             "linestyle": args.linestyle[seriesindex],
-            "color": args.color[refspecindex + artisindex],
+            "color": args.color[seriesindex],
         }
 
         if args.dashes[seriesindex]:
             plotkwargs["dashes"] = args.dashes[seriesindex]
         if args.linewidth[seriesindex]:
             plotkwargs["linewidth"] = args.linewidth[seriesindex]
 
         seriesdata = pd.DataFrame()
-
         if (
             Path(specpath).is_file()
             or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", specpath).is_file()
+            or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", f"{specpath!s}.xz").is_file()
+            or Path(at.get_config()["path_artistools_dir"], "data", "refspectra", f"{specpath!s}.zstd").is_file()
         ):
             # reference spectrum
             if "linewidth" not in plotkwargs:
                 plotkwargs["linewidth"] = 1.1
 
             if args.multispecplot:
                 plotkwargs["color"] = "k"
@@ -502,16 +515,17 @@
                     plotpacketcount=args.plotpacketcount,
                     directionbins=args.plotvspecpol or args.plotviewingangle,
                     average_over_phi=args.average_over_phi_angle,
                     average_over_theta=args.average_over_theta_angle,
                     usedegrees=args.usedegrees,
                     **plotkwargs,
                 )
-            except FileNotFoundError:
+            except FileNotFoundError as e:
                 print(f"WARNING: Skipping {specpath} because it does not exist")
+                print(e)
                 continue
 
             if seriesdata is not None:
                 seriesname = at.get_model_name(specpath)
                 artisindex += 1
 
         if args.write_data and not seriesdata.empty:
@@ -601,14 +615,17 @@
     assert args.timemax is not None
 
     print(f"Plotting {modelname} timesteps {timestepmin} to {timestepmax} ({args.timemin:.3f} to {args.timemax:.3f}d)")
 
     xmin, xmax = axis.get_xlim()
 
     if args.frompackets:
+        dirbin = (
+            args.plotviewingangle[0] if args.plotviewingangle else args.plotvspecpol[0] if args.plotvspecpol else None
+        )
         (
             contribution_list,
             array_flambda_emission_total,
             arraylambda_angstroms,
         ) = at.spectra.get_flux_contributions_from_packets(
             modelpath,
             args.timemin,
@@ -621,17 +638,18 @@
             filterfunc=filterfunc,
             groupby=args.groupby,
             fixedionlist=args.fixedionlist,
             maxseriescount=args.maxseriescount + 20,
             delta_lambda=args.deltalambda,
             use_lastemissiontype=not args.use_thermalemissiontype,
             emissionvelocitycut=args.emissionvelocitycut,
-            directionbin=args.plotviewingangle[0] if args.plotviewingangle else None,
+            directionbin=dirbin,
             average_over_phi=args.average_over_phi_angle,
             average_over_theta=args.average_over_theta_angle,
+            directionbins_are_vpkt_observers=args.plotvspecpol is not None,
         )
     else:
         arraylambda_angstroms = 2.99792458e18 / arraynu
         contribution_list, array_flambda_emission_total = at.spectra.get_flux_contributions(
             modelpath,
             filterfunc,
             timestepmin,
@@ -735,16 +753,18 @@
     plotobjectlabels.extend([x.linelabel for x in contributions_sorted_reduced])
     # print(plotobjectlabels)
     # print(len(plotobjectlabels), len(plotobjects))
 
     ymaxrefall = 0.0
     plotkwargs = {}
     for index, filepath in enumerate(args.specpath):
-        if Path(filepath).is_dir() or Path(filepath).name.endswith(".out"):
+        filepath = Path(filepath)
+        if path_is_artis_model(filepath):
             continue
+
         if index < len(args.color):
             plotkwargs["color"] = args.color[index]
             plotkwargs["label"] = args.label[index]
             plotkwargs["alpha"] = args.linealpha[index]
 
         supxmin, supxmax = axis.get_xlim()
         plotobj, serieslabel, ymaxref = plot_reference_spectrum(
@@ -821,15 +841,15 @@
         allnonemptymgilist = list(modeldata.index)
 
     else:
         estimators = at.estimators.read_estimators(modelpath=modelpath)
         allnonemptymgilist = list({modelgridindex for ts, modelgridindex in estimators})
 
     assert estimators is not None
-    packetsfiles = at.packets.get_packetsfilepaths(modelpath, args.maxpacketfiles)
+    packetsfiles = at.packets.get_packets_text_paths(modelpath, args.maxpacketfiles)
     assert args.timemin is not None
     assert args.timemax is not None
     # tdays_min = float(args.timemin)
     # tdays_max = float(args.timemax)
 
     c_ang_s = 2.99792458e18
     # nu_min = c_ang_s / args.xmax
@@ -1050,21 +1070,21 @@
 
     if not args.hidexticklabels:
         axes[-1].set_xlabel(args.xlabel)
 
     if not args.outputfile:
         args.outputfile = defaultoutputfile
     elif not Path(args.outputfile).suffixes:
-        args.outputfile = args.outputfile / defaultoutputfile
+        args.outputfile /= defaultoutputfile
 
     # plt.text(6000, (args.ymax * 0.9), f'{round(args.timemin) + 1} days', fontsize='large')
 
     if args.showtime and not args.multispecplot:
         if not args.ymax:
-            ymin, ymax = ax.get_ylim()
+            _ymin, ymax = ax.get_ylim()
         else:
             ymax = args.ymax
 
         timeavg = (args.timemin + args.timemax) / 2.0
         ax.annotate(
             f"{timeavg:.2f} days",
             xy=(0.03, 0.97),
@@ -1146,14 +1166,16 @@
 
     parser.add_argument(
         "-filtersavgol",
         nargs=2,
         help="Savitzky-Golay filter. Specify the window_length and poly_order.e.g. -filtersavgol 5 3",
     )
 
+    parser.add_argument("-filtermovingavg", type=int, default=0, help="Smoothing length (1 is same as none)")
+
     parser.add_argument("-timestep", "-ts", dest="timestep", nargs="?", help="First timestep or a range e.g. 45-65")
 
     parser.add_argument(
         "-timedays", "-time", "-t", dest="timedays", nargs="?", help="Range of times in days to plot (e.g. 50-100)"
     )
 
     parser.add_argument("-timemin", type=float, help="Lower time in days to integrate spectrum")
@@ -1335,18 +1357,14 @@
     )
 
     parser.add_argument("-timedayslist", nargs="+", help="List of times in days for time sequence subplots")
 
     parser.add_argument("--showtime", action="store_true", help="Write time on plot")
 
     parser.add_argument(
-        "-viewinganglelabelunits", type=str, default="deg", help="Choose viewing angle label in deg or rad"
-    )
-
-    parser.add_argument(
         "--classicartis", action="store_true", help="Flag to show using output from classic ARTIS branch"
     )
 
 
 def main(args: argparse.Namespace | None = None, argsraw: t.Sequence[str] | None = None, **kwargs) -> None:
     """Plot spectra from ARTIS and reference data."""
     if args is None:
@@ -1382,15 +1400,15 @@
     if not args.color:
         args.color = []
         artismodelcolors = [f"C{i}" for i in range(10)]
         refspeccolors = ["0.0", "0.4", "0.6", "0.7"]
         refspecnum = 0
         artismodelnum = 0
         for filepath in args.specpath:
-            if Path(filepath).is_dir() or Path(filepath).name.endswith(".out"):
+            if path_is_artis_model(filepath):
                 args.color.append(artismodelcolors[artismodelnum])
                 artismodelnum += 1
             else:
                 args.color.append(refspeccolors[refspecnum])
                 refspecnum += 1
 
     args.color, args.label, args.linestyle, args.linealpha, args.dashes, args.linewidth = at.trim_or_pad(
@@ -1417,15 +1435,15 @@
             at.spectra.write_flambda_spectra(modelpath)
 
     else:
         if args.emissionabsorption:
             args.showemission = True
             args.showabsorption = True
 
-        fig, axes, dfalldata = make_plot(args)
+        fig, _axes, dfalldata = make_plot(args)
 
         strdirectionbins = (
             "_direction" + "_".join([f"{angle:02d}" for angle in args.plotviewingangle])
             if args.plotviewingangle
             else ""
         )
         filenameout = str(args.outputfile).format(
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/sampleblackbodyfrompacket_tr.py` & `artistools-2024.4.23/artistools/spectra/sampleblackbodyfrompacket_tr.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     specpol_data_bb[time] = np.zeros_like(arr_min_nu_hz)
     packet_contribution_count[time] = 0
 
 specpol_res_data_bb = [copy.deepcopy(specpol_data_bb) for _ in range(n_angle_bins)]
 # need deep copy to make new empty array of same size
 
 
-packetsfiles = at.packets.get_packetsfilepaths(modelpath)
+packetsfiles = at.packets.get_packets_text_paths(modelpath)
 nprocs = at.get_nprocs(modelpath)
 # nprocs = 100
 for npacketfile in range(nprocs):
     dfpackets = at.packets.readfile(packetsfiles[npacketfile])  # , type='TYPE_ESCAPE', escape_type='TYPE_RPKT')
     dfpackets = at.packets.bin_packet_directions(modelpath, dfpackets)
     dfpackets = dfpackets.query(f'type_id == {type_ids["TYPE_ESCAPE"]} and escape_type_id == {type_ids["TYPE_RPKT"]}')
 
@@ -135,15 +135,15 @@
 
             if nu > 0.0:
                 angle = int(row["angle_bin"])
                 if angle > 99:  # 100 is getting in there somehow??
                     continue
                 e_rf = row["e_rf"]
                 hist, _ = np.histogram([nu], bins=arr_nu_hz)  # get frequency bin - returns array with 1 in correct bin
-                hist = hist * e_rf  # multiply by packet rf energy to get the energy in the right bin
+                hist *= e_rf  # multiply by packet rf energy to get the energy in the right bin
                 freq_bin_number = np.nonzero(hist)  # the frequency bin number is where hist is non zero
 
                 # add to angle bin in this timestep
                 specpol_res_data_bb[angle][timedays] += (
                     hist
                     / (timehigh - timelow)
                     / arr_delta_nu_hz[freq_bin_number[0][0]]
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/spectra.py` & `artistools-2024.4.23/artistools/spectra/spectra.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import polars as pl
+import polars.selectors as cs
 
 import artistools as at
 
 fluxcontributiontuple = namedtuple(
     "fluxcontributiontuple", "fluxcontrib linelabel array_flambda_emission array_flambda_absorption color"
 )
 megaparsec_to_cm = 3.0856e24
 
 
 def timeshift_fluxscale_co56law(scaletoreftime: float | None, spectime: float) -> float:
     if scaletoreftime is not None:
         # Co56 decay flux scaling
         assert spectime > 150
-        return math.exp(float(spectime) / 113.7) / math.exp(scaletoreftime / 113.7)
+        return math.exp(spectime / 113.7) / math.exp(scaletoreftime / 113.7)
 
     return 1.0
 
 
 def get_exspec_bins(
     modelpath: str | Path | None = None,
     mnubins: int | None = None,
@@ -45,17 +46,19 @@
         dfspec = read_spec(modelpath, printwarningsonly=True)
         if mnubins is None:
             mnubins = dfspec.height
 
         nu_centre_min = dfspec.item(0, 0)
         nu_centre_max = dfspec.item(dfspec.height - 1, 0)
 
-        # This is an exact solution for dlognu since we're assuming the bin centre spacing matches the bin edge spacing
+        # This is not an exact solution for dlognu since we're assuming the bin centre spacing matches the bin edge spacing
         # but it's close enough for our purposes and avoids the difficulty of finding the exact solution (lots more algebra)
-        dlognu = math.log(dfspec.item(1, 0) / dfspec.item(0, 0))
+        dlognu = math.log(
+            dfspec.item(1, 0) / dfspec.item(0, 0)  # second nu value divided by the first nu value
+        )
 
         if nu_min_r is None:
             nu_min_r = nu_centre_min / (1 + 0.5 * dlognu)
 
         if nu_max_r is None:
             nu_max_r = nu_centre_max * (1 + 0.5 * dlognu)
 
@@ -117,162 +120,225 @@
     return get_spectrum(
         modelpath=modelpath,
         directionbins=[dirbin],
         timestepmin=timestep,
         timestepmax=timestep,
         average_over_phi=average_over_phi,
         average_over_theta=average_over_theta,
-    )[dirbin]
+    )[dirbin].to_pandas()
 
 
 def get_from_packets(
     modelpath: Path,
     timelowdays: float,
     timehighdays: float,
     lambda_min: float,
     lambda_max: float,
     delta_lambda: None | float | np.ndarray = None,
     use_time: t.Literal["arrival", "emission", "escape"] = "arrival",
     maxpacketfiles: int | None = None,
-    getpacketcount: bool = False,
     directionbins: t.Collection[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     nu_column: str = "nu_rf",
-    fnufilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
-    nprocs_read_dfpackets: tuple[int, pl.DataFrame] | None = None,
-) -> dict[int, pd.DataFrame]:
+    fluxfilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+    nprocs_read_dfpackets: tuple[int, pl.DataFrame | pl.LazyFrame] | None = None,
+    directionbins_are_vpkt_observers: bool = False,
+) -> dict[int, pl.DataFrame]:
     """Get a spectrum dataframe using the packets files as input."""
     if directionbins is None:
         directionbins = [-1]
 
     assert use_time in {"arrival", "emission", "escape"}
 
-    if use_time == "escape":
-        modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-        vmax_beta = modeldata.iloc[-1].vel_r_max_kmps * 299792.458
-        escapesurfacegamma = math.sqrt(1 - vmax_beta**2)
-    else:
-        escapesurfacegamma = None
+    if nu_column == "absorption_freq":
+        nu_column = "nu_absorbed"
 
     lambda_bin_edges: np.ndarray
     if delta_lambda is not None:
         lambda_bin_edges = np.arange(lambda_min, lambda_max + delta_lambda, delta_lambda)
         lambda_bin_centres = 0.5 * (lambda_bin_edges[:-1] + lambda_bin_edges[1:])  # bin centres
     else:
         lambda_bin_edges, lambda_bin_centres, delta_lambda = get_exspec_bins(modelpath=modelpath)
         lambda_min = lambda_bin_centres[0]
         lambda_max = lambda_bin_centres[-1]
 
-    nu_min = 2.99792458e18 / lambda_max
-    nu_max = 2.99792458e18 / lambda_min
-
-    timelow = timelowdays * 86400.0
-    timehigh = timehighdays * 86400.0
+    delta_time_s = (timehighdays - timelowdays) * 86400.0
 
     nphibins = at.get_viewingdirection_phibincount()
     ncosthetabins = at.get_viewingdirection_costhetabincount()
     ndirbins = at.get_viewingdirectionbincount()
 
-    nprocs_read, dfpackets = nprocs_read_dfpackets or at.packets.get_packets_pl(
-        modelpath, maxpacketfiles=maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT"
+    if nprocs_read_dfpackets:
+        nprocs_read = nprocs_read_dfpackets[0]
+        dfpackets = nprocs_read_dfpackets[1].lazy()
+    elif directionbins_are_vpkt_observers:
+        nprocs_read, dfpackets = at.packets.get_virtual_packets_pl(modelpath, maxpacketfiles=maxpacketfiles)
+    else:
+        nprocs_read, dfpackets = at.packets.get_packets_pl(
+            modelpath, maxpacketfiles=maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT"
+        )
+
+    dfpackets = dfpackets.with_columns(
+        [
+            (2.99792458e18 / pl.col(colname)).alias(
+                colname.replace("absorption_freq", "nu_absorbed").replace("nu_", "lambda_angstroms_")
+            )
+            for colname in dfpackets.columns
+            if "nu_" in colname or colname == "absorption_freq"
+        ]
     )
 
-    if use_time == "arrival":
-        dfpackets = dfpackets.filter(pl.col("t_arrive_d").is_between(float(timelowdays), float(timehighdays)))
-    elif use_time == "escape":
-        assert escapesurfacegamma is not None
-        dfpackets = dfpackets.filter(
-            pl.col("escape_time").is_between(timelow / escapesurfacegamma, timehigh / escapesurfacegamma)
-        )
-    elif use_time == "emission":
-        mean_correction = float(
-            dfpackets.select((pl.col("em_time") - pl.col("t_arrive_d") * 86400.0).mean())
-            .lazy()
-            .collect()
-            .to_numpy()[0][0]
+    dfbinned_lazy = (
+        pl.DataFrame(
+            {"lambda_angstroms": lambda_bin_centres, "lambda_binindex": range(len(lambda_bin_centres))},
+            schema_overrides={"lambda_binindex": pl.Int32},
         )
+        .sort(["lambda_binindex", "lambda_angstroms"])
+        .lazy()
+    )
 
-        em_time_low = float(timelowdays) * 86400.0 + mean_correction
-        em_time_high = float(timehighdays) * 86400.0 + mean_correction
-        dfpackets = dfpackets.filter(pl.col("em_time").is_between(em_time_low, em_time_high))
+    if directionbins_are_vpkt_observers:
+        vpkt_config = at.get_vpkt_config(modelpath)
+        for dirbin in directionbins:
+            obsdirindex = dirbin // vpkt_config["nspectraperobs"]
+            opacchoiceindex = dirbin % vpkt_config["nspectraperobs"]
+            lambda_column = (
+                f"dir{obsdirindex}_lambda_angstroms_rf"
+                if nu_column == "nu_rf"
+                else nu_column.replace("absorption_freq", "nu_absorbed").replace("nu_", "lambda_angstroms_")
+            )
+            energy_column = f"dir{obsdirindex}_e_rf_{opacchoiceindex}"
 
-    dfpackets = dfpackets.filter(pl.col(nu_column).is_between(float(nu_min), float(nu_max)))
+            pldfpackets_dirbin_lazy = dfpackets.filter(pl.col(lambda_column).is_between(lambda_min, lambda_max)).filter(
+                pl.col(f"dir{obsdirindex}_t_arrive_d").is_between(timelowdays, timehighdays)
+            )
 
-    if fnufilterfunc:
-        print("Applying filter to ARTIS spectrum")
+            dfbinned_dirbin = at.packets.bin_and_sum(
+                pldfpackets_dirbin_lazy,
+                bincol=lambda_column,
+                bins=list(lambda_bin_edges),
+                sumcols=[energy_column],
+                getcounts=True,
+            ).select(
+                [
+                    pl.col(f"{lambda_column}_bin").alias("lambda_binindex"),
+                    (
+                        pl.col(f"{energy_column}_sum")
+                        / delta_lambda
+                        / delta_time_s
+                        / (megaparsec_to_cm**2)
+                        / nprocs_read
+                    ).alias(f"f_lambda_dirbin{dirbin}"),
+                    pl.col("count").alias(f"count_dirbin{dirbin}"),
+                ]
+            )
 
-    encol = "e_cmf" if use_time == "escape" else "e_rf"
-    getcols = {nu_column, encol}
-    if directionbins != [-1]:
-        if average_over_phi:
-            getcols.add("costhetabin")
-        elif average_over_theta:
-            getcols.add("phibin")
-        else:
-            getcols.add("dirbin")
+            dfbinned_lazy = dfbinned_lazy.join(dfbinned_dirbin, on="lambda_binindex", how="left")
 
-    dfpackets = dfpackets.select(getcols).lazy().collect().lazy()
+        assert use_time == "arrival"
+    else:
+        lambda_column = nu_column.replace("nu_", "lambda_angstroms_")
+        energy_column = "e_cmf" if use_time == "escape" else "e_rf"
 
-    dfdict = {}
-    for dirbin in directionbins:
-        if dirbin == -1:
-            solidanglefactor = 1.0
-            pldfpackets_dirbin_lazy = dfpackets
-        elif average_over_phi:
-            assert not average_over_theta
-            solidanglefactor = ncosthetabins
-            pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("costhetabin") * 10 == dirbin)
-        elif average_over_theta:
-            solidanglefactor = nphibins
-            pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("phibin") == dirbin)
-        else:
-            solidanglefactor = ndirbins
-            pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("dirbin") == dirbin)
+        if use_time == "arrival":
+            dfpackets = dfpackets.filter(pl.col("t_arrive_d").is_between(timelowdays, timehighdays))
+        elif use_time == "escape":
+            modeldata, _ = at.inputmodel.get_modeldata(modelpath)
+            vmax_beta = modeldata.iloc[-1].vel_r_max_kmps * 299792.458
+            escapesurfacegamma = math.sqrt(1 - vmax_beta**2)
+
+            dfpackets = dfpackets.filter(
+                (pl.col("escape_time") * escapesurfacegamma / 86400.0).is_between(timelowdays, timehighdays)
+                for dirbin in directionbins
+            )
 
-        pldfpackets_dirbin = pldfpackets_dirbin_lazy.with_columns(
-            [(2.99792458e18 / pl.col(nu_column)).alias("lambda_angstroms")]
-        ).select(["lambda_angstroms", encol])
-
-        dfbinned = at.packets.bin_and_sum(
-            pldfpackets_dirbin,
-            bincol="lambda_angstroms",
-            bins=list(lambda_bin_edges),
-            sumcols=[encol],
-            getcounts=getpacketcount,
-        )
-        array_flambda = (
-            dfbinned[f"{encol}_sum"]
-            / delta_lambda
-            / (timehigh - timelow)
-            / (4 * math.pi)
-            * solidanglefactor
-            / (megaparsec_to_cm**2)
-            / nprocs_read
-        ).to_numpy()
-
-        if use_time == "escape":
-            assert escapesurfacegamma is not None
-            array_flambda /= escapesurfacegamma
-
-        if fnufilterfunc:
-            arr_nu = 2.99792458e18 / lambda_bin_centres
-            array_f_nu = array_flambda * lambda_bin_centres / arr_nu
-            array_f_nu = fnufilterfunc(array_f_nu)
-            array_flambda = array_f_nu * arr_nu / lambda_bin_centres
-
-        dfdict[dirbin] = pd.DataFrame(
-            {
-                "lambda_angstroms": lambda_bin_centres,
-                "f_lambda": array_flambda,
-            }
+        elif use_time == "emission":
+            mean_correction = float(
+                dfpackets.select((pl.col("em_time") - pl.col("t_arrive_d") * 86400.0).mean())
+                .lazy()
+                .collect()
+                .to_numpy()[0][0]
+            )
+
+            dfpackets = dfpackets.filter(
+                pl.col("em_time").is_between(
+                    timelowdays * 86400.0 + mean_correction,
+                    timehighdays * 86400.0 + mean_correction,
+                )
+            )
+
+        dfpackets = dfpackets.filter(pl.col(lambda_column).is_between(lambda_min, lambda_max))
+
+        for dirbin in directionbins:
+            if dirbin == -1:
+                solidanglefactor = 1.0
+                pldfpackets_dirbin_lazy = dfpackets
+            elif average_over_phi:
+                assert not average_over_theta
+                solidanglefactor = ncosthetabins
+                pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("costhetabin") * nphibins == dirbin)
+            elif average_over_theta:
+                solidanglefactor = nphibins
+                pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("phibin") == dirbin)
+            else:
+                solidanglefactor = ndirbins
+                pldfpackets_dirbin_lazy = dfpackets.filter(pl.col("dirbin") == dirbin)
+
+            dfbinned_dirbin = at.packets.bin_and_sum(
+                pldfpackets_dirbin_lazy,
+                bincol=lambda_column,
+                bins=list(lambda_bin_edges),
+                sumcols=[energy_column],
+                getcounts=True,
+            ).select(
+                [
+                    pl.col(f"{lambda_column}_bin").alias("lambda_binindex"),
+                    (
+                        pl.col(f"{energy_column}_sum")
+                        / delta_lambda
+                        / delta_time_s
+                        / (4 * math.pi)
+                        * solidanglefactor
+                        / (megaparsec_to_cm**2)
+                        / nprocs_read
+                    ).alias(f"f_lambda_dirbin{dirbin}"),
+                    pl.col("count").alias(f"count_dirbin{dirbin}"),
+                ]
+            )
+
+            if use_time == "escape":
+                assert escapesurfacegamma is not None
+                dfbinned_dirbin = dfbinned_dirbin.with_columns(
+                    pl.col(f"f_lambda_dirbin{dirbin}").mul(1.0 / escapesurfacegamma)
+                )
+
+            dfbinned_lazy = dfbinned_lazy.join(dfbinned_dirbin, on="lambda_binindex", how="left")
+
+    if fluxfilterfunc:
+        print("Applying filter to ARTIS spectrum")
+        dfbinned_lazy = dfbinned_lazy.with_columns(
+            cs.starts_with("f_lambda_dirbin").map(lambda x: fluxfilterfunc(x.to_numpy()))
         )
 
-        if getpacketcount:
-            dfdict[dirbin]["packetcount"] = dfbinned["count"]
+    dfbinned = dfbinned_lazy.collect(streaming=True)
+    assert isinstance(dfbinned, pl.DataFrame)
+
+    dfdict = {}
+    for dirbin in directionbins:
+        dfdict[dirbin] = dfbinned.select(
+            [
+                "lambda_angstroms",
+                pl.col(f"f_lambda_dirbin{dirbin}").alias("f_lambda"),
+                pl.col(f"count_dirbin{dirbin}").alias("packetcount"),
+            ]
+        )
+        if nprocs_read_dfpackets is None:
+            npkts_selected = dfdict[dirbin].get_column("packetcount").sum()
+            print(f"    dirbin {dirbin:2d} plots {npkts_selected:.2e} packets")
 
     return dfdict
 
 
 @lru_cache(maxsize=16)
 def read_spec(modelpath: Path, printwarningsonly: bool = False) -> pl.DataFrame:
     specfilename = at.firstexisting("spec.out", folder=modelpath, tryzipped=True)
@@ -369,19 +435,19 @@
 
 
 def get_spectrum(
     modelpath: Path,
     timestepmin: int,
     timestepmax: int | None = None,
     directionbins: t.Sequence[int] | None = None,
-    fnufilterfunc: t.Callable[[npt.NDArray[np.floating]], npt.NDArray[np.floating]] | None = None,
+    fluxfilterfunc: t.Callable[[npt.NDArray[np.floating]], npt.NDArray[np.floating]] | None = None,
     average_over_theta: bool = False,
     average_over_phi: bool = False,
     stokesparam: t.Literal["I", "Q", "U"] = "I",
-) -> dict[int, pd.DataFrame]:
+) -> dict[int, pl.DataFrame]:
     """Return a pandas DataFrame containing an ARTIS emergent spectrum."""
     if timestepmax is None or timestepmax < 0:
         timestepmax = timestepmin
 
     if directionbins is None:
         directionbins = [-1]
     # keys are direction bins (or -1 for spherical average)
@@ -408,42 +474,42 @@
 
             except FileNotFoundError:
                 specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
 
         else:
             specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
 
-    specdataout: dict[int, pd.DataFrame] = {}
+    specdataout: dict[int, pl.DataFrame] = {}
     for dirbin in directionbins:
+        if dirbin not in specdata:
+            print(f"WARNING: Direction bin {dirbin} not found in specdata. Dirbins: {list(specdata.keys())}")
+            continue
         arr_nu = specdata[dirbin]["nu"].to_numpy()
         arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
 
         try:
             arr_f_nu = stackspectra(
                 [
                     (specdata[dirbin][specdata[dirbin].columns[timestep + 1]].to_numpy(), arr_tdelta[timestep])
                     for timestep in range(timestepmin, timestepmax + 1)
                 ]
             )
         except IndexError:
             print(" ERROR: data not available for timestep range")
             return specdataout
 
-        # best to use the filter on this list because it
-        # has regular sampling
-        if fnufilterfunc:
+        if fluxfilterfunc:
             if dirbin == directionbins[0]:
                 print("Applying filter to ARTIS spectrum")
-            arr_f_nu = fnufilterfunc(arr_f_nu)
+            arr_f_nu = fluxfilterfunc(arr_f_nu)
 
-        c_ang_per_s = 2.99792458e18
-        arr_lambda = c_ang_per_s / arr_nu
-        arr_f_lambda = arr_f_nu * arr_nu / arr_lambda
-        dfspectrum = pd.DataFrame({"lambda_angstroms": arr_lambda, "f_lambda": arr_f_lambda})
-        dfspectrum = dfspectrum.sort_values(by="lambda_angstroms", ascending=True)
+        arr_lambda = 2.99792458e18 / arr_nu
+        dfspectrum = pl.DataFrame({"lambda_angstroms": arr_lambda, "f_lambda": arr_f_nu * arr_nu / arr_lambda}).sort(
+            by="lambda_angstroms"
+        )
 
         specdataout[dirbin] = dfspectrum
 
     return specdataout
 
 
 def make_virtual_spectra_summed_file(modelpath: Path) -> Path:
@@ -473,15 +539,15 @@
             chunk = (
                 vspecpolfile.iloc[index_spectrum_starts : index_of_new_spectrum[i + 1], :]
                 if index_spectrum_starts != index_of_new_spectrum[-1]
                 else vspecpolfile.iloc[index_spectrum_starts:, :]
             )
             vspecpol_data.append(chunk)
 
-        if len(vspecpol_data_old) > 0:
+        if vspecpol_data_old:
             for i in range(len(vspecpol_data)):
                 dftmp = vspecpol_data[i].copy()  # copy of vspectrum number i in a file
                 # add copy to the same spectrum number from previous file
                 # (don't need to copy row 1 = time or column 1 = freq)
                 dftmp.iloc[1:, 1:] += vspecpol_data_old[i].iloc[1:, 1:]
                 # spectrum i then equals the sum of all previous files spectrum number i
                 vspecpol_data[i] = dftmp
@@ -511,15 +577,15 @@
     filenames = sorted_by_number(filenames)
 
     for spec_index, filename in enumerate(filenames):  # vspecpol-total files
         vspecdata = [pd.read_csv(modelpath / filename, sep=r"\s+", header=None) for modelpath in args.modelpath]
         for i in range(1, len(vspecdata)):
             vspecdata[0].iloc[1:, 1:] += vspecdata[i].iloc[1:, 1:]
 
-        vspecdata[0].iloc[1:, 1:] = vspecdata[0].iloc[1:, 1:] / len(vspecdata)
+        vspecdata[0].iloc[1:, 1:] /= len(vspecdata)
         vspecdata[0].to_csv(
             args.modelpath[0] / f"vspecpol_averaged-{spec_index}.out", sep=" ", index=False, header=False
         )
 
 
 @lru_cache(maxsize=4)
 def get_specpol_data(
@@ -542,20 +608,17 @@
 @lru_cache(maxsize=4)
 def get_vspecpol_data(
     vspecangle: int | None = None, modelpath: Path | None = None, specdata: pd.DataFrame | None = None
 ) -> dict[str, pd.DataFrame]:
     if specdata is None:
         assert modelpath is not None
         # alternatively use f'vspecpol_averaged-{angle}.out' ?
-        vspecpath = modelpath
-        if (modelpath / "vspecpol").is_dir():
-            vspecpath = modelpath / "vspecpol"
 
         try:
-            specfilename = at.firstexisting(f"vspecpol_total-{vspecangle}.out", folder=vspecpath, tryzipped=True)
+            specfilename = at.firstexisting(f"vspecpol_total-{vspecangle}.out", folder=modelpath, tryzipped=True)
         except FileNotFoundError:
             print(f"vspecpol_total-{vspecangle}.out does not exist. Generating all-rank summed vspec files..")
             specfilename = make_virtual_spectra_summed_file(modelpath=modelpath)
 
         print(f"Reading {specfilename}")
         specdata = pd.read_csv(specfilename, sep=r"\s+")
 
@@ -576,69 +639,69 @@
         )
     }
     stokes_params["Q"] = pd.concat(
         [specdata["nu"], specdata.iloc[:, cols_to_split[1] : cols_to_split[2]]], axis="columns"
     )
     stokes_params["U"] = pd.concat([specdata["nu"], specdata.iloc[:, cols_to_split[2] :]], axis="columns")
 
-    for param in ["Q", "U"]:
+    for param in ("Q", "U"):
         stokes_params[param].columns = stokes_params["I"].keys()
         stokes_params[param + "/I"] = pd.concat(
             [specdata["nu"], stokes_params[param].iloc[:, 1:] / stokes_params["I"].iloc[:, 1:]], axis="columns"
         )
     return stokes_params
 
 
 def get_vspecpol_spectrum(
     modelpath: Path | str,
     timeavg: float,
     angle: int,
     args: argparse.Namespace,
-    fnufilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
-) -> pd.DataFrame:
+    fluxfilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+) -> pl.DataFrame:
     stokes_params = get_vspecpol_data(vspecangle=angle, modelpath=Path(modelpath))
     if "stokesparam" not in args:
         args.stokesparam = "I"
     vspecdata = stokes_params[args.stokesparam]
 
     nu = vspecdata.loc[:, "nu"].to_numpy()
 
-    arr_tmid = [float(i) for i in vspecdata.columns.to_numpy()[1:] if i[-2] != "."]
+    arr_tmid = [float(i) for i in vspecdata.columns.to_numpy()[1:]]
     arr_tdelta = [l1 - l2 for l1, l2 in zip(arr_tmid[1:], arr_tmid[:-1])] + [arr_tmid[-1] - arr_tmid[-2]]
 
     def match_closest_time(reftime: float) -> str:
-        return str(f"{min((float(x) for x in arr_tmid), key=lambda x: abs(x - reftime))}")
+        return str(min(arr_tmid, key=lambda x: abs(x - reftime)))
 
     # if 'timemin' and 'timemax' in args:
     #     timelower = match_closest_time(args.timemin)  # how timemin, timemax are used changed at some point
     #     timeupper = match_closest_time(args.timemax)  # to average over multiple timesteps needs to fix this
     # else:
     timelower = match_closest_time(timeavg)
     timeupper = match_closest_time(timeavg)
     timestepmin = vspecdata.columns.get_loc(timelower)
     timestepmax = vspecdata.columns.get_loc(timeupper)
+    print(f" vpacket spectrum timesteps {timestepmin} ({timelower}d) to {timestepmax} ({timeupper}d)")
 
     f_nu = stackspectra(
         [
             (vspecdata[vspecdata.columns[timestep + 1]].to_numpy(), arr_tdelta[timestep])
             for timestep in range(timestepmin - 1, timestepmax)
         ]
     )
 
-    # best to use the filter on this list because it
-    # has regular sampling
-    if fnufilterfunc:
+    if fluxfilterfunc:
         print("Applying filter to ARTIS spectrum")
-        f_nu = fnufilterfunc(f_nu)
+        f_nu = fluxfilterfunc(f_nu)
 
-    dfspectrum = pd.DataFrame({"nu": nu, "f_nu": f_nu})
-    dfspectrum = dfspectrum.sort_values(by="nu", ascending=False)
-
-    dfspectrum = dfspectrum.eval("lambda_angstroms = @c / nu", local_dict={"c": 2.99792458e18})
-    return dfspectrum.eval("f_lambda = f_nu * nu / lambda_angstroms")
+    return (
+        pl.DataFrame({"nu": nu, "f_nu": f_nu})
+        .sort(by="nu", descending=True)
+        .with_columns(lambda_angstroms=2.99792458e18 / pl.col("nu"))
+        .with_columns(f_lambda=pl.col("f_nu") * pl.col("nu") / pl.col("lambda_angstroms"))
+    )
 
 
 @lru_cache(maxsize=4)
 def get_flux_contributions(
     modelpath: Path,
     filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
     timestepmin: int = -1,
@@ -670,30 +733,30 @@
     elif average_over_theta:
         assert not average_over_phi
         assert directionbin < at.get_viewingdirection_phibincount()
         dbinlist = list(range(directionbin, at.get_viewingdirectionbincount(), at.get_viewingdirection_phibincount()))
     else:
         dbinlist = [directionbin]
 
-    emissiondata: dict[int, pd.DataFrame] = {}
-    absorptiondata: dict[int, pd.DataFrame] = {}
+    emissiondata = {}
+    absorptiondata = {}
     maxion: int | None = None
     for dbin in dbinlist:
         if getemission:
             emissionfilenames = ["emission.out", "emissionpol.out"] if use_lastemissiontype else ["emissiontrue.out"]
 
             if dbin != -1:
                 emissionfilenames = [x.replace(".out", f"_res_{dbin:02d}.out") for x in emissionfilenames]
 
             emissionfilename = at.firstexisting(emissionfilenames, folder=modelpath, tryzipped=True)
 
             if "pol" in str(emissionfilename):
                 print("This artis run contains polarisation data")
                 # File contains I, Q and U and so times are repeated 3 times
-                arr_tmid = np.array(arr_tmid.tolist() * 3)
+                arr_tmid = np.tile(np.array(arr_tmid), 3)
 
             emissiondata[dbin] = read_emission_absorption_file(emissionfilename)
 
             maxion_float = (emissiondata[dbin].shape[1] - 1) / 2 / nelements  # also known as MIONS in ARTIS sn3d.h
             assert maxion_float.is_integer()
             if maxion is None:
                 maxion = int(maxion_float)
@@ -774,15 +837,14 @@
                             for timestep in range(timestepmin, timestepmax + 1)
                             for dbin in dbinlist
                         ]
                     )
                 else:
                     array_fnu_absorption = np.zeros_like(arraylambda, dtype=float)
 
-                # best to use the filter on fnu (because it hopefully has regular sampling)
                 if filterfunc:
                     array_fnu_emission = filterfunc(array_fnu_emission)
                     if selectedcolumn <= nelements * maxion:
                         array_fnu_absorption = filterfunc(array_fnu_absorption)
 
                 array_flambda_emission = array_fnu_emission * arraynu / arraylambda
                 array_flambda_absorption = array_fnu_absorption * arraynu / arraylambda
@@ -829,52 +891,79 @@
     modelgridindex: int | None = None,
     use_time: t.Literal["arrival", "emission", "escape"] = "arrival",
     use_lastemissiontype: bool = True,
     emissionvelocitycut: float | None = None,
     directionbin: int | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
+    directionbins_are_vpkt_observers: bool = False,
 ) -> tuple[list[fluxcontributiontuple], np.ndarray, np.ndarray]:
     assert groupby in {"ion", "line"}
 
     if directionbin is None:
         directionbin = -1
 
     emtypecolumn = "emissiontype" if use_lastemissiontype else "trueemissiontype"
 
     linelistlazy = at.get_linelist_pldf(modelpath=modelpath, get_ion_str=True)
     bflistlazy = at.get_bflist(modelpath, get_ion_str=True)
 
-    nprocs_read, lzdfpackets = at.packets.get_packets_pl(
-        modelpath, maxpacketfiles=maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT"
-    )
+    cols = {"e_rf"}
+    cols.add({"arrival": "t_arrive_d", "emission": "em_time", "escape": "escape_time"}[use_time])
+
+    nu_min = 2.99792458e18 / lambda_max
+    nu_max = 2.99792458e18 / lambda_min
+
+    if directionbins_are_vpkt_observers:
+        vpkt_config = at.get_vpkt_config(modelpath)
+        obsdirindex = directionbin // vpkt_config["nspectraperobs"]
+        opacchoiceindex = directionbin % vpkt_config["nspectraperobs"]
+        nprocs_read, lzdfpackets = at.packets.get_virtual_packets_pl(modelpath, maxpacketfiles=maxpacketfiles)
+        lzdfpackets = lzdfpackets.with_columns(
+            e_rf=pl.col(f"dir{obsdirindex}_e_rf_{opacchoiceindex}"),
+        )
+        dirbin_nu_column = f"dir{obsdirindex}_nu_rf"
+
+        cols |= {
+            dirbin_nu_column,
+            f"dir{obsdirindex}_t_arrive_d",
+            f"dir{obsdirindex}_e_rf_{opacchoiceindex}",
+        }
+        lzdfpackets = lzdfpackets.filter(pl.col(f"dir{obsdirindex}_t_arrive_d").is_between(timelowdays, timehighdays))
+
+    else:
+        nprocs_read, lzdfpackets = at.packets.get_packets_pl(
+            modelpath, maxpacketfiles=maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT"
+        )
+        dirbin_nu_column = "nu_rf"
+
+        lzdfpackets = lzdfpackets.filter(pl.col("t_arrive_d").is_between(timelowdays, timehighdays))
+
+    condition_nu_emit = pl.col(dirbin_nu_column).is_between(nu_min, nu_max) if getemission else pl.lit(False)
+    condition_nu_abs = pl.col("absorption_freq").is_between(nu_min, nu_max) if getabsorption else pl.lit(False)
+    lzdfpackets = lzdfpackets.filter(condition_nu_emit | condition_nu_abs)
 
     if emissionvelocitycut is not None:
         lzdfpackets = at.packets.add_derived_columns_lazy(lzdfpackets)
         lzdfpackets = lzdfpackets.filter(pl.col("emission_velocity") > emissionvelocitycut)
 
-    lzdfpackets = lzdfpackets.filter(pl.col("t_arrive_d").is_between(float(timelowdays), float(timehighdays)))
-
-    cols = {"e_rf"}
-    cols.add({"arrival": "t_arrive_d", "emission": "em_time", "escape": "excape_time"}[use_time])
-
     expr_linelist_to_str = (
         pl.col("ion_str")
         if groupby == "ion"
         else pl.format(
             "{} λ{} {}-{}",
             pl.col("ion_str"),
             pl.col("lambda_angstroms_air").sub(0.5).round(0).cast(pl.String).str.strip_suffix(".0"),
             pl.col("upperlevelindex"),
             pl.col("lowerlevelindex"),
         )
     )
 
     if getemission:
-        cols |= {"emissiontype_str", "nu_rf"}
+        cols |= {"emissiontype_str", dirbin_nu_column}
         bflistlazy = bflistlazy.with_columns((-1 - pl.col("bfindex").cast(pl.Int32)).alias(emtypecolumn))
         expr_bflist_to_str = (
             pl.col("ion_str") + " bound-free"
             if groupby == "ion"
             else pl.format("{} bound-free {}-{}", pl.col("ion_str"), pl.col("lowerlevel"), pl.col("upperionlevel"))
         )
 
@@ -920,26 +1009,18 @@
         ).with_columns(pl.col("absorptiontype_str").cast(pl.Categorical))
 
         lzdfpackets = lzdfpackets.join(abstypestrings, on="absorption_type", how="left")
 
     if directionbin != -1:
         cols |= {"costhetabin", "phibin", "dirbin"}
 
-    nu_min = 2.99792458e18 / lambda_max
-    nu_max = 2.99792458e18 / lambda_min
-    dfpackets = (
-        lzdfpackets.filter(
-            (pl.col("nu_rf").is_between(nu_min, nu_max)) | (pl.col("absorption_freq").is_between(nu_min, nu_max))
-        )
-        .select([col for col in cols if col in lzdfpackets.columns])
-        .collect()
-    )
+    dfpackets = lzdfpackets.select([col for col in cols if col in lzdfpackets.columns]).collect()
 
     emissiongroups = (
-        dict(dfpackets.filter(pl.col("nu_rf").is_between(nu_min, nu_max)).group_by("emissiontype_str"))
+        dict(dfpackets.filter(pl.col(dirbin_nu_column).is_between(nu_min, nu_max)).group_by("emissiontype_str"))
         if getemission
         else {}
     )
 
     absorptiongroups = (
         dict(dfpackets.filter(pl.col("absorption_freq").is_between(nu_min, nu_max)).group_by("absorptiontype_str"))
         if getabsorption
@@ -1008,17 +1089,18 @@
                 modelpath=modelpath,
                 timelowdays=timelowdays,
                 timehighdays=timehighdays,
                 lambda_min=lambda_min,
                 lambda_max=lambda_max,
                 use_time=use_time,
                 delta_lambda=delta_lambda,
-                fnufilterfunc=filterfunc,
+                fluxfilterfunc=filterfunc,
                 nprocs_read_dfpackets=(nprocs_read, emissiongroups[groupname]),
                 directionbins=[directionbin],
+                directionbins_are_vpkt_observers=directionbins_are_vpkt_observers,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
             )[directionbin]
 
             if array_lambda is None:
                 array_lambda = spec_group["lambda_angstroms"].to_numpy()
 
@@ -1032,19 +1114,24 @@
         if groupname in absorptiongroups:
             spec_group = get_from_packets(
                 modelpath=modelpath,
                 timelowdays=timelowdays,
                 timehighdays=timehighdays,
                 lambda_min=lambda_min,
                 lambda_max=lambda_max,
+                use_time=use_time,
                 delta_lambda=delta_lambda,
                 nu_column="absorption_freq",
-                fnufilterfunc=filterfunc,
+                fluxfilterfunc=filterfunc,
                 nprocs_read_dfpackets=(nprocs_read, absorptiongroups[groupname]),
-            )[-1]
+                directionbins=[directionbin],
+                directionbins_are_vpkt_observers=directionbins_are_vpkt_observers,
+                average_over_phi=average_over_phi,
+                average_over_theta=average_over_theta,
+            )[directionbin]
 
             if array_lambda is None:
                 array_lambda = spec_group["lambda_angstroms"].to_numpy()
 
             array_flambda_absorption = spec_group["f_lambda"].to_numpy()
         else:
             array_flambda_absorption = np.zeros_like(array_flambda_emission, dtype=float)
@@ -1182,21 +1269,24 @@
             )
         )
 
     return contribution_list_out
 
 
 def print_integrated_flux(
-    arr_f_lambda: np.ndarray | pd.Series, arr_lambda_angstroms: np.ndarray | pd.Series, distance_megaparsec: float = 1.0
+    arr_f_lambda: np.ndarray | pd.Series | pl.Series,
+    arr_lambda_angstroms: np.ndarray | pd.Series | pl.Series,
+    distance_megaparsec: float = 1.0,
 ) -> float:
     integrated_flux = abs(np.trapz(np.nan_to_num(arr_f_lambda, nan=0.0), x=arr_lambda_angstroms))
-    print(
-        f" integrated flux ({arr_lambda_angstroms.min():.1f} to "
-        f"{arr_lambda_angstroms.max():.1f} A): {integrated_flux:.3e} erg/s/cm2"
-    )
+    lambda_min = arr_lambda_angstroms.min()
+    lambda_max = arr_lambda_angstroms.max()
+    assert isinstance(lambda_min, int | float)
+    assert isinstance(lambda_max, int | float)
+    print(f" integrated flux ({lambda_min:.1f} to " f"{lambda_max:.1f} A): {integrated_flux:.3e} erg/s/cm2")
     return integrated_flux
 
 
 def get_reference_spectrum(filename: Path | str) -> tuple[pd.DataFrame, dict[t.Any, t.Any]]:
     if Path(filename).is_file():
         filepath = Path(filename)
     else:
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/test_spectra.py` & `artistools-2024.4.23/artistools/spectra/test_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     )
 
 
 def test_spectra_get_spectrum() -> None:
     def check_spectrum(dfspectrumpkts) -> None:
         assert math.isclose(max(dfspectrumpkts["f_lambda"]), 2.548532804918824e-13, abs_tol=1e-5)
         assert min(dfspectrumpkts["f_lambda"]) < 1e-9
-        assert math.isclose(np.mean(dfspectrumpkts["f_lambda"]), 1.0314682640070206e-14, abs_tol=1e-5)
+        assert math.isclose(dfspectrumpkts["f_lambda"].mean(), 1.0314682640070206e-14, abs_tol=1e-5)
 
-    dfspectrum = at.spectra.get_spectrum(modelpath, 55, 65, fnufilterfunc=None)[-1]
+    dfspectrum = at.spectra.get_spectrum(modelpath, 55, 65, fluxfilterfunc=None)[-1]
     assert len(dfspectrum["lambda_angstroms"]) == 1000
     assert len(dfspectrum["f_lambda"]) == 1000
     assert abs(dfspectrum["lambda_angstroms"].to_numpy()[-1] - 29920.601421214415) < 1e-5
     assert abs(dfspectrum["lambda_angstroms"].to_numpy()[0] - 600.75759482509852) < 1e-5
 
     check_spectrum(dfspectrum)
 
@@ -142,18 +142,20 @@
         60: (7.964029031817186e-12, 2.637892822134082e-11),
         70: (7.691392868658026e-12, 2.1262113332060223e-11),
         80: (8.450665096838155e-12, 2.352725654000879e-11),
         90: (8.828105146277665e-12, 2.534549767123003e-11),
     }
 
     for dirbin in spectra:
-        assert isinstance(results[dirbin][0], float)
-        assert np.isclose(results[dirbin][0], expected_results[dirbin][0], rtol=1e-3)
-        assert isinstance(results[dirbin][1], float)
-        assert np.isclose(results[dirbin][1], expected_results[dirbin][1], rtol=1e-3)
+        result_mean = results[dirbin][0]
+        assert isinstance(result_mean, float)
+        assert np.isclose(result_mean, expected_results[dirbin][0], rtol=1e-3)
+        result_std = results[dirbin][1]
+        assert isinstance(result_std, float)
+        assert np.isclose(result_std, expected_results[dirbin][1], rtol=1e-3)
 
 
 def test_spectra_get_spectrum_polar_angles_frompackets() -> None:
     timelowdays = at.get_timestep_times(modelpath_classic_3d, loc="start")[0]
     timehighdays = at.get_timestep_times(modelpath_classic_3d, loc="end")[25]
 
     spectrafrompkts = at.spectra.get_from_packets(
@@ -187,32 +189,34 @@
         60: (3.858248734817849e-12, 9.158354676696867e-12),
         70: (3.997311747521441e-12, 9.53473201327172e-12),
         80: (4.121620503814969e-12, 9.481333902503268e-12),
         90: (4.29975310930973e-12, 9.95760966920298e-12),
     }
 
     for dirbin, i in itertools.product(results_pkts, range(2)):
-        assert np.isclose(results_pkts[dirbin][i], expected_results[dirbin][i], rtol=1e-3)
+        result = results_pkts[dirbin][i]
+        assert isinstance(result, float)
+        assert np.isclose(result, expected_results[dirbin][i], rtol=1e-3)
 
 
 def test_spectra_get_flux_contributions() -> None:
     timestepmin = 40
     timestepmax = 80
     dfspectrum = at.spectra.get_spectrum(
-        modelpath=modelpath, timestepmin=timestepmin, timestepmax=timestepmax, fnufilterfunc=None
+        modelpath=modelpath, timestepmin=timestepmin, timestepmax=timestepmax, fluxfilterfunc=None
     )[-1]
 
     integrated_flux_specout = np.trapz(dfspectrum["f_lambda"], x=dfspectrum["lambda_angstroms"])
 
     specdata = pd.read_csv(modelpath / "spec.out", sep=r"\s+")
     arraynu = specdata.loc[:, "0"].to_numpy()
     c_ang_per_s = 2.99792458e18
     arraylambda_angstroms = c_ang_per_s / arraynu
 
-    contribution_list, array_flambda_emission_total = at.spectra.get_flux_contributions(
+    _contribution_list, array_flambda_emission_total = at.spectra.get_flux_contributions(
         modelpath,
         timestepmin=timestepmin,
         timestepmax=timestepmax,
         use_lastemissiontype=False,
     )
 
     integrated_flux_emission = -np.trapz(array_flambda_emission_total, x=arraylambda_angstroms)
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/test_vspectra.py` & `artistools-2024.4.23/artistools/spectra/test_vspectra.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,43 +2,109 @@
 from unittest import mock
 
 import matplotlib.axes
 import numpy as np
 
 import artistools as at
 
-modelpath = at.get_config()["path_testdata"] / "vspecpolmodel"
-outputpath = at.get_config()["path_testoutput"]
-
 
 @mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
 def test_vspectraplot(mockplot):
     at.spectra.plot(
         argsraw=[],
-        specpath=[modelpath, "sn2011fe_PTF11kly_20120822_norm.txt"],
-        outputfile=outputpath,
+        specpath=[at.get_config()["path_testdata"] / "vspecpolmodel", "sn2011fe_PTF11kly_20120822_norm.txt"],
+        outputfile=at.get_config()["path_testoutput"] / "test_vspectra.pdf",
         plotvspecpol=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
         timemin=10,
         timemax=12,
     )
 
     arr_time_d = np.array(mockplot.call_args_list[0][0][1])
     assert all(np.array_equal(arr_time_d, np.array(mockplot.call_args_list[vspecdir][0][1])) for vspecdir in range(10))
 
     arr_allvspec = np.vstack([np.array(mockplot.call_args_list[vspecdir][0][2]) for vspecdir in range(10)])
+
+    assert np.allclose(
+        arr_allvspec.std(axis=1),
+        [
+            2.01529689e-12,
+            2.05807110e-12,
+            2.01551623e-12,
+            2.18216916e-12,
+            2.85477069e-12,
+            3.34384407e-12,
+            2.94892344e-12,
+            2.29084411e-12,
+            2.05916843e-12,
+            2.00515984e-12,
+        ],
+        atol=1e-20,
+    )
+
+    assert np.allclose(
+        arr_allvspec.mean(axis=1),
+        [
+            2.9864681492951925e-12,
+            3.0063451037690416e-12,
+            2.9785924608537284e-12,
+            3.2028094816751935e-12,
+            4.097482117229833e-12,
+            4.663450168092402e-12,
+            4.231106733071208e-12,
+            3.350080172063692e-12,
+            3.0234533505898177e-12,
+            2.9721539798925583e-12,
+        ],
+        atol=1e-20,
+    )
+
+
+@mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
+def test_vpkt_contrib_spectrum_plot(mockplot):
+    at.spectra.plot(
+        argsraw=[],
+        specpath=[at.get_config()["path_testdata"] / "vpktcontrib"],
+        outputfile=at.get_config()["path_testoutput"] / "test_vpktscontrib_spectra.pdf",
+        plotvspecpol=[0, 1, 2, 3, 4, 5, 6, 7, 8],
+        frompackets=True,
+        maxpacketfiles=2,
+        timemin=130,
+        timemax=135,
+    )
+
+    arr_time_d = np.array(mockplot.call_args_list[0][0][1])
+    assert all(np.array_equal(arr_time_d, np.array(mockplot.call_args_list[vspecdir][0][1])) for vspecdir in range(9))
+
+    arr_allvspec = np.vstack([np.array(mockplot.call_args_list[vspecdir][0][2]) for vspecdir in range(9)])
+    print(list(arr_allvspec.std(axis=1)))
     assert np.allclose(
         arr_allvspec.std(axis=1),
-        np.array(
-            [
-                2.01529689e-12,
-                2.05807110e-12,
-                2.01551623e-12,
-                2.18216916e-12,
-                2.85477069e-12,
-                3.34384407e-12,
-                2.94892344e-12,
-                2.29084411e-12,
-                2.05916843e-12,
-                2.00515984e-12,
-            ]
-        ),
+        [
+            2.250169934569213e-15,
+            1.5100666673940305e-14,
+            4.869648743602329e-15,
+            2.2088584226201254e-15,
+            1.4772661475549563e-14,
+            4.81122573011189e-15,
+            2.3113250841019364e-15,
+            1.45676358684038e-14,
+            4.589891035117792e-15,
+        ],
+        atol=1e-18,
+    )
+
+    print(list(arr_allvspec.mean(axis=1)))
+    assert np.allclose(
+        arr_allvspec.mean(axis=1),
+        [
+            1.1359234428755927e-15,
+            9.615508017438282e-15,
+            2.959189512289016e-15,
+            1.1078180792141745e-15,
+            9.453979816323599e-15,
+            2.981925804875244e-15,
+            1.1359823034815934e-15,
+            9.316807974058103e-15,
+            2.9236313925953637e-15,
+        ],
+        atol=1e-18,
     )
```

### Comparing `artistools-2024.2.22.2/artistools/spectra/writespectra.py` & `artistools-2024.4.23/artistools/spectra/writespectra.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     tmids = at.get_timestep_times(modelpath, loc="mid")
 
     tslast, tmin_d_valid, tmax_d_valid = at.get_escaped_arrivalrange(modelpath)
 
     timesteps = [ts for ts in range(tslast + 1) if tmids[ts] >= tmin_d_valid and tmids[ts] <= tmax_d_valid]
 
     for timestep in timesteps:
-        dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[-1]
+        dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[
+            -1
+        ].to_pandas()
 
         write_spectrum(dfspectrum, outfilepath=outdirectory / f"spectrum_ts{timestep:02.0f}_{tmids[timestep]:.2f}d.txt")
 
     for timestep in timesteps:
         if dfspectrum_polar := at.spectra.get_spectrum(
             modelpath=modelpath, timestepmin=timestep, timestepmax=timestep, average_over_phi=True, directionbins=[0]
         ).get(0, None):
```

### Comparing `artistools-2024.2.22.2/artistools/stats.py` & `artistools-2024.4.23/artistools/stats.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/test_artistools.py` & `artistools-2024.4.23/artistools/test_artistools.py`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/artistools/transitions.py` & `artistools-2024.4.23/artistools/transitions.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,64 +19,74 @@
 
 iontuple = namedtuple("iontuple", "Z ion_stage")
 
 
 def get_kurucz_transitions() -> tuple[pd.DataFrame, list[iontuple]]:
     hc_evcm = (const.h * const.c).to("eV cm").value
     transitiontuple = namedtuple(
-        "transitiontuple", "Z ion_stage lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g"
+        "transitiontuple",
+        "Z ion_stage lambda_angstroms A lower_energy_ev upper_energy_ev lower_statweight upper_statweight",
     )
     translist = []
     ionlist = []
     with Path("gfall.dat").open() as fnist:
         for line in fnist:
             row = line.split()
             if len(row) >= 24:
                 Z, ion_stage = int(row[2].split(".")[0]), int(row[2].split(".")[1]) + 1
                 if Z < 44 or ion_stage >= 2:  # and Z not in [26, 27]
                     continue
                 lambda_angstroms = float(line[:12]) * 10
                 loggf = float(line[11:18])
                 lower_energy_ev, upper_energy_ev = hc_evcm * float(line[24:36]), hc_evcm * float(line[52:64])
-                lower_g, upper_g = 2 * float(line[36:42]) + 1, 2 * float(line[64:70]) + 1
-                fij = (10**loggf) / lower_g
-                A = fij / (1.49919e-16 * upper_g / lower_g * lambda_angstroms**2)
+                lower_statweight, upper_statweight = 2 * float(line[36:42]) + 1, 2 * float(line[64:70]) + 1
+                fij = (10**loggf) / lower_statweight
+                A = fij / (1.49919e-16 * upper_statweight / lower_statweight * lambda_angstroms**2)
                 translist.append(
                     transitiontuple(
-                        Z, ion_stage, lambda_angstroms, A, lower_energy_ev, upper_energy_ev, lower_g, upper_g
+                        Z,
+                        ion_stage,
+                        lambda_angstroms,
+                        A,
+                        lower_energy_ev,
+                        upper_energy_ev,
+                        lower_statweight,
+                        upper_statweight,
                     )
                 )
 
                 if iontuple(Z, ion_stage) not in ionlist:
                     ionlist.append(iontuple(Z, ion_stage))
 
     dftransitions = pd.DataFrame(translist, columns=transitiontuple._fields)
     return dftransitions, ionlist
 
 
 def get_nist_transitions(filename: Path | str) -> pd.DataFrame:
     transitiontuple = namedtuple(
-        "transitiontuple", "lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g"
+        "transitiontuple", "lambda_angstroms A lower_energy_ev upper_energy_ev lower_statweight upper_statweight"
     )
     translist = []
     with Path(filename).open() as fnist:
         for line in fnist:
             row = line.split("|")
             if len(row) == 17 and "-" in row[5]:
-                if len(row[0].strip()) > 0:
+                if row[0].strip():
                     lambda_angstroms = float(row[0])
-                elif len(row[1].strip()) > 0:
+                elif row[1].strip():
                     lambda_angstroms = float(row[1])
                 else:
                     continue
-                A = float(row[3]) if len(row[3].strip()) > 0 else 1e8
+                A = float(row[3]) if row[3].strip() else 1e8
                 lower_energy_ev, upper_energy_ev = (float(x.strip(" []")) for x in row[5].split("-"))
-                lower_g, upper_g = (float(x.strip()) for x in row[12].split("-"))
+                lower_statweight, upper_statweight = (float(x.strip()) for x in row[12].split("-"))
                 translist.append(
-                    transitiontuple(lambda_angstroms, A, lower_energy_ev, upper_energy_ev, lower_g, upper_g)
+                    transitiontuple(
+                        lambda_angstroms, A, lower_energy_ev, upper_energy_ev, lower_statweight, upper_statweight
+                    )
                 )
 
     return pd.DataFrame(translist, columns=transitiontuple._fields)
 
 
 def generate_ion_spectrum(transitions, xvalues, popcolumn, plot_resolution, args):
     yvalues = np.zeros(len(xvalues))
@@ -177,15 +187,15 @@
 
 
 def add_upper_lte_pop(dftransitions, T_exc, ionpop, ltepartfunc, columnname=None) -> pd.DataFrame:
     K_B = const.k_B.to("eV / K").value  # noqa: F841
     scalefactor = ionpop / ltepartfunc  # noqa: F841
     if columnname is None:
         columnname = f"upper_pop_lte_{T_exc:.0f}K"
-    return dftransitions.eval(f"{columnname} = @scalefactor * upper_g * exp(-upper_energy_ev / @K_B / @T_exc)")
+    return dftransitions.eval(f"{columnname} = @scalefactor * upper_statweight * exp(-upper_energy_ev / @K_B / @T_exc)")
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=None, type=Path, help="Path to ARTIS folder")
 
     parser.add_argument("-xmin", type=int, default=3500, help="Plot range: minimum wavelength in Angstroms")
 
@@ -205,17 +215,17 @@
 
     parser.add_argument("-timestep", "-ts", type=int, default=70, help="Timestep number to plot")
 
     parser.add_argument("-modelgridindex", "-cell", type=int, default=0, help="Modelgridindex to plot")
 
     parser.add_argument("--normalised", action="store_true", help="Normalise all spectra to their peak values")
 
-    parser.add_argument(
-        "--print-lines", action="store_true", help="Output details of matching line details to standard out"
-    )
+    parser.add_argument("--print-lines", action="store_true", help="Output details of matching lines to standard out")
+
+    parser.add_argument("--save-lines", action="store_true", help="Output details of all lines to transitionlines.txt")
 
     parser.add_argument(
         "--atomicdatabase",
         default="artis",
         choices=["artis", "kurucz", "nist"],
         help="Source of atomic data for excitation transitions",
     )
@@ -313,15 +323,15 @@
 
         Te = estimators["Te"]
         TR = estimators["TR"]
         figure_title = f"{modelname}\n"
         figure_title += (
             f"Cell {modelgridindex} ({velocity} km/s) with Te = {Te:.1f} K, TR = {TR:.1f} K at timestep {timestep}"
         )
-        time_days = float(at.get_timestep_time(modelpath, timestep))
+        time_days = at.get_timestep_time(modelpath, timestep)
         if time_days != -1:
             figure_title += f" ({time_days:.1f}d)"
 
         # -1 means use NLTE populations
         temperature_list = ["Te", "TR", "NOTEMPNLTE"]
         temperature_list = ["NOTEMPNLTE"]
         vardict = {"Te": Te, "TR": TR}
@@ -341,21 +351,21 @@
 
         # Fe3overFe2 = 8  # number ratio
         # ionpopdict = {
         #     (26, 2): 1 / (1 + Fe3overFe2),
         #     (26, 3): Fe3overFe2 / (1 + Fe3overFe2),
         #     (28, 2): 1.0e-2,
         # }
-        ionpopdict = {ion: 1 for ion in ionlist}
+        ionpopdict = dict.fromkeys(ionlist, 1)
 
     hc = (const.h * const.c).to("eV Angstrom").value  # noqa: F841
 
     xvalues = np.arange(args.xmin, args.xmax, step=plot_resolution)
     yvalues = np.zeros((len(temperature_list) + 1, len(ionlist), len(xvalues)))
-
+    dftransitions_all = None
     fe2depcoeff, ni2depcoeff = None, None
     for _, ion in adata.iterrows() if args.atomicdatabase == "artis" else enumerate(ionlist):
         ionid = iontuple(ion.Z, ion.ion_stage)
         if ionid not in ionlist:
             continue
 
         ionindex = ionlist.index(ionid)
@@ -377,31 +387,42 @@
             print(f"  ({len(ion.transitions):6d} forbidden)")
 
         if not dftransitions.empty:
             if args.atomicdatabase == "artis":
                 dftransitions = dftransitions.eval("upper_energy_ev = @ion.levels.loc[upper].energy_ev.to_numpy()")
                 dftransitions = dftransitions.eval("lower_energy_ev = @ion.levels.loc[lower].energy_ev.to_numpy()")
                 dftransitions = dftransitions.eval("lambda_angstroms = @hc / (upper_energy_ev - lower_energy_ev)")
+                dftransitions["upper_level"] = [ion.levels.loc[upper].levelname for upper in dftransitions["upper"]]
+                dftransitions["lower_level"] = [ion.levels.loc[lower].levelname for lower in dftransitions["lower"]]
 
-            dftransitions = dftransitions.query(
-                "lambda_angstroms >= @plot_xmin_wide & lambda_angstroms <= @plot_xmax_wide"
-            )
+            # dftransitions = dftransitions.query(
+            #     "lambda_angstroms >= @plot_xmin_wide & lambda_angstroms <= @plot_xmax_wide"
+            # )
 
             dftransitions = dftransitions.sort_values(by="lambda_angstroms")
 
             print(f"  {len(dftransitions)} plottable transitions")
 
             if args.atomicdatabase == "artis":
-                dftransitions = dftransitions.eval("upper_g = @ion.levels.loc[upper].g.to_numpy()")
+                dftransitions["lower_statweight"] = [ion.levels.loc[lower].g for lower in dftransitions["lower"]]
+                dftransitions = dftransitions.eval("upper_statweight = @ion.levels.loc[upper].g.to_numpy()")
                 K_B = const.k_B.to("eV / K").value
                 T_exc = vardict["Te"]
                 ltepartfunc = ion.levels.eval("g * exp(-energy_ev / @K_B / @T_exc)").sum()
             else:
                 ltepartfunc = 1.0
 
+            if args.save_lines:
+                dftransitions["Z"] = ion.Z
+                dftransitions["ion_stage"] = ion.ion_stage
+                if dftransitions_all is None:
+                    dftransitions_all = dftransitions
+                else:
+                    dftransitions_all = pd.concat([dftransitions_all, dftransitions])
+
             dftransitions = dftransitions.eval("flux_factor = (upper_energy_ev - lower_energy_ev) * A")
             dftransitions = add_upper_lte_pop(
                 dftransitions, vardict["Te"], ionpopdict[ionid], ltepartfunc, columnname="upper_pop_Te"
             )
 
             for seriesindex, temperature in enumerate(temperature_list):
                 if temperature == "NOTEMPNLTE":
@@ -427,15 +448,15 @@
 
                     with pd.option_context("display.width", 200):
                         print(dftransitions.nlargest(1, "flux_factor_nlte"))
                 else:
                     T_exc = vardict[temperature]
                     popcolumnname = f"upper_pop_lte_{T_exc:.0f}K"
                     if args.atomicdatabase == "artis":
-                        dftransitions = dftransitions.eval("upper_g = @ion.levels.loc[upper].g.to_numpy()")
+                        dftransitions = dftransitions.eval("upper_statweight = @ion.levels.loc[upper].g.to_numpy()")
                         K_B = const.k_B.to("eV / K").value  # noqa: F841
                         ltepartfunc = ion.levels.eval("g * exp(-energy_ev / @K_B / @T_exc)").sum()
                     else:
                         ltepartfunc = 1.0
                     dftransitions = add_upper_lte_pop(
                         dftransitions, T_exc, ionpopdict[ionid], ltepartfunc, columnname=popcolumnname
                     )
@@ -447,21 +468,43 @@
                     dftransitions, xvalues, popcolumnname, plot_resolution, args
                 )
                 if args.normalised:
                     yvalues[seriesindex][ionindex] /= max(yvalues[seriesindex][ionindex])  # TODO: move to ax.plot line
 
         if args.print_lines:
             print(dftransitions.columns)
-            print(
-                dftransitions[
-                    ["lower", "upper", "forbidden", "A", "lambda_angstroms", "flux_factor_upper_pop_lte_3000K"]
-                ].to_string(index=False)
-            )
+            print(dftransitions[["lower", "upper", "forbidden", "A", "lambda_angstroms"]].to_string(index=False))
     print()
 
+    if args.save_lines:
+        from tabulate import tabulate
+
+        assert dftransitions_all is not None
+        dftransitions_all = dftransitions_all[dftransitions_all["A"] > 0]
+        dftransitions_all = dftransitions_all.rename(
+            {"lower_energy_ev": "lower_energy_Ev", "upper_energy_ev": "upper_energy_Ev"}, axis=1
+        )
+        dftransitions_all = dftransitions_all.astype({"forbidden": "int32"})
+        dftransitions_all["lambda_angstroms"] /= 1.0003
+        dftransitions_all = dftransitions_all.sort_values(by=["Z", "ion_stage", "lower", "upper"], ascending=True)
+        dftransitions_all = dftransitions_all[
+            "lambda_angstroms A            Z   ion_stage lower_energy_Ev   lower_statweight  forbidden  lower_level               upper_level               upper_statweight  upper_energy_Ev".split()
+        ]
+        print(dftransitions_all)
+        # dftransitions_all.to_csv("transitions.txt", index=False, sep=" ")
+        content = tabulate(dftransitions_all.to_numpy().tolist(), list(dftransitions_all.columns), tablefmt="plain")
+        # print(content)
+
+        outpath = (
+            Path(args.outputfile).parent if Path(args.outputfile).suffix else Path(args.outputfile)
+        ) / "transitionlines.txt"
+        print(f"Writing {outpath}")
+        with outpath.open("w") as f:
+            f.write(content)
+
     if from_model:
         feions = [2, 3]
 
         def get_strionfracs(atomic_number, ion_stages):
             elsym = at.get_elsymbol(atomic_number)
             est_ionfracs = [
                 estimators[f"nnion_{at.get_ionstring(atomic_number, ion_stage, sep='_', style='spectral')}"]
```

### Comparing `artistools-2024.2.22.2/artistools/viewing_angles_visualization.py` & `artistools-2024.4.23/artistools/viewing_angles_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         import plotly.express as px
         import plotly.graph_objects as go
     except ModuleNotFoundError:
         print("Cannot run visualization without plotly...")
         sys.exit()
 
     # Load model contents
-    dfmodel, modelmeta = at.get_modeldata(modelfile, derived_cols=["pos_mid"])
+    dfmodel, _modelmeta = at.get_modeldata(modelfile, derived_cols=["pos_mid"])
     x, y, z = (dfmodel[f"pos_{ax}_mid"].to_numpy() for ax in ("x", "y", "z"))
     rho = dfmodel["rho"].to_numpy()
 
     if isomin is None:
         isomin = min(rho.flatten())
     if isomax is None:
         isomax = max(rho.flatten())
```

### Comparing `artistools-2024.2.22.2/artistools/writecomparisondata.py` & `artistools-2024.4.23/artistools/writecomparisondata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """Tools to get artis output in the required format for the code comparison workshop."""
 
-
 import argparse
 import math
 import typing as t
 from io import TextIOWrapper
 from pathlib import Path
 
 import numpy as np
@@ -47,17 +46,17 @@
             )
 
         outfile.close()
 
 
 def write_ntimes_nvel(outfile: TextIOWrapper, selected_timesteps: t.Sequence[int], modelpath: str | Path) -> None:
     times = at.get_timestep_times(modelpath)
-    modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
+    _, modelmeta = at.inputmodel.get_modeldata(modelpath, getheadersonly=True)
     outfile.write(f"#NTIMES: {len(selected_timesteps)}\n")
-    outfile.write(f"#NVEL: {len(modeldata)}\n")
+    outfile.write(f"#NVEL: {modelmeta['npts_model']}\n")
     outfile.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
 
 
 def write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist, outfile, keyname) -> None:
     modeldata, _modelmeta = at.inputmodel.get_modeldata(modelpath, derived_cols=["vel_r_min_kmps"])
     with Path(outfile).open("w") as f:
         write_ntimes_nvel(f, selected_timesteps, modelpath)
@@ -209,15 +208,14 @@
 
     args.outputpath.mkdir(parents=True, exist_ok=True)
 
     for modelpath in modelpathlist:
         model_id = str(modelpath.name).split("_")[0]
         print(f"{model_id=}")
 
-        modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
         estimators = at.estimators.read_estimators(modelpath=modelpath)
         allnonemptymgilist = list({modelgridindex for ts, modelgridindex in estimators if ts == selected_timesteps[0]})
 
         try:
             write_lbol_edep(
                 modelpath,
                 model_id,
```

### Comparing `artistools-2024.2.22.2/artistools.egg-info/SOURCES.txt` & `artistools-2024.4.23/artistools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artistools-2024.2.22.2/pyproject.toml` & `artistools-2024.4.23/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 dynamic = ["version", "dependencies"]
 requires-python = ">=3.10"
 license = {text = "MIT"}
 readme = {file = "README.md", content-type='text/markdown'}
 
 [project.urls]
-Repository ="https://www.github.com/artis-mcrt/artistools/"
+Repository ="https://www.github.com/artis-mcrt/artistools"
 
 [project.scripts]
 #atcompletions = "artistoolscompletions.sh"
 at = 'artistools:main'
 artistools = 'artistools:main'
 makeartismodel1dslicefromcone = 'artistools.inputmodel.slice1dfromconein3dmodel:main'
 makeartismodel = 'artistools.inputmodel.makeartismodel:main'
@@ -50,14 +50,15 @@
 plotartisviewingangles = 'artistools.viewing_angles_visualization:main'
 
 [tool.black]
 line-length = 120
 target-versions = ["py310", "py311", "py312"]
 
 [tool.mypy]
+local_partial_types = true
 check_untyped_defs = false
 disallow_any_explicit = false
 disallow_any_generics = false
 disallow_any_unimported = false
 disallow_incomplete_defs = false
 disallow_subclassing_any = false
 disallow_untyped_calls = false
@@ -162,19 +163,31 @@
 [tool.pyright]
 exclude=['**/node_modules','**/__pycache__','**/.*', 'build', 'dist']
 useLibraryCodeForTypes = false
 
 [tool.pytest.ini_options]
 addopts = " --durations=0 --typeguard-packages=artistools -n auto"
 
+[tool.refurb]
+ignore = ["FURB120"]
+quiet = false
+enable_all = true
+python_version = "3.10"
+sort_by = "error"
+
+[[tool.refurb.amend]]
+path = "./artistools/inputmodel/fromcmfgen/rd_cmfgen.py"
+ignore = ["FURB108"]
+
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 fix = true
 show-fixes = true
+extend-exclude = ["_version.py"]
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "ARG001", # ignored because variables in df.eval() are not detected
     "ANN",
     "B005",  # strip-with-multi-characters
@@ -198,14 +211,18 @@
     "FBT",
     "FIX002",  # line contains TODO
     "ISC001", # single-line-implicit-string-concatenation
     "N802",  # Function name should be lowercase
     "N803",  # Argument name should be lowercase
     "N806",  # non-lowercase-variable-in-function
     "N999",  # invalid-module-name
+    "PLC0415", # import-outside-toplevel
+    "PLR0914", # too-many-locals
+    "PLR0917", # too-many-positional
+    "PLR1702", # too-many-nested-blocks
     "PD901",  # df is a bad variable name
     "PERF203", # try-except-in-loop
     #"PGH001",  # No builtin `eval()` allowed
     "PLR0911",  # too-many-return-statements
     "PLR0912",  # too-many-branches
     "PLR0913",  # too-many-arguments
     "PLR0915",  # too-many-statements
```

### Comparing `artistools-2024.2.22.2/requirements.txt` & `artistools-2024.4.23/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-argcomplete>=3.2.2
-astropy>=6.0.0
-coverage>=7.4.2
+argcomplete>=3.3.0
+astropy>=6.0.1
+coverage>=7.4.4
 extinction>=0.4.6
-imageio>=2.34.0
-matplotlib>=3.8.3
-mypy>=1.8.0
+imageio>=2.34.1
+matplotlib>=3.8.4
+mypy>=1.9.0
+numexpr>=2.10.0
 numpy>=1.26.4
-pandas[compression,consortium-standard,parquet,performance]>=2.2.0
-polars>=0.20.10
-pre-commit>=3.6.2
-pyarrow>=15.0.0
+pandas[compression,parquet,pyarrow]>=2.2.2
+polars>=0.20.22
+pre-commit>=3.7.0
+pyarrow>=16.0.0
 pynonthermal>=2024.2.17
 pypdf2>=3.0.1
-pytest>=8.0.1
-pytest-cov>=4.1.0
+pytest>=8.1.1
+pytest-cov>=5.0.0
 pytest-xdist[psutil]>=3.5.0
 python-xz>=0.5
-pyvista>=0.43.3
+pyvista>=0.43.5
 PyYAML>=6.0.1
-pyzstd>=0.15.9
-ruff>=0.2.2
-scipy>=1.12.0
+pyzstd>=0.15.10
+ruff>=0.4.1
+scipy>=1.13.0
 setuptools_scm[toml]>=8.0.4
-typeguard>=4.1.5
-types-PyYAML>=6.0.12.12
+tabulate>=0.9
+typeguard>=4.2.1
+types-PyYAML>=6.0.12.20240311
+types-tabulate>=0.9.0.20240106
 #vtk>=9.2.3
-uv>=0.1.7
-wheel>=0.42.0
+wheel>=0.43.0
```

