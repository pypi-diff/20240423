# Comparing `tmp/YaraForge-0.1.3b1.tar.gz` & `tmp/YaraForge-0.1.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YaraForge-0.1.3b1.tar", last modified: Sun Mar 17 19:21:54 2024, max compression
+gzip compressed data, was "YaraForge-0.1.4b1.tar", last modified: Tue Apr 23 05:17:45 2024, max compression
```

## Comparing `YaraForge-0.1.3b1.tar` & `YaraForge-0.1.4b1.tar`

### file list

```diff
@@ -1,264 +1,267 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.335641 YaraForge-0.1.3b1/
--rw-rw-rw-   0        0        0        0 2024-03-12 14:12:32.000000 YaraForge-0.1.3b1/MANIFEST.in
--rw-rw-rw-   0        0        0      791 2024-03-17 19:21:54.335641 YaraForge-0.1.3b1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.155595 YaraForge-0.1.3b1/YaraForge.egg-info/
--rw-rw-rw-   0        0        0      791 2024-03-17 19:21:54.000000 YaraForge-0.1.3b1/YaraForge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8202 2024-03-17 19:21:54.000000 YaraForge-0.1.3b1/YaraForge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 19:21:54.000000 YaraForge-0.1.3b1/YaraForge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-03-17 19:21:54.000000 YaraForge-0.1.3b1/YaraForge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-17 19:21:54.000000 YaraForge-0.1.3b1/YaraForge.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.155595 YaraForge-0.1.3b1/python/
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.204629 YaraForge-0.1.3b1/python/3/
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.205623 YaraForge-0.1.3b1/python/3/PyQt5/
--rw-rw-rw-   0        0        0     1235 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.212657 YaraForge-0.1.3b1/python/3/PyQt5/uic/
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.217687 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/__init__.py
--rw-rw-rw-   0        0        0     4645 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/compiler.py
--rw-rw-rw-   0        0        0     2742 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/indenter.py
--rw-rw-rw-   0        0        0     2374 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/misc.py
--rw-rw-rw-   0        0        0     4324 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py
--rw-rw-rw-   0        0        0     5903 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py
--rw-rw-rw-   0        0        0    16315 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/qtproxies.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.220687 YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/loader.py
--rw-rw-rw-   0        0        0     5022 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/qobjectcreator.py
--rw-rw-rw-   0        0        0     9507 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/driver.py
--rw-rw-rw-   0        0        0     2279 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/exceptions.py
--rw-rw-rw-   0        0        0     4566 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/icon_cache.py
--rw-rw-rw-   0        0        0     5970 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/objcreator.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.224698 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/__init__.py
--rw-rw-rw-   0        0        0      979 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/as_string.py
--rw-rw-rw-   0        0        0      869 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/ascii_upper.py
--rw-rw-rw-   0        0        0      763 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/proxy_base.py
--rw-rw-rw-   0        0        0      674 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/string_io.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.228703 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/
--rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/__init__.py
--rw-rw-rw-   0        0        0      956 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/as_string.py
--rw-rw-rw-   0        0        0      866 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/ascii_upper.py
--rw-rw-rw-   0        0        0      745 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/proxy_base.py
--rw-rw-rw-   0        0        0      604 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/string_io.py
--rw-rw-rw-   0        0        0    17761 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/properties.py
--rw-rw-rw-   0        0        0     3094 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/pyuic.py
--rw-rw-rw-   0        0        0    38150 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/uiparser.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.235209 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py
--rw-rw-rw-   0        0        0     1097 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py
--rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py
--rw-rw-rw-   0        0        0     1132 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py
--rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py
--rw-rw-rw-   0        0        0     1112 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py
--rw-rw-rw-   0        0        0     2507 2023-06-08 15:50:59.000000 YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.3b1/python/3/__init__.py
--rw-rw-rw-   0        0        0   832972 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_allins.py
--rw-rw-rw-   0        0        0    14032 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_auto.py
--rw-rw-rw-   0        0        0     8502 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_bitrange.py
--rw-rw-rw-   0        0        0   136649 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_bytes.py
--rw-rw-rw-   0        0        0   129129 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_dbg.py
--rw-rw-rw-   0        0        0    40649 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_dirtree.py
--rw-rw-rw-   0        0        0    16401 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_diskio.py
--rw-rw-rw-   0        0        0     5818 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_entry.py
--rw-rw-rw-   0        0        0    19054 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_enum.py
--rw-rw-rw-   0        0        0    38928 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_expr.py
--rw-rw-rw-   0        0        0    18628 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_fixup.py
--rw-rw-rw-   0        0        0     8436 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_fpro.py
--rw-rw-rw-   0        0        0    34902 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_frame.py
--rw-rw-rw-   0        0        0    59731 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_funcs.py
--rw-rw-rw-   0        0        0    24940 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_gdl.py
--rw-rw-rw-   0        0        0   106310 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_graph.py
--rw-rw-rw-   0        0        0   788487 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_hexrays.py
--rw-rw-rw-   0        0        0   100897 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_ida.py
--rw-rw-rw-   0        0        0    40739 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_idaapi.py
--rw-rw-rw-   0        0        0     2719 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_idc.py
--rw-rw-rw-   0        0        0   134230 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_idd.py
--rw-rw-rw-   0        0        0   264974 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_idp.py
--rw-rw-rw-   0        0        0    16171 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_ieee.py
--rw-rw-rw-   0        0        0   379220 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_kernwin.py
--rw-rw-rw-   0        0        0    23145 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_lines.py
--rw-rw-rw-   0        0        0    37073 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_loader.py
--rw-rw-rw-   0        0        0    28642 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_moves.py
--rw-rw-rw-   0        0        0    91052 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_nalt.py
--rw-rw-rw-   0        0        0    39716 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_name.py
--rw-rw-rw-   0        0        0    43940 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_netnode.py
--rw-rw-rw-   0        0        0    11454 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_offset.py
--rw-rw-rw-   0        0        0    83307 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_pro.py
--rw-rw-rw-   0        0        0     6353 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_problems.py
--rw-rw-rw-   0        0        0    28927 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_range.py
--rw-rw-rw-   0        0        0     9907 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_registry.py
--rw-rw-rw-   0        0        0     7877 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_search.py
--rw-rw-rw-   0        0        0    51938 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_segment.py
--rw-rw-rw-   0        0        0     9757 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_segregs.py
--rw-rw-rw-   0        0        0     5334 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_srclang.py
--rw-rw-rw-   0        0        0     6429 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_strlist.py
--rw-rw-rw-   0        0        0    36082 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_struct.py
--rw-rw-rw-   0        0        0    22949 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_tryblks.py
--rw-rw-rw-   0        0        0   289055 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_typeinf.py
--rw-rw-rw-   0        0        0    69494 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_ua.py
--rw-rw-rw-   0        0        0    27691 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/ida_xref.py
--rw-rw-rw-   0        0        0     2993 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/idaapi.py
--rw-rw-rw-   0        0        0    19673 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/idadex.py
--rw-rw-rw-   0        0        0    23522 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/idautils.py
--rw-rw-rw-   0        0        0   195546 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/idc.py
--rw-rw-rw-   0        0        0     6547 2023-06-08 15:50:57.000000 YaraForge-0.1.3b1/python/3/init.py
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.3b1/python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.236208 YaraForge-0.1.3b1/python/examples/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.237208 YaraForge-0.1.3b1/python/examples/analysis/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/analysis/__init__.py
--rw-rw-rw-   0        0        0     3401 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/analysis/dump_func_info.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.260784 YaraForge-0.1.3b1/python/examples/core/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/core/__init__.py
--rw-rw-rw-   0        0        0     8158 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/actions.py
--rw-rw-rw-   0        0        0      996 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/add_hotkey.py
--rw-rw-rw-   0        0        0      736 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/add_idc_hotkey.py
--rw-rw-rw-   0        0        0     3758 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/auto_instantiate_widget_plugin.py
--rw-rw-rw-   0        0        0     3349 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/bin_search.py
--rw-rw-rw-   0        0        0      790 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/colorize_disassembly.py
--rw-rw-rw-   0        0        0     4898 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/colorize_disassembly_on_the_fly.py
--rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/create_structure_programmatically.py
--rw-rw-rw-   0        0        0     2623 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/custom_cli.py
--rw-rw-rw-   0        0        0     8878 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/custom_data_types_and_formats.py
--rw-rw-rw-   0        0        0     2683 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/dump_extra_comments.py
--rw-rw-rw-   0        0        0     1932 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/dump_flowchart.py
--rw-rw-rw-   0        0        0     2574 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/dump_selection.py
--rw-rw-rw-   0        0        0      741 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/extend_idc.py
--rw-rw-rw-   0        0        0      827 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/idapythonrc.py
--rw-rw-rw-   0        0        0     1266 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/install_user_defined_prefix.py
--rw-rw-rw-   0        0        0     1337 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_bookmarks.py
--rw-rw-rw-   0        0        0     3285 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_function_items.py
--rw-rw-rw-   0        0        0      804 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_imports.py
--rw-rw-rw-   0        0        0     1183 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_patched_bytes.py
--rw-rw-rw-   0        0        0     1021 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_problems.py
--rw-rw-rw-   0        0        0     1350 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_segment_functions.py
--rw-rw-rw-   0        0        0     1318 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_segment_functions_using_idautils.py
--rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_stkvar_xrefs.py
--rw-rw-rw-   0        0        0      670 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/list_strings.py
--rw-rw-rw-   0        0        0      933 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/produce_c_file.py
--rw-rw-rw-   0        0        0     1067 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/produce_lst_file.py
--rw-rw-rw-   0        0        0     1223 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/register_timer.py
--rw-rw-rw-   0        0        0     2820 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/core/trigger_actions_programmatically.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.261789 YaraForge-0.1.3b1/python/examples/cvt64/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/cvt64/__init__.py
--rw-rw-rw-   0        0        0     2815 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/cvt64/py_cvt64_sample.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.264042 YaraForge-0.1.3b1/python/examples/debugging/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/debugging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.267048 YaraForge-0.1.3b1/python/examples/debugging/appcall/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/debugging/appcall/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_common.py
--rw-rw-rw-   0        0        0      895 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_linux.py
--rw-rw-rw-   0        0        0     1284 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_win.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.269041 YaraForge-0.1.3b1/python/examples/debugging/dbghooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/debugging/dbghooks/__init__.py
--rw-rw-rw-   0        0        0     3770 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/dbghooks/automatic_steps.py
--rw-rw-rw-   0        0        0     3813 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/dbghooks/dbg_trace.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.272548 YaraForge-0.1.3b1/python/examples/debugging/misc/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/debugging/misc/__init__.py
--rw-rw-rw-   0        0        0     2127 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/misc/print_call_stack.py
--rw-rw-rw-   0        0        0     1753 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/misc/print_registers.py
--rw-rw-rw-   0        0        0     1899 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/misc/registers_context_menu.py
--rw-rw-rw-   0        0        0      661 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/debugging/show_debug_names.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.292713 YaraForge-0.1.3b1/python/examples/hexrays/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/hexrays/__init__.py
--rw-rw-rw-   0        0        0     3512 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/colorize_pseudocode_lines.py
--rw-rw-rw-   0        0        0     3638 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/curpos_details.py
--rw-rw-rw-   0        0        0     2453 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/decompile_entry_points.py
--rw-rw-rw-   0        0        0      732 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds1.py
--rw-rw-rw-   0        0        0     2518 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds10.py
--rw-rw-rw-   0        0        0     2875 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds11.py
--rw-rw-rw-   0        0        0     5949 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds12.py
--rw-rw-rw-   0        0        0     1162 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds13.py
--rw-rw-rw-   0        0        0    10835 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds17.py
--rw-rw-rw-   0        0        0     2325 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds19.py
--rw-rw-rw-   0        0        0     3913 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds21.py
--rw-rw-rw-   0        0        0     7264 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds3.py
--rw-rw-rw-   0        0        0     3569 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds4.py
--rw-rw-rw-   0        0        0    12037 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds5.py
--rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds6.py
--rw-rw-rw-   0        0        0     1147 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds7.py
--rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds8.py
--rw-rw-rw-   0        0        0     1128 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds_create_hint.py
--rw-rw-rw-   0        0        0     4700 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds_hooks.py
--rw-rw-rw-   0        0        0     1860 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds_modify_user_lvars.py
--rw-rw-rw-   0        0        0     9292 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/hexrays/vds_xrefs.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.295747 YaraForge-0.1.3b1/python/examples/idbhooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/idbhooks/__init__.py
--rw-rw-rw-   0        0        0     9228 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/idbhooks/log_idb_events.py
--rw-rw-rw-   0        0        0     2882 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/idbhooks/operand_changed.py
--rw-rw-rw-   0        0        0     3116 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/idbhooks/replay_prototypes_changes.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.298744 YaraForge-0.1.3b1/python/examples/idphooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/idphooks/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/idphooks/ana_emu_out.py
--rw-rw-rw-   0        0        0     1329 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/idphooks/assemble.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.302748 YaraForge-0.1.3b1/python/examples/pyqt/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/pyqt/__init__.py
--rw-rw-rw-   0        0        0     3335 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/pyqt/inject_command.py
--rw-rw-rw-   0        0        0     5627 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/pyqt/paint_over_graph.py
--rw-rw-rw-   0        0        0     2599 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/pyqt/paint_over_navbar.py
--rw-rw-rw-   0        0        0     1130 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.306259 YaraForge-0.1.3b1/python/examples/uihooks/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/uihooks/__init__.py
--rw-rw-rw-   0        0        0      972 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/uihooks/func_chooser_coloring.py
--rw-rw-rw-   0        0        0     4757 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/uihooks/lines_rendering.py
--rw-rw-rw-   0        0        0     5181 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/uihooks/log_misc_events.py
--rw-rw-rw-   0        0        0      644 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/uihooks/prevent_jump.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.307264 YaraForge-0.1.3b1/python/examples/widgets/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.308777 YaraForge-0.1.3b1/python/examples/widgets/forms/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/forms/__init__.py
--rw-rw-rw-   0        0        0    11536 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/forms/askusingform.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.310809 YaraForge-0.1.3b1/python/examples/widgets/graphs/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/graphs/__init__.py
--rw-rw-rw-   0        0        0     5336 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/graphs/custom_graph_with_actions.py
--rw-rw-rw-   0        0        0     3115 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/graphs/sync_two_graphs.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.312805 YaraForge-0.1.3b1/python/examples/widgets/idaview/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/idaview/__init__.py
--rw-rw-rw-   0        0        0     4003 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/idaview/wrap_idaview.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.315315 YaraForge-0.1.3b1/python/examples/widgets/listings/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/listings/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/listings/custom_viewer.py
--rw-rw-rw-   0        0        0     3956 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/listings/jump_next_comment.py
--rw-rw-rw-   0        0        0     3160 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/listings/save_and_restore_listing_pos.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.317320 YaraForge-0.1.3b1/python/examples/widgets/misc/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/misc/__init__.py
--rw-rw-rw-   0        0        0     1829 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/misc/add_menus.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.318315 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.322821 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/__init__.py
--rw-rw-rw-   0        0        0     5338 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/choose.py
--rw-rw-rw-   0        0        0     1634 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/choose_multi.py
--rw-rw-rw-   0        0        0    10380 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py
--rw-rw-rw-   0        0        0     1579 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/func_chooser.py
--rw-rw-rw-   0        0        0     3142 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.324092 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/string_window/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/string_window/__init__.py
--rw-rw-rw-   0        0        0     3204 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.325094 YaraForge-0.1.3b1/python/examples/widgets/waitbox/
--rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.3b1/python/examples/widgets/waitbox/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-06-08 15:50:58.000000 YaraForge-0.1.3b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py
--rw-rw-rw-   0        0        0       42 2024-03-17 19:21:54.335641 YaraForge-0.1.3b1/setup.cfg
--rw-rw-rw-   0        0        0     1120 2024-03-17 19:15:22.000000 YaraForge-0.1.3b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.327093 YaraForge-0.1.3b1/yaraforge/
--rw-rw-rw-   0        0        0        0 2024-03-09 20:13:15.000000 YaraForge-0.1.3b1/yaraforge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.330094 YaraForge-0.1.3b1/yaraforge/maker/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:42:22.000000 YaraForge-0.1.3b1/yaraforge/maker/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-03-12 15:06:48.000000 YaraForge-0.1.3b1/yaraforge/maker/dump_maker.py
--rw-rw-rw-   0        0        0     2622 2024-03-12 15:06:41.000000 YaraForge-0.1.3b1/yaraforge/maker/instruction_maker.py
--rw-rw-rw-   0        0        0     4988 2024-03-13 05:11:00.000000 YaraForge-0.1.3b1/yaraforge/maker/yara_maker.py
--rw-rw-rw-   0        0        0     1322 2024-03-17 19:14:10.000000 YaraForge-0.1.3b1/yaraforge/metadata.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.331094 YaraForge-0.1.3b1/yaraforge/plugin/
--rw-rw-rw-   0        0        0     2306 2024-03-12 12:08:25.000000 YaraForge-0.1.3b1/yaraforge/plugin/__init__.py
--rw-rw-rw-   0        0        0      294 2024-03-10 08:08:40.000000 YaraForge-0.1.3b1/yaraforge/plugin/yaraforge.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.331094 YaraForge-0.1.3b1/yaraforge/tests/
--rw-rw-rw-   0        0        0        0 2024-03-12 14:12:08.000000 YaraForge-0.1.3b1/yaraforge/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 19:21:54.334641 YaraForge-0.1.3b1/yaraforge/utils/
--rw-rw-rw-   0        0        0        0 2024-03-11 07:42:44.000000 YaraForge-0.1.3b1/yaraforge/utils/__init__.py
--rw-rw-rw-   0        0        0     1413 2024-03-12 15:06:41.000000 YaraForge-0.1.3b1/yaraforge/utils/cache_dumper.py
--rw-rw-rw-   0        0        0     4659 2024-03-12 15:06:48.000000 YaraForge-0.1.3b1/yaraforge/utils/common.py
--rw-rw-rw-   0        0        0     2413 2024-03-12 15:06:41.000000 YaraForge-0.1.3b1/yaraforge/utils/logger.py
--rw-rw-rw-   0        0        0     1280 2024-03-12 15:06:48.000000 YaraForge-0.1.3b1/yaraforge/utils/opcode_processor.py
--rw-rw-rw-   0        0        0      342 2024-03-17 17:53:25.000000 YaraForge-0.1.3b1/yaraforge/version.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.040077 YaraForge-0.1.4b1/
+-rw-rw-rw-   0        0        0        0 2024-03-12 14:12:32.000000 YaraForge-0.1.4b1/MANIFEST.in
+-rw-rw-rw-   0        0        0      807 2024-04-23 05:17:45.040077 YaraForge-0.1.4b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:43.763084 YaraForge-0.1.4b1/YaraForge.egg-info/
+-rw-rw-rw-   0        0        0      807 2024-04-23 05:17:43.000000 YaraForge-0.1.4b1/YaraForge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8270 2024-04-23 05:17:43.000000 YaraForge-0.1.4b1/YaraForge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 05:17:43.000000 YaraForge-0.1.4b1/YaraForge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-23 05:17:43.000000 YaraForge-0.1.4b1/YaraForge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 05:17:43.000000 YaraForge-0.1.4b1/YaraForge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:43.764078 YaraForge-0.1.4b1/python/
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.228082 YaraForge-0.1.4b1/python/3/
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.234081 YaraForge-0.1.4b1/python/3/PyQt5/
+-rw-rw-rw-   0        0        0     1235 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.287078 YaraForge-0.1.4b1/python/3/PyQt5/uic/
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.329082 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/__init__.py
+-rw-rw-rw-   0        0        0     4645 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/compiler.py
+-rw-rw-rw-   0        0        0     2742 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/indenter.py
+-rw-rw-rw-   0        0        0     2374 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/misc.py
+-rw-rw-rw-   0        0        0     4324 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py
+-rw-rw-rw-   0        0        0     5903 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py
+-rw-rw-rw-   0        0        0    16315 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/qtproxies.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.342081 YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/loader.py
+-rw-rw-rw-   0        0        0     5022 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/qobjectcreator.py
+-rw-rw-rw-   0        0        0     9507 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/__init__.py
+-rw-rw-rw-   0        0        0     4192 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/driver.py
+-rw-rw-rw-   0        0        0     2279 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/exceptions.py
+-rw-rw-rw-   0        0        0     4566 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/icon_cache.py
+-rw-rw-rw-   0        0        0     5970 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/objcreator.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.362082 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/__init__.py
+-rw-rw-rw-   0        0        0      979 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/as_string.py
+-rw-rw-rw-   0        0        0      869 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/ascii_upper.py
+-rw-rw-rw-   0        0        0      763 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/proxy_base.py
+-rw-rw-rw-   0        0        0      674 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/string_io.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.383079 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/
+-rw-rw-rw-   0        0        0      548 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/__init__.py
+-rw-rw-rw-   0        0        0      956 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/as_string.py
+-rw-rw-rw-   0        0        0      866 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/ascii_upper.py
+-rw-rw-rw-   0        0        0      745 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/proxy_base.py
+-rw-rw-rw-   0        0        0      604 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/string_io.py
+-rw-rw-rw-   0        0        0    17761 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/properties.py
+-rw-rw-rw-   0        0        0     3094 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/pyuic.py
+-rw-rw-rw-   0        0        0    38150 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/uiparser.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.426082 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py
+-rw-rw-rw-   0        0        0     1097 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py
+-rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py
+-rw-rw-rw-   0        0        0     1132 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py
+-rw-rw-rw-   0        0        0     1106 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py
+-rw-rw-rw-   0        0        0     1112 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py
+-rw-rw-rw-   0        0        0     2507 2023-06-08 15:50:59.000000 YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.4b1/python/3/__init__.py
+-rw-rw-rw-   0        0        0   832972 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_allins.py
+-rw-rw-rw-   0        0        0    14032 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_auto.py
+-rw-rw-rw-   0        0        0     8502 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_bitrange.py
+-rw-rw-rw-   0        0        0   136649 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_bytes.py
+-rw-rw-rw-   0        0        0   129129 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_dbg.py
+-rw-rw-rw-   0        0        0    40649 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_dirtree.py
+-rw-rw-rw-   0        0        0    16401 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_diskio.py
+-rw-rw-rw-   0        0        0     5818 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_entry.py
+-rw-rw-rw-   0        0        0    19054 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_enum.py
+-rw-rw-rw-   0        0        0    38928 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_expr.py
+-rw-rw-rw-   0        0        0    18628 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_fixup.py
+-rw-rw-rw-   0        0        0     8436 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_fpro.py
+-rw-rw-rw-   0        0        0    34902 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_frame.py
+-rw-rw-rw-   0        0        0    59731 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_funcs.py
+-rw-rw-rw-   0        0        0    24940 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_gdl.py
+-rw-rw-rw-   0        0        0   106310 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_graph.py
+-rw-rw-rw-   0        0        0   788487 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_hexrays.py
+-rw-rw-rw-   0        0        0   100897 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_ida.py
+-rw-rw-rw-   0        0        0    40739 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_idaapi.py
+-rw-rw-rw-   0        0        0     2719 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_idc.py
+-rw-rw-rw-   0        0        0   134230 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_idd.py
+-rw-rw-rw-   0        0        0   264974 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_idp.py
+-rw-rw-rw-   0        0        0    16171 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_ieee.py
+-rw-rw-rw-   0        0        0   379220 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_kernwin.py
+-rw-rw-rw-   0        0        0    23145 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_lines.py
+-rw-rw-rw-   0        0        0    37073 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_loader.py
+-rw-rw-rw-   0        0        0    28642 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_moves.py
+-rw-rw-rw-   0        0        0    91052 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_nalt.py
+-rw-rw-rw-   0        0        0    39716 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_name.py
+-rw-rw-rw-   0        0        0    43940 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_netnode.py
+-rw-rw-rw-   0        0        0    11454 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_offset.py
+-rw-rw-rw-   0        0        0    83307 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_pro.py
+-rw-rw-rw-   0        0        0     6353 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_problems.py
+-rw-rw-rw-   0        0        0    28927 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_range.py
+-rw-rw-rw-   0        0        0     9907 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_registry.py
+-rw-rw-rw-   0        0        0     7877 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_search.py
+-rw-rw-rw-   0        0        0    51938 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_segment.py
+-rw-rw-rw-   0        0        0     9757 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_segregs.py
+-rw-rw-rw-   0        0        0     5334 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_srclang.py
+-rw-rw-rw-   0        0        0     6429 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_strlist.py
+-rw-rw-rw-   0        0        0    36082 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_struct.py
+-rw-rw-rw-   0        0        0    22949 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_tryblks.py
+-rw-rw-rw-   0        0        0   289055 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_typeinf.py
+-rw-rw-rw-   0        0        0    69494 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_ua.py
+-rw-rw-rw-   0        0        0    27691 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/ida_xref.py
+-rw-rw-rw-   0        0        0     2993 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/idaapi.py
+-rw-rw-rw-   0        0        0    19673 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/idadex.py
+-rw-rw-rw-   0        0        0    23522 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/idautils.py
+-rw-rw-rw-   0        0        0   195546 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/idc.py
+-rw-rw-rw-   0        0        0     6547 2023-06-08 15:50:57.000000 YaraForge-0.1.4b1/python/3/init.py
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:22.000000 YaraForge-0.1.4b1/python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.428082 YaraForge-0.1.4b1/python/examples/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.435081 YaraForge-0.1.4b1/python/examples/analysis/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/analysis/__init__.py
+-rw-rw-rw-   0        0        0     3401 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/analysis/dump_func_info.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.615083 YaraForge-0.1.4b1/python/examples/core/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/core/__init__.py
+-rw-rw-rw-   0        0        0     8158 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/actions.py
+-rw-rw-rw-   0        0        0      996 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/add_hotkey.py
+-rw-rw-rw-   0        0        0      736 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/add_idc_hotkey.py
+-rw-rw-rw-   0        0        0     3758 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/auto_instantiate_widget_plugin.py
+-rw-rw-rw-   0        0        0     3349 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/bin_search.py
+-rw-rw-rw-   0        0        0      790 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/colorize_disassembly.py
+-rw-rw-rw-   0        0        0     4898 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/colorize_disassembly_on_the_fly.py
+-rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/create_structure_programmatically.py
+-rw-rw-rw-   0        0        0     2623 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/custom_cli.py
+-rw-rw-rw-   0        0        0     8878 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/custom_data_types_and_formats.py
+-rw-rw-rw-   0        0        0     2683 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/dump_extra_comments.py
+-rw-rw-rw-   0        0        0     1932 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/dump_flowchart.py
+-rw-rw-rw-   0        0        0     2574 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/dump_selection.py
+-rw-rw-rw-   0        0        0      741 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/extend_idc.py
+-rw-rw-rw-   0        0        0      827 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/idapythonrc.py
+-rw-rw-rw-   0        0        0     1266 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/install_user_defined_prefix.py
+-rw-rw-rw-   0        0        0     1337 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_bookmarks.py
+-rw-rw-rw-   0        0        0     3285 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_function_items.py
+-rw-rw-rw-   0        0        0      804 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_imports.py
+-rw-rw-rw-   0        0        0     1183 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_patched_bytes.py
+-rw-rw-rw-   0        0        0     1021 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_problems.py
+-rw-rw-rw-   0        0        0     1350 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_segment_functions.py
+-rw-rw-rw-   0        0        0     1318 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_segment_functions_using_idautils.py
+-rw-rw-rw-   0        0        0     2373 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_stkvar_xrefs.py
+-rw-rw-rw-   0        0        0      670 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/list_strings.py
+-rw-rw-rw-   0        0        0      933 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/produce_c_file.py
+-rw-rw-rw-   0        0        0     1067 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/produce_lst_file.py
+-rw-rw-rw-   0        0        0     1223 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/register_timer.py
+-rw-rw-rw-   0        0        0     2820 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/core/trigger_actions_programmatically.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.622081 YaraForge-0.1.4b1/python/examples/cvt64/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/cvt64/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/cvt64/py_cvt64_sample.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.629083 YaraForge-0.1.4b1/python/examples/debugging/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/debugging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.657081 YaraForge-0.1.4b1/python/examples/debugging/appcall/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/debugging/appcall/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_common.py
+-rw-rw-rw-   0        0        0      895 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_linux.py
+-rw-rw-rw-   0        0        0     1284 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_win.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.671082 YaraForge-0.1.4b1/python/examples/debugging/dbghooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/debugging/dbghooks/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/dbghooks/automatic_steps.py
+-rw-rw-rw-   0        0        0     3813 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/dbghooks/dbg_trace.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.689077 YaraForge-0.1.4b1/python/examples/debugging/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/debugging/misc/__init__.py
+-rw-rw-rw-   0        0        0     2127 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/misc/print_call_stack.py
+-rw-rw-rw-   0        0        0     1753 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/misc/print_registers.py
+-rw-rw-rw-   0        0        0     1899 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/misc/registers_context_menu.py
+-rw-rw-rw-   0        0        0      661 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/debugging/show_debug_names.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.812081 YaraForge-0.1.4b1/python/examples/hexrays/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/hexrays/__init__.py
+-rw-rw-rw-   0        0        0     3512 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/colorize_pseudocode_lines.py
+-rw-rw-rw-   0        0        0     3638 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/curpos_details.py
+-rw-rw-rw-   0        0        0     2453 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/decompile_entry_points.py
+-rw-rw-rw-   0        0        0      732 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds1.py
+-rw-rw-rw-   0        0        0     2518 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds10.py
+-rw-rw-rw-   0        0        0     2875 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds11.py
+-rw-rw-rw-   0        0        0     5949 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds12.py
+-rw-rw-rw-   0        0        0     1162 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds13.py
+-rw-rw-rw-   0        0        0    10835 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds17.py
+-rw-rw-rw-   0        0        0     2325 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds19.py
+-rw-rw-rw-   0        0        0     3913 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds21.py
+-rw-rw-rw-   0        0        0     7264 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds3.py
+-rw-rw-rw-   0        0        0     3569 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds4.py
+-rw-rw-rw-   0        0        0    12037 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds5.py
+-rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds6.py
+-rw-rw-rw-   0        0        0     1147 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds7.py
+-rw-rw-rw-   0        0        0     3037 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds8.py
+-rw-rw-rw-   0        0        0     1128 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds_create_hint.py
+-rw-rw-rw-   0        0        0     4700 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds_hooks.py
+-rw-rw-rw-   0        0        0     1860 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds_modify_user_lvars.py
+-rw-rw-rw-   0        0        0     9292 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/hexrays/vds_xrefs.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.830081 YaraForge-0.1.4b1/python/examples/idbhooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/idbhooks/__init__.py
+-rw-rw-rw-   0        0        0     9228 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/idbhooks/log_idb_events.py
+-rw-rw-rw-   0        0        0     2882 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/idbhooks/operand_changed.py
+-rw-rw-rw-   0        0        0     3116 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/idbhooks/replay_prototypes_changes.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.842081 YaraForge-0.1.4b1/python/examples/idphooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/idphooks/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/idphooks/ana_emu_out.py
+-rw-rw-rw-   0        0        0     1329 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/idphooks/assemble.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.865081 YaraForge-0.1.4b1/python/examples/pyqt/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/pyqt/__init__.py
+-rw-rw-rw-   0        0        0     3335 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/pyqt/inject_command.py
+-rw-rw-rw-   0        0        0     5627 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/pyqt/paint_over_graph.py
+-rw-rw-rw-   0        0        0     2599 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/pyqt/paint_over_navbar.py
+-rw-rw-rw-   0        0        0     1130 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.887076 YaraForge-0.1.4b1/python/examples/uihooks/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/uihooks/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/uihooks/func_chooser_coloring.py
+-rw-rw-rw-   0        0        0     4757 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/uihooks/lines_rendering.py
+-rw-rw-rw-   0        0        0     5181 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/uihooks/log_misc_events.py
+-rw-rw-rw-   0        0        0      644 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/uihooks/prevent_jump.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.887076 YaraForge-0.1.4b1/python/examples/widgets/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.896083 YaraForge-0.1.4b1/python/examples/widgets/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/forms/__init__.py
+-rw-rw-rw-   0        0        0    11536 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/forms/askusingform.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.912076 YaraForge-0.1.4b1/python/examples/widgets/graphs/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/graphs/__init__.py
+-rw-rw-rw-   0        0        0     5336 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/graphs/custom_graph_with_actions.py
+-rw-rw-rw-   0        0        0     3115 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/graphs/sync_two_graphs.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.922083 YaraForge-0.1.4b1/python/examples/widgets/idaview/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/idaview/__init__.py
+-rw-rw-rw-   0        0        0     4003 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/idaview/wrap_idaview.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.943077 YaraForge-0.1.4b1/python/examples/widgets/listings/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/listings/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/listings/custom_viewer.py
+-rw-rw-rw-   0        0        0     3956 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/listings/jump_next_comment.py
+-rw-rw-rw-   0        0        0     3160 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/listings/save_and_restore_listing_pos.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.950081 YaraForge-0.1.4b1/python/examples/widgets/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/misc/__init__.py
+-rw-rw-rw-   0        0        0     1829 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/misc/add_menus.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.951081 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.983076 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/__init__.py
+-rw-rw-rw-   0        0        0     5338 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/choose.py
+-rw-rw-rw-   0        0        0     1634 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/choose_multi.py
+-rw-rw-rw-   0        0        0    10380 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py
+-rw-rw-rw-   0        0        0     1579 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/func_chooser.py
+-rw-rw-rw-   0        0        0     3142 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.990078 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/string_window/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/string_window/__init__.py
+-rw-rw-rw-   0        0        0     3204 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:44.997081 YaraForge-0.1.4b1/python/examples/widgets/waitbox/
+-rw-rw-rw-   0        0        0        0 2024-03-09 11:48:23.000000 YaraForge-0.1.4b1/python/examples/widgets/waitbox/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-06-08 15:50:58.000000 YaraForge-0.1.4b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 05:17:45.042081 YaraForge-0.1.4b1/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2024-03-17 19:15:22.000000 YaraForge-0.1.4b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.001077 YaraForge-0.1.4b1/yaraforge/
+-rw-rw-rw-   0        0        0        0 2024-03-09 20:13:15.000000 YaraForge-0.1.4b1/yaraforge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.007081 YaraForge-0.1.4b1/yaraforge/config/
+-rw-rw-rw-   0        0        0        0 2024-04-12 19:45:41.000000 YaraForge-0.1.4b1/yaraforge/config/__init__.py
+-rw-rw-rw-   0        0        0     1363 2024-04-12 19:46:01.000000 YaraForge-0.1.4b1/yaraforge/config/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.020083 YaraForge-0.1.4b1/yaraforge/maker/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:42:22.000000 YaraForge-0.1.4b1/yaraforge/maker/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/maker/dump_maker.py
+-rw-rw-rw-   0        0        0     2622 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/maker/instruction_maker.py
+-rw-rw-rw-   0        0        0     5293 2024-04-23 05:10:03.000000 YaraForge-0.1.4b1/yaraforge/maker/yara_maker.py
+-rw-rw-rw-   0        0        0     1322 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.026081 YaraForge-0.1.4b1/yaraforge/plugin/
+-rw-rw-rw-   0        0        0     2306 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/plugin/__init__.py
+-rw-rw-rw-   0        0        0      294 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/plugin/yaraforge.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.027077 YaraForge-0.1.4b1/yaraforge/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-12 14:12:08.000000 YaraForge-0.1.4b1/yaraforge/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 05:17:45.039081 YaraForge-0.1.4b1/yaraforge/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-11 07:42:44.000000 YaraForge-0.1.4b1/yaraforge/utils/__init__.py
+-rw-rw-rw-   0        0        0     1413 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/utils/cache_dumper.py
+-rw-rw-rw-   0        0        0     4659 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/utils/common.py
+-rw-rw-rw-   0        0        0     2413 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/utils/logger.py
+-rw-rw-rw-   0        0        0     1280 2024-04-12 20:13:05.000000 YaraForge-0.1.4b1/yaraforge/utils/opcode_processor.py
+-rw-rw-rw-   0        0        0      342 2024-04-23 05:17:25.000000 YaraForge-0.1.4b1/yaraforge/version.py
```

### Comparing `YaraForge-0.1.3b1/PKG-INFO` & `YaraForge-0.1.4b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: YaraForge
-Version: 0.1.3b1
+Version: 0.1.4b1
 Summary: A plugin for IDA Pro to generate Yara rules from binary files.
 Home-page: https://github.com/zhaoxinnZ/YaraForge
 Author: Zhao Xinn, Tsai YA-HSUAN, Ting0525
 Author-email: zhaoxinzhang0429@gmail.com, aooood456@gmail.com, zg45154551@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8, <3.12
