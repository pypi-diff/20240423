# Comparing `tmp/nkululeko-0.81.6.tar.gz` & `tmp/nkululeko-0.81.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.81.6.tar", last modified: Mon Apr 22 11:56:19 2024, max compression
+gzip compressed data, was "nkululeko-0.81.7.tar", last modified: Tue Apr 23 12:15:35 2024, max compression
```

## Comparing `nkululeko-0.81.6.tar` & `nkululeko-0.81.7.tar`

### file list

```diff
@@ -1,226 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16764 2024-04-22 09:11:55.000000 nkululeko-0.81.6/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.6/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34905 2024-04-22 11:56:19.551355 nkululeko-0.81.6/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.6/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.6/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.6/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.6/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.6/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.6/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.6/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.6/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.6/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.6/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.6/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.6/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.6/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.6/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.6/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.6/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.6/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.6/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.6/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.6/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.6/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.6/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.6/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.6/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.6/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.81.6/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.6/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.6/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.6/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.6/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.6/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.81.6/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.6/meta/demos/demo_best_model.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/meta/demos/multiple_exeriments/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.6/meta/demos/multiple_exeriments/do_experiments.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.6/meta/demos/multiple_exeriments/parse_nkulu.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.6/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.6/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.6/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.543355 nkululeko-0.81.6/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.6/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.6/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.6/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.6/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.6/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.6/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.6/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.6/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.6/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-22 09:11:06.000000 nkululeko-0.81.6/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.6/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.81.6/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.6/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.6/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29576 2024-04-22 11:37:24.000000 nkululeko-0.81.6/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.6/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.6/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3043 2024-04-18 12:11:23.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3083 2024-04-22 11:33:57.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3109 2024-04-22 11:25:34.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-04-22 09:19:06.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4150 2024-04-22 11:34:20.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3037 2024-04-22 09:16:13.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4504 2024-04-22 11:25:07.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.6/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.81.6/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3814 2024-04-22 11:30:38.000000 nkululeko-0.81.6/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.6/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.6/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.6/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.6/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.6/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.6/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9335 2024-04-17 13:01:44.000000 nkululeko-0.81.6/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.547355 nkululeko-0.81.6/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.6/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.81.6/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.6/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.81.6/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.6/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.6/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.6/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.6/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.81.6/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.81.6/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.81.6/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.6/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.6/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.6/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.6/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.6/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5825 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.6/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.6/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/predict.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12427 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/reporter.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.6/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.6/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.6/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.6/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.6/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.81.6/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.81.6/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.6/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.6/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.6/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.6/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.6/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.6/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1525 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2753 2024-04-22 11:13:11.000000 nkululeko-0.81.6/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.6/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.6/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.81.6/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.6/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34905 2024-04-22 11:56:19.000000 nkululeko-0.81.6/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5127 2024-04-22 11:56:19.000000 nkululeko-0.81.6/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-22 11:56:19.000000 nkululeko-0.81.6/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-22 11:56:19.000000 nkululeko-0.81.6/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-22 11:56:19.000000 nkululeko-0.81.6/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.6/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-22 11:56:19.551355 nkululeko-0.81.6/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.6/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.539355 nkululeko-0.81.6/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-22 11:56:19.551355 nkululeko-0.81.6/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.6/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16840 2024-04-23 12:15:09.000000 nkululeko-0.81.7/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.7/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34981 2024-04-23 12:15:35.274922 nkululeko-0.81.7/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.7/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.262922 nkululeko-0.81.7/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.7/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.7/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.7/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.7/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.7/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.7/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.7/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.7/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.7/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.7/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.7/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.7/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.7/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.7/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.7/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.7/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.7/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.7/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.7/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.7/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.7/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.7/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.7/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.7/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.81.7/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.7/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.7/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.7/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.7/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.7/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.262922 nkululeko-0.81.7/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.81.7/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.262922 nkululeko-0.81.7/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.7/meta/demos/demo_best_model.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.266922 nkululeko-0.81.7/meta/demos/multiple_exeriments/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.7/meta/demos/multiple_exeriments/do_experiments.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.7/meta/demos/multiple_exeriments/parse_nkulu.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.7/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.7/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.7/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.270922 nkululeko-0.81.7/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.7/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.7/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.7/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.270922 nkululeko-0.81.7/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.7/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.7/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.7/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.7/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.7/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.270922 nkululeko-0.81.7/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.7/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.7/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-23 09:17:12.000000 nkululeko-0.81.7/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.270922 nkululeko-0.81.7/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.7/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.81.7/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.7/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3264 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.7/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4755 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29576 2024-04-22 11:37:24.000000 nkululeko-0.81.7/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2310 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.7/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.7/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3346 2024-04-16 13:29:59.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5289 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-23 09:51:49.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4528 2024-04-23 10:02:24.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3319 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5285 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4604 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-04-23 11:35:51.000000 nkululeko-0.81.7/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.81.7/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.81.7/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.81.7/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.7/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.7/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.7/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.7/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.7/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.7/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9335 2024-04-17 13:01:44.000000 nkululeko-0.81.7/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.7/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11569 2024-04-17 13:01:47.000000 nkululeko-0.81.7/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.7/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9726 2024-04-16 11:54:29.000000 nkululeko-0.81.7/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.7/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.7/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.7/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.7/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9107 2024-04-16 11:54:31.000000 nkululeko-0.81.7/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10083 2024-04-16 13:48:13.000000 nkululeko-0.81.7/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      914 2024-04-17 12:17:54.000000 nkululeko-0.81.7/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.7/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.7/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.7/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.7/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.7/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5825 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.7/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.7/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/predict.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12427 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/reporter.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.7/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.7/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.7/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.7/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.7/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12670 2024-04-16 13:43:47.000000 nkululeko-0.81.7/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.81.7/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.7/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.7/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.7/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.7/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.7/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.7/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1525 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2753 2024-04-22 11:13:11.000000 nkululeko-0.81.7/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.7/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.7/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.81.7/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.7/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34981 2024-04-23 12:15:35.000000 nkululeko-0.81.7/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5167 2024-04-23 12:15:35.000000 nkululeko-0.81.7/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-23 12:15:35.000000 nkululeko-0.81.7/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-04-23 12:15:35.000000 nkululeko-0.81.7/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-23 12:15:35.000000 nkululeko-0.81.7/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.7/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-04-23 12:15:35.274922 nkululeko-0.81.7/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.7/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.262922 nkululeko-0.81.7/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-23 12:15:35.274922 nkululeko-0.81.7/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.7/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.81.6/CHANGELOG.md` & `nkululeko-0.81.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.81.7
+--------------
+* bugfixes
+* added whisper feature extractor
+
 Version 0.81.6
 --------------
 * updated documentation
 * updated crema-d
 * updated tests
 
 Version 0.81.5
