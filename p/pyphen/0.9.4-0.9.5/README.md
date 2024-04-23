# Comparing `tmp/Pyphen-0.9.4.tar.gz` & `tmp/Pyphen-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Pyphen-0.9.4.tar", last modified: Sun Jan 24 16:12:24 2016, max compression
+gzip compressed data, was "dist/Pyphen-0.9.5.tar", last modified: Fri Aug 24 09:17:42 2018, max compression
```

## Comparing `Pyphen-0.9.4.tar` & `Pyphen-0.9.5.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2016-01-24 16:12:24.000000 Pyphen-0.9.4/
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2016-01-24 16:12:24.000000 Pyphen-0.9.4/Pyphen.egg-info/
--rw-r--r--   0 lize      (1000) lize      (1000)     2951 2016-01-24 16:12:23.000000 Pyphen-0.9.4/Pyphen.egg-info/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)     4854 2016-01-24 16:12:24.000000 Pyphen-0.9.4/Pyphen.egg-info/SOURCES.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        1 2016-01-24 16:12:23.000000 Pyphen-0.9.4/Pyphen.egg-info/dependency_links.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        1 2016-01-06 03:24:08.000000 Pyphen-0.9.4/Pyphen.egg-info/not-zip-safe
--rw-r--r--   0 lize      (1000) lize      (1000)        7 2016-01-24 16:12:23.000000 Pyphen-0.9.4/Pyphen.egg-info/top_level.txt
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2016-01-24 16:12:24.000000 Pyphen-0.9.4/pyphen/
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2016-01-24 16:12:24.000000 Pyphen-0.9.4/pyphen/dictionaries/
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2016-01-24 16:09:55.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_af.dic -> hyph_af_ZA.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    62925 2016-01-24 15:20:23.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_af_ZA.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_bg.dic -> hyph_bg_BG.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    30366 2016-01-24 15:20:28.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_bg_BG.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    18394 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_ca.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_cs.dic -> hyph_cs_CZ.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    20049 2016-01-24 15:20:32.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_cs_CZ.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_da.dic -> hyph_da_DK.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     6049 2016-01-24 15:20:34.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_da_DK.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_de.dic -> hyph_de_DE.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   124645 2016-01-24 15:28:33.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_de_AT.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   124645 2016-01-24 15:28:33.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_de_CH.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   124645 2016-01-24 15:28:33.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_de_DE.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_el.dic -> hyph_el_GR.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     3205 2016-01-24 15:20:40.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_el_GR.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_en.dic -> hyph_en_US.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   107031 2016-01-24 15:20:41.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_en_GB.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_en_Latn_GB.dic -> hyph_en_GB.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_en_Latn_US.dic -> hyph_en_US.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   106414 2016-01-24 15:20:43.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_en_US.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     5580 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_es.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_et.dic -> hyph_et_EE.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    22637 2016-01-24 15:20:46.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_et_EE.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    23253 2016-01-24 15:28:33.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_fr.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     1420 2016-01-24 15:20:49.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_gl.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_hr.dic -> hyph_hr_HR.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     7789 2016-01-24 15:20:54.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_hr_HR.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_hu.dic -> hyph_hu_HU.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   860918 2016-01-24 15:20:55.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_hu_HU.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    50011 2016-01-24 15:21:00.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_is.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_it.dic -> hyph_it_IT.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     2158 2016-01-24 15:21:01.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_it_IT.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_lt.dic -> hyph_lt_LT.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     7817 2016-01-24 15:21:04.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_lt_LT.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_lv.dic -> hyph_lv_LV.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    79409 2016-01-24 15:21:06.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_lv_LV.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nb.dic -> hyph_nb_NO.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   186678 2016-01-24 15:21:10.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nb_NO.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nl.dic -> hyph_nl_NL.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   116507 2016-01-24 15:21:08.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nl_NL.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nn.dic -> hyph_nn_NO.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   186678 2016-01-24 15:21:12.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_nn_NO.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pl.dic -> hyph_pl_PL.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    37931 2016-01-24 15:21:15.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pl_PL.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pt.dic -> hyph_pt_PT.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    10293 2016-01-24 15:21:16.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_BR.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_Latn_BR.dic -> hyph_pt_BR.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_Latn_PT.dic -> hyph_pt_PT.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     1288 2016-01-24 15:21:18.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_PT.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_ro.dic -> hyph_ro_RO.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    34597 2016-01-24 15:21:19.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_ro_RO.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_ru.dic -> hyph_ru_RU.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    22071 2016-01-24 15:21:20.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_ru_RU.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sk.dic -> hyph_sk_SK.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    18205 2016-01-24 15:21:23.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sk_SK.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sl.dic -> hyph_sl_SI.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     8245 2016-01-24 15:21:24.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sl_SI.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    27355 2016-01-24 15:21:27.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sr.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    28392 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sr_Latn.dic
--rw-r--r--   0 lize      (1000) lize      (1000)   102979 2016-01-24 15:21:28.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_sv.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_te.dic -> hyph_te_IN.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     1592 2016-01-24 15:21:31.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_te_IN.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_uk.dic -> hyph_uk_UA.dic
--rw-r--r--   0 lize      (1000) lize      (1000)    20222 2016-01-24 15:21:33.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_uk_UA.dic
-lrwxrwxrwx   0 lize      (1000) lize      (1000)        0 2015-10-30 15:15:48.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_zu.dic -> hyph_zu_ZA.dic
--rw-r--r--   0 lize      (1000) lize      (1000)     1956 2016-01-24 15:21:36.000000 Pyphen-0.9.4/pyphen/dictionaries/hyph_zu_ZA.dic
--rwxr-xr-x   0 lize      (1000) lize      (1000)    10375 2016-01-08 00:31:47.000000 Pyphen-0.9.4/pyphen/__init__.py
--rw-r--r--   0 lize      (1000) lize      (1000)      402 2015-10-30 15:15:48.000000 Pyphen-0.9.4/COPYING
--rw-r--r--   0 lize      (1000) lize      (1000)    18325 2015-10-30 15:15:48.000000 Pyphen-0.9.4/COPYING.GPL
--rw-r--r--   0 lize      (1000) lize      (1000)    26532 2015-10-30 15:15:48.000000 Pyphen-0.9.4/COPYING.LGPL
--rw-r--r--   0 lize      (1000) lize      (1000)    56815 2015-10-30 15:15:48.000000 Pyphen-0.9.4/COPYING.MPL
--rw-r--r--   0 lize      (1000) lize      (1000)      105 2016-01-08 00:05:49.000000 Pyphen-0.9.4/MANIFEST.in
--rw-r--r--   0 lize      (1000) lize      (1000)     1236 2015-10-30 15:15:48.000000 Pyphen-0.9.4/README
--rwxr-xr-x   0 lize      (1000) lize      (1000)     1608 2016-01-24 16:10:09.000000 Pyphen-0.9.4/setup.py
--rw-r--r--   0 lize      (1000) lize      (1000)     2951 2016-01-24 16:12:24.000000 Pyphen-0.9.4/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)       88 2016-01-24 16:12:24.000000 Pyphen-0.9.4/setup.cfg
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2018-08-24 09:17:42.000000 Pyphen-0.9.5/
+-rw-r--r--   0 lize      (1000) lize      (1000)      402 2015-10-30 15:15:48.000000 Pyphen-0.9.5/COPYING
+-rw-r--r--   0 lize      (1000) lize      (1000)    18325 2015-10-30 15:15:48.000000 Pyphen-0.9.5/COPYING.GPL
+-rw-r--r--   0 lize      (1000) lize      (1000)    26532 2015-10-30 15:15:48.000000 Pyphen-0.9.5/COPYING.LGPL
+-rw-r--r--   0 lize      (1000) lize      (1000)    56815 2015-10-30 15:15:48.000000 Pyphen-0.9.5/COPYING.MPL
+-rw-r--r--   0 lize      (1000) lize      (1000)      105 2016-01-08 00:05:49.000000 Pyphen-0.9.5/MANIFEST.in
+-rw-r--r--   0 lize      (1000) lize      (1000)     2851 2018-08-24 09:17:42.000000 Pyphen-0.9.5/PKG-INFO
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2018-08-24 09:17:41.000000 Pyphen-0.9.5/Pyphen.egg-info/
+-rw-r--r--   0 lize      (1000) lize      (1000)     2851 2018-08-24 09:17:41.000000 Pyphen-0.9.5/Pyphen.egg-info/PKG-INFO
+-rw-r--r--   0 lize      (1000) lize      (1000)     4889 2018-08-24 09:17:41.000000 Pyphen-0.9.5/Pyphen.egg-info/SOURCES.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)        1 2018-08-24 09:17:41.000000 Pyphen-0.9.5/Pyphen.egg-info/dependency_links.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)        1 2016-01-06 03:24:08.000000 Pyphen-0.9.5/Pyphen.egg-info/not-zip-safe
+-rw-r--r--   0 lize      (1000) lize      (1000)        7 2018-08-24 09:17:41.000000 Pyphen-0.9.5/Pyphen.egg-info/top_level.txt
+-rw-r--r--   0 lize      (1000) lize      (1000)     1236 2015-10-30 15:15:48.000000 Pyphen-0.9.5/README
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2018-08-24 09:17:41.000000 Pyphen-0.9.5/pyphen/
+-rwxr-xr-x   0 lize      (1000) lize      (1000)    10375 2016-01-08 00:31:47.000000 Pyphen-0.9.5/pyphen/__init__.py
+drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2018-08-24 09:17:42.000000 Pyphen-0.9.5/pyphen/dictionaries/
+-rw-r--r--   0 lize      (1000) lize      (1000)    62925 2018-08-24 09:07:13.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_af.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    62925 2018-08-24 09:07:13.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_af_ZA.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    59388 2018-08-24 09:07:20.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_bg.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    59388 2018-08-24 09:07:20.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_bg_BG.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    18394 2015-10-30 15:15:48.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_ca.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    20049 2018-08-24 09:07:30.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_cs.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    20049 2018-08-24 09:07:30.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_cs_CZ.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     6049 2018-08-24 09:07:32.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_da.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     6049 2018-08-24 09:07:32.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_da_DK.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)  1093611 2018-08-24 09:07:41.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_de.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)  1093611 2018-08-24 09:07:35.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_de_AT.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)  1093611 2018-08-24 09:07:38.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_de_CH.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)  1093611 2018-08-24 09:07:41.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_de_DE.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     3205 2018-08-24 09:07:45.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_el.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     3205 2018-08-24 09:07:45.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_el_GR.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   106414 2018-08-24 09:07:49.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_en.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   107031 2018-08-24 09:07:47.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_en_GB.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   107031 2018-08-24 09:07:47.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_en_Latn_GB.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   106414 2018-08-24 09:07:49.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_en_Latn_US.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   106414 2018-08-24 09:07:49.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_en_US.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     3657 2018-08-24 09:07:52.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_es.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    22637 2018-08-24 09:07:55.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_et.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    22637 2018-08-24 09:07:55.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_et_EE.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    23253 2018-08-24 09:07:57.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_fr.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1420 2018-08-24 09:08:01.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_gl.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     7789 2018-08-24 09:08:08.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_hr.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     7789 2018-08-24 09:08:08.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_hr_HR.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   860918 2018-08-24 09:08:10.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_hu.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   860918 2018-08-24 09:08:10.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_hu_HU.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   104072 2018-08-24 09:08:13.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_id_ID.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    50011 2018-08-24 09:08:16.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_is.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     2158 2018-08-24 09:08:19.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_it.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     2158 2018-08-24 09:08:19.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_it_IT.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     7817 2018-08-24 09:08:23.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_lt.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     7817 2018-08-24 09:08:23.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_lt_LT.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    79409 2018-08-24 09:08:25.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_lv.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    79409 2018-08-24 09:08:25.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_lv_LV.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   186678 2018-08-24 09:08:32.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nb.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   186678 2018-08-24 09:08:32.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nb_NO.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   116507 2018-08-24 09:08:29.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nl.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   116507 2018-08-24 09:08:29.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nl_NL.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   186678 2018-08-24 09:08:34.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nn.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   186678 2018-08-24 09:08:34.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_nn_NO.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    37931 2018-08-24 09:08:39.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pl.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    37931 2018-08-24 09:08:39.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pl_PL.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1288 2018-08-24 09:08:44.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pt.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    10293 2018-08-24 09:08:41.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pt_BR.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    10293 2018-08-24 09:08:41.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pt_Latn_BR.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1288 2018-08-24 09:08:44.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pt_Latn_PT.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1288 2018-08-24 09:08:44.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_pt_PT.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    34597 2018-08-24 09:08:46.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_ro.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    34597 2018-08-24 09:08:46.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_ro_RO.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    22071 2018-08-24 09:08:49.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_ru.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    22071 2018-08-24 09:08:49.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_ru_RU.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    18205 2018-08-24 09:08:52.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sk.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    18205 2018-08-24 09:08:52.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sk_SK.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     8245 2018-08-24 09:08:55.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sl.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     8245 2018-08-24 09:08:55.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sl_SI.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    27355 2018-08-24 09:08:59.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sr.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    28392 2018-08-24 09:08:58.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sr_Latn.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)   102979 2018-08-24 09:09:01.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_sv.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1592 2018-08-24 09:09:05.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_te.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1592 2018-08-24 09:09:05.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_te_IN.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    20222 2018-08-24 09:09:10.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_uk.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)    20222 2018-08-24 09:09:10.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_uk_UA.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1956 2018-08-24 09:09:14.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_zu.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)     1956 2018-08-24 09:09:14.000000 Pyphen-0.9.5/pyphen/dictionaries/hyph_zu_ZA.dic
+-rw-r--r--   0 lize      (1000) lize      (1000)       67 2018-08-24 09:17:42.000000 Pyphen-0.9.5/setup.cfg
+-rwxr-xr-x   0 lize      (1000) lize      (1000)     1518 2018-08-24 09:14:23.000000 Pyphen-0.9.5/setup.py
```

### Comparing `Pyphen-0.9.4/Pyphen.egg-info/PKG-INFO` & `Pyphen-0.9.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Pyphen
-Version: 0.9.4
+Version: 0.9.5
 Summary: Pure Python module to hyphenate text
 Home-page: https://github.com/Kozea/Pyphen
 Author: Guillaume Ayoub
 Author-email: guillaume.ayoub@kozea.fr
 License: UNKNOWN
 Description: Pyphen
         ======