-
-UNKNOWN
-
+Requires-Dist: capstone>=5.0.1
+Requires-Dist: flare-capa>=7.0.1
```

### Comparing `YaraForge-0.1.3b1/YaraForge.egg-info/PKG-INFO` & `YaraForge-0.1.4b1/YaraForge.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: YaraForge
-Version: 0.1.3b1
+Version: 0.1.4b1
 Summary: A plugin for IDA Pro to generate Yara rules from binary files.
 Home-page: https://github.com/zhaoxinnZ/YaraForge
 Author: Zhao Xinn, Tsai YA-HSUAN, Ting0525
 Author-email: zhaoxinzhang0429@gmail.com, aooood456@gmail.com, zg45154551@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8, <3.12
-
-UNKNOWN
-
+Requires-Dist: capstone>=5.0.1
+Requires-Dist: flare-capa>=7.0.1
```

### Comparing `YaraForge-0.1.3b1/YaraForge.egg-info/SOURCES.txt` & `YaraForge-0.1.4b1/YaraForge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+setup.cfg
 setup.py
 YaraForge.egg-info/PKG-INFO
 YaraForge.egg-info/SOURCES.txt
 YaraForge.egg-info/dependency_links.txt
 YaraForge.egg-info/requires.txt
 YaraForge.egg-info/top_level.txt
 python/__init__.py