```

### Comparing `nkululeko-0.81.6/LICENSE` & `nkululeko-0.81.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/PKG-INFO` & `nkululeko-0.81.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.6
+Version: 0.81.7
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -319,14 +319,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.7
+--------------
+* bugfixes
+* added whisper feature extractor
+
 Version 0.81.6
 --------------
 * updated documentation
 * updated crema-d
 * updated tests
 
 Version 0.81.5
```

### Comparing `nkululeko-0.81.6/README.md` & `nkululeko-0.81.7/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/aesdd/process_database.py` & `nkululeko-0.81.7/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/androids/process_database.py` & `nkululeko-0.81.7/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/androids_orig/process_database.py` & `nkululeko-0.81.7/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/androids_test/process_database.py` & `nkululeko-0.81.7/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/ased/process_database.py` & `nkululeko-0.81.7/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/asvp-esd/process_database.py` & `nkululeko-0.81.7/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/baved/process_database.py` & `nkululeko-0.81.7/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/cafe/process_database.py` & `nkululeko-0.81.7/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/clac/process_database.py` & `nkululeko-0.81.7/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/cmu-mosei/process_database.py` & `nkululeko-0.81.7/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/demos/process_database.py` & `nkululeko-0.81.7/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/ekorpus/process_database.py` & `nkululeko-0.81.7/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emns/process_database.py` & `nkululeko-0.81.7/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emofilm/convert_to_16k.py` & `nkululeko-0.81.7/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emofilm/process_database.py` & `nkululeko-0.81.7/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emorynlp/process_database.py` & `nkululeko-0.81.7/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emov-db/process_database.py` & `nkululeko-0.81.7/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emovo/process_database.py` & `nkululeko-0.81.7/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/emozionalmente/create.py` & `nkululeko-0.81.7/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/enterface/process_database.py` & `nkululeko-0.81.7/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/esd/process_database.py` & `nkululeko-0.81.7/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/gerparas/process_database.py` & `nkululeko-0.81.7/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/iemocap/process_database.py` & `nkululeko-0.81.7/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/jl/process_database.py` & `nkululeko-0.81.7/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/jtes/process_database.py` & `nkululeko-0.81.7/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/meld/process_database.py` & `nkululeko-0.81.7/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/mesd/process_database.py` & `nkululeko-0.81.7/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/mess/process_database.py` & `nkululeko-0.81.7/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/mlendsnd/process_database.py` & `nkululeko-0.81.7/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/msp-improv/process_database2.py` & `nkululeko-0.81.7/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/msp-podcast/process_database.py` & `nkululeko-0.81.7/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/oreau2/process_database.py` & `nkululeko-0.81.7/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/portuguese/process_database.py` & `nkululeko-0.81.7/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/ravdess/process_database.py` & `nkululeko-0.81.7/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/ravdess/process_database_speaker.py` & `nkululeko-0.81.7/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/savee/process_database.py` & `nkululeko-0.81.7/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/shemo/process_database.py` & `nkululeko-0.81.7/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/subesco/process_database.py` & `nkululeko-0.81.7/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/tess/process_database.py` & `nkululeko-0.81.7/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/thorsten-emotional/process_database.py` & `nkululeko-0.81.7/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/urdu/process_database.py` & `nkululeko-0.81.7/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/data/vivae/process_database.py` & `nkululeko-0.81.7/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/docs/source/conf.py` & `nkululeko-0.81.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/demo_best_model.py` & `nkululeko-0.81.7/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/multiple_exeriments/do_experiments.py` & `nkululeko-0.81.7/meta/demos/multiple_exeriments/do_experiments.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/multiple_exeriments/parse_nkulu.py` & `nkululeko-0.81.7/meta/demos/multiple_exeriments/parse_nkulu.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/my_experiment.py` & `nkululeko-0.81.7/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/my_experiment_local.py` & `nkululeko-0.81.7/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/meta/demos/plot_faster_anim.py` & `nkululeko-0.81.7/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/aug_train.py` & `nkululeko-0.81.7/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/augment.py` & `nkululeko-0.81.7/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/augmenting/augmenter.py` & `nkululeko-0.81.7/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.81.7/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.81.7/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/augmenting/resampler.py` & `nkululeko-0.81.7/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_age.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.81.7/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.81.7/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/cacheddataset.py` & `nkululeko-0.81.7/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/data/dataset.py` & `nkululeko-0.81.7/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/data/dataset_csv.py` & `nkululeko-0.81.7/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/demo.py` & `nkululeko-0.81.7/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/demo_feats.py` & `nkululeko-0.81.7/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/demo_predictor.py` & `nkululeko-0.81.7/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/experiment.py` & `nkululeko-0.81.7/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/explore.py` & `nkululeko-0.81.7/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/export.py` & `nkululeko-0.81.7/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_agender.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 import audeer
 import nkululeko.glob_conf as glob_conf
 import audonnx
 import numpy as np
 import audinterface
 
 
