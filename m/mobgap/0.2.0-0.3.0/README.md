# Comparing `tmp/mobgap-0.2.0.tar.gz` & `tmp/mobgap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobgap-0.2.0.tar", max compression
+gzip compressed data, was "mobgap-0.3.0.tar", max compression
```

## Comparing `mobgap-0.2.0.tar` & `mobgap-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,76 @@
--rw-r--r--   0        0        0    10817 2024-03-22 17:40:35.938343 mobgap-0.2.0/LICENSE
--rw-r--r--   0        0        0       99 2024-03-22 17:40:35.938343 mobgap-0.2.0/NOTICE
--rw-r--r--   0        0        0     8448 2024-03-22 17:40:35.938343 mobgap-0.2.0/README.md
--rw-r--r--   0        0        0      206 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/__init__.py
--rw-r--r--   0        0        0     2106 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/_docutils.py
--rw-r--r--   0        0        0      316 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/_dmo_thresholds/__init__.py
--rw-r--r--   0        0        0     2807 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/_dmo_thresholds/official_mobilised_dmo_thresholds.csv
--rw-r--r--   0        0        0    17174 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/_mobilised_aggregator.py
--rw-r--r--   0        0        0     7197 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/_threshold_check.py
--rw-r--r--   0        0        0     3081 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/aggregation/base.py
--rw-r--r--   0        0        0      215 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/cad/__init__.py
--rw-r--r--   0        0        0    13664 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/cad/_cad_from_ic.py
--rw-r--r--   0        0        0     3735 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/cad/base.py
--rw-r--r--   0        0        0       76 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/consts.py
--rw-r--r--   0        0        0     1211 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/data/__init__.py
--rw-r--r--   0        0        0     4657 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/data/_dataset_from_data.py
--rw-r--r--   0        0        0     4501 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/data/_example_data.py
--rw-r--r--   0        0        0     2838 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/data/_example_data_registry.txt
--rw-r--r--   0        0        0    21074 2024-03-22 17:40:35.962343 mobgap-0.2.0/mobgap/data/_mobilised_cvs_dmo_dataset.py
--rw-r--r--   0        0        0    45831 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data/_mobilised_matlab_loader.py
--rw-r--r--   0        0        0     2444 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data/_mobilsed_weartime_loader.py
--rw-r--r--   0        0        0     4761 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data/base.py
--rw-r--r--   0        0        0      871 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/__init__.py
--rw-r--r--   0        0        0     3232 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_cwt.py
--rw-r--r--   0        0        0     9238 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_filter.py
--rw-r--r--   0        0        0        0 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_filter_coeffs/__init__.py
--rw-r--r--   0        0        0     2066 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_filter_coeffs/epfl_gait_filter.csv
--rw-r--r--   0        0        0     2445 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_gaussian_filter.py
--rw-r--r--   0        0        0     6502 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_padding.py
--rw-r--r--   0        0        0     4644 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_resample.py
--rw-r--r--   0        0        0     3521 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_savgol_filter.py
--rw-r--r--   0        0        0     1385 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/_utils.py
--rw-r--r--   0        0        0    16333 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/data_transform/base.py
--rw-r--r--   0        0        0      128 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/gsd/__init__.py
--rw-r--r--   0        0        0    14807 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/gsd/_gsd_iluz.py
--rw-r--r--   0        0        0     3056 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/gsd/base.py
--rw-r--r--   0        0        0    23538 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/gsd/evaluation.py
--rw-r--r--   0        0        0      308 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/__init__.py
--rw-r--r--   0        0        0    11444 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/_hklee_algo_improved.py
--rw-r--r--   0        0        0     6857 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/_icd_ionescu.py
--rw-r--r--   0        0        0     9022 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/_shin_algo_improved.py
--rw-r--r--   0        0        0     3182 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/_utils.py
--rw-r--r--   0        0        0     3178 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/base.py
--rw-r--r--   0        0        0    14150 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/icd/evaluation.py
--rw-r--r--   0        0        0      173 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/lrd/__init__.py
--rw-r--r--   0        0        0     4847 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/lrd/_lrd_mccamley.py
--rw-r--r--   0        0        0     3521 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/lrd/base.py
--rw-r--r--   0        0        0      243 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/pipeline/__init__.py
--rw-r--r--   0        0        0    13108 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/pipeline/_gs_iterator.py
--rw-r--r--   0        0        0       41 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/__init__.py
--rw-r--r--   0        0        0       47 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/_filter.py
--rw-r--r--   0        0        0     9553 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/array_handling.py
--rw-r--r--   0        0        0     1146 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/conversions.py
--rw-r--r--   0        0        0     4120 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/dtypes.py
--rw-r--r--   0        0        0    23398 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/evaluation.py
--rw-r--r--   0        0        0     5613 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/utils/interpolation.py
--rw-r--r--   0        0        0      743 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/__init__.py
--rw-r--r--   0        0        0     7113 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_interval_criteria.py
--rw-r--r--   0        0        0     6241 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_stride_selection.py
--rw-r--r--   0        0        0     2096 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_utils.py
--rw-r--r--   0        0        0    18721 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_wb_assembly.py
--rw-r--r--   0        0        0     8192 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_wb_criteria.py
--rw-r--r--   0        0        0     6940 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/_wb_criteria_base.py
--rw-r--r--   0        0        0     5523 2024-03-22 17:40:35.966343 mobgap-0.2.0/mobgap/wba/plot.py
--rw-r--r--   0        0        0     3055 2024-03-22 17:40:35.966343 mobgap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9486 1970-01-01 00:00:00.000000 mobgap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10817 2024-04-23 11:03:58.282380 mobgap-0.3.0/LICENSE
+-rw-r--r--   0        0        0       99 2024-04-23 11:03:58.282380 mobgap-0.3.0/NOTICE
+-rw-r--r--   0        0        0     8448 2024-04-23 11:03:58.282380 mobgap-0.3.0/README.md
+-rw-r--r--   0        0        0      206 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/__init__.py
+-rw-r--r--   0        0        0     2106 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/_docutils.py
+-rw-r--r--   0        0        0      316 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/_dmo_thresholds/__init__.py
+-rw-r--r--   0        0        0     2807 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/_dmo_thresholds/official_mobilised_dmo_thresholds.csv
+-rw-r--r--   0        0        0    17174 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/_mobilised_aggregator.py
+-rw-r--r--   0        0        0     7197 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/_threshold_check.py
+-rw-r--r--   0        0        0     3081 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/aggregation/base.py
+-rw-r--r--   0        0        0      215 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/cad/__init__.py
+-rw-r--r--   0        0        0    13664 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/cad/_cad_from_ic.py
+-rw-r--r--   0        0        0     3735 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/cad/base.py
+-rw-r--r--   0        0        0       76 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/consts.py
+-rw-r--r--   0        0        0     1211 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/__init__.py
+-rw-r--r--   0        0        0     5403 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_dataset_from_data.py
+-rw-r--r--   0        0        0     4501 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_example_data.py
+-rw-r--r--   0        0        0     2838 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_example_data_registry.txt
+-rw-r--r--   0        0        0    21082 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_mobilised_cvs_dmo_dataset.py
+-rw-r--r--   0        0        0    49361 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_mobilised_matlab_loader.py
+-rw-r--r--   0        0        0     2444 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/_mobilsed_weartime_loader.py
+-rw-r--r--   0        0        0     5230 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data/base.py
+-rw-r--r--   0        0        0      871 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/__init__.py
+-rw-r--r--   0        0        0     3232 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_cwt.py
+-rw-r--r--   0        0        0     9238 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_filter.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_filter_coeffs/__init__.py
+-rw-r--r--   0        0        0     2066 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_filter_coeffs/epfl_gait_filter.csv
+-rw-r--r--   0        0        0     2445 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_gaussian_filter.py
+-rw-r--r--   0        0        0     6502 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_padding.py
+-rw-r--r--   0        0        0     4644 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_resample.py
+-rw-r--r--   0        0        0     3521 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_savgol_filter.py
+-rw-r--r--   0        0        0     1385 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/_utils.py
+-rw-r--r--   0        0        0    16333 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/data_transform/base.py
+-rw-r--r--   0        0        0      128 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/gsd/__init__.py
+-rw-r--r--   0        0        0    14811 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/gsd/_gsd_iluz.py
+-rw-r--r--   0        0        0     4779 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/gsd/base.py
+-rw-r--r--   0        0        0    25737 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/gsd/evaluation.py
+-rw-r--r--   0        0        0     6100 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/gsd/pipeline.py
+-rw-r--r--   0        0        0      308 2024-04-23 11:03:58.310380 mobgap-0.3.0/mobgap/icd/__init__.py
+-rw-r--r--   0        0        0    11490 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/_hklee_algo_improved.py
+-rw-r--r--   0        0        0     6883 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/_icd_ionescu.py
+-rw-r--r--   0        0        0     9026 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/_shin_algo_improved.py
+-rw-r--r--   0        0        0     3182 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/_utils.py
+-rw-r--r--   0        0        0     3178 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/base.py
+-rw-r--r--   0        0        0    14415 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/icd/evaluation.py
+-rw-r--r--   0        0        0      234 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/__init__.py
+-rw-r--r--   0        0        0     4894 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_lrc_mccamley.py
+-rw-r--r--   0        0        0    13073 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_lrc_ullrich.py
+-rw-r--r--   0        0        0   396072 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_all_model.gz
+-rw-r--r--   0        0        0      731 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_all_scaler.gz
+-rw-r--r--   0        0        0    47194 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_hc_model.gz
+-rw-r--r--   0        0        0      733 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_hc_scaler.gz
+-rw-r--r--   0        0        0   137433 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_ms_model.gz
+-rw-r--r--   0        0        0      731 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/_ullrich_pretrained_models/msproject_ms_scaler.gz
+-rw-r--r--   0        0        0     5934 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/base.py
+-rw-r--r--   0        0        0     7067 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/lrc/pipeline.py
+-rw-r--r--   0        0        0      243 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/pipeline/__init__.py
+-rw-r--r--   0        0        0    13108 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/pipeline/_gs_iterator.py
+-rw-r--r--   0        0        0       41 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/__init__.py
+-rw-r--r--   0        0        0      662 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/_sklearn_protocol_types.py
+-rw-r--r--   0        0        0     9553 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/array_handling.py
+-rw-r--r--   0        0        0     1150 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/conversions.py
+-rw-r--r--   0        0        0     4120 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/dtypes.py
+-rw-r--r--   0        0        0    23398 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/evaluation.py
+-rw-r--r--   0        0        0     5613 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/utils/interpolation.py
+-rw-r--r--   0        0        0      743 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/__init__.py
+-rw-r--r--   0        0        0     7113 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_interval_criteria.py
+-rw-r--r--   0        0        0     6241 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_stride_selection.py
+-rw-r--r--   0        0        0     2096 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_utils.py
+-rw-r--r--   0        0        0    18721 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_wb_assembly.py
+-rw-r--r--   0        0        0     8192 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_wb_criteria.py
+-rw-r--r--   0        0        0     6940 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/_wb_criteria_base.py
+-rw-r--r--   0        0        0     5523 2024-04-23 11:03:58.314380 mobgap-0.3.0/mobgap/wba/plot.py
+-rw-r--r--   0        0        0     3227 2024-04-23 11:03:58.314380 mobgap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9494 1970-01-01 00:00:00.000000 mobgap-0.3.0/PKG-INFO
```

### Comparing `mobgap-0.2.0/LICENSE` & `mobgap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/README.md` & `mobgap-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/_docutils.py` & `mobgap-0.3.0/mobgap/_docutils.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/aggregation/_dmo_thresholds/official_mobilised_dmo_thresholds.csv` & `mobgap-0.3.0/mobgap/aggregation/_dmo_thresholds/official_mobilised_dmo_thresholds.csv`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/aggregation/_mobilised_aggregator.py` & `mobgap-0.3.0/mobgap/aggregation/_mobilised_aggregator.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/aggregation/_threshold_check.py` & `mobgap-0.3.0/mobgap/aggregation/_threshold_check.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/aggregation/base.py` & `mobgap-0.3.0/mobgap/aggregation/base.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/cad/_cad_from_ic.py` & `mobgap-0.3.0/mobgap/cad/_cad_from_ic.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/cad/base.py` & `mobgap-0.3.0/mobgap/cad/base.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data/__init__.py` & `mobgap-0.3.0/mobgap/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data/_dataset_from_data.py` & `mobgap-0.3.0/mobgap/data/_dataset_from_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         The sampling rate of the IMU data in Hz.
         If you have different sampling rates for different groups, you can pass a dictionary with the group label as
         key and the sampling rate as value.
     _participant_metadata
         Metadata for each group.
         The keys of the dictionary are expected to be the same as the keys of the ``_data`` dictionary.
         The content of the metadata is not specified and can be anything.
+    single_sensor_name
+        The name of the sensor that is considered the "single sensor".
+        The data of this sensor is available via the ``data_ss`` attribute.
+        The name should be a valid key in the ``data`` attribute.
     index_cols
         The name of the index columns.
         If your data keys are tuples, you can pass a list of strings to name the index columns.
     %(general_dataset_args)s
 
     Attributes
     ----------
@@ -53,38 +57,52 @@
 
     See Also
     --------
     %(dataset_see_also)s
 
     """
 
+    _data: dict[KEY_DTYPE, dict[str, pd.DataFrame]]
+    _sampling_rate_hz: Union[float, dict[KEY_DTYPE, float]]
+    _participant_metadata: Optional[dict[KEY_DTYPE, dict[str, Any]]]
+    single_sensor_name: str
+    index_cols: Optional[Union[list[str], str]]
+
     def __init__(
         self,
         _data: dict[KEY_DTYPE, dict[str, pd.DataFrame]],
         _sampling_rate_hz: Union[float, dict[KEY_DTYPE, float]],
         _participant_metadata: Optional[dict[KEY_DTYPE, dict[str, Any]]] = None,
         *,
+        single_sensor_name: str = "LowerBack",
         index_cols: Optional[Union[list[str], str]] = None,
         groupby_cols: Optional[Union[list[str], str]] = None,
         subset_index: Optional[pd.DataFrame] = None,
     ) -> None:
         self._data = _data
         self._sampling_rate_hz = _sampling_rate_hz
         self._participant_metadata = _participant_metadata
+        self.single_sensor_name = single_sensor_name
         self.index_cols = index_cols
 
         super().__init__(groupby_cols=groupby_cols, subset_index=subset_index)
 
     @property
     def data(self) -> IMU_DATA_DTYPE:
         self.assert_is_single(None, "data")
 
         return self._data[self._group_label_correct_format]
 
     @property
+    def data_ss(self) -> pd.DataFrame:
+        self.assert_is_single(None, "data_ss")
+
+        return self.data[self.single_sensor_name]
+
+    @property
     def sampling_rate_hz(self) -> float:
         self.assert_is_single(None, "sampling_rate_hz")
 
         sampling_rate = self._sampling_rate_hz
 
         if isinstance(sampling_rate, (int, float)):
             return sampling_rate
```