@@ -205,14 +206,16 @@
 python/examples/widgets/tabular_views/string_window/__init__.py
 python/examples/widgets/tabular_views/string_window/show_selected_strings.py
 python/examples/widgets/waitbox/__init__.py
 python/examples/widgets/waitbox/show_and_hide_waitbox.py
 yaraforge/__init__.py
 yaraforge/metadata.py
 yaraforge/version.py
+yaraforge/config/__init__.py
+yaraforge/config/settings.py
 yaraforge/maker/__init__.py
 yaraforge/maker/dump_maker.py
 yaraforge/maker/instruction_maker.py
 yaraforge/maker/yara_maker.py
 yaraforge/plugin/__init__.py
 yaraforge/plugin/yaraforge.py
 yaraforge/tests/__init__.py
```

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/compiler.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/indenter.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/indenter.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/misc.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/misc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/proxy_metaclass.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Compiler/qtproxies.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Compiler/qtproxies.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/loader.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/Loader/qobjectcreator.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/Loader/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/driver.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/driver.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/exceptions.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/exceptions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/icon_cache.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/icon_cache.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/objcreator.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/objcreator.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/as_string.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/as_string.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/ascii_upper.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/ascii_upper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/proxy_base.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/proxy_base.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v2/string_io.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v2/string_io.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/__init__.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/as_string.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/as_string.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/ascii_upper.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/ascii_upper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/proxy_base.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/proxy_base.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/port_v3/string_io.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/port_v3/string_io.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/properties.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/properties.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/pyuic.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/pyuic.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/uiparser.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/uiparser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qaxcontainer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qscintilla.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtcharts.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtprintsupport.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtquickwidgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtwebenginewidgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py` & `YaraForge-0.1.4b1/python/3/PyQt5/uic/widget-plugins/qtwebkit.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_allins.py` & `YaraForge-0.1.4b1/python/3/ida_allins.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_auto.py` & `YaraForge-0.1.4b1/python/3/ida_auto.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_bitrange.py` & `YaraForge-0.1.4b1/python/3/ida_bitrange.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_bytes.py` & `YaraForge-0.1.4b1/python/3/ida_bytes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_dbg.py` & `YaraForge-0.1.4b1/python/3/ida_dbg.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_dirtree.py` & `YaraForge-0.1.4b1/python/3/ida_dirtree.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_diskio.py` & `YaraForge-0.1.4b1/python/3/ida_diskio.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_entry.py` & `YaraForge-0.1.4b1/python/3/ida_entry.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_enum.py` & `YaraForge-0.1.4b1/python/3/ida_enum.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_expr.py` & `YaraForge-0.1.4b1/python/3/ida_expr.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_fixup.py` & `YaraForge-0.1.4b1/python/3/ida_fixup.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_fpro.py` & `YaraForge-0.1.4b1/python/3/ida_fpro.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_frame.py` & `YaraForge-0.1.4b1/python/3/ida_frame.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_funcs.py` & `YaraForge-0.1.4b1/python/3/ida_funcs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_gdl.py` & `YaraForge-0.1.4b1/python/3/ida_gdl.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_graph.py` & `YaraForge-0.1.4b1/python/3/ida_graph.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_hexrays.py` & `YaraForge-0.1.4b1/python/3/ida_hexrays.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_ida.py` & `YaraForge-0.1.4b1/python/3/ida_ida.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_idaapi.py` & `YaraForge-0.1.4b1/python/3/ida_idaapi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_idc.py` & `YaraForge-0.1.4b1/python/3/ida_idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_idd.py` & `YaraForge-0.1.4b1/python/3/ida_idd.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_idp.py` & `YaraForge-0.1.4b1/python/3/ida_idp.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_ieee.py` & `YaraForge-0.1.4b1/python/3/ida_ieee.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_kernwin.py` & `YaraForge-0.1.4b1/python/3/ida_kernwin.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_lines.py` & `YaraForge-0.1.4b1/python/3/ida_lines.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_loader.py` & `YaraForge-0.1.4b1/python/3/ida_loader.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_moves.py` & `YaraForge-0.1.4b1/python/3/ida_moves.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_nalt.py` & `YaraForge-0.1.4b1/python/3/ida_nalt.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_name.py` & `YaraForge-0.1.4b1/python/3/ida_name.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_netnode.py` & `YaraForge-0.1.4b1/python/3/ida_netnode.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_offset.py` & `YaraForge-0.1.4b1/python/3/ida_offset.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_pro.py` & `YaraForge-0.1.4b1/python/3/ida_pro.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_problems.py` & `YaraForge-0.1.4b1/python/3/ida_problems.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_range.py` & `YaraForge-0.1.4b1/python/3/ida_range.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_registry.py` & `YaraForge-0.1.4b1/python/3/ida_registry.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_search.py` & `YaraForge-0.1.4b1/python/3/ida_search.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_segment.py` & `YaraForge-0.1.4b1/python/3/ida_segment.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_segregs.py` & `YaraForge-0.1.4b1/python/3/ida_segregs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_srclang.py` & `YaraForge-0.1.4b1/python/3/ida_srclang.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_strlist.py` & `YaraForge-0.1.4b1/python/3/ida_strlist.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_struct.py` & `YaraForge-0.1.4b1/python/3/ida_struct.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_tryblks.py` & `YaraForge-0.1.4b1/python/3/ida_tryblks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_typeinf.py` & `YaraForge-0.1.4b1/python/3/ida_typeinf.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_ua.py` & `YaraForge-0.1.4b1/python/3/ida_ua.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/ida_xref.py` & `YaraForge-0.1.4b1/python/3/ida_xref.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/idaapi.py` & `YaraForge-0.1.4b1/python/3/idaapi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/idadex.py` & `YaraForge-0.1.4b1/python/3/idadex.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/idautils.py` & `YaraForge-0.1.4b1/python/3/idautils.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/idc.py` & `YaraForge-0.1.4b1/python/3/idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/3/init.py` & `YaraForge-0.1.4b1/python/3/init.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/analysis/dump_func_info.py` & `YaraForge-0.1.4b1/python/examples/analysis/dump_func_info.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/actions.py` & `YaraForge-0.1.4b1/python/examples/core/actions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/add_hotkey.py` & `YaraForge-0.1.4b1/python/examples/core/add_hotkey.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/add_idc_hotkey.py` & `YaraForge-0.1.4b1/python/examples/core/add_idc_hotkey.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/auto_instantiate_widget_plugin.py` & `YaraForge-0.1.4b1/python/examples/core/auto_instantiate_widget_plugin.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/bin_search.py` & `YaraForge-0.1.4b1/python/examples/core/bin_search.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/colorize_disassembly.py` & `YaraForge-0.1.4b1/python/examples/core/colorize_disassembly.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/colorize_disassembly_on_the_fly.py` & `YaraForge-0.1.4b1/python/examples/core/colorize_disassembly_on_the_fly.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/create_structure_programmatically.py` & `YaraForge-0.1.4b1/python/examples/core/create_structure_programmatically.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/custom_cli.py` & `YaraForge-0.1.4b1/python/examples/core/custom_cli.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/custom_data_types_and_formats.py` & `YaraForge-0.1.4b1/python/examples/core/custom_data_types_and_formats.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/dump_extra_comments.py` & `YaraForge-0.1.4b1/python/examples/core/dump_extra_comments.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/dump_flowchart.py` & `YaraForge-0.1.4b1/python/examples/core/dump_flowchart.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/dump_selection.py` & `YaraForge-0.1.4b1/python/examples/core/dump_selection.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/extend_idc.py` & `YaraForge-0.1.4b1/python/examples/core/extend_idc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/idapythonrc.py` & `YaraForge-0.1.4b1/python/examples/core/idapythonrc.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/install_user_defined_prefix.py` & `YaraForge-0.1.4b1/python/examples/core/install_user_defined_prefix.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_bookmarks.py` & `YaraForge-0.1.4b1/python/examples/core/list_bookmarks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_function_items.py` & `YaraForge-0.1.4b1/python/examples/core/list_function_items.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_imports.py` & `YaraForge-0.1.4b1/python/examples/core/list_imports.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_patched_bytes.py` & `YaraForge-0.1.4b1/python/examples/core/list_patched_bytes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_problems.py` & `YaraForge-0.1.4b1/python/examples/core/list_problems.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_segment_functions.py` & `YaraForge-0.1.4b1/python/examples/core/list_segment_functions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_segment_functions_using_idautils.py` & `YaraForge-0.1.4b1/python/examples/core/list_segment_functions_using_idautils.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_stkvar_xrefs.py` & `YaraForge-0.1.4b1/python/examples/core/list_stkvar_xrefs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/list_strings.py` & `YaraForge-0.1.4b1/python/examples/core/list_strings.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/produce_c_file.py` & `YaraForge-0.1.4b1/python/examples/core/produce_c_file.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/produce_lst_file.py` & `YaraForge-0.1.4b1/python/examples/core/produce_lst_file.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/register_timer.py` & `YaraForge-0.1.4b1/python/examples/core/register_timer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/core/trigger_actions_programmatically.py` & `YaraForge-0.1.4b1/python/examples/core/trigger_actions_programmatically.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/cvt64/py_cvt64_sample.py` & `YaraForge-0.1.4b1/python/examples/cvt64/py_cvt64_sample.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_common.py` & `YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_common.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_linux.py` & `YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_linux.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/appcall/simple_appcall_win.py` & `YaraForge-0.1.4b1/python/examples/debugging/appcall/simple_appcall_win.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/dbghooks/automatic_steps.py` & `YaraForge-0.1.4b1/python/examples/debugging/dbghooks/automatic_steps.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/dbghooks/dbg_trace.py` & `YaraForge-0.1.4b1/python/examples/debugging/dbghooks/dbg_trace.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/misc/print_call_stack.py` & `YaraForge-0.1.4b1/python/examples/debugging/misc/print_call_stack.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/misc/print_registers.py` & `YaraForge-0.1.4b1/python/examples/debugging/misc/print_registers.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/misc/registers_context_menu.py` & `YaraForge-0.1.4b1/python/examples/debugging/misc/registers_context_menu.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/debugging/show_debug_names.py` & `YaraForge-0.1.4b1/python/examples/debugging/show_debug_names.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/colorize_pseudocode_lines.py` & `YaraForge-0.1.4b1/python/examples/hexrays/colorize_pseudocode_lines.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/curpos_details.py` & `YaraForge-0.1.4b1/python/examples/hexrays/curpos_details.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/decompile_entry_points.py` & `YaraForge-0.1.4b1/python/examples/hexrays/decompile_entry_points.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds1.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds1.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds10.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds10.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds11.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds11.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds12.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds12.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds13.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds13.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds17.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds17.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds19.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds19.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds21.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds21.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds3.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds3.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds4.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds4.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds5.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds5.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds6.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds6.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds7.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds7.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds8.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds8.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds_create_hint.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds_create_hint.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds_hooks.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds_hooks.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds_modify_user_lvars.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds_modify_user_lvars.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/hexrays/vds_xrefs.py` & `YaraForge-0.1.4b1/python/examples/hexrays/vds_xrefs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/idbhooks/log_idb_events.py` & `YaraForge-0.1.4b1/python/examples/idbhooks/log_idb_events.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/idbhooks/operand_changed.py` & `YaraForge-0.1.4b1/python/examples/idbhooks/operand_changed.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/idbhooks/replay_prototypes_changes.py` & `YaraForge-0.1.4b1/python/examples/idbhooks/replay_prototypes_changes.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/idphooks/ana_emu_out.py` & `YaraForge-0.1.4b1/python/examples/idphooks/ana_emu_out.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/idphooks/assemble.py` & `YaraForge-0.1.4b1/python/examples/idphooks/assemble.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/pyqt/inject_command.py` & `YaraForge-0.1.4b1/python/examples/pyqt/inject_command.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/pyqt/paint_over_graph.py` & `YaraForge-0.1.4b1/python/examples/pyqt/paint_over_graph.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/pyqt/paint_over_navbar.py` & `YaraForge-0.1.4b1/python/examples/pyqt/paint_over_navbar.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py` & `YaraForge-0.1.4b1/python/examples/pyqt/populate_pluginform_with_pyqt_widgets.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/uihooks/func_chooser_coloring.py` & `YaraForge-0.1.4b1/python/examples/uihooks/func_chooser_coloring.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/uihooks/lines_rendering.py` & `YaraForge-0.1.4b1/python/examples/uihooks/lines_rendering.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/uihooks/log_misc_events.py` & `YaraForge-0.1.4b1/python/examples/uihooks/log_misc_events.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/uihooks/prevent_jump.py` & `YaraForge-0.1.4b1/python/examples/uihooks/prevent_jump.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/forms/askusingform.py` & `YaraForge-0.1.4b1/python/examples/widgets/forms/askusingform.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/graphs/custom_graph_with_actions.py` & `YaraForge-0.1.4b1/python/examples/widgets/graphs/custom_graph_with_actions.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/graphs/sync_two_graphs.py` & `YaraForge-0.1.4b1/python/examples/widgets/graphs/sync_two_graphs.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/idaview/wrap_idaview.py` & `YaraForge-0.1.4b1/python/examples/widgets/idaview/wrap_idaview.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/listings/custom_viewer.py` & `YaraForge-0.1.4b1/python/examples/widgets/listings/custom_viewer.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/listings/jump_next_comment.py` & `YaraForge-0.1.4b1/python/examples/widgets/listings/jump_next_comment.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/listings/save_and_restore_listing_pos.py` & `YaraForge-0.1.4b1/python/examples/widgets/listings/save_and_restore_listing_pos.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/misc/add_menus.py` & `YaraForge-0.1.4b1/python/examples/widgets/misc/add_menus.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/choose.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/choose.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/choose_multi.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/choose_multi.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/chooser_with_folders.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/func_chooser.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/func_chooser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/custom/lazy_loaded_chooser.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py` & `YaraForge-0.1.4b1/python/examples/widgets/tabular_views/string_window/show_selected_strings.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py` & `YaraForge-0.1.4b1/python/examples/widgets/waitbox/show_and_hide_waitbox.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/setup.py` & `YaraForge-0.1.4b1/setup.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/maker/dump_maker.py` & `YaraForge-0.1.4b1/yaraforge/maker/dump_maker.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/maker/instruction_maker.py` & `YaraForge-0.1.4b1/yaraforge/maker/instruction_maker.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/maker/yara_maker.py` & `YaraForge-0.1.4b1/yaraforge/maker/yara_maker.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,24 @@
             self.instructions_info = []  # Reset instructions_info list for each rule
             all_instructions_signature = []
             func = idaapi.get_func(address)
             if not func:
                 print(f"Address {hex(address)} does not belong to any function.")
                 continue
 
-            md = Cs(CS_ARCH_X86, CS_MODE_64)
+            # 取得目前的架構
+            info = idaapi.get_inf_structure()
+            if info.is_64bit():
+                md = Cs(CS_ARCH_X86, CS_MODE_64)
+            elif info.is_32bit():
+                md = Cs(CS_ARCH_X86, CS_MODE_32)
+            else:
+                print("Unsupported architecture.")
+                continue
+
             md.detail = True
 
             fci = idaapi.FlowChart(func)
             for block in fci:
                 if block.start_ea <= address < block.end_ea:
                     code_bytes = idc.get_bytes(block.start_ea, block.end_ea - block.start_ea)
                     disasm = md.disasm(code_bytes, block.start_ea)
```

### Comparing `YaraForge-0.1.3b1/yaraforge/metadata.py` & `YaraForge-0.1.4b1/yaraforge/metadata.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/plugin/__init__.py` & `YaraForge-0.1.4b1/yaraforge/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/utils/cache_dumper.py` & `YaraForge-0.1.4b1/yaraforge/utils/cache_dumper.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/utils/common.py` & `YaraForge-0.1.4b1/yaraforge/utils/common.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/utils/logger.py` & `YaraForge-0.1.4b1/yaraforge/utils/logger.py`

 * *Files identical despite different names*

### Comparing `YaraForge-0.1.3b1/yaraforge/utils/opcode_processor.py` & `YaraForge-0.1.4b1/yaraforge/utils/opcode_processor.py`

 * *Files identical despite different names*