-class AudModelAgenderSet(Featureset):
+class AgenderSet(Featureset):
     """
     Embeddings from the wav2vec2. based model finetuned on agender data, described in the paper
     "Speech-based Age and Gender Prediction with Transformers"
     https://arxiv.org/abs/2306.16962
     """
 
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type):
+        super().__init__(name, data_df, feats_type)
         self.model_loaded = False
+        self.feats_type = feats_type
 
     def _load_model(self):
         model_url = "https://zenodo.org/record/7761387/files/w2v2-L-robust-6-age-gender.25c844af-1.1.1.zip"
         model_root = self.util.config_val(
             "FEATS", "agender.model", "./audmodel_agender/"
         )
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir("cache")
             model_root = audeer.mkdir(model_root)
-            archive_path = audeer.download_url(model_url, cache_root, verbose=True)
+            archive_path = audeer.download_url(
+                model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
         device = self.util.config_val("MODEL", "device", "cpu")
         self.model = audonnx.load(model_root, device=device)
         self.util.debug(f"initialized agender model")
         self.model_loaded = True
 
     def extract(self):
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_auddim.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,27 @@
     """Emotional dimensions from the wav2vec2 model finetuned on MSPPodcast emotions.
 
     Described in the paper
     "Dawn of the transformer era in speech emotion recognition: closing the valence gap"
     https://arxiv.org/abs/2203.07378.
     """
 
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type):
+        super().__init__(name, data_df, feats_type)
         self.model_loaded = False
+        self.feats_types = feats_type
 
     def _load_model(self):
         model_url = "https://zenodo.org/record/6221127/files/w2v2-L-robust-12.6bc4a7fd-1.1.0.zip"
         model_root = self.util.config_val("FEATS", "aud.model", "./audmodel/")
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir("cache")
             model_root = audeer.mkdir(model_root)
-            archive_path = audeer.download_url(model_url, cache_root, verbose=True)
+            archive_path = audeer.download_url(
+                model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
         cuda = "cuda" if torch.cuda.is_available() else "cpu"
         device = self.util.config_val("MODEL", "device", cuda)
         self.model = audonnx.load(model_root, device=device)
         self.model_loaded = True
 
     def extract(self):
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_audmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,27 @@
     """Embeddings from the wav2vec2 based model finetuned on MSPPodcast emotions.
 
     Described in the paper:
     "Dawn of the transformer era in speech emotion recognition: closing the valence gap"
     https://arxiv.org/abs/2203.07378.
     """
 
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type):
+        super().__init__(name, data_df, feats_type)
         self.model_loaded = False
+        self.feats_type = feats_type
 
     def _load_model(self):
         model_url = "https://zenodo.org/record/6221127/files/w2v2-L-robust-12.6bc4a7fd-1.1.0.zip"
         model_root = self.util.config_val("FEATS", "aud.model", "./audmodel/")
         if not os.path.isdir(model_root):
             cache_root = audeer.mkdir("cache")
             model_root = audeer.mkdir(model_root)
-            archive_path = audeer.download_url(model_url, cache_root, verbose=True)
+            archive_path = audeer.download_url(
+                model_url, cache_root, verbose=True)
             audeer.extract_archive(archive_path, model_root)
         cuda = "cuda" if torch.cuda.is_available() else "cpu"
         device = self.util.config_val("MODEL", "device", cuda)
         self.model = audonnx.load(model_root, device=device)
         self.model_loaded = True
 
     def extract(self):
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_clap.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,55 +7,59 @@
 from tqdm import tqdm
 import os
 import nkululeko.glob_conf as glob_conf
 import laion_clap
 import audiofile
 
 
