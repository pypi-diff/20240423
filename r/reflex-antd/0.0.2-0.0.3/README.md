# Comparing `tmp/reflex_antd-0.0.2.tar.gz` & `tmp/reflex_antd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.2.tar", last modified: Fri Apr 19 01:08:50 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.3.tar", last modified: Tue Apr 23 01:01:51 2024, max compression
```

## Comparing `reflex_antd-0.0.2.tar` & `reflex_antd-0.0.3.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-19 01:08:50.798728 reflex_antd-0.0.2/
--rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.2/LICENSE
--rwxrwxrwx   0 see       (1000) see       (1000)      743 2024-04-19 01:08:50.792728 reflex_antd-0.0.2/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)      101 2024-04-09 02:24:43.000000 reflex_antd-0.0.2/README.md
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-19 01:08:47.349406 reflex_antd-0.0.2/custom_components/
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-19 01:08:47.585536 reflex_antd-0.0.2/custom_components/reflex_antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/__init__.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-19 01:08:50.757164 reflex_antd-0.0.2/custom_components/reflex_antd/antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/__init__.py
--rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/affix.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/affix.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/alert.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/alert.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/anchor.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/anchor.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1538 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/auto_complete.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/auto_complete.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1026 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/avatar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/avatar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/badge.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/badge.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2697 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5912 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/breadcrumb.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/breadcrumb.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/calendar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/calendar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1354 2024-04-17 06:32:19.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/card.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/card.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/carousel.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/carousel.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2264 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/cascader.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/cascader.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/checkbox.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/checkbox.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      919 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/collapse.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/collapse.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/color_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/color_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4951 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/date_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/date_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/descriptions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/descriptions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/divider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/divider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/drawer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/drawer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1507 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/dropdown.py
--rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/dropdown.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      329 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/empty.py
--rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/empty.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/flex.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/flex.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/float_button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/float_button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     3484 2024-04-17 06:35:06.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/form.py
--rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/form.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/grid.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/grid.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/icon.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/icon.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      962 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/image.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/image.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1936 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/input.py
--rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/input.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1554 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/input_number.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/input_number.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/layout.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/list.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/list.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1372 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/mentions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/mentions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2000 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/menu.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/menu.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-04-17 07:26:07.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/message.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/message.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/modal.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/modal.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-17 08:26:56.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/notification.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/pagination.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/pagination.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/popconfirm.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/popconfirm.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/popover.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/popover.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/progress.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/progress.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/qrcode.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/qrcode.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/radio.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/radio.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/rate.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/rate.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      534 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/result.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/result.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/segmented.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/segmented.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2851 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/skeleton.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/skeleton.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/slider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/slider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/space.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/space.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      577 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/spin.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/spin.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/statistic.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/statistic.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/steps.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/steps.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1031 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/switch.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/switch.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/table.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/table.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2096 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tabs.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tabs.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1052 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tag.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tag.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      555 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/timeline.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/timeline.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tooltip.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tooltip.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1226 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tour.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tour.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1986 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/transfer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/transfer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2858 2024-04-17 04:22:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree_select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree_select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/typography.py
--rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/typography.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/upload.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/upload.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/watermark.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.2/custom_components/reflex_antd/antd/watermark.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)    23350 2024-04-17 08:38:41.000000 reflex_antd-0.0.2/custom_components/reflex_antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.2/custom_components/reflex_antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/constant.py
--rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/display.py
--rwxrwxrwx   0 see       (1000) see       (1000)      873 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/entry.py
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/feedback.py
--rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/general.py
--rwxrwxrwx   0 see       (1000) see       (1000)      145 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/helper.py
--rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-04-17 04:22:46.000000 reflex_antd-0.0.2/custom_components/reflex_antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/navigation.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-04-17 04:22:49.000000 reflex_antd-0.0.2/custom_components/reflex_antd/util.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-19 01:08:50.782728 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/
--rwxrwxrwx   0 see       (1000) see       (1000)      743 2024-04-19 01:08:46.000000 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)     6899 2024-04-19 01:08:47.000000 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/SOURCES.txt
--rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-04-19 01:08:46.000000 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/dependency_links.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-04-19 01:08:46.000000 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/requires.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-04-19 01:08:46.000000 reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/top_level.txt
--rwxrwxrwx   0 see       (1000) see       (1000)      793 2024-04-19 01:08:34.000000 reflex_antd-0.0.2/pyproject.toml
--rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-04-19 01:08:50.799728 reflex_antd-0.0.2/setup.cfg
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 01:01:51.454683 reflex_antd-0.0.3/
+-rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.3/LICENSE
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-23 01:01:51.447682 reflex_antd-0.0.3/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.3/README.md
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 01:01:47.988183 reflex_antd-0.0.3/custom_components/
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 01:01:48.250440 reflex_antd-0.0.3/custom_components/reflex_antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/__init__.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 01:01:51.411109 reflex_antd-0.0.3/custom_components/reflex_antd/antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/__init__.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/affix.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/affix.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/alert.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/alert.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/anchor.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/anchor.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/auto_complete.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/auto_complete.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/avatar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/avatar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/badge.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/badge.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2697 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5912 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/breadcrumb.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/calendar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/calendar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/card.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/card.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/carousel.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/carousel.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/cascader.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/cascader.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/checkbox.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/checkbox.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/collapse.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/collapse.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/color_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/color_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/date_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/date_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/descriptions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/descriptions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/divider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/divider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/drawer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/drawer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/dropdown.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/dropdown.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/empty.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/empty.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/flex.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/flex.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/float_button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/float_button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     3495 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/form.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/form.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/grid.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/grid.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/icon.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/icon.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/image.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/image.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1947 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/input.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/input.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/input_number.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/input_number.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/layout.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/list.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/list.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/mentions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/mentions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/menu.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/menu.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-04-17 07:26:07.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/message.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/message.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/modal.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/modal.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-17 08:26:56.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/notification.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/pagination.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/pagination.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/popconfirm.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/popconfirm.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/popover.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/popover.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/progress.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/progress.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/qrcode.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/qrcode.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/radio.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/radio.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/rate.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/rate.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/result.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/result.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/segmented.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/segmented.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/skeleton.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/skeleton.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/slider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/slider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/space.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/space.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/spin.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/spin.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/statistic.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/statistic.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-04-17 04:22:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/steps.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/steps.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/switch.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/switch.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/table.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/table.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tabs.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tabs.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tag.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tag.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/timeline.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/timeline.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tooltip.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tooltip.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tour.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tour.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/transfer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/transfer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-04-23 00:49:43.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree_select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree_select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/typography.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/typography.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/upload.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/upload.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-17 04:22:48.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/watermark.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.3/custom_components/reflex_antd/antd/watermark.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)    23350 2024-04-17 08:38:41.000000 reflex_antd-0.0.3/custom_components/reflex_antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.3/custom_components/reflex_antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/constant.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/display.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      873 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/entry.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/feedback.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/general.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      145 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/helper.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-04-17 04:22:46.000000 reflex_antd-0.0.3/custom_components/reflex_antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/navigation.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-04-17 04:22:49.000000 reflex_antd-0.0.3/custom_components/reflex_antd/util.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-23 01:01:51.437685 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-23 01:01:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)     6899 2024-04-23 01:01:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-04-23 01:01:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-04-23 01:01:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/requires.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-04-23 01:01:47.000000 reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/top_level.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)      793 2024-04-23 01:01:16.000000 reflex_antd-0.0.3/pyproject.toml
+-rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-04-23 01:01:51.455683 reflex_antd-0.0.3/setup.cfg
```

### Comparing `reflex_antd-0.0.2/LICENSE` & `reflex_antd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/PKG-INFO` & `reflex_antd-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
@@ -15,14 +15,31 @@
 Requires-Dist: reflex>=0.4.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # reflex-antd
 