### Comparing `mobgap-0.2.0/mobgap/data/_example_data.py` & `mobgap-0.3.0/mobgap/data/_example_data.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data/_example_data_registry.txt` & `mobgap-0.3.0/mobgap/data/_example_data_registry.txt`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data/_mobilised_cvs_dmo_dataset.py` & `mobgap-0.3.0/mobgap/data/_mobilised_cvs_dmo_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                     "Follow-up (T4) – daily mobility": "T4",  # noqa: RUF001
                     "Follow-up (T5) – daily mobility": "T5",  # noqa: RUF001
                     "Follow-up (T6) – daily mobility": "T6",  # noqa: RUF001
                     "Unscheduled Visit (--) – daily mobility": "UV",  # noqa: RUF001
                 }
             )
         )
-        .astype({"participant_id": "string", "visit_type": "string", "measurement_id": int})
+        .astype({"participant_id": "string", "visit_type": "string", "measurement_id": "int64"})
         .set_index(["participant_id", "visit_type"])
     )
 
 
 def _load_dmo_data(
     dmo_path: Path, timezone_per_subject: pd.DataFrame, visit_type: str
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
@@ -417,15 +417,15 @@
                 total=len(filelist),
                 desc="Loading daily weartime reports for participants",
             )
         )
         results = (
             pd.concat(dict(results), names=["measurement_id", "measurement_date"])
             .reset_index()
-            .astype({"measurement_date": "string", "measurement_id": int})
+            .astype({"measurement_date": "string", "measurement_id": "int64"})
         )
 
         results = results.merge(pid_mid_map, on=["measurement_id"])
         return results
 
     def _get_dmo_data(self) -> tuple[pd.DataFrame, pd.DataFrame]:
         return hybrid_cache(self.memory, 1)(_load_dmo_data)(
```

### Comparing `mobgap-0.2.0/mobgap/data/_mobilised_matlab_loader.py` & `mobgap-0.3.0/mobgap/data/_mobilised_matlab_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,34 +15,44 @@
 
 import joblib
 import numpy as np
 import pandas as pd
 import scipy.io as sio
 
 from mobgap._docutils import make_filldoc
-from mobgap.data.base import BaseGaitDatasetWithReference, ReferenceData, base_gait_dataset_docfiller_dict
+from mobgap.data.base import (
+    BaseGaitDatasetWithReference,
+    ReferenceData,
+    base_gait_dataset_docfiller_dict,
+)
 
 T = TypeVar("T")
 
 PathLike = TypeVar("PathLike", str, Path)
 
 matlab_dataset_docfiller = make_filldoc(
     {
         **base_gait_dataset_docfiller_dict,
         "file_loader_args": """
     raw_data_sensor
         Which sensor to load the raw data for. One of "SU", "INDIP", "INDIP2".
         SU is usually the "normal" lower back sensor.
         INDIP and INDIP2 are only available under special circumstances for the Mobilise-D TVS data.
+        Note, that we don't support loading multiple sensors at once.
     reference_system
         When specified, reference gait parameters are loaded using the specified reference system.
     sensor_positions
         Which sensor positions to load the raw data for.
         For "SU", only "LowerBack" is available, but for other sensors, more positions might be available.
         If a sensor position is not available, an error is raised.
+    single_sensor_position
+        The sensor position that is considered the "single sensor".
+        This is the sensor that you expect to be the input to all pipelines and algorithms.
+        For most Mobilise-d datasets, this should be kept at "LowerBack".
+        But, we support using other sensors as well.
     sensor_types
         Which sensor types to load the raw data for.
         This can be used to reduce the amount of data loaded, if only e.g. acc and gyr data is required.
         Some sensors might only have a subset of the available sensor types.
         If a sensor type is not available, it is ignored.
     missing_sensor_error_type
         Whether to throw an error ("raise"), a warning ("warn") or ignore ("ignore") when a sensor is missing.
@@ -119,15 +129,17 @@
     """
 
     imu_data: Optional[dict[str, pd.DataFrame]]
     raw_reference_parameters: Optional[dict[Literal["wb", "lwb"], Any]]
     metadata: MobilisedMetadata
 
 
-def load_mobilised_participant_metadata_file(path: PathLike) -> dict[str, dict[str, Any]]:
+def load_mobilised_participant_metadata_file(
+    path: PathLike,
+) -> dict[str, dict[str, Any]]:
     """Load the participant metadata file (usually called infoForAlgo.mat).
 
     This file contains various metadata about the participant and the measurement setup.
     There should be one file per corresponding data file.
 
     Parameters
     ----------
@@ -221,15 +233,17 @@
                 # Convert acc columns to m/s-2
                 data_per_test_dict[test].imu_data[sensor_position][["acc_x", "acc_y", "acc_z"]] *= 9.81
 
     return data_per_test_dict
 
 
 def _parse_until_test_level(
-    data: sio.matlab.mat_struct, test_level_marker: Sequence[str], _parent_key: tuple[str, ...] = ()
+    data: sio.matlab.mat_struct,
+    test_level_marker: Sequence[str],
+    _parent_key: tuple[str, ...] = (),
 ) -> Iterator[tuple[tuple[str, ...], sio.matlab.mat_struct]]:
     # If one of the test level markers is in the field names, we reached the level of a test.
     if any(marker in data._fieldnames for marker in test_level_marker):
         yield _parent_key, data
         return  # We don't need to parse any further
 
     for key in data._fieldnames:
@@ -343,20 +357,23 @@
                 "for either LWBs/MicroWBs or WBs/ContinuousWalkingPeriods or parsing of the respective data failed."
             ) from e
     else:
         reference_data = None
         meta_data["reference_sampling_rate_hz"] = None
 
     return MobilisedTestData(
-        imu_data=all_imu_data, raw_reference_parameters=reference_data, metadata=MobilisedMetadata(**meta_data)
+        imu_data=all_imu_data,
+        raw_reference_parameters=reference_data,
+        metadata=MobilisedMetadata(**meta_data),
     )
 
 
 def _parse_single_sensor_data(
-    sensor_data: sio.matlab.mat_struct, sensor_types: Sequence[Literal["acc", "gyr", "mag", "bar"]]
+    sensor_data: sio.matlab.mat_struct,
+    sensor_types: Sequence[Literal["acc", "gyr", "mag", "bar"]],
 ) -> pd.DataFrame:
     parsed_data = []
     for sensor_type in sensor_types:
         if (sensor_type_mat := sensor_type.capitalize()) in sensor_data._fieldnames:
             if sensor_type == "bar":
                 column_names = [f"{sensor_type}"]
             else:
@@ -401,15 +418,15 @@
     if isinstance(value, np.ndarray):
         value = value.tolist()
     if not isinstance(value, list):
         return [value]
     return value
 
 
-def parse_reference_parameters(
+def parse_reference_parameters(  # noqa: C901, PLR0915
     ref_data: list[dict[str, Union[str, float, int, np.ndarray]]],
     *,
     ref_sampling_rate_hz: float,
     data_sampling_rate_hz: float,
     relative_to_wb: bool = False,
 ) -> ReferenceData:
     """Parse the reference data (stored per WB) into the per recording data structures used in mobgap.
@@ -464,14 +481,75 @@
 
     """
     walking_bouts = []
     ics = []
     turn_paras = []
     stride_paras = []
 
+    wb_df_dtypes = {
+        "wb_id": "int64",
+        "start": "int64",
+        "end": "int64",
+        "n_strides": "int64",
+        "duration_s": "float64",
+        "length_m": "float64",
+        "avg_speed_mps": "float64",
+        "avg_cadence_spm": "float64",
+        "avg_stride_length_m": "float64",
+        "termination_reason": "string",
+    }
+
+    ic_df_dtypes = {
+        "wb_id": "int64",
+        "step_id": "int64",
+        "ic": "int64",
+        "lr_label": pd.CategoricalDtype(categories=["left", "right"]),
+    }
+
+    turn_df_dtypes = {
+        "wb_id": "int64",
+        "turn_id": "int64",
+        "start": "int64",
+        "end": "int64",
+        "duration_s": "float64",
+        "angle_deg": "float64",
+    }
+
+    stride_df_dtypes = {
+        "wb_id": "int64",
+        "s_id": "int64",
+        "start": "int64",
+        "end": "int64",
+        "duration_s": "float64",
+        "length_m": "float64",
+        "speed_mps": "float64",
+        "stance_time_s": "float64",
+        "swing_time_s": "float64",
+    }
+
+    def _unify_wb_df(df: pd.DataFrame) -> pd.DataFrame:
+        return df.astype(wb_df_dtypes).set_index("wb_id")
+
+    def _unify_ic_df(df: pd.DataFrame) -> pd.DataFrame:
+        return df.reset_index().astype(ic_df_dtypes).set_index(["wb_id", "step_id"])
+
+    def _unify_turn_df(df: pd.DataFrame) -> pd.DataFrame:
+        return df.reset_index().astype(turn_df_dtypes).set_index(["wb_id", "turn_id"])
+
+    def _unify_stride_df(df: pd.DataFrame) -> pd.DataFrame:
+        return df.reset_index().astype(stride_df_dtypes).set_index(["wb_id", "s_id"])
+
+    if len(ref_data) == 0:
+        return ReferenceData(
+            _unify_wb_df(pd.DataFrame(columns=list(wb_df_dtypes.keys()))),
+            _unify_ic_df(pd.DataFrame(columns=list(ic_df_dtypes.keys()))),
+            _unify_turn_df(pd.DataFrame(columns=list(turn_df_dtypes.keys()))),
+            _unify_stride_df(pd.DataFrame(columns=list(stride_df_dtypes.keys()))),
+        )
+
     for wb_id, wb in enumerate(ref_data, start=1):
         walking_bouts.append(
             {
                 "wb_id": wb_id,
                 "start": wb["Start"],
                 "end": wb["End"],
                 "n_strides": int(wb["NumberStrides"]),
@@ -509,68 +587,88 @@
         starts, ends = zip(*_ensure_is_list(wb["Stride_InitialContacts"]))
         stride_paras.append(
             pd.DataFrame.from_dict(
                 {
                     "wb_id": [wb_id] * len(starts),
                     "start": starts,
                     "end": ends,
-                    "duration_s": _ensure_is_list(wb["Stride_Duration"]),
-                    "length_m": _ensure_is_list(wb["Stride_Length"]),
-                    "speed_mps": _ensure_is_list(wb["Stride_Speed"]),
-                    "stance_time_s": _ensure_is_list(wb["Stance_Duration"]),
-                    "swing_time_s": _ensure_is_list(wb["Swing_Duration"]),
+                    # For some reason, the matlab code contains empty arrays to signal a "missing" value in the data
+                    # columns for the Stereiphoto system. We replace them with NaN using `to_numeric`.
+                    "duration_s": pd.to_numeric(_ensure_is_list(wb["Stride_Duration"])),
+                    "length_m": pd.to_numeric(_ensure_is_list(wb["Stride_Length"])),
+                    "speed_mps": pd.to_numeric(_ensure_is_list(wb["Stride_Speed"])),
+                    "stance_time_s": pd.to_numeric(_ensure_is_list(wb["Stance_Duration"])),
+                    "swing_time_s": pd.to_numeric(_ensure_is_list(wb["Swing_Duration"])),
                 }
             )
         )
 
-    walking_bouts = pd.DataFrame.from_records(walking_bouts).set_index("wb_id")
-    walking_bouts[["start", "end"]] = (walking_bouts[["start", "end"]] * data_sampling_rate_hz).round().astype(int)
+    walking_bouts = pd.DataFrame.from_records(walking_bouts)
+    # For some reason, the matlab code contains empty arrays to signal a "missing" value in the data
+    # columns for the Stereiphoto system. We replace them with NaN using `to_numeric`.
+    for col in [
+        "n_strides",
+        "duration_s",
+        "n_strides",
+        "duration_s",
+        "length_m",
+        "avg_speed_mps",
+        "avg_cadence_spm",
+        "avg_stride_length_m",
+    ]:
+        walking_bouts[col] = pd.to_numeric(walking_bouts[col])
+    walking_bouts[["start", "end"]] = (walking_bouts[["start", "end"]] * data_sampling_rate_hz).round()
+
+    walking_bouts = walking_bouts.replace(np.array([]), np.nan)
+    walking_bouts = _unify_wb_df(walking_bouts)
 
     ics = pd.concat(ics, ignore_index=True)
     ics_is_na = ics["ic"].isna()
     ics = ics[~ics_is_na].drop_duplicates()
-    ics["ic"] = (ics["ic"] * data_sampling_rate_hz).round().astype(int)
-    ics.index.name = "step_id"
-    ics = ics.reset_index().set_index(["wb_id", "step_id"])
     # make left-right labels lowercase
     ics["lr_label"] = ics["lr_label"].str.lower()
+    ics.index.name = "step_id"
+    ics["ic"] = (ics["ic"] * data_sampling_rate_hz).round()
+    ics = _unify_ic_df(ics)
 
     turn_paras = pd.concat(turn_paras, ignore_index=True)
     turn_paras.index.name = "turn_id"
-    turn_paras = turn_paras.reset_index().set_index(["wb_id", "turn_id"])
+    turn_paras = _unify_turn_df(turn_paras)
 
     stride_paras = pd.concat(stride_paras, ignore_index=True)
     stride_ics_is_na = stride_paras[["start", "end"]].isna().any(axis=1)
     stride_paras = stride_paras[~stride_ics_is_na]
     # Note: For the INDIP system it seems like start and end are provided in samples already and not in seconds.
     #       I am not sure what the correct behavior is, but we try to handle it to avoid confusion on the user side.
     #       Unfortunately, there is no 100% reliable way to detect this, so we just check if the values are in the IC
     #       list (which seems to be provided in time in all ref systems I have seen).
     #
     # If we assume the values are in samples of the reference system, than we attempt to convert them to samples of the
     # single sensor system.
     # For the INDIP system, that shouldn't matter, as the sampling rates are the same, but hey you can never be too
     # safe.
     assume_stride_paras_in_samples = (
-        (stride_paras["start"] * (data_sampling_rate_hz / ref_sampling_rate_hz)).round().astype(int)
+        (stride_paras["start"] * (data_sampling_rate_hz / ref_sampling_rate_hz)).round().astype("int64")
     )
     # ICs are already converted to samples here -> I.e. if they are not all in here, we assume that the stride
     # parameters are also in seconds not in samples.
     if not assume_stride_paras_in_samples.isin(ics["ic"]).all():
-        stride_paras[["start", "end"]] = (stride_paras[["start", "end"]] * data_sampling_rate_hz).round().astype(int)
+        stride_paras[["start", "end"]] = (
+            (stride_paras[["start", "end"]] * data_sampling_rate_hz).round().astype("int64")
+        )
         # We check again, just to be sure and if they are still not there, we throw an error.
         if not stride_paras["start"].isin(ics["ic"]).all():
             raise ValueError(
                 "There seems to be a mismatch between the provided stride parameters and the provided initial "
                 "contacts of the reference system. "
                 "At least some of the ICs marking the start of a stride are not found in the dedicated IC list."
             )
     else:
         stride_paras[["start", "end"]] = (
-            (stride_paras[["start", "end"]] * (data_sampling_rate_hz / ref_sampling_rate_hz)).round().astype(int)
+            (stride_paras[["start", "end"]] * (data_sampling_rate_hz / ref_sampling_rate_hz)).round().astype("int64")
         )
 
     # We also get the correct LR-label for the stride parameters from the ICs.
     ic_duplicate_as_nan = ics.copy()
     # We set the values to Nan first and then drop one of the duplicates.
     ic_duplicate_as_nan.loc[ics["ic"].duplicated(keep=False), "lr_label"] = pd.NA
     ic_duplicate_as_nan = ic_duplicate_as_nan.drop_duplicates()
@@ -580,15 +678,15 @@
             "This is likely an issue with the reference system you should further investigate. "
             "For now, we set the `lr_label` of the stride corresponding to this IC to Nan. "
             "However, both values still remain in the IC list.",
             stacklevel=2,
         )
     stride_paras["lr_label"] = ic_duplicate_as_nan.set_index("ic").loc[stride_paras["start"], "lr_label"].to_numpy()
     stride_paras.index.name = "s_id"
-    stride_paras = stride_paras.reset_index().set_index(["wb_id", "s_id"])
+    stride_paras = _unify_stride_df(stride_paras)
 
     # Due to the way, on how the data is used on matlab side, we need to adjust the indices of all time values.
     # We need to fix 2 things:
     # 1. In Matlab time value were calculated to samples (as done here), but then used as indices in Matlabs 1-based
     #    indexing. To make them correspond to the 0-based indexing in python, we need to subtract 1 from all values.
     # 2. In Matlab slicing is inclusive, but in python it is exclusive. Hence, we need to add 1 to all end values in
     #    python.
@@ -606,15 +704,19 @@
         turn_paras = _relative_to_gs(turn_paras, walking_bouts, "wb_id", columns_to_cut=["start", "end"])
         stride_paras = _relative_to_gs(stride_paras, walking_bouts, "wb_id", columns_to_cut=["start", "end"])
 
     return ReferenceData(walking_bouts, ics, turn_paras, stride_paras)
 
 
 def _relative_to_gs(
-    event_data: pd.DataFrame, gait_sequences: pd.DataFrame, gs_index_col: str, *, columns_to_cut: Sequence[str]
+    event_data: pd.DataFrame,
+    gait_sequences: pd.DataFrame,
+    gs_index_col: str,
+    *,
+    columns_to_cut: Sequence[str],
 ) -> pd.DataFrame:
     """Convert the start and end values or event values to values relative to the start of GSs or WBs.
 
     Note, that this assumes that the input data already has an index level indicating to which GS/WB the entry belongs
     to.
     It does not check if events are actually within the provided GSs/WBs.
 
@@ -665,34 +767,37 @@
 
     """
 
     raw_data_sensor: Literal["SU", "INDIP", "INDIP2"]
     reference_system: Optional[Literal["INDIP", "Stereophoto"]]
     reference_para_level: Literal["wb", "lwb"]
     sensor_positions: Sequence[str]
+    single_sensor_position: str
     sensor_types: Sequence[Literal["acc", "gyr", "mag", "bar"]]
     memory: joblib.Memory
 
     def __init__(
         self,
         *,
         raw_data_sensor: Literal["SU", "INDIP", "INDIP2"] = "SU",
         reference_system: Optional[Literal["INDIP", "Stereophoto"]] = None,
         reference_para_level: Literal["wb", "lwb"] = "wb",
         sensor_positions: Sequence[str] = ("LowerBack",),
+        single_sensor_position: str = "LowerBack",
         sensor_types: Sequence[Literal["acc", "gyr", "mag", "bar"]] = ("acc", "gyr"),
         missing_sensor_error_type: Literal["raise", "warn", "ignore"] = "raise",
         memory: joblib.Memory = joblib.Memory(None),
         groupby_cols: Optional[Union[list[str], str]] = None,
         subset_index: Optional[pd.DataFrame] = None,
     ) -> None:
         self.raw_data_sensor = raw_data_sensor
         self.reference_system = reference_system
         self.reference_para_level = reference_para_level
         self.sensor_positions = sensor_positions
+        self.single_sensor_position = single_sensor_position
         self.sensor_types = sensor_types
         self.memory = memory
         self.missing_sensor_error_type = missing_sensor_error_type
 
         super().__init__(groupby_cols=groupby_cols, subset_index=subset_index)
 
     @property
@@ -719,14 +824,18 @@
         raise NotImplementedError
 
     @property
     def data(self) -> MobilisedTestData.imu_data:
         return self._load_selected_data("data").imu_data
 
     @property
+    def data_ss(self) -> pd.DataFrame:
+        return self.data[self.single_sensor_position]
+
+    @property
     def raw_reference_parameters_(self) -> MobilisedTestData.raw_reference_parameters:
         if self.reference_system is None:
             raise ValueError(
                 "The raw_reference_parameters_ and all attributes that depend on it are only available, if a reference "
                 "system is specified. "
                 "Specify a reference system when creating the dataset object."
             )
@@ -770,15 +879,17 @@
         participant_metadata = load_mobilised_participant_metadata_file(info_for_algo_file)
 
         first_level_selected_test_name = self.index.iloc[0][next(iter(self._test_level_names))]
 
         return participant_metadata[first_level_selected_test_name]
 
     @property
-    def _cached_data_load(self) -> Callable[[PathLike], dict[tuple[str, ...], MobilisedTestData]]:
+    def _cached_data_load(
+        self,
+    ) -> Callable[[PathLike], dict[tuple[str, ...], MobilisedTestData]]:
         return partial(
             self.memory.cache(load_mobilised_matlab_format),
             raw_data_sensor=self.raw_data_sensor,
             reference_system=self.reference_system,
             sensor_positions=self.sensor_positions,
             sensor_types=self.sensor_types,
             missing_sensor_error_type=self.missing_sensor_error_type,
@@ -842,15 +953,18 @@
                     "We can not distinguish between the files in this case and build a correct index. "
                     "Provide sufficient information that metadata can be loaded for each file. "
                     "How this works depends on the implementation of the Dataset class you are using."
                 )
             return None
 
         metadata_per_level = [
-            {"__path": path, **dict(zip(self._metadata_level_names, self._get_file_index_metadata(path)))}
+            {
+                "__path": path,
+                **dict(zip(self._metadata_level_names, self._get_file_index_metadata(path))),
+            }
             for path in self._paths_list
         ]
         metadata_per_level = pd.DataFrame.from_records(metadata_per_level).set_index("__path")
 
         # We test that the meta data for each path is unique. Otherwise we will run into problems later.
         if metadata_per_level.duplicated().any():
             raise ValueError(
```

### Comparing `mobgap-0.2.0/mobgap/data/_mobilsed_weartime_loader.py` & `mobgap-0.3.0/mobgap/data/_mobilsed_weartime_loader.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data/base.py` & `mobgap-0.3.0/mobgap/data/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,21 @@
     memory
         A joblib memory object to cache the results of the data loading.
         This is highly recommended, if you have many large data files.
         Otherwise, the initial index creation can take a long time.
     """,
     "common_dataset_data_attrs": """
     data
-        The raw IMU data.
+        The raw IMU data of all available sensors.
+        This is a dictionary with the sensor name as key and the data as value.
+    data_ss
+        The IMU data of the "single sensor".
+        Compared to ``data``, this is only just the data of a single sensor.
+        Which sensor is considered the "single sensor" might be different for each dataset.
+        Most datasets use a configuration of ``single_sensor_name=...`` to allow the user to select the sensor.
     sampling_rate_hz
         The sampling rate of the IMU data in Hz.
     participant_metadata
         The participant metadata loaded from the `infoForAlgo.mat` file.
     """,
     "common_dataset_reference_attrs": """
     reference_parameters_
@@ -121,14 +127,15 @@
 
         acc: str = "ms^-2"
         gyr: str = "deg/s"
         mag: str = "uT"
 
     sampling_rate_hz: float
     data: IMU_DATA_DTYPE
+    data_ss: pd.DataFrame
     # TODO: Make that more specific, once we know what metadata is needed for the pipelines
     participant_metadata: dict[str, Any]
 
 
 @base_gait_dataset_docfiller
 class BaseGaitDatasetWithReference(BaseGaitDataset):
     """Base class for all gait datasets that have reference parameters.
```

### Comparing `mobgap-0.2.0/mobgap/data_transform/__init__.py` & `mobgap-0.3.0/mobgap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_cwt.py` & `mobgap-0.3.0/mobgap/data_transform/_cwt.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_filter.py` & `mobgap-0.3.0/mobgap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_filter_coeffs/epfl_gait_filter.csv` & `mobgap-0.3.0/mobgap/data_transform/_filter_coeffs/epfl_gait_filter.csv`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_gaussian_filter.py` & `mobgap-0.3.0/mobgap/data_transform/_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_padding.py` & `mobgap-0.3.0/mobgap/data_transform/_padding.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_resample.py` & `mobgap-0.3.0/mobgap/data_transform/_resample.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_savgol_filter.py` & `mobgap-0.3.0/mobgap/data_transform/_savgol_filter.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/_utils.py` & `mobgap-0.3.0/mobgap/data_transform/_utils.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/data_transform/base.py` & `mobgap-0.3.0/mobgap/data_transform/base.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/gsd/_gsd_iluz.py` & `mobgap-0.3.0/mobgap/gsd/_gsd_iluz.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             np.abs((first_second_mean - last_second_mean) / first_second_mean) <= self.allowed_acc_v_change_per_window
         )
 
         # Now we turn the selected windows into a list of gait sequences
         selected_windows_index = np.where(selected_windows)[0]
         # We initialize an empty array with two columns, where each row represents a gsd. First column is the start
         # index, second column is the end index.
-        gs_list = np.empty((len(selected_windows_index), 2), dtype=int)
+        gs_list = np.empty((len(selected_windows_index), 2), dtype="int64")
         # We convert the window indices to sample indices of the original data
         gs_list[:, 0] = selected_windows_index * (window_length_samples - window_overlap_samples)
         # We add one to make the end index inclusive
         gs_list[:, 1] = gs_list[:, 0] + window_length_samples + 1
 
         # Merge overlapping windows
         gs_list = merge_intervals(gs_list)
```

### Comparing `mobgap-0.2.0/mobgap/gsd/base.py` & `mobgap-0.3.0/mobgap/icd/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""Base class for GSD detectors."""
+"""Base class for ICs detectors."""
 
 from typing import Any
 
 import pandas as pd
 from tpcp import Algorithm
 from typing_extensions import Self, Unpack
 
 from mobgap._docutils import make_filldoc
 
-base_gsd_docfiller = make_filldoc(
+base_icd_docfiller = make_filldoc(
     {
         "other_parameters": """
     data
-        The raw IMU data passed to the ``detect`` method.
+        The raw IMU data of the gait sequence passed to the ``detect`` method.
     sampling_rate_hz
         The sampling rate of the IMU data in Hz passed to the ``detect`` method.
     """,
-        "gs_list_": """
-    gs_list_
-        A dataframe specifying the detected gait sequences.
-        The dataframe has a ``start`` and ``end`` column, specifying the start and end index of the gait sequence.
-        The values are specified as samples after the start of the recording (i.e. the start of the ``data``).
+        "ic_list_": """
+    ic_list_
+        A pandas dataframe with the indices of the detected initial contacts in the input data.
+        It only has one column, ``ic``, which contains the indices of the detected initial contacts.
     """,
         "detect_short": """
-    Detect gait sequences in the passed data
+    Detect Initial contacts in the passed data
+    """,
+        "detect_info": """
+    We expect the data to be a single gait sequence.
+    If the data does not contain any gait sequences, the algorithm might behave unexpectedly.
     """,
         "detect_para": """
     data
         The raw IMU of a single sensor.
     sampling_rate_hz
         The sampling rate of the IMU data in Hz.
     """,
         "detect_return": """
     Returns
     -------
     self
-        The instance of the class with the ``gs_list_`` attribute set to the detected gait sequences.
+        The instance of the class with the ``icd_list_`` attribute set to the detected initial contacts.
     """,
     },
-    doc_summary="Decorator to fill common parts of the docstring for subclasses of :class:`BaseGsdDetector`.",
+    doc_summary="Decorator to fill common parts of the docstring for subclasses of :class:`BaseIcdDetector`.",
 )
 
 
-@base_gsd_docfiller
-class BaseGsDetector(Algorithm):
-    """Base class for GS-detectors.
+@base_icd_docfiller
+class BaseIcDetector(Algorithm):
+    """Base class for IC-detectors.
 
-    This base class should be used for all gait sequence detection algorithms.
+    This base class should be used for all initial contacts detection algorithms.
     Algorithms should implement the ``detect`` method, which will perform all relevant processing steps.
-    The method should then return the instance of the class, with the ``gs_list_`` attribute set to the detected
-    gait sequences.
+    The method should then return the instance of the class, with the ``ic_list_`` attribute set to the detected
+    initial contacts.
     Further, the detect method should set ``self.data`` and ``self.sampling_rate_hz`` to the parameters passed to the
     method.
-
     We allow that subclasses specify further parameters for the detect methods (hence, this baseclass supports
     ``**kwargs``).
     However, you should only use them, if you really need them and apply active checks, that they are passed correctly.
     In 99%% of the time, you should add a new parameter to the algorithm itself, instead of adding a new parameter to
     the detect method.
 
     Other Parameters
     ----------------
     %(other_parameters)s
 
     Attributes
     ----------
-    %(gs_list_)s
+    %(ic_list_)s
 
     Notes
     -----
-    You can use the :func:`~base_gsd_docfiller` decorator to fill common parts of the docstring for your subclass.
+    You can use the :func:`~base_icd_docfiller` decorator to fill common parts of the docstring for your subclass.
     See the source of this class for an example.
-
     """
 
     _action_methods = ("detect",)
 
     # Other Parameters
     data: pd.DataFrame
     sampling_rate_hz: float
 
     # results
-    gs_list_: pd.DataFrame
+    ic_list_: pd.DataFrame
 
-    @base_gsd_docfiller
+    @base_icd_docfiller
     def detect(self, data: pd.DataFrame, *, sampling_rate_hz: float, **kwargs: Unpack[dict[str, Any]]) -> Self:
         """%(detect_short)s.
 
         Parameters
         ----------
         %(detect_para)s
-
         %(detect_return)s
         """
         raise NotImplementedError
 
 
-__all__ = ["BaseGsDetector", "base_gsd_docfiller"]
+__all__ = ["BaseIcDetector", "base_icd_docfiller"]
```

### Comparing `mobgap-0.2.0/mobgap/gsd/evaluation.py` & `mobgap-0.3.0/mobgap/gsd/evaluation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Class to validate gait sequence detection results."""
 
-from typing import Any, Optional, Union
+import warnings
+from typing import Any, Literal, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from intervaltree import IntervalTree
 from intervaltree.interval import Interval
 from matplotlib.axes import Axes
@@ -18,15 +19,15 @@
     npv_score,
     precision_recall_f1_score,
     specificity_score,
 )
 
 
 def calculate_matched_gsd_performance_metrics(
-    matches: pd.DataFrame,
+    matches: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn"
 ) -> dict[str, Union[float, int]]:
     """
     Calculate commonly known performance metrics for based on the matched overlap with the reference.
 
     This method assumes that you already calculated the overlapping regions between the ground truth and the detected
     gait sequences using the :func:`~mobgap.gsd.evaluation.categorize_intervals` method.
     This function then calculates the performance metrics based on the number of true positive, false positive,
@@ -61,14 +62,17 @@
 
     Parameters
     ----------
     matches: pd.DataFrame
         A DataFrame as returned by :func:`~mobgap.gsd.evaluation.categorize_intervals`.
         It contains the matched intervals between algorithm output and reference with their `start` and `end` index
         and the respective `match_type`.
+    zero_division : "warn", 0 or 1, default="warn"
+        Sets the value to return when there is a zero division. If set to
+        "warn", this acts as 0, but warnings are also raised.
 
     Returns
     -------
     gsd_metrics: dict
 
     See Also
     --------
@@ -83,33 +87,34 @@
 
     tp_samples = count_samples_in_match_intervals(matches, match_type="tp")
     fp_samples = count_samples_in_match_intervals(matches, match_type="fp")
     fn_samples = count_samples_in_match_intervals(matches, match_type="fn")
     tn_samples = count_samples_in_match_intervals(matches, match_type="tn")
 
     # estimate performance metrics
-    precision_recall_f1 = precision_recall_f1_score(matches)
+    precision_recall_f1 = precision_recall_f1_score(matches, zero_division=zero_division)
 
     gsd_metrics = {"tp_samples": tp_samples, "fp_samples": fp_samples, "fn_samples": fn_samples, **precision_recall_f1}
 
     # tn-dependent metrics
     if tn_samples != 0:
         gsd_metrics["tn_samples"] = tn_samples
-        gsd_metrics["specificity"] = specificity_score(matches)
-        gsd_metrics["accuracy"] = accuracy_score(matches)
-        gsd_metrics["npv"] = npv_score(matches)
+        gsd_metrics["specificity"] = specificity_score(matches, zero_division=zero_division)
+        gsd_metrics["accuracy"] = accuracy_score(matches, zero_division=zero_division)
+        gsd_metrics["npv"] = npv_score(matches, zero_division=zero_division)
 
     return gsd_metrics
 
 
 def calculate_unmatched_gsd_performance_metrics(
     *,
     gsd_list_detected: pd.DataFrame,
     gsd_list_reference: pd.DataFrame,
     sampling_rate_hz: float,
+    zero_division_hint: Union[Literal["warn", "raise"], float] = "warn",
 ) -> dict[str, Union[float, int]]:
     """
     Calculate general performance metrics that don't rely on matching the detected and reference gait sequences.
 
     Metrics calculated by this function are just based on the overall amount of gait detected.
     The following metrics are calculated:
 
@@ -134,43 +139,76 @@
        Each row contains a detected gait sequence interval as output from the GSD algorithms.
        The respective start index is stored in a column named `start` and the stop index in a column named `end`.
     gsd_list_reference
        Gold standard to validate the detected gait sequences against.
        Should have the same format as `gsd_list_detected`.
     sampling_rate_hz
         Sampling frequency of the recording in Hz.
+    zero_division_hint : "warn", "raise" or np.nan, default="warn"
+        Controls the behavior when there is a zero division. If set to "warn",
+        affected metrics are set to NaN and a warning is raised.
+        If set to "raise", a ZeroDivisionError is raised.
+        If set to `np.nan`, the warning is suppressed and the affected metrics are set to NaN.
+        Zero division can occur if there are no gait sequences in the reference data, i.e., reference_gs_duration_s = 0
 
     Returns
     -------
     gsd_metrics: dict
 
     See Also
     --------
     calculate_matched_gsd_performance_metrics
         For calculating performance metrics based on the matched overlap with the reference.
     categorize_intervals
         For categorizing the detected and reference gait sequences on a sample-wise level.
 
     """
-    # estimate duration metrics
+    if sampling_rate_hz <= 0:
+        raise ValueError("The sampling rate must be larger than 0.")
+
+    # estimate basic duratnoch mit Isomatte dazugesellen will sollte kein Problem sein, ion metrics
     reference_gs_duration_s = count_samples_in_intervals(gsd_list_reference) / sampling_rate_hz
     detected_gs_duration_s = count_samples_in_intervals(gsd_list_detected) / sampling_rate_hz
     gs_duration_error_s = detected_gs_duration_s - reference_gs_duration_s
-    gs_relative_duration_error = gs_duration_error_s / reference_gs_duration_s
     gs_absolute_duration_error_s = abs(gs_duration_error_s)
-    gs_absolute_relative_duration_error = gs_absolute_duration_error_s / reference_gs_duration_s
-    gs_absolute_relative_duration_error_log = np.log(1 + gs_absolute_relative_duration_error)
 
-    # estimate gs count metrics
+    # estimate basic gs count metrics
     detected_num_gs = len(gsd_list_detected)
     reference_num_gs = len(gsd_list_reference)
     num_gs_error = detected_num_gs - reference_num_gs
-    num_gs_relative_error = num_gs_error / reference_num_gs
     num_gs_absolute_error = abs(num_gs_error)
-    num_gs_absolute_relative_error = num_gs_absolute_error / reference_num_gs
+
+    # check if reference gs are present to prevent zero division
+    if reference_gs_duration_s == 0:
+        if zero_division_hint not in ["warn", "raise", np.nan]:
+            raise ValueError('"zero_division" must be set to "warn", "raise" or `np.nan`!')
+        if zero_division_hint == "raise":
+            raise ZeroDivisionError(
+                "Zero division occurred because no gait sequences were detected in the reference data."
+            )
+        if zero_division_hint == "warn":
+            warnings.warn(
+                "Zero division occurred because no gait sequences were detected in the reference data. "
+                "Affected metrics are set to NaN.",
+                UserWarning,
+                stacklevel=2,
+            )
+        gs_relative_duration_error = np.nan
+        gs_absolute_relative_duration_error = np.nan
+        num_gs_relative_error = np.nan
+        num_gs_absolute_relative_error = np.nan
+    # no zero division, calculate relative metrics
+    else:
+        gs_relative_duration_error = np.array(gs_duration_error_s) / reference_gs_duration_s
+        gs_absolute_relative_duration_error = np.array(gs_absolute_duration_error_s) / reference_gs_duration_s
+        num_gs_relative_error = num_gs_error / np.array(reference_num_gs)
+        num_gs_absolute_relative_error = num_gs_absolute_error / np.array(reference_num_gs)
+
+    # logarithmic relative metrics
+    gs_absolute_relative_duration_error_log = np.log(1 + gs_absolute_relative_duration_error)
     num_gs_absolute_relative_error_log = np.log(1 + num_gs_absolute_relative_error)
 
     gsd_metrics = {
         "reference_gs_duration_s": reference_gs_duration_s,
         "detected_gs_duration_s": detected_gs_duration_s,
         "gs_duration_error_s": gs_duration_error_s,
         "gs_relative_duration_error": gs_relative_duration_error,
```

### Comparing `mobgap-0.2.0/mobgap/icd/_hklee_algo_improved.py` & `mobgap-0.3.0/mobgap/icd/_hklee_algo_improved.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,17 @@
                 detected_ics.append(imax)
 
             final_detected_ics["ic"] = detected_ics
 
         self.ic_list_internal_ = final_detected_ics
 
         # Downsample initial contacts to original sampling rate
-        ic_downsampled = (final_detected_ics * sampling_rate_hz / self._UPSAMPLED_SAMPLING_RATE_HZ).round().astype(int)
+        ic_downsampled = (
+            (final_detected_ics * sampling_rate_hz / self._UPSAMPLED_SAMPLING_RATE_HZ).round().astype("int64")
+        )
 
         self.ic_list_ = ic_downsampled
 
         return self
 
 
 def groupfind(bool_array: np.ndarray) -> np.ndarray:
@@ -246,12 +248,14 @@
         raise ValueError("Input must be boolean array")
 
     if len(bool_array) == 0:
         return np.array([])
 
     nonzero = np.where(bool_array)[0]  # Find non-zeros
     endzero = np.where(np.diff(nonzero) > 1)[0]  # Find end of non-zero groups
-    seq = np.zeros((len(endzero) + 1, 2), dtype=int)  # Initializing array (+1 because last sequence is not calculated))
+    seq = np.zeros(
+        (len(endzero) + 1, 2), dtype="int64"
+    )  # Initializing array (+1 because last sequence is not calculated))
     seq[:, 1] = nonzero[np.append(endzero, -1)]  # End
     seq[:, 0] = nonzero[np.insert(endzero, 0, -1) + 1]  # Start
     seq = seq[seq[:, 1] - seq[:, 0] != 0]
     return seq
```

### Comparing `mobgap-0.2.0/mobgap/icd/_icd_ionescu.py` & `mobgap-0.3.0/mobgap/icd/_icd_ionescu.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,23 +132,23 @@
 
         # 5. INTRA-ZERO-CROSSINGS PEAK DETECTION
         # Detect the extrema between the zero crossings
         icd_array = _find_minima_between_zero_crossings(acc_v_lp_int_cwt)
 
         detected_ics = pd.DataFrame({"ic": icd_array}).rename_axis(index="step_id")
         detected_ics_unsampled = (
-            (detected_ics * sampling_rate_hz / self._INTERNAL_FILTER_SAMPLING_RATE_HZ).round().astype(int)
+            (detected_ics * sampling_rate_hz / self._INTERNAL_FILTER_SAMPLING_RATE_HZ).round().astype("int64")
         )
         self.ic_list_ = detected_ics_unsampled
 
         return self
 
 
 def _find_minima_between_zero_crossings(signal: np.ndarray) -> np.ndarray:
-    zero_crossings = find_zero_crossings(signal, "both", refine=False).astype(int)
+    zero_crossings = find_zero_crossings(signal, "both", refine=False).astype("int64")
 
     if len(zero_crossings) == 0:
         return np.array([])
 
     # We are then looking for minimas between the zero crossings.
     # Minimas can only happen between a positive to negative zero crossing and a negative to positive zero crossing.
     bool_map = signal[zero_crossings] >= 0
@@ -156,10 +156,12 @@
     # select the range between the zero crossings.
     pos_to_neg = zero_crossings[bool_map] + 1
     neg_to_pos = zero_crossings[~bool_map] + 1
     # If the first zero crossing is a negative to positive zero crossing, we need to remove it.
     if not bool_map[0]:
         neg_to_pos = neg_to_pos[1:]
 
-    minima = np.array([np.argmin(signal[start:end]) + start for start, end in zip(pos_to_neg, neg_to_pos)]).astype(int)
+    minima = np.array([np.argmin(signal[start:end]) + start for start, end in zip(pos_to_neg, neg_to_pos)]).astype(
+        "int64"
+    )
 
     return minima
```

### Comparing `mobgap-0.2.0/mobgap/icd/_shin_algo_improved.py` & `mobgap-0.3.0/mobgap/icd/_shin_algo_improved.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,13 +187,13 @@
         detected_ics = find_zero_crossings(final_filtered, "negative_to_positive")
         detected_ics = pd.DataFrame({"ic": detected_ics}).rename_axis(index="step_id")
 
         self.ic_list_internal_ = detected_ics
 
         # Upsample initial contacts to original sampling rate
         detected_ics_unsampled = (
-            (detected_ics * sampling_rate_hz / self._INTERNAL_FILTER_SAMPLING_RATE_HZ).round().astype(int)
+            (detected_ics * sampling_rate_hz / self._INTERNAL_FILTER_SAMPLING_RATE_HZ).round().astype("int64")
         )
 
         self.ic_list_ = detected_ics_unsampled
 
         return self
```

### Comparing `mobgap-0.2.0/mobgap/icd/_utils.py` & `mobgap-0.3.0/mobgap/icd/_utils.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/icd/evaluation.py` & `mobgap-0.3.0/mobgap/icd/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 from scipy.spatial import KDTree
 
 from mobgap.utils.evaluation import precision_recall_f1_score
 
 
 def calculate_matched_icd_performance_metrics(
-    matches: pd.DataFrame,
+    matches: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn"
 ) -> dict[str, Union[float, int]]:
     """
     Calculate performance metrics for initial contact detection results.
 
     This function assumes that you already classified the detected initial contacts as true positive (tp), false
     positive (fp), or false negative (fn) matches using the :func:`~mobgap.icd.evaluation.categorize_ic_list`
     function.
@@ -34,14 +34,17 @@
     precision, and F1 score.
 
     Parameters
     ----------
     matches: pd.DataFrame
         A dataframe containing the matches between detected and reference initial contacts as output
         by :func:`~mobgap.icd.evaluation.evaluate_initial_contact_list`.
+    zero_division : "warn", 0 or 1, default="warn"
+        Sets the value to return when there is a zero division. If set to
+        "warn", this acts as 0, but warnings are also raised.
 
     Returns
     -------
     icd_metrics: dict
 
     See Also
     --------
@@ -53,15 +56,15 @@
 
     # estimate tp, fp, fn
     tp_samples = len(matches[matches["match_type"] == "tp"])
     fp_samples = len(matches[matches["match_type"] == "fp"])
     fn_samples = len(matches[matches["match_type"] == "fn"])
 
     # estimate performance metrics
-    precision_recall_f1 = precision_recall_f1_score(matches)
+    precision_recall_f1 = precision_recall_f1_score(matches, zero_division=zero_division)
 
     icd_metrics = {
         "tp_samples": tp_samples,
         "fp_samples": fp_samples,
         "fn_samples": fn_samples,
         **precision_recall_f1,
     }
```

### Comparing `mobgap-0.2.0/mobgap/lrd/_lrd_mccamley.py` & `mobgap-0.3.0/mobgap/lrc/_lrc_mccamley.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import numpy as np
 import pandas as pd
 from tpcp import cf
 from typing_extensions import Self, Unpack
 
 from mobgap.data_transform import ButterworthFilter
 from mobgap.data_transform.base import BaseFilter
-from mobgap.lrd.base import BaseLRDetector, base_lrd_docfiller
+from mobgap.lrc.base import BaseLRClassifier, base_lrc_docfiller
 
 
-@base_lrd_docfiller
-class LrdMcCamley(BaseLRDetector):
+@base_lrc_docfiller
+class LrcMcCamley(BaseLRClassifier):
     """McCamley algorithm for laterality detection of initial contacts.
 
     The McCamley algorithm [1]_ uses the sign of the angular velocity either yaw or roll (or a combination of both) as
     the distinguishing factor for identifying left and right ICs.
 
     For this the respective signal is filtered (high-pass to remove DC offset and low-pass to remove noise) and the sign
     at the position of the IC is used to determine the laterality.
@@ -71,16 +71,16 @@
         # TODO: Change axis names, once we are using them consistently everywhere
         axis: Literal["yaw", "roll", "combined"] = "combined",
         smoothing_filter: BaseFilter = cf(ButterworthFilter(order=4, cutoff_freq_hz=(0.5, 2), filter_type="bandpass")),
     ) -> None:
         self.axis = axis
         self.smoothing_filter = smoothing_filter
 
-    @base_lrd_docfiller
-    def detect(
+    @base_lrc_docfiller
+    def predict(
         self,
         data: pd.DataFrame,
         ic_list: pd.DataFrame,
         *,
         sampling_rate_hz: float,
         **_: Unpack[dict[str, Any]],
     ) -> Self:
@@ -92,14 +92,16 @@
 
         %(detect_return)s
         """
         self.sampling_rate_hz = sampling_rate_hz
         self.data = data
         self.ic_list = ic_list
 
+        # TODO: Handle no data or no ICs
+
         # create a copy of ic_list, otherwise they will get modified when adding the predicted labels
         # We also remove the "lr_label" column, if it exists, to avoid conflicts
         ic_list = ic_list.copy().drop(columns="lr_label", errors="ignore")
 
         if self.axis == "yaw":
             selected_data = data["gyr_x"]
         elif self.axis == "roll":
```

### Comparing `mobgap-0.2.0/mobgap/pipeline/_gs_iterator.py` & `mobgap-0.3.0/mobgap/pipeline/_gs_iterator.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/utils/array_handling.py` & `mobgap-0.3.0/mobgap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/utils/conversions.py` & `mobgap-0.3.0/mobgap/utils/conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     Returns
     -------
     int or Sequence[int]
         The value in samples.
 
     """
     if isinstance(sec_value, np.ndarray):
-        return np.round(sec_value * sampling_rate_hz).astype(int)
+        return np.round(sec_value * sampling_rate_hz).astype("int64")
     if isinstance(sec_value, (int, float)):
         return int(np.round(sec_value * sampling_rate_hz))
     return type(sec_value)(int(np.round(s * sampling_rate_hz)) for s in sec_value)
 
 
 __all__ = ["as_samples"]
```

### Comparing `mobgap-0.2.0/mobgap/utils/dtypes.py` & `mobgap-0.3.0/mobgap/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/utils/evaluation.py` & `mobgap-0.3.0/mobgap/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/utils/interpolation.py` & `mobgap-0.3.0/mobgap/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/__init__.py` & `mobgap-0.3.0/mobgap/wba/__init__.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_interval_criteria.py` & `mobgap-0.3.0/mobgap/wba/_interval_criteria.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_stride_selection.py` & `mobgap-0.3.0/mobgap/wba/_stride_selection.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_utils.py` & `mobgap-0.3.0/mobgap/wba/_utils.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_wb_assembly.py` & `mobgap-0.3.0/mobgap/wba/_wb_assembly.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_wb_criteria.py` & `mobgap-0.3.0/mobgap/wba/_wb_criteria.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/_wb_criteria_base.py` & `mobgap-0.3.0/mobgap/wba/_wb_criteria_base.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/mobgap/wba/plot.py` & `mobgap-0.3.0/mobgap/wba/plot.py`

 * *Files identical despite different names*

### Comparing `mobgap-0.2.0/pyproject.toml` & `mobgap-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mobgap"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python implementation of the Mobilise-D algorithm pipeline for gait analysis using IMU worn at the lower back."
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
     "Felix Kluge <felix.kluge@novartis.com>",
     "Paolo Tasca <paolo.tasca@polito.it>",
     "Annika Mücke <annika-muecke@outlook.de>",
     "dmegaritis <dmgrei3@gmail.com>",
@@ -12,32 +12,32 @@
     "Björn Eskofier <bjoern.eskofier@fau.de>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-tpcp = ">=0.31.2"
+tpcp = "^0.32.0"
 pandas = ">=2.1.0"
 scipy = ">=1.11.2"
 numpy = ">=1.25.2"
 scikit-learn = ">=1.3.0"
 # TODO: Remove this dependency at some point
-gaitmap = "^2.3.0"
+gaitmap = "^2.4.0"
 joblib = ">=1.3.2"
 openpyxl = "^3.1.2"
 intervaltree = "^3.1.0"
 pywavelets = "^1.5.0"
 pooch = "^1.8.1"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.22.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 sphinx = "^7.2.6"
 sphinx-gallery = "^0.14.0"
 memory-profiler = "^0.61.0"
 matplotlib = "^3.7.2"
 toml = "^0.10.2"
 pydata-sphinx-theme = "^0.14.1"
 myst-parser = "^2.0.0"
@@ -55,14 +55,15 @@
 format = ["_auto_fix", "_format"]
 format_unsafe = ["_auto_fix_unsafe", "_format"]
 lint = { cmd = "ruff check mobgap --fix", help = "Lint all files with ruff." }
 _lint_ci = "ruff check mobgap --output-format=github"
 _check_format = "ruff format . --check"
 ci_check = { sequence = ["_check_format", "_lint_ci", "_check_update_example_data"], help = "Check all potential format and linting issues." }
 test = { cmd = "pytest --cov=mobgap --cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
+test_ci = { cmd = "pytest --cov=mobgap --cov-report=term-missing --cov-report=xml --snapshot-only-check", help = "Run Pytest with coverage and fail on missing snapshots." }
 docs = { "script" = "_tasks:task_docs()",  help = "Build the html docs using Sphinx." }
 docs_clean = { "script" = "_tasks:task_docs(clean=True)",  help = "Remove all old build files and build a clean version of the docs." }
 docs_linkcheck = { "script" = "_tasks:task_docs(builder='linkcheck')", help = "Check all links in the built html docs." }
 docs_preview = { cmd = "python -m http.server --directory docs/_build/html", help = "Preview the built html docs." }
 version = { script = "_tasks:task_update_version()", help="Bump the version number in all relevant files."}
 conf_jupyter = { cmd = "python -m ipykernel install --user --name mobgap", help = "Add a new jupyter kernel for the project." }
 remove_jupyter = { cmd = "jupyter kernelspec uninstall mobgap", help = "Remove the project specific jupyter kernel."}
```

### Comparing `mobgap-0.2.0/PKG-INFO` & `mobgap-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: mobgap
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python implementation of the Mobilise-D algorithm pipeline for gait analysis using IMU worn at the lower back.
 License: Apache-2.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gaitmap (>=2.3.0,<3.0.0)
+Requires-Dist: gaitmap (>=2.4.0,<3.0.0)
 Requires-Dist: intervaltree (>=3.1.0,<4.0.0)
 Requires-Dist: joblib (>=1.3.2)
 Requires-Dist: numpy (>=1.25.2)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.0)
 Requires-Dist: pooch (>=1.8.1,<2.0.0)
 Requires-Dist: pywavelets (>=1.5.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.0)
 Requires-Dist: scipy (>=1.11.2)
-Requires-Dist: tpcp (>=0.31.2)
+Requires-Dist: tpcp (>=0.32.0,<0.33.0)
 Description-Content-Type: text/markdown
 
 > [!CAUTION]
 > mobgap is currently under active development and not ready for production use.
 > Do not use any of the algorithm results for actual research purposes. 
 > Most of them are not in their final state and are not properly validated yet.
 >
```