@@ -59,20 +59,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: License :: OSI Approved :: Mozilla Public License 1.1 (MPL 1.1)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Provides: pyphen
```

### Comparing `Pyphen-0.9.4/Pyphen.egg-info/SOURCES.txt` & `Pyphen-0.9.5/Pyphen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 pyphen/dictionaries/hyph_et_EE.dic
 pyphen/dictionaries/hyph_fr.dic
 pyphen/dictionaries/hyph_gl.dic
 pyphen/dictionaries/hyph_hr.dic
 pyphen/dictionaries/hyph_hr_HR.dic
 pyphen/dictionaries/hyph_hu.dic
 pyphen/dictionaries/hyph_hu_HU.dic
+pyphen/dictionaries/hyph_id_ID.dic
 pyphen/dictionaries/hyph_is.dic
 pyphen/dictionaries/hyph_it.dic
 pyphen/dictionaries/hyph_it_IT.dic
 pyphen/dictionaries/hyph_lt.dic
 pyphen/dictionaries/hyph_lt_LT.dic
 pyphen/dictionaries/hyph_lv.dic
 pyphen/dictionaries/hyph_lv_LV.dic
```

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_af_ZA.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_af.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_ca.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_ca.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_cs_CZ.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_cs.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_da_DK.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_da.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_el_GR.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_el.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_en_GB.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_en_GB.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_en_US.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_en.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_et_EE.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_et.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_fr.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_fr.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_gl.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_gl.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_hr_HR.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_hr.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_hu_HU.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_hu.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_is.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_is.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_it_IT.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_it.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_lt_LT.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_lt.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_lv_LV.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_lv.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_nb_NO.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_nb.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_nl_NL.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_nl.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_nn_NO.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_nb_NO.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_pl_PL.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_pl.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_BR.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_pt_BR.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_pt_PT.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_pt.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_ro_RO.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_ro.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_ru_RU.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_ru.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_sk_SK.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_sk.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_sl_SI.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_sl.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_sr.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_sr.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_sr_Latn.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_sr_Latn.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_sv.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_sv.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_te_IN.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_te.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_uk_UA.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_uk.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/dictionaries/hyph_zu_ZA.dic` & `Pyphen-0.9.5/pyphen/dictionaries/hyph_zu.dic`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/pyphen/__init__.py` & `Pyphen-0.9.5/pyphen/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/COPYING.GPL` & `Pyphen-0.9.5/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/COPYING.LGPL` & `Pyphen-0.9.5/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/COPYING.MPL` & `Pyphen-0.9.5/COPYING.MPL`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/README` & `Pyphen-0.9.5/README`

 * *Files identical despite different names*