-class Clap(Featureset):
+class ClapSet(Featureset):
     """Class to extract laion's clap embeddings (https://github.com/LAION-AI/CLAP)"""
 
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feats_type):
         """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feats_type)
         self.device = self.util.config_val("MODEL", "device", "cpu")
         self.model_initialized = False
+        self.feat_type = feats_type
 
     def init_model(self):
         # load model
         self.util.debug("loading clap model...")
         self.model = laion_clap.CLAP_Module(enable_fusion=False)
         self.model.load_ckpt()  # download the default pretrained checkpoint.
         print(f"loaded clap model")
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path("store")
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
         storage = f"{store}{self.name}.{store_format}"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
-            self.util.debug("extracting clap embeddings, this might take a while...")
+            self.util.debug(
+                "extracting clap embeddings, this might take a while...")
             emb_series = pd.Series(index=self.data_df.index, dtype=object)
             length = len(self.data_df.index)
             for idx, (file, start, end) in enumerate(
                 tqdm(self.data_df.index.to_list())
             ):
                 signal, sampling_rate = audiofile.read(
                     file,
                     offset=start.total_seconds(),
                     duration=(end - start).total_seconds(),
                     always_2d=True,
                 )
                 emb = self.get_embeddings(signal, sampling_rate)
                 emb_series[idx] = emb
-            self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index)
+            self.df = pd.DataFrame(
+                emb_series.values.tolist(), index=self.data_df.index)
             self.util.write_store(self.df, storage, store_format)
             try:
                 glob_conf.config["DATA"]["needs_feature_extraction"] = "false"
             except KeyError:
                 pass
         else:
             self.util.debug("reusing extracted wav2vec2 embeddings")
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_hubert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # feats_hubert.py
 # HuBERT feature extractor for Nkululeko
-# example feat_type = "hubert-large-ll60k", "hubert-xlarge-ll60k"
+# example feat_type = "hubert-large-ll60k", "hubert-xlarge-ll60k",
+# "hubert-base-ls960", hubert-large-ls960-ft", "hubert-xlarge-ls960-ft"
 
 
 import os
 
 import audeer
 import nkululeko.glob_conf as glob_conf
 import pandas as pd
@@ -18,15 +19,15 @@
 
 class Hubert(Featureset):
     """Class to extract HuBERT embedding)"""
 
     def __init__(self, name, data_df, feat_type):
         """Constructor. is_train is needed to distinguish from test/dev sets,
         because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feat_type)
         # check if device is not set, use cuda if available
         cuda = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = self.util.config_val("MODEL", "device", cuda)
         self.model_initialized = False
         self.feat_type = feat_type
 
     def init_model(self):
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_import.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from nkululeko.utils.util import Util
 from nkululeko.feat_extract.featureset import Featureset
 
 
 class ImportSet(Featureset):
     """Class to import features that have been compiled elsewhere"""
 
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type):
+        super().__init__(name, data_df, feats_type)
 
     def extract(self):
         """Import the features."""
         self.util.debug(f"importing features for {self.name}")
         try:
             feat_import_files = self.util.config_val("FEATS", "import_file", False)
             feat_import_files = ast.literal_eval(feat_import_files)
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_mos.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from nkululeko.utils.util import Util
 from nkululeko.feat_extract.featureset import Featureset
 
 
 class MosSet(Featureset):
     """Class to predict MOS (mean opinion score)"""
 
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feats_type):
         """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feats_type)
         self.device = self.util.config_val("MODEL", "device", "cpu")
         self.model_initialized = False
 
     def init_model(self):
         # load model
         self.util.debug("loading MOS model...")
         self.subjective_model = SQUIM_SUBJECTIVE.get_model()
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_opensmile.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,53 +4,41 @@
 import pandas as pd
 import nkululeko.glob_conf as glob_conf
 import ast
 import opensmile
 
 
 class Opensmileset(Featureset):
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type=None, config_file=None):
+        super().__init__(name, data_df, feats_type)
         self.featset = self.util.config_val("FEATS", "set", "eGeMAPSv02")
         try:
             self.feature_set = eval(f"opensmile.FeatureSet.{self.featset}")
-            #'eGeMAPSv02, ComParE_2016, GeMAPSv01a, eGeMAPSv01a':
+            # 'eGeMAPSv02, ComParE_2016, GeMAPSv01a, eGeMAPSv01a':
         except AttributeError:
-            self.util.error(
-                f"something is wrong with feature set: {self.featset}"
-            )
+            self.util.error(f"something is wrong with feature set: {self.featset}")
         self.featlevel = self.util.config_val("FEATS", "level", "functionals")
         try:
-            self.featlevel = self.featlevel.replace(
-                "lld", "LowLevelDescriptors"
-            )
-            self.featlevel = self.featlevel.replace(
-                "functionals", "Functionals"
-            )
-            self.feature_level = eval(
-                f"opensmile.FeatureLevel.{self.featlevel}"
-            )
+            self.featlevel = self.featlevel.replace("lld", "LowLevelDescriptors")
+            self.featlevel = self.featlevel.replace("functionals", "Functionals")
+            self.feature_level = eval(f"opensmile.FeatureLevel.{self.featlevel}")
         except AttributeError:
-            self.util.error(
-                f"something is wrong with feature level: {self.featlevel}"
-            )
+            self.util.error(f"something is wrong with feature level: {self.featlevel}")
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path("store")
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
         storage = f"{store}{self.name}.{store_format}"
         extract = eval(
             self.util.config_val("FEATS", "needs_feature_extraction", "False")
         )
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or not os.path.isfile(storage) or no_reuse:
-            self.util.debug(
-                "extracting openSmile features, this might take a while..."
-            )
+            self.util.debug("extracting openSmile features, this might take a while...")
             smile = opensmile.Smile(
                 feature_set=self.feature_set,
                 feature_level=self.feature_level,
                 num_workers=5,
                 verbose=True,
             )
             if isinstance(self.data_df.index, pd.MultiIndex):
@@ -81,17 +69,15 @@
         # use only the features that are indexed in the target dataframes
         self.df = self.df[self.df.index.isin(self.data_df.index)]
         try:
             # use only some features
             selected_features = ast.literal_eval(
                 glob_conf.config["FEATS"]["os.features"]
             )
-            self.util.debug(
-                f"selecting features from opensmile: {selected_features}"
-            )
+            self.util.debug(f"selecting features from opensmile: {selected_features}")
             sel_feats_df = pd.DataFrame()
             hit = False
             for feat in selected_features:
                 try:
                     sel_feats_df[feat] = self.df[feat]
                     hit = True
                 except KeyError:
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_oxbow.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 import pandas as pd
 import opensmile
 
 
 class Openxbow(Featureset):
     """Class to extract openXBOW processed opensmile features (https://github.com/openXBOW)"""
 
-    def __init__(self, name, data_df, is_train=False):
+    def __init__(self, name, data_df, feats_type, is_train=False):
         """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feats_type)
+        self.feats_types = feats_type
         self.is_train = is_train
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         self.featset = self.util.config_val("FEATS", "set", "eGeMAPSv02")
         self.feature_set = eval(f"opensmile.FeatureSet.{self.featset}")
         store = self.util.get_path("store")
         storage = f"{store}{self.name}_{self.featset}.pkl"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             # extract smile features first
-            self.util.debug("extracting openSmile features, this might take a while...")
+            self.util.debug(
+                "extracting openSmile features, this might take a while...")
             smile = opensmile.Smile(
                 feature_set=self.feature_set,
                 feature_level=opensmile.FeatureLevel.LowLevelDescriptors,
                 num_workers=5,
             )
             if isinstance(self.data_df.index, pd.MultiIndex):
                 is_multi_index = True
@@ -44,33 +47,35 @@
                 "llds.csv",
                 "xbow.csv",
                 "xbow_codebook",
             )
             # save the smile features
             smile_df.to_csv(lld_name, sep=";", header=False)
             # get the path of the xbow java jar file
-            xbow_path = self.util.config_val("FEATS", "xbow.model", "../openXBOW/")
+            xbow_path = self.util.config_val(
+                "FEATS", "xbow.model", "openXBOW")
+            # check if JAR file exist
+            if not os.path.isfile(f"{xbow_path}/openXBOW.jar"):
+                # download using wget if not exist and locate in xbow_path
+                os.system(
+                    f"git clone https://github.com/openXBOW/openXBOW")
             # get the size of the codebook
             size = self.util.config_val("FEATS", "size", 500)
             # get the number of assignements
             assignments = self.util.config_val("FEATS", "assignments", 10)
             # differentiate between train and test
             if self.is_train:
                 # store the codebook
                 os.system(
-                    f"java -jar {xbow_path}openXBOW.jar -i"
-                    f" {lld_name} -standardizeInput -log                     -o"
-                    f" {xbow_name} -size {size} -a {assignments} -B"
-                    f" {codebook_name}"
+                    f"java -jar {xbow_path}/openXBOW.jar -i {lld_name} -standardizeInput -log -o {xbow_name} -size {size} -a {assignments} -B {codebook_name}"
                 )
             else:
                 # use the codebook
                 os.system(
-                    f"java -jar {xbow_path}openXBOW.jar -i {lld_name}          "
-                    f"           -o {xbow_name} -b {codebook_name}"
+                    f"java -jar {xbow_path}/openXBOW.jar -i {lld_name} -o {xbow_name} -b {codebook_name}"
                 )
             # read in the result from disk
             xbow_df = pd.read_csv(xbow_name, sep=";", header=None)
             # set the index
             xbow_df = xbow_df.set_index(self.data_df.index)
             # check if smile features should be added
             with_os = self.util.config_val("FEATS", "with_os", False)
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_praat.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     """A feature extractor for the Praat software.
 
     Based on David R. Feinberg's Praat scripts for the parselmouth python interface.
     https://osf.io/6dwr3/
 
     """
 
-    def __init__(self, name, data_df):
-        super().__init__(name, data_df)
+    def __init__(self, name, data_df, feats_type):
+        super().__init__(name, data_df, feats_type)
 
     def extract(self):
         """Extract the features based on the initialized dataset or re-open them when found on disk."""
         store = self.util.get_path("store")
         store_format = self.util.config_val("FEATS", "store_format", "pkl")
         storage = f"{store}{self.name}.{store_format}"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
-            self.util.debug("extracting Praat features, this might take a while...")
+            self.util.debug(
+                "extracting Praat features, this might take a while...")
             self.df = feinberg_praat.compute_features(self.data_df.index)
             self.df = self.df.set_index(self.data_df.index)
             for i, col in enumerate(self.df.columns):
                 if self.df[col].isnull().values.any():
                     self.util.debug(
                         f"{col} includes {self.df[col].isnull().sum()} nan,"
                         " inserting mean values"
@@ -48,15 +50,16 @@
         else:
             self.util.debug(f"reusing extracted Praat features: {storage}.")
             self.df = self.util.get_store(storage, store_format)
         self.util.debug(f"praat feature names: {self.df.columns}")
         self.df = self.df.astype(float)
 
     def extract_sample(self, signal, sr):
-        import audiofile, audformat
+        import audiofile
+        import audformat
 
         tmp_audio_names = ["praat_audio_tmp.wav"]
         audiofile.write(tmp_audio_names[0], signal, sr)
         df = pd.DataFrame(index=tmp_audio_names)
         index = audformat.utils.to_segmented_index(df.index, allow_nat=False)
         df = feinberg_praat.compute_features(index)
         df.set_index(index)
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 feats_spectra.py
 
 Inspired by code from Su Lei
 
 """
+
 import os
 import torchaudio
 import torchaudio.transforms as T
 import torch
 from torch.utils.data import Dataset
 from PIL import Image, ImageOps
 import pandas as pd
@@ -19,17 +20,17 @@
 
 from nkululeko.feat_extract.featureset import Featureset
 from nkululeko.constants import SAMPLING_RATE
 import nkululeko.glob_conf as glob_conf
 
 
 class Spectraloader(Featureset):
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feat_type):
         """Constructor setting the name"""