-A Reflex custom component demo1.
+A Reflex custom component wrap [ant.design](https://ant.design/).
 
 ## Installation
 
 ```bash
 pip install reflex-antd
 ```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/affix.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/affix.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/alert.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/anchor.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/auto_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Dict, Any
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import VariantType, SizeType
 
 
 class AutoComplete(AntdComponent):
     tag = "AutoComplete"
 
     allow_clear: Optional[Var[bool]]
@@ -17,15 +17,15 @@
     default_active_first_option: Optional[Var[bool]]
     default_open: Optional[Var[bool]]
     default_value: Optional[Var[str]]
     disabled: Optional[Var[bool]]
     popup_class_name: Optional[Var[str]]
     dropdown_match_select_width: Optional[Var[Union[bool, int]]]
     filter_option: Optional[Var[bool]]
-    not_found_content: Optional[Var[Component]]
+    not_found_content: Optional[Var[ReactNode]]
     open: Optional[Var[bool]]
     options: Optional[Var[list]]
     placeholder: Optional[Var[str]]
     status: Optional[Var[str]]
     size: Optional[Var[SizeType]]
     value: Optional[Var[str]]
     variant: Optional[Var[VariantType]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/avatar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Optional, Union, Dict, Any
 
 from reflex import Component, Var
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 
 class Avatar(AntdComponent):
     tag = 'Avatar'
 
     alt: Optional[Var[str]]
     gap: Optional[Var[int]]
-    icon: Optional[Var[Component]]
+    icon: Optional[Var[ReactNode]]
     shape: Optional[Var[str]]
     size: Optional[Var[Union[str, int, Dict]]]
-    src: Optional[Var[Union[Component, str]]]
+    src: Optional[Var[ReactNode]]
     src_set: Optional[Var[str]]
     draggable: Optional[Var[bool]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            "on_error": lambda :[],
+            "on_error": lambda: [],
         })
         return _triggers
 
 
 class AvatarGroup(AntdComponent):
     tag = 'Avatar.Group'
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/badge.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/badge.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/base.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/base.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/base.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/calendar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/card.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import Optional, Union, Dict, Any, List
 
 from reflex import Component, Var
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 
 class Card(AntdComponent):
     tag = 'Card'
 
     actions: Optional[Var[ContainVar]]
     active_tab_key: Optional[Var[str]]
     bordered: Optional[Var[bool]]
-    cover: Optional[Var[Component]]
+    cover: Optional[Var[ReactNode]]
     default_active_tab_key: Optional[Var[str]]
-    extra: Optional[Var[Component]]
+    extra: Optional[Var[ReactNode]]
     hoverable: Optional[Var[bool]]
     loading: Optional[Var[bool]]
     size: Optional[Var[str]]
-    tab_bar_extra_content: Optional[Var[Component]]
+    tab_bar_extra_content: Optional[Var[ReactNode]]
     tab_list: Optional[Var[list[ContainVar]]]
-    title: Optional[Var[Component]]
+    title: Optional[Var[ReactNode]]
     type: Optional[Var[str]]
-    tab_props: Optional[Var[Union[ContainVar,dict]]]
+    tab_props: Optional[Var[Union[ContainVar, dict]]]
     class_names: Optional[Var[dict]]
     styles: Optional[Var[dict]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             'on_tab_change': lambda key: [key],
@@ -38,15 +38,15 @@
 
     hoverable: Optional[Var[bool]]
 
 
 class CardMeta(AntdComponent):
     tag = 'Card.Meta'
 
-    avatar: Optional[Var[Component]]
-    description: Optional[Var[Component]]
-    title: Optional[Var[Component]]
+    avatar: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
 
 
 card = Card.create
 card_grid = CardGrid.create
 card_meta = CardMeta.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/carousel.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/cascader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Dict, Any, List
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
 
 
 class Cascader(AntdComponent):
     tag = 'Cascader'
 
     allow_clear: Optional[Var[bool]]
@@ -17,39 +17,39 @@
     change_on_select: Optional[Var[bool]]
     default_value: Optional[Var[Union[List[int], List[str]]]]
     disabled: Optional[Var[bool]]
     display_render: Optional[Var[JsValue]]
     tag_render: Optional[Var[JsValue]]
     popup_class_name: Optional[Var[str]]
     dropdown_render: Optional[Var[JsValue]]
-    expand_icon: Optional[Var[Component]]
+    expand_icon: Optional[Var[ReactNode]]
     expand_trigger: Optional[Var[TriggerType]]
     field_names: Optional[Var[ContainVar]]
     get_popup_container: Optional[Var[JsValue]]
     load_data: Optional[Var[JsValue]]
     max_tag_count: Optional[Var[int]]
-    max_tag_placeholder: Optional[Var[Union[Component, JsValue]]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
     max_tag_text_length: Optional[Var[int]]
     not_found_content: Optional[Var[str]]
     open: Optional[Var[bool]]
-    options: Optional[Var[Union[ContainVar,list]]]
-    placeholder: Optional[Var[str]]
+    options: Optional[Var[Union[ContainVar, list]]]
+    placeholder: Optional[Var[ReactNode]]
     placement: Optional[Var[PlacementType]]
     show_search: Optional[Var[Union[bool, ContainVar]]]
     size: Optional[Var[SizeType]]
     status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[Component]]
+    suffix_icon: Optional[Var[ReactNode]]
     value: Optional[Var[Union[List[str], List[int]]]]
     variant: Optional[Var[VariantType]]
     multiple: Optional[Var[bool]]
-    remove_icon: Optional[Var[Component]]
+    remove_icon: Optional[Var[ReactNode]]
     show_checked_strategy: Optional[Var[str]]
     search_value: Optional[Var[str]]
     dropdown_menu_column_style: Optional[Var[ContainVar]]
-    loading_icon: Optional[Var[Component]]
+    loading_icon: Optional[Var[ReactNode]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             EventTriggers.ON_CHANGE: lambda value, options: [value, options],
             "on_dropdown_visible_change": lambda value: [value],
             "on_search": lambda search: [search]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/cascader.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/checkbox.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/collapse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional, Union, Dict, Any, List
 
 from reflex import Component, Var
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 
 class Collapse(AntdComponent):
     tag = 'Collapse'
 
     accordion: Optional[Var[bool]]
-    active_key: Optional[Var[Union[list[str],str, list[int],int]]]
+    active_key: Optional[Var[Union[list[str], str, list[int], int]]]
     bordered: Optional[Var[bool]]
-    default_active_key: Optional[Var[Union[list[str],str, list[int],int]]]
+    default_active_key: Optional[Var[Union[list[str], str, list[int], int]]]
     destroy_inactive_panel: Optional[Var[bool]]
-    expand_icon: Optional[Var[Component]]
+    expand_icon: Optional[Var[ReactNode]]
     collapsible: Optional[Var[str]]
     expand_icon_position: Optional[Var[str]]
     ghost: Optional[Var[bool]]
     size: Optional[Var[str]]
-    items: Optional[Var[Union[ContainVar,list]]]
+    items: Optional[Var[Union[ContainVar, list]]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             'on_change': lambda: [],
         })
         return _triggers
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/color_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/date_picker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
 
 from .base import Locale
 
 
 class DayJS(JsValue):
     def serialize(self) -> str:
@@ -17,42 +17,42 @@
 
 class BaseDatePicker(AntdComponent):
 
     allow_clear: Optional[Var[bool]]
     auto_focus: Optional[Var[bool]]
     date_render: Optional[Var[JsValue]]
     cell_render: Optional[Var[JsValue]]
-    components: Optional[Var[Component]]
+    components: Optional[Var[Union[ReactNode, list, dict, ContainVar]]]
     disabled: Optional[Var[bool]]
     disabled_date: Optional[Var[JsValue]]
     format: Optional[Var[ContainVar]]
     order: Optional[Var[bool]]
     popup_class_name: Optional[Var[str]]
     preserve_invalidOn_blur: Optional[Var[bool]]
     getPopup_container: Optional[Var[JsValue]]
     input_readOnly: Optional[Var[bool]]
     locale: Optional[Var[Locale]]
     min_date: Optional[Var[JsValue]]
     max_date: Optional[Var[JsValue]]
     mode: Optional[Var[DatePickerModeType]]
     need_confirm: Optional[Var[bool]]
-    next_icon: Optional[Var[Component]]
+    next_icon: Optional[Var[ReactNode]]
     open: Optional[Var[bool]]
     panel_render: Optional[Var[JsValue]]
     picker: Optional[Var[DatePickerType]]
     placeholder: Optional[Var[Union[str, List[str]]]]
     placement: Optional[Var[PlacementType]]
     popup_style: Optional[Var[ContainVar]]
     presets: Optional[Var[ContainVar]]
-    prev_icon: Optional[Var[Component]]
+    prev_icon: Optional[Var[ReactNode]]
     size: Optional[Var[SizeType]]
     status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[Component]]
-    super_next_icon: Optional[Var[Component]]
-    super_prev_icon: Optional[Var[Component]]
+    suffix_icon: Optional[Var[ReactNode]]
+    super_next_icon: Optional[Var[ReactNode]]
+    super_prev_icon: Optional[Var[ReactNode]]
     variant: Optional[Var[VariantType]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
             'on_panel_change': lambda value, mode: [value, mode],
@@ -104,15 +104,15 @@
     disabled: Optional[Var[Tuple[bool, bool]]]
     disabled_time: Optional[Var[JsValue]]
     format: Optional[Var[ContainVar]]
     id: Optional[Var[Dict[str, str]]]
     picker_value: Optional[Var[ContainVar]]
     presets: Optional[Var[ContainVar]]
     render_extra_footer: Optional[Var[JsValue]]
-    separator: Optional[Var[Component]]
+    separator: Optional[Var[ReactNode]]
     show_time: Optional[Var[Union[bool, ContainVar]]]
     # showTime.defaultValue
     value: Optional[Var[ContainVar]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/descriptions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/dropdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Dict, Any
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import PlacementType, DirectionType
 
 
 class Dropdown(AntdComponent):
     tag = 'Dropdown'
 
     arrow: Optional[Var[bool]]
@@ -33,15 +33,15 @@
 
 class DropdownButton(Dropdown):
     tag = 'Dropdown.Button'
 
     buttons_render: Optional[Var[JsValue]]
     loading: Optional[Var[bool]]
     danger: Optional[Var[bool]]
-    icon: Optional[Var[Component]]
+    icon: Optional[Var[ReactNode]]
     size: Optional[Var[str]]
     type: Optional[Var[str]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
 
         _triggers.update({
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/empty.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/float_button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/form.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import AlignType, DirectionType, SizeType, VariantType
 
 
 class Form(AntdComponent):
     tag = 'Form'
 
     colon: Optional[Var[bool]]
@@ -39,19 +39,19 @@
 
 
 class FormItem(AntdComponent):
     tag = 'Form.Item'
 
     colon: Optional[Var[bool]]
     dependencies: Optional[Var[List[Union[str, int, List[Union[str, int]]]]]]
-    extra: Optional[Var[Component]]
+    extra: Optional[Var[ReactNode]]
     getValue_from_event: Optional[Var[JsValue]]
     get_value_props: Optional[Var[JsValue]]
     has_feedback: Optional[Var[Union[bool, ContainVar]]]
-    help: Optional[Var[Component]]
+    help: Optional[Var[ReactNode]]
     hidden: Optional[Var[bool]]
     html_for: Optional[Var[str]]
     initial_value: Optional[Var[str]]
     label: Optional[Var[str]]
     label_align: Optional[Var[AlignType]]
     label_col: Optional[Var[Dict]]
     message_variables: Optional[Var[JsValue]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/grid.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/icon.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, Union, Dict, Any, List
 
 from reflex import Component, Var
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 
 
 class Image(AntdComponent):
     tag = 'Image'
 
     alt: Optional[Var[str]]
     fallback: Optional[Var[str]]
     height: Optional[Var[Union[str, int]]]
-    placeholder: Optional[Var[Component]]
-    description: Optional[Var[Component]]
+    placeholder: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
     preview: Optional[Var[Union[bool, dict]]]
     src: Optional[Var[str]]
     width: Optional[Var[Union[str, int]]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/transfer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,56 @@
-from typing import Optional, Union, Dict, Any
+from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, VariantType
+from ..base import AntdComponent, ContainVar, JsValue, js_value, ReactNode
+from ..constant import StatusType
 
 
-class Input(AntdComponent):
-    tag = "Input"
+class Transfer(AntdComponent):
+    tag = 'Transfer'
+    _rename_props: Dict[str, str] = {"itemRender": "render"}
 
-    addon_after: Optional[Var[Component]]
-    addon_before: Optional[Var[Component]]
-    allow_clear: Optional[Var[Union[bool, ContainVar]]]
-    count: Optional[Var[Union[Dict, ContainVar]]]
-    default_value: Optional[Var[str]]
+    data_source: Optional[Var[List]]
     disabled: Optional[Var[bool]]
-    id: Optional[Var[str]]
-    max_length: Optional[Var[int]]
-    prefix: Optional[Var[Component]]
-    show_count: Optional[Var[Union[bool, JsValue]]]
+    selections_icon: Optional[Var[ReactNode]]
+    filter_option: Optional[Var[JsValue]]
+    footer: Optional[Var[JsValue]]
+    list_style: Optional[Var[Union[Dict, JsValue]]]
+    locale: Optional[Var[Union[Dict, ContainVar]]]
+    one_way: Optional[Var[bool]]
+    operations: Optional[Var[List[str]]]
+    operation_style: Optional[Var[Dict]]
+    pagination: Optional[Var[Union[bool, ContainVar]]]
+    item_render: Optional[Var[Union[JsValue, ContainVar]]]
+    row_key: Optional[Var[JsValue]]
+    select_all_labels: Optional[Var[JsValue]]
+    selected_keys: Optional[Var[List[str]]]
+    show_search: Optional[Var[bool]]
+    showSelect_all: Optional[Var[bool]]
     status: Optional[Var[StatusType]]
-    size: Optional[Var[SizeType]]
-    suffix: Optional[Var[Component]]
-    type: Optional[Var[str]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-    placeholder: Optional[Var[str]]
+    target_keys: Optional[Var[List[str]]]
+    titles: Optional[Var[ContainVar]]
 
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-            'on_press_enter': lambda e: [e],
-        })
-        return _triggers
-
-
-class TextArea(Input):
-    tag = "Input.TextArea"
-
-    auto_size: Optional[Var[Union[bool, Dict]]]
-
-
-class Search(Input):
-    tag = 'Input.Search'
-
-    enter_button: Optional[Var[Component]]
-    loading: Optional[Var[bool]]
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        if 'item_render' not in props:
+            props['item_render'] = js_value(lambda record: 'return record.title;')
+        com = super().create(*children, **props)
+        return com
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            'on_search': lambda value, event, info: [value, event, info],
+            EventTriggers.ON_CHANGE: lambda target_keys, direction, move_keys: [target_keys, direction, move_keys],
+            EventTriggers.ON_SCROLL: lambda direction, ev: [direction, ev],
+            "on_search": lambda direction, value: [direction, value],
+            "on_select_change": lambda s_keys, t_keys: [s_keys, t_keys],
         })
         return _triggers
 
 
-class Password(Input):
-    tag = 'Input.Password'
-
-    icon_render: Optional[Var[JsValue]]
-    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
-
+transfer = Transfer.create
 
-input = Input.create  # noqa
-text_area = TextArea.create
-search = Search.create
-password = Password.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/input_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional, Union, Dict, Any
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, VariantType
 
 
 class InputNumber(AntdComponent):
     tag = "InputNumber"
 
-    addon_after: Optional[Var[Component]]
-    addon_before: Optional[Var[Component]]
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
     auto_focus: Optional[Var[bool]]
     change_on_blur: Optional[Var[bool]]
     change_on_wheel: Optional[Var[bool]]
     controls: Optional[Var[Union[bool, ContainVar]]]
     decimal_separator: Optional[Var[str]]
     placeholder: Optional[Var[str]]
     default_value: Optional[Var[int]]
@@ -23,15 +23,15 @@
     keyboard: Optional[Var[bool]]
     max: Optional[Var[int]]
     min: Optional[Var[int]]
     parser: Optional[Var[JsValue]]
     precision: Optional[Var[int]]
     read_only: Optional[Var[bool]]
     status: Optional[Var[StatusType]]
-    prefix: Optional[Var[Component]]
+    prefix: Optional[Var[ReactNode]]
     size: Optional[Var[SizeType]]
     step: Optional[Var[Union[int, str]]]
     string_mode: Optional[Var[bool]]
     value: Optional[Var[int]]
     variant: Optional[Var[VariantType]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/layout.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/layout.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/list.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 class AList(AntdComponent):
     tag = 'List'
 
     bordered: Optional[Var[bool]]
     data_source: Optional[Var[Any]]
-    footer: Optional[Var[Component]]
+    footer: Optional[Var[ReactNode]]
     grid: Optional[Var[dict]]
-    header: Optional[Var[Component]]
+    header: Optional[Var[ReactNode]]
     item_layout: Optional[Var[str]]
     loading: Optional[Var[Union[bool, dict]]]
-    load_more: Optional[Var[Component]]
+    load_more: Optional[Var[ReactNode]]
     locale: Optional[Var[dict]]
     pagination: Optional[Var[Union[bool, dict]]]
     render_item: Optional[Var[JsValue]]
     size: Optional[Var[SizeType]]
     split: Optional[Var[bool]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/mentions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, VariantType, PlacementType
 
 
 class Mention(AntdComponent):
     tag = 'Mention'
 
     allow_clear: Optional[Var[Union[bool, ContainVar]]]
     auto_focus: Optional[Var[bool]]
     auto_size: Optional[Var[Union[bool, Dict]]]
     default_value: Optional[Var[str]]
     filter_option: Optional[Var[Union[bool, JsValue]]]
     get_popup_container: Optional[Var[JsValue]]
-    not_found_content: Optional[Var[Component]]
+    not_found_content: Optional[Var[ReactNode]]
     placement: Optional[Var[PlacementType]]
     prefix: Optional[Var[Union[str, List[str]]]]
     split: Optional[Var[str]]
     status: Optional[Var[StatusType]]
     validate_search: Optional[Var[JsValue]]
     value: Optional[Var[str]]
     variant: Optional[Var[VariantType]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union, Type, Dict, List, Any, Iterator
 from pydantic import BaseModel
 from reflex import Component, Var, EventChain, Base
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, AntdSubComponent, ContainVar
+from ..base import AntdComponent, AntdSubComponent, ContainVar, ReactNode
 from ..constant import ThemeType, DirectionType, TriggerType
 
 
 class MenuItem(BaseModel):
     key: str
     label: str
     icon: Component
@@ -26,24 +26,24 @@
 
 
 class Menu(AntdComponent):
     tag = 'Menu'
 
     default_open_keys: Optional[Var[List[str]]]
     default_selected_keys: Optional[Var[List[str]]]
-    expand_icon: Optional[Var[Component]]
+    expand_icon: Optional[Var[ReactNode]]
     force_sub_menu_render: Optional[Var[bool]]
     inline_collapsed: Optional[Var[bool]]
     inline_indent: Optional[Var[bool]]
 
     items: Var[Union[ContainVar, list]]
     mode: Optional[Var[DirectionType]]
     multiple: Optional[Var[bool]]
     open_keys: Optional[Var[List[str]]]
-    overflowed_indicator: Optional[Var[Component]]
+    overflowed_indicator: Optional[Var[ReactNode]]
     selectable: Optional[Var[bool]]
     selected_keys: Optional[Var[List[str]]]
     sub_menu_close_delay: Optional[Var[float]]
     sub_menu_open_delay: Optional[Var[float]]
 
     theme: Optional[Var[ThemeType]]
     trigger_sub_menu_action: Optional[Var[TriggerType]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/message.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/message.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/modal.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/modal.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     keyboard: Optional[Var[bool]]
     mask: Optional[Var[bool]]
     mask_closable: Optional[Var[bool]]
     modal_render: Optional[Var[ReactNode]]
     ok_button_props: Optional[Var[ContainVar]]
     ok_text: Optional[Var[ReactNode]]
     ok_type: Optional[Var[TypeType]]
-    title: Optional[Var[Component]]
+    title: Optional[Var[ReactNode]]
     open: Optional[Var[bool]]
     width: Optional[Var[Union[str, int]]]
     wrapClassName: Optional[Var[str]]
     zIndex: Optional[Var[int]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/notification.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/pagination.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/pagination.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/popconfirm.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     disabled: Optional[Var[bool]]
     icon: Optional[Var[ReactNode]]
     ok_button_props: Optional[Var[dict]]
     ok_text: Optional[Var[str]]
     ok_type: Optional[Var[TypeType]]
     open: Optional[Var[bool]]
     show_cancel: Optional[Var[bool]]
-    title: Optional[Var[Component]]
-    description: Optional[Var[Component]]
+    title: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             "on_cancel": lambda e: [e],
             "on_confirm": lambda e: [e],
             "on_popup_click": lambda e: [e],
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/progress.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/qrcode.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/qrcode.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/radio.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/rate.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/rate.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/rate.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/result.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType
 
 
 class Result(AntdComponent):
     tag = 'Result'
 
-    extra: Optional[Var[Component]]
-    icon: Optional[Var[Component]]
+    extra: Optional[Var[ReactNode]]
+    icon: Optional[Var[ReactNode]]
     status: Optional[Var[Union[StatusType, str]]]
-    sub_title: Optional[Var[Component]]
-    title: Optional[Var[Component]]
+    sub_title: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
 
 
 result = Result.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/result.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/segmented.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/select.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
 
 
 class Select(AntdComponent):
     tag = 'Select'
 
     allow_clear: Optional[Var[bool]]
@@ -25,32 +25,32 @@
     filter_sort: Optional[Var[JsValue]]
     get_popup_container: Optional[Var[JsValue]]
     label_in_value: Optional[Var[bool]]
     list_height: Optional[Var[int]]
     loading: Optional[Var[bool]]
     max_count: Optional[Var[int]]
     max_tag_count: Optional[Var[Union[int, str]]]
-    max_tag_placeholder: Optional[Var[Union[Component, JsValue]]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
     max_tag_text_length: Optional[Var[int]]
-    menu_item_selected_icon: Optional[Var[Component]]
+    menu_item_selected_icon: Optional[Var[ReactNode]]
     mode: Optional[Var[SelectModeType]]
-    not_found_content: Optional[Var[Component]]
+    not_found_content: Optional[Var[ReactNode]]
     open: Optional[Var[bool]]
     option_filter_prop: Optional[Var[str]]
     option_label_prop: Optional[Var[str]]
     options: Optional[Var[Union[list, ContainVar]]]
     option_render: Optional[Var[JsValue]]
-    placeholder: Optional[Var[Component]]
+    placeholder: Optional[Var[ReactNode]]
     placement: Optional[Var[PlacementType]]
-    remove_icon: Optional[Var[Component]]
+    remove_icon: Optional[Var[ReactNode]]
     search_value: Optional[Var[str]]
     show_search: Optional[Var[bool]]
     size: Optional[Var[SizeType]]
     status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[Component]]
+    suffix_icon: Optional[Var[ReactNode]]
     tag_render: Optional[Var[JsValue]]
     label_render: Optional[Var[JsValue]]
     token_separators: Optional[Var[List[str]]]
     value: Optional[Var[Union[str, int, List[str], List[int], ContainVar]]]
     variant: Optional[Var[VariantType]]
     virtual: Optional[Var[bool]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/slider.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/space.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/space.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/space.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/spin.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/spin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import SizeType
 
 
 class Spin(AntdComponent):
     tag = 'Spin'
 
     delay: Optional[Var[int]]
-    indicator: Optional[Var[Component]]
+    indicator: Optional[Var[ReactNode]]
     size: Optional[Var[SizeType]]
     spinning: Optional[Var[bool]]
-    tip: Optional[Var[Component]]
+    tip: Optional[Var[ReactNode]]
     wrapper_class_name: Optional[Var[str]]
     fullscreen: Optional[Var[bool]]
 
 
 spin = Spin.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/spin.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/statistic.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/statistic.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/steps.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/steps.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/switch.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/switch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
 
 
 class Switch(AntdComponent):
     tag = 'Switch'
 
     auto_focus: Optional[Var[bool]]
     checked: Optional[Var[bool]]
-    checked_children: Optional[Var[Component]]
+    checked_children: Optional[Var[ReactNode]]
     default_checked: Optional[Var[bool]]
     default_value: Optional[Var[bool]]
     disabled: Optional[Var[bool]]
     loading: Optional[Var[bool]]
     size: Optional[Var[SizeType]]
-    un_checked_children: Optional[Var[Component]]
+    un_checked_children: Optional[Var[ReactNode]]
     value: Optional[Var[bool]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             EventTriggers.ON_CHANGE: lambda checked, e: [checked, e],
             EventTriggers.ON_CLICK: lambda checked, e: [checked, e],
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/table.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 from dataclasses import dataclass
 
 from reflex import Component, Var, Base
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import SizeType, PlacementType, TabsType
 
 
 @dataclass(frozen=True)
 class TabItem:
-    close_icon: Optional[Var[Component]] = None
+    close_icon: Optional[Var[ReactNode]] = None
     destroy_inactive_tab_pane: Optional[Var[bool]] = None
     disabled: Optional[Var[bool]] = None
     force_render: Optional[Var[bool]] = None
     key: Optional[Union[str, Var[str]]] = None
-    label: Optional[Union[str, Component, Var]] = None
-    icon: Optional[Var[Component]] = None
-    children: Optional[Union[str, Component, Var[Component]]] = None
+    label: Optional[Union[ReactNode, Var[ReactNode]]] = None
+    icon: Optional[Var[ReactNode]] = None
+    children: Optional[Union[ReactNode, Var[ReactNode]]] = None
     closable: Optional[Var[bool]] = None
 
 
 class Tabs(AntdComponent):
     tag = 'Tabs'
 
     active_key: Optional[Var[str]]
-    add_icon: Optional[Var[Component]]
+    add_icon: Optional[Var[ReactNode]]
     animated: Optional[Var[Union[bool, Dict]]]
     centered: Optional[Var[bool]]
     default_active_key: Optional[Var[str]]
     hide_add: Optional[Var[bool]]
     indicator: Optional[Var[Union[Dict, ContainVar]]]
     items: Optional[Var[Union[ContainVar, List]]]
-    more_icon: Optional[Var[Component]]
-    remove_icon: Optional[Var[Component]]
+    more_icon: Optional[Var[ReactNode]]
+    remove_icon: Optional[Var[ReactNode]]
     popup_class_name: Optional[Var[str]]
     render_tab_bar: Optional[Var[JsValue]]
     size: Optional[Var[SizeType]]
-    tab_bar_extra_content: Optional[Var[Union[Component, ContainVar]]]
+    tab_bar_extra_content: Optional[Var[Union[ReactNode, ContainVar]]]
     tab_bar_gutter: Optional[Var[int]]
     tab_bar_style: Optional[Var[Dict]]
     tab_position: Optional[Var[PlacementType]]
     destroy_inactive_tab_pane: Optional[Var[bool]]
     type: Optional[Var[TabsType]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tag.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import TimelineModeType
 
 
 class Tag(AntdComponent):
     tag = 'Tag'
 
-    close_icon: Optional[Var[Union[bool, Component]]]
+    close_icon: Optional[Var[Union[bool, ReactNode]]]
     color: Optional[Var[str]]
-    icon: Optional[Var[Component]]
+    icon: Optional[Var[ReactNode]]
     bordered: Optional[Var[bool]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
             'on_close': lambda e: [e],
         })
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/timeline.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/timeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import TimelineModeType
 
 
 class Timeline(AntdComponent):
     tag = 'Timeline'
 
     mode: Optional[Var[TimelineModeType]]
-    pending: Optional[Var[Component]]
-    pending_dot: Optional[Var[Component]]
+    pending: Optional[Var[ReactNode]]
+    pending_dot: Optional[Var[ReactNode]]
     reverse: Optional[Var[bool]]
     items: Optional[Var[Union[List, ContainVar]]]
 
 
 timeline = Timeline.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tour.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tour.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, Union, Dict, Any, List, Tuple
 
 from reflex import Component, Var
 from reflex.utils import imports
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
 from ..constant import StatusType, PlacementType, TypeType
 
 
 class Tour(AntdComponent):
     tag = 'Tour'
 
     arrow: Optional[Var[bool]]
-    close_icon: Optional[Var[Component]]
+    close_icon: Optional[Var[ReactNode]]
     disabled_interaction: Optional[Var[bool]]
     placement: Optional[Var[PlacementType]]
     mask: Optional[Var[Union[bool, Dict]]]
     type: Optional[Var[TypeType]]
     open: Optional[Var[bool]]
     current: Optional[Var[int]]
     scroll_into_view_options: Optional[Var[Union[bool, Dict]]]
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tour.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tour.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/transfer.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,72 @@
-from typing import Optional, Union, Dict, Any, List
+from typing import Optional, Union, Dict, Any
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsValue, js_value
-from ..constant import StatusType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
 
 
-class Transfer(AntdComponent):
-    tag = 'Transfer'
-    _rename_props: Dict[str, str] = {"itemRender": "render"}
+class Input(AntdComponent):
+    tag = "Input"
 
-    data_source: Optional[Var[List]]
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    allow_clear: Optional[Var[Union[bool, ContainVar]]]
+    count: Optional[Var[Union[Dict, ContainVar]]]
+    default_value: Optional[Var[str]]
     disabled: Optional[Var[bool]]
-    selections_icon: Optional[Var[Component]]
-    filter_option: Optional[Var[JsValue]]
-    footer: Optional[Var[JsValue]]
-    list_style: Optional[Var[Union[Dict, JsValue]]]
-    locale: Optional[Var[Union[Dict, ContainVar]]]
-    one_way: Optional[Var[bool]]
-    operations: Optional[Var[List[str]]]
-    operation_style: Optional[Var[Dict]]
-    pagination: Optional[Var[Union[bool, ContainVar]]]
-    item_render: Optional[Var[Union[JsValue, ContainVar]]]
-    row_key: Optional[Var[JsValue]]
-    select_all_labels: Optional[Var[JsValue]]
-    selected_keys: Optional[Var[List[str]]]
-    show_search: Optional[Var[bool]]
-    showSelect_all: Optional[Var[bool]]
+    id: Optional[Var[str]]
+    max_length: Optional[Var[int]]
+    prefix: Optional[Var[ReactNode]]
+    show_count: Optional[Var[Union[bool, JsValue]]]
     status: Optional[Var[StatusType]]
-    target_keys: Optional[Var[List[str]]]
-    titles: Optional[Var[ContainVar]]
+    size: Optional[Var[SizeType]]
+    suffix: Optional[Var[ReactNode]]
+    type: Optional[Var[str]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+    placeholder: Optional[Var[str]]
 
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        if 'item_render' not in props:
-            props['item_render'] = js_value(lambda record: 'return record.title;')
-        com = super().create(*children, **props)
-        return com
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+            'on_press_enter': lambda e: [e],
+        })
+        return _triggers
+
+
+class TextArea(Input):
+    tag = "Input.TextArea"
+
+    auto_size: Optional[Var[Union[bool, Dict]]]
+
+
+class Search(Input):
+    tag = 'Input.Search'
+
+    enter_button: Optional[Var[ReactNode]]
+    loading: Optional[Var[bool]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            EventTriggers.ON_CHANGE: lambda target_keys, direction, move_keys: [target_keys, direction, move_keys],
-            EventTriggers.ON_SCROLL: lambda direction, ev: [direction, ev],
-            "on_search": lambda direction, value: [direction, value],
-            "on_select_change": lambda s_keys, t_keys: [s_keys, t_keys],
+            'on_search': lambda value, event, info: [value, event, info],
         })
         return _triggers
 
 
-transfer = Transfer.create
+class Password(Input):
+    tag = 'Input.Password'
+
+    icon_render: Optional[Var[JsValue]]
+    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
+
 
+input = Input.create  # noqa
+text_area = TextArea.create
+search = Search.create
+password = Password.create
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree_select.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,47 @@
 from typing import Optional, Union, Dict, Any, List
 from reflex import Var, Component
 from reflex.constants import EventTriggers
 
-from ..base import AntdComponent, ContainVar, JsNode
+from ..base import AntdComponent, ContainVar, JsValue
 
 
-class TreeSelect(AntdComponent):
-    tag = 'TreeSelect'
+class Upload(AntdComponent):
+    tag = 'Upload'
 
-    allow_clear: Optional[Var[Union[bool, Component]]]
-    auto_clear_search_value: Optional[Var[bool]]
-    default_value: Optional[Var[Union[str, List[str]]]]
+    accept: Optional[Var[str]]
+    action: Optional[Var[Union[str, JsValue]]]
+    before_upload: Optional[Var[JsValue]]
+    custom_request: Optional[Var[JsValue]]
+    data: Optional[Var[Union[ContainVar, JsValue]]]
+    default_file_list: Optional[Var[List[ContainVar]]]
+    directory: Optional[Var[bool]]
     disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    dropdown_render: Optional[Var[JsNode]]
-    dropdown_style: Optional[Var[Dict]]
-    field_names: Optional[Var[Dict]]
-    filter_tree_node: Optional[Var[Union[bool, JsNode]]]
-    get_popup_container: Optional[Var[JsNode]]
-    label_in_value: Optional[Var[bool]]
-    list_height: Optional[Var[int]]
-    load_data: Optional[Var[JsNode]]
-    max_tag_count: Optional[Var[int]]
-    max_tag_placeholder: Optional[Var[Union[Component, JsNode]]]
-    max_tag_text_length: Optional[Var[int]]
+    file_list: Optional[Var[List[ContainVar]]]
+    headers: Optional[Var[Dict]]
+    icon_render: Optional[Var[JsValue]]
+    is_image_url: Optional[Var[JsValue]]
+    list_type: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+    method: Optional[Var[str]]
     multiple: Optional[Var[bool]]
-    not_found_content: Optional[Var[Component]]
-    placeholder: Optional[Var[str]]
-    placement: Optional[Var[str]]
-    search_value: Optional[Var[str]]
-    show_checked_strategy: Optional[Var[str]]
-    show_search: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    status: Optional[Var[str]]
-    suffix_icon: Optional[Var[Component]]
-    switcher_icon: Optional[Var[Union[Component, ContainVar]]]
-    tag_render: Optional[Var[JsNode]]
-    tree_checkable: Optional[Var[bool]]
-    tree_check_strictly: Optional[Var[bool]]
-    tree_data: Optional[Var[List[Dict]]]
-    tree_data_simple_mode: Optional[Var[Union[bool, Dict]]]
-    tree_default_expand_all: Optional[Var[bool]]
-    tree_default_expanded_keys: Optional[Var[List]]
-    tree_expand_action: Optional[Var[Union[str, bool]]]
-    tree_expanded_keys: Optional[Var[List[str]]]
-    tree_icon: Optional[Var[bool]]
-    tree_line: Optional[Var[Union[bool, Dict]]]
-    tree_loaded_keys: Optional[Var[List[str]]]
-    tree_node_filter_prop: Optional[Var[str]]
-    tree_node_label_prop: Optional[Var[str]]
-    value: Optional[Var[Union[str, List[str]]]]
-    variant: Optional[Var[str]]
-    virtual: Optional[Var[str]]
+    name: Optional[Var[str]]
+    open_file_dialog_on_click: Optional[Var[bool]]
+    preview_file: Optional[Var[JsValue]]
+    progress: Optional[Var[Dict]]
+    show_upload_list: Optional[Var[Union[bool, Dict]]]
+    with_credentials: Optional[Var[Union[bool]]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, label, extra: [value, label, extra],
-            EventTriggers.ON_SELECT: lambda value, node, extra: [value, node, extra],
-            "on_dropdown_visible_change": lambda open: [open],
-            "on_search": lambda value: [value],
-            "on_tree_expand": lambda keys: [keys],
-
-            "filter_tree_node": lambda node: [node],
-            "load_data": lambda node: [node],
+            EventTriggers.ON_CHANGE: lambda file, file_list: [file, file_list],
+            "on_drop": lambda event: [event],
+            "on_download": lambda file: [file],
+            "on_preview": lambda file: [file],
+            "on_remove": lambda file: [file]
         })
         return _triggers
 
 
-tree_select = TreeSelect.create
+upload = Upload.create
+
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/typography.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/watermark.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/antd/watermark.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/base.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/base.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.3/custom_components/reflex_antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/constant.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/display.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/entry.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd/util.py` & `reflex_antd-0.0.3/custom_components/reflex_antd/util.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
@@ -15,14 +15,31 @@
 Requires-Dist: reflex>=0.4.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # reflex-antd
 
-A Reflex custom component demo1.
+A Reflex custom component wrap [ant.design](https://ant.design/).
 
 ## Installation
 
 ```bash
 pip install reflex-antd
 ```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.2/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.3/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.2/pyproject.toml` & `reflex_antd-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-antd"
-version = "0.0.2"
+version = "0.0.3"
 description = "Reflex custom component antd"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
 keywords = [
     "reflex",
```