### Comparing `Pyphen-0.9.4/setup.py` & `Pyphen-0.9.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,29 @@
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
     'License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)',
     'License :: OSI Approved :: Mozilla Public License 1.1 (MPL 1.1)',
     'Programming Language :: Python',
     'Programming Language :: Python :: 2',
-    'Programming Language :: Python :: 2.6',
     'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.1',
-    'Programming Language :: Python :: 3.2',
-    'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: Implementation :: CPython',
     'Programming Language :: Python :: Implementation :: PyPy',
     'Topic :: Text Processing',
     'Topic :: Text Processing :: Linguistic',
 ]
 
 setup(
     name='Pyphen',
-    version='0.9.4',
+    version='0.9.5',
     provides=['pyphen'],
     packages=['pyphen'],
     package_data={'pyphen': [os.path.join(
         os.path.dirname(__file__), 'dictionaries', '*.dic')]},
     include_package_data=True,
     author='Guillaume Ayoub',
     author_email='guillaume.ayoub@kozea.fr',
```

### Comparing `Pyphen-0.9.4/PKG-INFO` & `Pyphen-0.9.5/Pyphen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Pyphen
-Version: 0.9.4
+Version: 0.9.5
 Summary: Pure Python module to hyphenate text
 Home-page: https://github.com/Kozea/Pyphen
 Author: Guillaume Ayoub
 Author-email: guillaume.ayoub@kozea.fr
 License: UNKNOWN
 Description: Pyphen
         ======
@@ -59,20 +59,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: License :: OSI Approved :: Mozilla Public License 1.1 (MPL 1.1)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Provides: pyphen
```