-        Featureset.__init__(self, name, data_df)
+        super().__init__(name, data_df, feat_type)
         self.sampling_rate = SAMPLING_RATE
         self.num_bands = int(self.util.config_val("FEATS", "fft_nbands", "64"))
         self.win_dur = int(self.util.config_val("FEATS", "fft_win_dur", "25"))
         self.hop_dur = int(self.util.config_val("FEATS", "fft_hop_dur", "10"))
 
     def extract(self):
         """Extract the features or load them from disk if present."""
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_squim.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 import nkululeko.glob_conf as glob_conf
 from nkululeko.utils.util import Util
 
 
 class SquimSet(Featureset):
     """Class to predict SQUIM features"""
 
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feats_type):
         """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feats_type)
         self.device = self.util.config_val("MODEL", "device", "cpu")
         self.model_initialized = False
 
     def init_model(self):
         # load model
         self.util.debug("loading model...")
         self.objective_model = SQUIM_OBJECTIVE.get_model()
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_trill.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 # feats_trill.py
+import tensorflow_hub as hub
 import os
 import tensorflow as tf
 from numpy.core.numeric import tensordot
 from tqdm import tqdm
 import pandas as pd
 import audiofile as af
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 from nkululeko.feat_extract.featureset import Featureset
 
 # Import TF 2.X and make sure we're running eager.
 assert tf.executing_eagerly()
-import tensorflow_hub as hub
 
 
 class TRILLset(Featureset):
     """A feature extractor for the Google TRILL embeddings"""
 
     """https://ai.googleblog.com/2020/06/improving-speech-representations-and.html"""
 
     # Initialization of the class
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feats_type):
         """
         Initialize the class with name, data and Util instance
         Also loads the model from hub
 
         :param name: Name of the class
         :type name: str
         :param data_df: Data of the class
         :type data_df: DataFrame
         :return: None
         """
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feats_type)
         # Load the model from the configured path
         model_path = self.util.config_val(
             "FEATS",
             "trill.model",
             "https://tfhub.dev/google/nonsemantic-speech-benchmark/trill/3",
         )
         self.module = hub.load(model_path)
+        self.feats_type = feats_type
 
     def extract(self):
         store = self.util.get_path("store")
         storage = f"{store}{self.name}.pkl"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
-            self.util.debug("extracting TRILL embeddings, this might take a while...")
+            self.util.debug(
+                "extracting TRILL embeddings, this might take a while...")
             emb_series = pd.Series(index=self.data_df.index, dtype=object)
             length = len(self.data_df.index)
             for idx, file in enumerate(tqdm(self.data_df.index.get_level_values(0))):
                 emb = self.getEmbeddings(file)
                 emb_series[idx] = emb
-            self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index)
+            self.df = pd.DataFrame(
+                emb_series.values.tolist(), index=self.data_df.index)
             self.df.to_pickle(storage)
             try:
                 glob_conf.config["DATA"]["needs_feature_extraction"] = "false"
             except KeyError:
                 pass
         else:
             self.util.debug("reusing extracted TRILL embeddings")
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
-# feats_wav2vec2.py
-# feat_types example = wav2vec2-large-robust-ft-swbd-300h
+""" feats_wav2vec2.py
+feat_types example = [wav2vec2-large-robust-ft-swbd-300h,
+wav2vec2-xls-r-2b, wav2vec2-large, wav2vec2-large-xlsr-53, wav2vec2-base]
+
+Complete list: https://huggingface.co/facebook?search_models=wav2vec2
+Currently only supports wav2vec2
+"""
+
 import os
 from tqdm import tqdm
 import pandas as pd
 import torch
 import torchaudio
 from transformers import Wav2Vec2FeatureExtractor, Wav2Vec2Model
 import transformers
@@ -12,47 +18,49 @@
 
 
 class Wav2vec2(Featureset):
     """Class to extract wav2vec2 embeddings"""
 
     def __init__(self, name, data_df, feat_type):
         """Constructor. is_train is needed to distinguish from test/dev sets, because they use the codebook from the training"""
-        super().__init__(name, data_df)
+        super().__init__(name, data_df, feat_type)
         cuda = "cuda" if torch.cuda.is_available() else "cpu"
         self.device = self.util.config_val("MODEL", "device", cuda)
         self.model_initialized = False
-        if feat_type == "wav2vec" or feat_type == "wav2vec2":
+        if feat_type == "wav2vec2":
             self.feat_type = "wav2vec2-large-robust-ft-swbd-300h"
         else:
             self.feat_type = feat_type
 
     def init_model(self):
         # load model
         self.util.debug("loading wav2vec2 model...")
         model_path = self.util.config_val(
             "FEATS", "wav2vec2.model", f"facebook/{self.feat_type}"
         )
         config = transformers.AutoConfig.from_pretrained(model_path)
         layer_num = config.num_hidden_layers
-        hidden_layer = int(self.util.config_val("FEATS", "wav2vec2.layer", "0"))
+        hidden_layer = int(self.util.config_val(
+            "FEATS", "wav2vec2.layer", "0"))
         config.num_hidden_layers = layer_num - hidden_layer
         self.util.debug(f"using hidden layer #{config.num_hidden_layers}")
         self.processor = Wav2Vec2FeatureExtractor.from_pretrained(model_path)
         self.model = Wav2Vec2Model.from_pretrained(model_path, config=config).to(
             self.device
         )
         print(f"intialized Wav2vec model on {self.device}")
         self.model.eval()
         self.model_initialized = True
 
     def extract(self):
         """Extract the features or load them from disk if present."""
         store = self.util.get_path("store")
         storage = f"{store}{self.name}.pkl"
-        extract = self.util.config_val("FEATS", "needs_feature_extraction", False)
+        extract = self.util.config_val(
+            "FEATS", "needs_feature_extraction", False)
         no_reuse = eval(self.util.config_val("FEATS", "no_reuse", "False"))
         if extract or no_reuse or not os.path.isfile(storage):
             if not self.model_initialized:
                 self.init_model()
             self.util.debug(
                 "extracting wav2vec2 embeddings, this might take a while..."
             )
@@ -65,15 +73,16 @@
                     frame_offset=int(start.total_seconds() * 16000),
                     num_frames=int((end - start).total_seconds() * 16000),
                 )
                 assert sampling_rate == 16000, f"got {sampling_rate} instead of 16000"
                 emb = self.get_embeddings(signal, sampling_rate, file)
                 emb_series[idx] = emb
             # print(f"emb_series shape: {emb_series.shape}")
-            self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index)
+            self.df = pd.DataFrame(
+                emb_series.values.tolist(), index=self.data_df.index)
             # print(f"df shape: {self.df.shape}")
             self.df.to_pickle(storage)
             try:
                 glob_conf.config["DATA"]["needs_feature_extraction"] = "false"
             except KeyError:
                 pass
         else:
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feats_wavlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,15 @@
                 tqdm(self.data_df.index.to_list())
             ):
                 signal, sampling_rate = torchaudio.load(
                     file,
                     frame_offset=int(start.total_seconds() * 16000),
                     num_frames=int((end - start).total_seconds() * 16000),
                 )
-                if sampling_rate != 16000:
-                    self.util.error(
-                        f"sampling rate should be 16000 but is {sampling_rate}"
-                    )
+                assert sampling_rate == 16000, f"sampling rate should be 16000 but is {sampling_rate}"
                 emb = self.get_embeddings(signal, sampling_rate, file)
                 emb_series.iloc[idx] = emb
             self.df = pd.DataFrame(emb_series.values.tolist(), index=self.data_df.index)
             self.df.to_pickle(storage)
             try:
                 glob_conf.config["DATA"]["needs_feature_extraction"] = "false"
             except KeyError:
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/featureset.py` & `nkululeko-0.81.7/nkululeko/feat_extract/featureset.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 from nkululeko.utils.util import Util
 import nkululeko.glob_conf as glob_conf
 import ast
 
 
 class Featureset:
     name = ""  # designation
-    df = None  # pandas dataframe to store the features (and indexed with the data from the sets)
+    df = None  # pandas dataframe to store the features
+    # (and indexed with the data from the sets)
     data_df = None  # dataframe to get audio paths
 
-    def __init__(self, name, data_df):
+    def __init__(self, name, data_df, feats_type):
         self.name = name
         self.data_df = data_df
         self.util = Util("featureset")
+        self.feats_types = feats_type
 
     def extract(self):
         pass
 
     def filter(self):
         # use only the features that are indexed in the target dataframes
         self.df = self.df[self.df.index.isin(self.data_df.index)]
         try:
             # use only some features
-            selected_features = ast.literal_eval(glob_conf.config["FEATS"]["features"])
+            selected_features = ast.literal_eval(
+                glob_conf.config["FEATS"]["features"])
             self.util.debug(f"selecting features: {selected_features}")
             sel_feats_df = pd.DataFrame()
             hit = False
             for feat in selected_features:
                 try:
                     sel_feats_df[feat] = self.df[feat]
                     hit = True
```

### Comparing `nkululeko-0.81.6/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.81.7/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/feature_extractor.py` & `nkululeko-0.81.7/nkululeko/feature_extractor.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,32 +49,43 @@
         return self.feat_extractor.extract_sample(signal, sr)
 
     def _get_feat_extractor(self, store_name, feats_type):
         feat_extractor_class = self._get_feat_extractor_class(feats_type)
         if feat_extractor_class is None:
             self.util.error(f"unknown feats_type: {feats_type}")
         return feat_extractor_class(
-            f"{store_name}_{self.feats_designation}", self.data_df
+            f"{store_name}_{self.feats_designation}", self.data_df, feats_type
         )
 
     def _get_feat_extractor_class(self, feats_type):
         if feats_type == "os":
             from nkululeko.feat_extract.feats_opensmile import Opensmileset
 
             return Opensmileset
+
         elif feats_type == "spectra":
             from nkululeko.feat_extract.feats_spectra import Spectraloader
 
             return Spectraloader
+
         elif feats_type == "trill":
             from nkululeko.feat_extract.feats_trill import TRILLset
 
             return TRILLset
-        elif feats_type.startswith(("wav2vec", "hubert", "wavlm", "spkrec")):
+
+        elif feats_type.startswith(
+            ("wav2vec2", "hubert", "wavlm", "spkrec", "whisper")
+        ):
             return self._get_feat_extractor_by_prefix(feats_type)
+
+        elif feats_type == "xbow":
+            from nkululeko.feat_extract.feats_oxbow import Openxbow
+
+            return Openxbow
+
         elif feats_type in (
             "audmodel",
             "auddim",
             "agender",
             "agender_agender",
             "snr",
             "mos",
@@ -85,19 +96,19 @@
             "import",
         ):
             return self._get_feat_extractor_by_name(feats_type)
         else:
             return None
 
     def _get_feat_extractor_by_prefix(self, feats_type):
-        prefix, _, ext = feats_type.partition("_")
+        prefix, _, ext = feats_type.partition("-")
         from importlib import import_module
 
         module = import_module(f"nkululeko.feat_extract.feats_{prefix.lower()}")
-        class_name = f"{prefix.capitalize()}{ext.capitalize()}set"
+        class_name = f"{prefix.capitalize()}"
         return getattr(module, class_name)
 
     def _get_feat_extractor_by_name(self, feats_type):
         from importlib import import_module
 
         module = import_module(f"nkululeko.feat_extract.feats_{feats_type.lower()}")
         class_name = f"{feats_type.capitalize()}Set"
```

### Comparing `nkululeko-0.81.6/nkululeko/file_checker.py` & `nkululeko-0.81.7/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/filter_data.py` & `nkululeko-0.81.7/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/losses/loss_ccc.py` & `nkululeko-0.81.7/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.81.7/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/modelrunner.py` & `nkululeko-0.81.7/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model.py` & `nkululeko-0.81.7/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_cnn.py` & `nkululeko-0.81.7/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_gmm.py` & `nkululeko-0.81.7/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_knn.py` & `nkululeko-0.81.7/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_knn_reg.py` & `nkululeko-0.81.7/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_mlp.py` & `nkululeko-0.81.7/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.81.7/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_svm.py` & `nkululeko-0.81.7/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/models/model_svr.py` & `nkululeko-0.81.7/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/multidb.py` & `nkululeko-0.81.7/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/nkululeko.py` & `nkululeko-0.81.7/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/plots.py` & `nkululeko-0.81.7/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/predict.py` & `nkululeko-0.81.7/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporter.py` & `nkululeko-0.81.7/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/defines.py` & `nkululeko-0.81.7/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/latex_writer.py` & `nkululeko-0.81.7/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/report.py` & `nkululeko-0.81.7/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/report_item.py` & `nkululeko-0.81.7/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/reporter.py` & `nkululeko-0.81.7/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/reporting/result.py` & `nkululeko-0.81.7/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/resample.py` & `nkululeko-0.81.7/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/runmanager.py` & `nkululeko-0.81.7/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/scaler.py` & `nkululeko-0.81.7/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/segment.py` & `nkululeko-0.81.7/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.81.7/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.81.7/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/syllable_nuclei.py` & `nkululeko-0.81.7/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/test.py` & `nkululeko-0.81.7/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/test_predictor.py` & `nkululeko-0.81.7/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/utils/files.py` & `nkululeko-0.81.7/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/utils/stats.py` & `nkululeko-0.81.7/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko/utils/util.py` & `nkululeko-0.81.7/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.81.7/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.6
+Version: 0.81.7
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -319,14 +319,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.7
+--------------
+* bugfixes
+* added whisper feature extractor
+
 Version 0.81.6
 --------------
 * updated documentation
 * updated crema-d
 * updated tests
 
 Version 0.81.5
```

### Comparing `nkululeko-0.81.6/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.81.7/nkululeko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 nkululeko/feat_extract/feats_snr.py
 nkululeko/feat_extract/feats_spectra.py
 nkululeko/feat_extract/feats_spkrec.py
 nkululeko/feat_extract/feats_squim.py
 nkululeko/feat_extract/feats_trill.py
 nkululeko/feat_extract/feats_wav2vec2.py
 nkululeko/feat_extract/feats_wavlm.py
+nkululeko/feat_extract/feats_whisper.py
 nkululeko/feat_extract/featureset.py
 nkululeko/feat_extract/feinberg_praat.py
 nkululeko/losses/__init__.py
 nkululeko/losses/loss_ccc.py
 nkululeko/losses/loss_softf1loss.py
 nkululeko/models/__init__.py
 nkululeko/models/model.py
```

### Comparing `nkululeko-0.81.6/setup.cfg` & `nkululeko-0.81.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.6/venv/bin/activate_this.py` & `nkululeko-0.81.7/venv/bin/activate_this.py`

 * *Files identical despite different names*

